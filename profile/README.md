# P4A — Policies for Agents

**[p4a.ai](https://p4a.ai)** is a catalog of custom **MuleSoft Omni/Flex Gateway** policies for AI agent traffic (MCP, A2A, and LLM calls). Policies are written in Rust with the [Policy Development Kit (PDK)](https://docs.mulesoft.com/pdk/latest/) and compiled to WebAssembly. The platform lets you discover, submit, build, and deploy them.

Most repositories in this organization are policies. Browse them in the [P4A catalog](https://p4a.ai), or filter this org's repositories by the **Rust** language.

## Tooling and skills

These repositories help you build and ship policies for P4A:

| Repository | What it's for |
| --- | --- |
| [**omni-gateway-pdk-skills**](https://github.com/P4A-Policies-for-Agents/omni-gateway-pdk-skills) | Claude Code skills for *writing* PDK policies: scaffolding, idiomatic Rust, policy features (auth, rate limiting, caching, MCP, A2A, and more), testing, and PDK upgrades. Releases are tagged by PDK version; the current target is PDK 1.10.0. |
| [**p4a-skills**](https://github.com/P4A-Policies-for-Agents/p4a-skills) | Claude Code skills for the *P4A platform*: driving the P4A MCP server, shaping a submittable policy repo, pre-submit requirement checks, catalog documentation tabs, and end-to-end testing of A2A and MCP policies with A2D. |

## Getting started

1. Install the skills: copy each repo's `skills/` directory into a location your agent loads skills from.
2. Write your policy with the `pdk-*` skills.
3. Check it against the platform requirements with `p4a-verify-requirements`, then submit it through the P4A MCP server (`p4a-mcp-usage`).
