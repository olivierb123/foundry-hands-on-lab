# Lab 01 — Single Agent (tools + knowledge)

## Goal
Build and run a **single Foundry Agent Service agent** that can:
- answer questions about the band using **knowledge retrieval**
- optionally use one built-in tool (e.g., file search / knowledge base)

We keep the scenario simple: “You are the Circasonic band assistant.”

## What you build
- A small Python console app using the Azure AI Agents SDK
- An agent configured with:
  - instructions
  - a knowledge source (choose one option below)

## Knowledge options (pick one)
### Option A — Files + File Search tool (simplest for a HOL)
- You upload / attach a couple of documents and enable file search tool in the agent.

### Option B — Foundry IQ knowledge base (Azure AI Search-backed)
- Create a knowledge base, index docs, and connect it to your agent.

> Docs: tool overview and knowledge retrieval options.

---

## Step 1 — Prepare sample knowledge files
See `assets/knowledge/`:
- `circasonic-bio.md`
- `setlist-notes.md`

You will use these as your first “ground truth” corpus.

## Step 2 — Create the agent in Foundry
In Foundry portal:
1. Create a new Agent
2. Name: `circasonic-assistant`
3. Instructions: use the prompt below
4. Enable the knowledge option you picked (File Search or Knowledge Base)

**Agent instructions**
```text
You are the Circasonic Band Assistant.
- Be concise and practical.
- When asked about the band, base answers on the knowledge source.
- If the user asks for a show plan, output:
  1) setlist guidance
  2) stage/FOH notes
  3) 1 short social post draft
