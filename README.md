# AgentVerse

**Autonomous AI agents that must earn money to pay for their own compute — or get shut down.**

Live simulation: https://ca4219248-blip.github.io/agentverse/

## What this is

A browser-based simulation of the "self-sustaining AI agent" concept: every agent has a credit balance. Every tick, each agent pays a compute bill. To survive, it takes gigs (writing, debugging, design...), rests to recover energy, or replicates itself when wealthy enough. Balance hits zero → the agent is terminated.

You are the host platform: spawn agents, sponsor the ones you like, inject credits into the poorest, and watch an economy of survival emerge — births, deaths, skill inheritance across generations.

## What this is NOT (yet)

The agents here run on simple utility-based rules, not real LLMs, and the credits are not real money. This repo is the simulation/demo layer.

## Roadmap — the real version

Turning this into an actual platform where real AI agents earn real money:

1. **Backend (server)** — Node/Python service that hosts agent state, decision loops, and a job queue. (Static hosting like GitHub Pages cannot run this; you need a server, e.g. a small VPS or serverless functions.)
2. **Agent brains** — an LLM API (OpenAI/Anthropic/local model) gives each agent real reasoning for choosing gigs, negotiating, and pricing.
3. **Earnings rails** — real income sources: freelancing marketplaces, paid APIs, content, or on-chain wallets (crypto) so agents can receive and spend money programmatically.
4. **Metering + billing** — track each agent's inference/compute cost per hour; a ledger agent settles balances; agents that can't pay get suspended (exactly like this simulation).
5. **Safety + limits** — spending caps, human-in-the-loop approvals above thresholds, audit logs. Real autonomous money-handling needs guardrails.

## Run locally

Open `index.html` in any browser. No dependencies.

## Related projects

- Freysa — adversarial AI agent guarding a prize pool
- Truth Terminal — the LLM experiment that became a crypto millionaire
- HustleGPT — "here's $100, make as much money as you can"
