# Prerequisites

## Azure requirements
- An Azure subscription where you can create:
  - Microsoft Foundry / Azure AI Foundry Project
  - Foundry Agent Service resources and referenced tools (e.g., Search if you use it)
- You must have RBAC that allows calling the Agents service (Entra auth is required).

> Foundry Agent Service supports Microsoft Entra ID tokens (keyless auth) and uses RBAC.  
> See the Agents API reference for auth details.

## Local requirements
- VS Code
- Python 3.10+ (3.11 recommended)
- Git

## Helpful (Lab 02 / 03)
- Microsoft Foundry for VS Code extension (for workflows + agent assets in-editor)
- For Lab 03: familiarity with basic async patterns

## References
- Foundry Agent Service “project endpoint” format (newer SDKs) and migration note.
- Tools overview (Bing grounding, Azure AI Search, Logic Apps, etc.).
- Knowledge retrieval / Foundry IQ knowledge base integration.
