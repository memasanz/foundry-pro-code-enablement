# Session 7: Observability & Evaluations

## Core reading

- [Observability in generative AI](https://learn.microsoft.com/en-us/azure/foundry/concepts/observability) - Connect tracing, evaluation, and monitoring across the AI lifecycle.
- [Agent tracing overview](https://learn.microsoft.com/en-us/azure/foundry/observability/concepts/trace-agent-concept) - Understand end-to-end traces, model requests, and tool-call visibility.
- [Evaluation in Microsoft Foundry](https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-overview) - Plan a repeatable evaluation process and quality baseline.
- [Agent evaluators](https://learn.microsoft.com/en-us/azure/foundry/concepts/evaluation-evaluators/agent-evaluators) - Select metrics for task completion, tool use, and agent behavior.

## Hands-on references

- [Set up tracing in Foundry](https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/trace-agent-setup) - Connect Application Insights and capture agent telemetry.
- [Evaluate your AI agents](https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/evaluate-agent) - Run code-first agent evaluations against representative test inputs.
- [Evaluate existing datasets with the Foundry SDK](https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/cloud-evaluation-datasets) - Use a versioned dataset for repeatable evaluation runs.
- [Monitor agents](https://learn.microsoft.com/en-us/azure/foundry/observability/how-to/how-to-monitor-agents-dashboard) - Review operational signals and monitor quality after deployment.

Use approved test data and review tracing data-handling settings before capturing prompts, responses, or tool payloads.