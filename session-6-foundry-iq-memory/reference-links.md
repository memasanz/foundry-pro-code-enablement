# Session 6: Foundry IQ & Memory

## Core reading

- [What is Foundry IQ?](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/what-is-foundry-iq) - Understand knowledge bases, knowledge sources, grounding, and citations.
- [Knowledge sources for agentic retrieval](https://learn.microsoft.com/en-us/azure/search/agentic-knowledge-source-overview) - Review indexed and remote source options and their access requirements.
- [Memory in Foundry Agent Service](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/what-is-memory) - Distinguish persistent memory from conversation state and enterprise knowledge; review limitations.
- [Govern MCP tools using an AI gateway](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/governance) - Explore the gateway integration and its governance requirements.

## Hands-on references

- [Connect a Foundry IQ knowledge base to Agent Service](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/foundry-iq-connect) - Ground an agent in an approved knowledge base.
- [Add a Foundry IQ knowledge base to a hosted agent with a toolbox](https://learn.microsoft.com/en-us/azure/foundry/agents/quickstarts/quickstart-foundry-iq-hosted-agent) - Apply knowledge retrieval to the hosted reference agent.
- [Create and use memory](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/memory-usage) - Configure memory scope, retrieval, updates, and remember/forget behavior.

## Authentication and lab constraints

- [How toolbox authentication works](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/tool-authentication) - Review caller identity, downstream permissions, and per-user authentication.

Discuss when an AI gateway is appropriate rather than assuming it is required for every tool. Check current preview and network restrictions before the lab; memory stores currently do not support VNet integration.