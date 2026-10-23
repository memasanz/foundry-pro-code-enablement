# Session 8: Optimization, Publishing & Agent 365

## Core reading

- [Agent 365 overview](https://learn.microsoft.com/en-us/microsoft-agent-365/overview) - Understand the enterprise agent control plane, enablement, and prerequisites.
- [Agent 365 integration with Foundry](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-365-integration) - Review registry integration, supported agent types, and telemetry requirements.
- [Agent identity concepts in Foundry](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-identity) - Understand Entra agent identities, ownership, and downstream authorization.

## Optimization and publishing

- [Optimize a prompt agent](https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-optimize-prompt-agent) - Compare optimized candidates with a baseline and promote a selected version.
- [Optimize a hosted agent](https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-optimize-hosted-agent) - Explore the hosted-agent optimization workflow and its prerequisites.
- [Publish agents to Microsoft Copilot and Teams](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/publish-copilot) - Review publishing, audience scope, administrator approval, and updates.
- [Publish using the REST API, including private-network projects](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/publish-copilot-virtual-network) - Review the publishing route and connectivity requirements when public network access is disabled.

## Release readiness

- [Hosted-agent CI/CD quickstart](https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/set-up-cicd-hosted-agent) - Revisit the deployment/smoke-test pipeline before adding quality gates.
- [Agent development lifecycle](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/development-lifecycle) - Review versioning, permissions, publishing, monitoring, and controlled rollout.

Confirm tenant licensing, enablement, publishing permissions, and administrator support before the session. The CI/CD quickstart provides a deployment smoke test, not a quality-evaluation gate; use the Session 7 evaluation references to design that additional check.