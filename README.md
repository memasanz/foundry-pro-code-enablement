# Microsoft Foundry Pro-Code Enablement

## From foundations to pro-code agents

A four-week working engagement for development teams.

## Engagement overview

| Item | Plan |
| --- | --- |
| Duration | Four weeks; eight sessions. |
| Cadence | Tuesdays and Thursdays; 60 minutes per session. Dates and times to be confirmed. |
| Audience | Developers building pro-code AI applications and agents, with platform/security support for prerequisites. |
| Format | Engineer-led working sessions, guided demonstrations, and implementation exercises between meetings. |
| Goal | Enable developers to use Foundry models and Agent Service, integrate tools and knowledge, and apply a repeatable AI development lifecycle. |
| Final outcome | A version-controlled reference implementation spanning model calls, prompt and hosted agents, tools, knowledge, evaluation results, and a deployment/release pattern. |

## The four-week journey

| Week | Focus |
| --- | --- |
| 1 | Foundry Foundations & Models |
| 2 | Foundry Agent Service & Pro-Code Agents |
| 3 | Foundry Tools, IQ & Memory |
| 4 | Evaluate, optimize & publish with Agent 365 |

One reference scenario evolves throughout the engagement. Sandbox readiness is a prerequisite, not the primary delivery objective.

## Environment approach: start in a sandbox, plan for private networking

The workshop can begin in an approved Foundry sandbox environment so participants can start learning and building without waiting for a full enterprise deployment.

