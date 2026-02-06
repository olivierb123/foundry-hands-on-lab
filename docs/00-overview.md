# Overview

## What you will learn
This HOL focuses on three “levels” of Azure AI Foundry agents:

### Level 1 — Single managed agent
- Create an agent in Foundry Agent Service
- Add **tools** and **knowledge** (retrieval)
- Run it via SDK from a local terminal

### Level 2 — Managed multi-agent orchestration
- Use Foundry **Workflows** to orchestrate multiple agents
- Implement both:
  - **Sequential**: agent output feeds the next agent
  - **Parallel**: multiple agents run in parallel, then you merge

### Level 3 — Pro-code multi-agent orchestration
- Use **Microsoft Agent Framework** to orchestrate agents in code
- Run locally, then (optionally) deploy

## Recommended scenario for the lab
We use a consistent domain throughout (music / band operations) to keep prompts and outputs easy to validate:
- “Circasonic band assistant” agent
- knowledge base includes a short “bio” and “setlist notes”
- workflow produces a show plan + social post + technical stage notes

You can replace the content with any domain later (support, finance, HR, etc.).
