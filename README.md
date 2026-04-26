# Model Context Protocol (MCP)

Anthropic's open protocol for connecting LLMs to tools and data &mdash; JSON-RPC primitives, transports, server-building, security and the ecosystem.

**Live index:** https://brendanjameslynskey.github.io/LLM_Hub_MCP/

## Presentations in this series

| # | Title | Status | Description |
|---|-------|--------|-------------|
| 01 | [The Model Context Protocol — A Visual Tour](https://brendanjameslynskey.github.io/MCP_01_Protocol_Overview/) | live | JSON-RPC 2.0 base, host/client/server roles, the five primitives (tools/resources/prompts/sampling/elicitation), capability negotiation, lifecycle, version timeline, fully-annotated handshake. |
| 02 | [Transports &amp; The Wire](https://brendanjameslynskey.github.io/MCP_02_Transports_and_Wire/) | live | stdio framing, deprecated HTTP+SSE, modern Streamable HTTP, sessions, resumability via Last-Event-ID, security headers, annotated wire capture. |
| 03 | [Building an MCP Server](https://brendanjameslynskey.github.io/MCP_03_Building_a_Server/) | live | From a 30-line skeleton to production servers &mdash; tools, resources, prompts, sampling, elicitation, errors/progress/cancellation/logging, MCP Inspector. Python and TypeScript SDKs side-by-side. |
| 04 | [Security &amp; OAuth 2.1](https://brendanjameslynskey.github.io/MCP_04_Security_and_OAuth/) | live | Threat model, OAuth 2.1 + PKCE, RFC 9728/8414/7591/8707, audience binding, confused-deputy, prompt injection, tool poisoning, sandboxing tiers. |
| 05 | [Ecosystem &amp; Patterns](https://brendanjameslynskey.github.io/MCP_05_Ecosystem_and_Patterns/) | live | Every host that speaks MCP, the reference servers, the MCP Registry, the four canonical server-design patterns, distribution (uvx/npx/Docker). |

## Where this fits

Part of the [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs) &mdash; an index of presentation series for AI/LLM engineers.
