# Contributing

Agency OS is open source and contributions are welcome.

## What We're Looking For

**New agent files for different industries.** If you run a dev shop, marketing agency, consulting firm, content studio, or any other service business and you've adapted this framework, share your agents back.

**Better "Talks To" configurations.** If you've found information flows between agents that work better than what's documented here, open a PR.

**Edge cases and new principles.** If you deployed an agent and discovered a scenario its principles didn't cover, add the principle and explain why.

**Integration guides.** If you got these agents running on a specific platform (Slack bots, API orchestration, custom UIs), write up how you did it.

**Performance stories.** Before/after data on what changed when you deployed agents. What worked. What didn't. What you'd do differently.

## How to Contribute

1. Fork the repo
2. Create a branch for your changes
3. Follow the agent file anatomy (Identity, Soul, Principles, Guardrails, Inputs, Outputs, Talks To)
4. Open a PR with a clear description of what you changed and why

## Agent File Standards

Every agent file should:

- Follow the same structure as existing agents
- Have a clear, one-sentence role definition
- Include a "What You Are Not" section in the Soul
- Have principles written as concrete instructions for real scenarios (not abstract values)
- Include guardrails that are actual hard limits
- Map its "Talks To" connections honestly

## What We Won't Merge

- Agents without guardrails
- Generic personality descriptions ("professional and friendly" is not a soul)
- Agents that duplicate existing functionality without clear improvement
- Changes to shared-soul.md without strong justification

## Questions

Open an issue. Keep it specific.
