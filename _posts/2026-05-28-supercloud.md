---
title: 'Extend Compute Node Time on the MIT Supercloud'
date: 2026-05-28
permalink: /posts/2026/05/extend-compute-node-time/
tags:
  - MIT Supercloud
---

MIT SuperCloud assign interactive compute nodes with a default 30 minutes time limit, which is often not enough to debug the code. To get around this, we can use `salloc` instead of `LLsub`. Here's how you can set up GPU longer than 30 minutes:

*Verified on 05/28/2026*

## 1. Request GPU allocation

```bash
salloc --gres=gpu:volta:1 \
       --cpus-per-task=20 \
       --time=04:00:00
```

Example output:

```text
salloc: Granted job allocation 4852189
salloc: Waiting for resource configuration
salloc: Nodes d-12-1-1 are ready for job
```

At this stage, the GPU node is reserved, but you are still on the login node.

---

## 2. Enter the compute node interactively

```bash
srun --pty bash
```

Now the prompt should become something like:

```text
(periodicwaveboson) (py313) hlo1@d-12-1-1:~$
```

You are now inside the GPU compute node.

---

## 3. Verify GPU access

```bash
hostname
nvidia-smi
```