# Azure AI Foundry Hands-on Lab (HOL)

This repo is a hands-on lab to explore Azure AI Foundry / Foundry Agent Service in 3 progressively deeper ways:

1. **Lab 01 — Single Agent (Managed)**  
   Build a simple agent with **tools + knowledge** (retrieval) and run it from code.

2. **Lab 02 — Multi-agent Workflows (Managed Orchestration)**  
   Create **sequential** and **parallel** multi-agent workflows using Foundry Workflows, and iterate in VS Code.

3. **Lab 03 — Microsoft Agent Framework (Pro-code Orchestration)**  
   Run a multi-agent system using **Microsoft Agent Framework** with agent code in this repo.

> Notes:
> - Authentication uses **Microsoft Entra ID** + RBAC (not API keys).  
> - Modern Agents SDK uses a **Foundry project endpoint** format (not the older hub connection string).
>
> See docs: `docs/01-prereqs.md` and `docs/02-environment-setup.md`.

## Quick navigation
- Start here: `docs/00-overview.md`
- Prereqs: `docs/01-prereqs.md`
- Environment setup: `docs/02-environment-setup.md`
- Lab 01: `labs/lab-01-single-agent/README.md`
- Lab 02: `labs/lab-02-workflows/README.md`
- Lab 03: `labs/lab-03-agent-framework/README.md`
- Troubleshooting: `docs/03-troubleshooting.md`
- Cleanup: `docs/99-cleanup.md`
