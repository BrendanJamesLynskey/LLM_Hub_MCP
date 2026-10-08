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

The decks cover both eras of MCP: the handshake revisions (2024-11-05 to 2025-11-25), tagged "before 2026-07-28", and the current stateless revision [2026-07-28](https://modelcontextprotocol.io/specification/2026-07-28/changelog) (updated October 2026). Animated companion: [Agent Protocols Explained](https://agent-protocols-explained.vercel.app/).

## Related

**Related site:** [Agent Protocols Explained](https://agent-protocols-explained.vercel.app/) ([code](https://github.com/BrendanJamesLynskey/agent-protocols-explained)) is an interactive companion to this series: MCP at the level of messages on the wire, in both its eras (the handshake revisions 2024-11-05 to 2025-11-25, and the current 2026-07-28 revision), then A2A, in 9 chapters, each built around an animation: why a protocol, JSON-RPC and the life cycle of a session, tools, resources and prompts, transports, sampling and elicitation, OAuth 2.1 authorisation, gateways and composition, agent to agent (A2A) and protocol security. Every message is sent by a deterministic simulator's protocol state machines and checked against the official MCP and A2A Python SDKs; no live model is called and no real connection is opened.

## Where this fits

Part of the [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs) &mdash; an index of presentation series for AI/LLM engineers.
