# Environment setup (once)

## 1) Create a Foundry Project
1. Go to Microsoft Foundry (Azure AI Foundry) portal.
2. Create a **Project** in a resource group/region of your choice.
3. In the project overview, locate the **Project endpoint** (used by SDKs).

The endpoint pattern looks like:
`https://<resource>.services.ai.azure.com/api/projects/<project>`

> Starting in May 2025, Agents SDKs use the **Foundry project endpoint** (not the old hub connection string).

## 2) Deploy / select a model
- Ensure your project has access to an LLM deployment supported by Agent Service.
- Record the deployment name (you’ll set it as `MODEL_DEPLOYMENT_NAME`).

## 3) Assign RBAC
- Ensure your user (or your dev principal) has the roles required to call the agents endpoint.
- If you get 403s later, check IAM on the Foundry resource + project.

## 4) Configure local environment variables
Create a `.env` file (do not commit) with:

```bash
FOUNDRY_PROJECT_ENDPOINT="https://<resource>.services.ai.azure.com/api/projects/<project>"
MODEL_DEPLOYMENT_NAME="<your-model-deployment>"
