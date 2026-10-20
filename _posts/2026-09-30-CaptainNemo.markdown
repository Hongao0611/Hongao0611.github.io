---
layout: post
title:  "captain-nemo: running large batches of GPU jobs on Nautilus"
date:   2026-09-30 12:00:00 -0700
---

I released [captain-nemo](https://github.com/Hongao0611/captain-nemo), a small toolkit for running large batches of Kubernetes Jobs on the [Nautilus (NRP)](https://nrp.ai) cluster. I wrote it while running about 700 GPU jobs for my critical-period project,<!-- TODO(Hongao): verify "about 700 GPU jobs"; it is not in the CV or the repo --> where most of the work was keeping the batch moving rather than training the models.

The problems it handles:

- **The fair-use gate.** NRP refuses new pods while more than four of your pods "violate" its usage bands: GPU use under 40%, or CPU and memory far from what you requested. Every new GPU pod counts as a violator until its setup finishes, so launching a big batch at once can lock you out for an hour or more. captain-nemo counts violators the way NRP does and launches only when there is room.
- **Bad nodes.** A node with a broken GPU kills pods within seconds, looks free, and keeps attracting retries. captain-nemo keeps your jobs off the nodes listed in one file and tells you which nodes to add.
- **Checking in.** An hourly health report lists violators, failures grouped by node, jobs running out of retries, hung or stuck pods, and whether NRP is accepting new pods.
- **Manifests.** A preflight check flags setup steps that can hang (apt, pip, git, dataset copies) and recommends CPU and memory requests from your pods' measured usage.

The tools are plain Python and bash, with written instructions that a coding agent such as Claude Code, Codex, or Cursor can follow; you can also run the scripts yourself. The [reference notes](https://github.com/Hongao0611/captain-nemo/blob/main/skills/nautilus-scheduler/reference.md) collect what I learned along the way: how NRP scores pods, what bad nodes look like in logs, and how to size requests. The code is MIT-licensed.