As the workshop progresses, we encourage teams to deploy Foundry in a private network configuration, working with their platform, networking, and security teams. Use the [Foundry private-network agent tools deployment sample](https://github.com/microsoft-foundry/foundry-samples/tree/main/infrastructure/infrastructure-setup-bicep/19-private-network-agent-tools) as a reference for planning and deployment.

Private-network deployment can proceed alongside the workshop; it is not a prerequisite for the first session. Validate connectivity, permissions, and feature compatibility before moving labs into the private environment. Enterprise deployment and approvals remain a separately owned workstream.

## Week 1: Foundry Foundations & Models

**Weekly milestone:** Understand the platform and AI lifecycle, then deploy and invoke an approved model.

### [Tuesday - Session 1: Foundry Overview, Foundations & AI Lifecycle](./sessions/session-1-foundry-overview-foundations-ai-lifecycle/reference-links.md)

**Working agenda**

- Foundry overview covering the platform, key capabilities, and how models, agents, tools, and knowledge fit together.
- Foundry Foundations and AI lifecycle. Start with accounts/resources, projects, connections, and responsibility boundaries.
- Review identity, RBAC, and developer versus deployment access.
- Map the AI lifecycle: experiment, version, deploy, evaluate, operate, and improve.
- Introduce source control, CI/CD, environment separation, and release ownership.
- Select the reference use case and initial success criteria.

**Outcomes**

- Shared platform and lifecycle understanding.
- Confirmed access needs and ownership.
- Agreed reference scenario and starter repository.

### [Thursday - Session 2: Hello World to Models](./sessions/session-2-hello-world-to-models/reference-links.md)

**Working agenda**

- Compare model deployment types, availability, capacity, cost, and data-residency tradeoffs.
- Distinguish permissions to create/manage deployments from permissions to invoke models.
- Deploy or use an approved model and make a first SDK/API call.
- Explore Model Router and when model routing is useful.
- Introduce Content Safety, content filtering, and safe-response behavior.

**Outcomes**

- Successful model invocation from code.
- Documented deployment and permission choices.
- Initial routing and safety observations.

### Materials & preparation

Approved sandbox and model capacity; access matrix; local development environment; starter repository; model deployment comparison; safe sample prompts.

### Between-session follow-through

Repeat the model invocation independently. Commit the sample code and configuration template; record permission issues and model-selection decisions.

CI/CD is introduced here as a lifecycle practice. Hosted-agent deployment automation is applied in Week 2.

## Week 2: Foundry Agent Service & Pro-Code Agents

**Weekly milestone:** Create a tool-enabled prompt agent and deploy a minimal hosted agent.

### [Tuesday - Session 3: Agent Service Hello World & Prompt Agents](./sessions/session-3-agent-service-prompt-agents/reference-links.md)

**Working agenda**

- Introduce Agent Service and compare prompt agents with hosted agents.
- Create and invoke a prompt agent from code; explore instructions and conversations.
- Add an approved tool and inspect tool-call behavior.
- Explain MCP and connect a prepared MCP server.
- Introduce toolboxes for shared tool access, authentication, and governance.

**Outcomes**

- Working prompt agent invoked from code.
- A successful tool-backed interaction.
- Versioned instructions and agent configuration.

### [Thursday - Session 4: Hosted Agents & Agent Framework](./sessions/session-4-hosted-agents-agent-framework/reference-links.md)

**Working agenda**

- Build and debug a minimal hosted agent locally with Microsoft Agent Framework.
- Add custom logic and reuse an approved tool or toolbox.
- Deploy to Foundry and invoke the hosted endpoint.
- Explore multi-agent orchestration.

**Outcomes**

- Hosted reference agent deployed and invoked.
- A repeatable deployment/smoke-test pattern.

### Materials & preparation

Prompt and hosted starter samples; prepared MCP server/toolbox; Agent Framework example; deployment identity and approvals. Optional: CI/CD pipeline.

### Between-session follow-through

Modify the reference agent, redeploy through the prepared pipeline, and capture a tool interaction. Record a few expected answers for later evaluations.

Use scaffolded examples to fit the session length. Custom MCP-server development and complex multi-agent systems are outside the core labs.

## Week 3: Foundry Tools, IQ & Memory

**Weekly milestone:** Extend the reference scenario with a useful service, grounded knowledge, and a scoped memory demonstration.

### [Tuesday - Session 5: Foundry Tools](./sessions/session-5-foundry-tools/reference-links.md)

**Working agenda**

- Survey Foundry Tools and select a capability relevant to the reference scenario.
- Distinguish AI service capabilities from the agent-callable tools introduced in Week 2.
- Invoke the capability from the reference agent.
- Review authentication.

**Outcomes**

- One useful service integrated into the scenario.
- A repeatable invocation and error-handling pattern.

### [Thursday - Session 6: Foundry IQ & Memory](./sessions/session-6-foundry-iq-memory/reference-links.md)

**Working agenda**

- Explain knowledge sources, knowledge bases, and agentic retrieval.
- Discuss AI Gateway requirements for tool authentication and authorization.
- Connect one approved source; test grounding, citations, and access behavior.
- Compare enterprise knowledge, conversation state, and persistent memory.
- Demonstrate scoped memory across conversations using non-sensitive sample data.
- Discuss isolation, retention, deletion, and what the agent should not remember.

**Outcomes**

- Reference agent grounded in approved content.
- Recorded retrieval, citation, and access checks.
- Memory demonstration and documented usage boundaries.

### Materials & preparation

Approved sample documents and knowledge source; source permission matrix; selected service connection; prepared knowledge base; memory-compatible demonstration environment.

### Between-session follow-through

Add representative knowledge questions and failure cases to the test set. Record citation quality, access results, and decisions on memory scope and retention.

Confirm feature, region, and network support before the labs. Use an approved demonstration if preview capabilities cannot run in the team's environment.

## Week 4: Evaluate, Optimize & Publish

**Weekly milestone:** Measure and improve the reference agent, then publish it and review Agent 365 identity and governance.

### [Tuesday - Session 7: Observability & Evaluations](./sessions/session-7-observability-evaluations/reference-links.md)

**Working agenda**

- Inspect end-to-end traces, model requests, tool calls, and failures.
- Review latency, token consumption, and usage/cost signals.
- Run a small, versioned evaluation dataset built from the reference scenario.
- Assess task success, groundedness, tool use, and safety.
- Identify failure patterns and prioritize improvements.

**Outcomes**

- Operational visibility demonstrated.
- Evaluation baseline and agreed quality criteria.
- Prioritized improvement backlog.

### [Thursday - Session 8: Optimization, Publishing & Agent 365](./sessions/session-8-optimization-publishing-agent-365/reference-links.md)

**Working agenda**

- Compare a targeted improvement against the baseline; discuss quality, latency, and cost tradeoffs.
- Introduce Agent 365 as the enterprise agent control plane; cover Entra Agent ID, agent identity, ownership, and least-privilege permissions.
- Publish the reference agent; inspect its Agent 365 registry entry and review audience access and administrator approvals.
- Extend the pipeline with evaluation gates; review promotion and rollback.
- Have participants demonstrate invocation, modification, deployment, and diagnosis.
- Confirm ownership, documentation, open gaps, and next-phase priorities.

**Outcomes**

- Measured before/after comparison.
- Published agent and Agent 365 registry/identity walkthrough.
- Release checklist, participant-led demonstration, and agreed ownership.

### Materials & preparation

Earlier traces and test set; monitoring access; prepared pipeline extension; release checklist; publishing permissions; Agent 365-enabled demo tenant and administrator support.

### Between-session follow-through

Finalize the repository and runbook. Record the published agent, identity, permissions, owner, and access decisions; assign unresolved readiness gaps.

Use prepared examples to keep publishing, identity, and optimization focused. Confirm Agent 365 licensing, enablement, and approvals; use an approved demo if unavailable.

## Completion & handoff

| Area | Evidence of completion |
| --- | --- |
| Foundations | Participants can explain resource/project boundaries, access roles, and the AI development lifecycle. |
| Models & safety | Approved model invoked from code; deployment options, permissions, Model Router, and Content Safety discussed. |
| Agents & integrations | Prompt and hosted examples work; tool/MCP interaction demonstrated; Agent Framework and toolboxes covered. |
| Tools, IQ & memory | One service integrated; knowledge retrieval/citations checked; scoped memory demonstrated or an approved limitation recorded. |
| Evaluation & optimization | Versioned test set, baseline, and a measured improvement comparison recorded. |
| Release & Agent 365 | CI/CD, traces, and release controls reviewed; agent publishing and Agent 365 registry/identity demonstrated; owner and access decisions recorded. |
| Handoff | Participants lead a demonstration, and the team owns the reference repository, runbook, and prioritized follow-on backlog. |

## Prerequisites & delivery assumptions

- Before hands-on work: provide an approved Foundry sandbox/project, suitable model capacity, required RBAC, connectivity, local tooling, and repository access.
- An approved sandbox is sufficient to start. A private-network Foundry deployment is encouraged in parallel, with platform, networking, and security ownership.
- Prepare deployment/OIDC and publishing permissions, approved content, and safe sample data. Use no sensitive production data. Confirm Agent 365 licensing, tenant enablement, and administrator support before Week 4.
- Scope is one reference scenario, a small approved model set, prompt and hosted examples, one service integration, and one knowledge source.
- Sessions combine concepts, guided demonstrations, and hands-on exercises, with implementation continuing between meetings.
- Availability and preview restrictions are checked before delivery; memory currently does not support VNet integration. Record demonstrations, substitutions, and exceptions explicitly.

## Selected implementation references

- [Hosted-agent CI/CD quickstart (applied in Week 2)](https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/set-up-cicd-hosted-agent)
- [Foundry Agent Service overview](https://learn.microsoft.com/en-us/azure/foundry/agents/overview)
- [Foundry IQ overview](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/what-is-foundry-iq)
- [Memory overview and limitations](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/what-is-memory)
- [Agent 365 integration, publishing, and agent identity](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/agent-365-integration)
