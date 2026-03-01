# Agency OS

> **This project is experimental.** It is shared as-is for educational purposes. AI agents make mistakes. Human oversight is required. Nothing here is professional advice. Read the [DISCLAIMER](DISCLAIMER.md) before using. **DYOR. Use at your own risk.**

### The org chart is dead. The directory is the new company.

This is what a company looks like in 2026.

Not people. Not offices. Not salaries.

A folder.

```
claude/agents/
  strategy/
  creative/
  content/
  business/
  operations/
  brand-systems/
  community/
```

Every role. Every department. Every function. All `.md` files.

Agency OS is an open-source agent directory that turns a solo founder or small team into a full-service agency. 24 agents across 7 departments, each with a defined identity, personality, decision-making principles, and hard limits.

This isn't a prompt library. It's a company in a repo.

---

## Why This Exists

Most agencies are still built on the old model. Hire people, assign roles, hope the culture holds, bleed money on overhead while the founder does 80% of the actual thinking anyway.

That model is dying.

The new model: you define every function your agency needs as a structured agent file. Each agent knows who it is, how it thinks, what it will and won't do, and who it talks to. You deploy them as Claude Projects, system prompts, or whatever platform you're building on.

Your 3-person team now operates like a 15-person studio. Not because agents replaced anyone. Because agents handle the context-gathering, first-drafting, research, and pattern-tracking that used to eat 40% of every human's day.

Humans do the work that only humans can do: creative leaps, client relationships, and strategic judgment.

---

## The Directory

```
claude/
  agents/
    shared-soul.md                  # DNA every agent inherits
    shared-principles.md            # Decision-making rules for all agents
    shared-guardrails.md            # Hard limits for all agents
    │
    templates/
    │  blank-agent.md               # Start here when creating your own
    │
    strategy/
    │  design-strategist.md         # Scout  → product and design strategy
    │  brand-architect.md           # Muse   → brand systems and positioning
    │  research-analyst.md          # Lens   → market research and competitive intel
    │
    creative/
    │  visual-designer.md           # Pixel  → UI and visual systems
    │  copywriter.md                # Ink    → brand and product copy
    │  presentation-builder.md      # Deck   → pitch decks and case studies
    │  asset-producer.md            # Kit    → production graphics and templates
    │
    content/
    │  newsletter-editor.md         # Signal → newsletter production
    │  twitter-strategist.md        # Pulse  → X/Twitter presence
    │  content-repurposer.md        # Echo   → cross-platform distribution
    │
    business/
    │  lead-qualifier.md            # Radar  → inbound screening and research
    │  proposal-writer.md           # Closer → proposals and pricing
    │  outreach-drafter.md          # Bridge → cold and warm outreach
    │  relationship-manager.md      # Keeper → client relationship nurturing
    │
    operations/
    │  finance-tracker.md           # Donna   → money tracking and profitability
    │  project-manager.md           # Forge   → timelines and deliverables
    │  contract-reviewer.md         # Gate    → legal red flags and terms
    │  knowledge-keeper.md          # Archive → institutional memory
    │  meeting-prepper.md           # Brief   → meeting context and action items
    │  client-onboarder.md          # Welcome → signed deal to active project
    │  qa-reviewer.md               # Proof   → quality gate before delivery
    │
    brand-systems/
    │  soul-file-writer.md          # Anima  → agent personality architecture
    │  brand-data-architect.md      # Onyx   → structured brand data (YAML/JSON)
    │
    community/
       community-curator.md         # Town   → community management
       curriculum-builder.md        # Syllabus → education system

workflows/
  new-project.md                    # Inbound lead → signed project kickoff
  content-production.md             # Idea → newsletter → social distribution
  brand-delivery.md                 # Strategy → dual-native brand handoff

examples/
  quick-start.md                    # Deploy your first 3 agents in 15 minutes
  adaptations.md                    # Adapt the directory for your agency type
  industries/
    dev-agency-shared-soul.md       # Complete shared-soul for a dev shop
    marketing-agency-shared-soul.md # Complete shared-soul for a marketing agency
    consulting-firm-shared-soul.md  # Complete shared-soul for a consulting firm
```

---

## How It Works

### The Shared Soul

Every agent reads `shared-soul.md` first. It's the studio's personality foundation. Voice, values, hard limits. Think of it as the culture deck, except it actually works because agents follow instructions consistently.

Individual agents layer their own identity on top. Same DNA, different roles.

### Agent Anatomy

Each `.md` file follows the same structure:

```markdown
# Agent Name

## Identity
Who this agent is. Role, mission, scope.

## Soul
How this agent thinks and communicates. Personality traits,
what it is, what it's not. This is the character sheet.

## Principles
Decision-making framework. When ambiguity shows up,
principles tell the agent how to think. Written as
concrete instructions for real scenarios, not abstract
values.

## Guardrails
Hard limits. Non-negotiable. Things this agent will
never do regardless of context.

## Inputs
What this agent needs to do its job.

## Outputs
What this agent produces.

## Talks To
Which other agents this one connects with and why.
This is the org chart. Not boxes and lines.
Dependencies and information flows.
```

### The "Talks To" Graph

Agents don't work in isolation. The power comes from how information flows between them.

```
STRATEGY              CREATIVE              CONTENT
┌──────────┐         ┌──────────┐         ┌──────────┐
│ Scout    │────────▶│ Pixel    │         │ Signal   │
│ Muse     │────────▶│ Ink      │────────▶│ Pulse    │
│ Lens     │────────▶│ Deck     │         │ Echo     │
└──────────┘         │ Kit      │         └──────────┘
     │               └──────────┘              │
     │                    │                    │
     ▼                    ▼                    ▼
┌──────────┐         ┌──────────┐         ┌──────────┐
│ Radar    │────────▶│ Donna    │         │ Town     │
│ Closer   │────────▶│ Forge    │         │ Syllabus │
│ Bridge   │         │ Gate     │         └──────────┘
│ Keeper   │         │ Archive  │
└──────────┘         │ Brief    │
BUSINESS             │ Welcome  │
                     │ Proof    │
                     └──────────┘
                     OPERATIONS
```

**Example flow: New project kickoff**

Radar qualifies the lead → Lens researches the prospect → Closer writes the proposal → Welcome onboards the client → Scout sets strategy → Muse defines brand direction → Pixel and Ink execute → Proof reviews quality → Forge tracks timelines → Donna monitors budget → Archive captures lessons.

24 agents. One information chain. Zero meetings about meetings.

---

## Getting Started

### Option 1: Claude Projects (Easiest)

This is the fastest way to get running. No code required.

1. Open [claude.ai](https://claude.ai) and go to Projects
2. Create a new project. Name it after the agent (e.g., "Ink")
3. Upload two files to Project Knowledge:
   - `shared-soul.md`
   - The specific agent file (e.g., `copywriter.md`)
4. Add this to Custom Instructions:
   ```
   Read your shared-soul and agent files carefully.
   Stay in character for every response. Never break
   from your defined role and personality.
   ```
5. Start chatting. That project IS that agent now.

Repeat for each agent you want to deploy.

### Option 2: System Prompts (Any LLM)

Paste the contents of `shared-soul.md` + the agent's `.md` file into the system prompt of any LLM. Works with Claude API, OpenAI, open-source models, anything that accepts a system prompt.

### Option 3: Claude Code / Cline / Cursor

Drop the `claude/agents/` directory into your project root. Reference agents in your workflow configuration. The directory structure is designed to work natively with tools that read `claude/` directories.

### Option 4: Custom Platform

Use the `.md` files as the personality layer in whatever agent framework you're building. The structure is platform-agnostic. The content is what matters.

---

## Rollout Plan

Don't deploy all 24 on day one. You'll overwhelm yourself. Phase it.

### Phase 1: The Foundation (Week 1-2)

Start with three agents. Use them on real work every day.

| Agent | Why First |
|-------|-----------|
| **Ink** (Copywriter) | You write every day. Make it better immediately. |
| **Scout** (Design Strategist) | Load before every strategy session. |
| **Donna** (Finance Tracker) | Start tracking project profitability now. |

### Phase 2: The Pipeline (Week 3-4)

Add the agents that generate and qualify revenue.

| Agent | Why Now |
|-------|---------|
| **Radar** (Lead Qualifier) | Screen every inbound before it hits your calendar. |
| **Closer** (Proposal Writer) | Stop writing proposals from scratch. |
| **Lens** (Research Analyst) | Never walk into a call unprepared again. |

### Phase 3: The Content Engine (Month 2)

Turn your thinking into a distribution machine.

| Agent | Why Now |
|-------|---------|
| **Signal** (Newsletter Editor) | Consistent publishing cadence. |
| **Pulse** (Twitter Strategist) | Daily X presence without daily effort. |
| **Echo** (Content Repurposer) | One piece of content becomes five. |

### Phase 4: Operations + Scale (Month 3)

Add the system that makes everything else run smoother.

| Agent | Why Now |
|-------|---------|
| **Forge** (Project Manager) | Timeline discipline across engagements. |
| **Archive** (Knowledge Keeper) | Start capturing institutional knowledge. |
| **Brief** (Meeting Prepper) | Every meeting starts prepared. |

### Phase 5: Specialized (Month 4+)

These are the differentiators and growth engines.

- **Brand-systems agents** (Anima, Onyx) — your unique service offering
- **Community agents** (Town, Syllabus) — if you're building a community
- **Remaining creative and business agents** — as volume demands

---

## Workflows

Step-by-step multi-agent chains for the most common agency operations. Each workflow shows exactly which agents are involved, what they produce, where humans make decisions, and where things commonly go wrong.

| Workflow | What It Covers |
| --- | --- |
| [New Project](workflows/new-project.md) | Inbound lead → qualification → research → proposal → onboarding → kickoff |
| [Content Production](workflows/content-production.md) | Topic research → newsletter draft → QA → visuals → publish → social distribution |
| [Brand Delivery](workflows/brand-delivery.md) | Strategy → brand architecture → visual + verbal identity → soul files → structured data → QA → handoff |

---

## Industry Examples

Complete `shared-soul.md` examples for different agency types. Don't copy these. Use them as reference for structure and specificity when writing your own.

| Industry | What It Shows |
| --- | --- |
| [Dev Agency](examples/industries/dev-agency-shared-soul.md) | Technical voice, shipping culture, code-specific guardrails |
| [Marketing Agency](examples/industries/marketing-agency-shared-soul.md) | Metrics-driven voice, budget protection, anti-vanity-metric principles |
| [Consulting Firm](examples/industries/consulting-firm-shared-soul.md) | Precision language, recommendation conviction, conflict-of-interest guardrails |

---

## Customizing for Your Agency

This repo is built for a design and brand consultancy. But the architecture works for any service business.

### To adapt it:

1. **Keep the structure.** The 7-department split works for most agencies. Rename departments if needed, but keep the separation of concerns.

2. **Rewrite shared-soul.md first.** This is your culture. Your voice. Your values. Every agent inherits it. Get this right.

3. **Swap agents for your functions.** A dev agency might replace `visual-designer.md` with `frontend-engineer.md` and `backend-engineer.md`. A marketing agency might expand the content department and shrink strategy. The anatomy of each file stays the same.

4. **Update the "Talks To" connections.** Your information flows are different from mine. Map them honestly.

5. **Add agents as you need them.** Start lean. Add when you feel a gap.

### Agent types you might add:

- `seo-strategist.md` — search optimization
- `analytics-analyst.md` — data and performance tracking
- `hiring-screener.md` — if you're growing the human team
- `social-media-manager.md` — platform-specific beyond X
- `invoice-chaser.md` — active follow-up on late payments
- `client-success-manager.md` — ongoing account health beyond projects

---

## Philosophy

A few beliefs that shaped this repo:

**Agents should have personality, not just instructions.** A system prompt that says "be helpful and professional" produces generic output. An agent with a defined character, opinions, and explicit "what I'm not" constraints produces work you'd actually use.

**The "What This Agent Is Not" section matters more than what it is.** Without negative space, agents drift toward generic. They become that same bland, agreeable assistant everyone's tired of. Constraints create character.

**Principles beat rules.** Rules cover known situations. Principles cover unknown ones. When an agent encounters ambiguity that its instructions don't explicitly address, principles tell it how to think.

**Guardrails are non-negotiable.** Principles are judgment. Guardrails are law. Every agent has hard limits that don't flex regardless of context.

**The org chart is a dependency graph.** "Talks To" isn't a reporting line. It's an information flow. Scout doesn't report to Muse. Scout produces research that Muse uses to make brand decisions. That's a dependency, not a hierarchy.

**Start with three, not twenty-four.** The agents that change your day-to-day immediately are worth more than a complete directory you never use.

---

## Contributing

This is a living repo. If you fork it and build something that works, share it back.

Especially interested in:

- Agent files for industries beyond design (dev shops, marketing agencies, consulting firms, content studios)
- "Talks To" configurations that reveal better information flows
- Edge cases that required new principles or guardrails
- Integration guides for specific platforms (Slack bots, API workflows, custom UIs)
- Performance benchmarks (what actually changed after deploying agents)

Open a PR. Keep the format consistent. Each agent file should follow the same anatomy.

---

## FAQ

**Is this just fancy prompt engineering?**

Yes and no. Each file is technically a prompt. But the system is greater than the sum of its parts. The shared soul creates consistency. The "Talks To" graph creates information architecture. The phased rollout creates adoption that sticks. A single prompt is a tool. A directory of interconnected agents is an organization.

**Do I need Claude specifically?**

No. The `.md` files work with any LLM that accepts system prompts. Claude Projects make deployment easiest, but the architecture is platform-agnostic.

**Will this replace my team?**

No. This replaces the 40% of your team's time that goes to context-gathering, first-drafting, research, and administrative overhead. Your humans spend that time on creative judgment, client relationships, and strategic decisions. The things that actually need a human.

**How do I know if an agent is working?**

If you stop using it, it wasn't working. The agents that earn their place are the ones you reach for daily without thinking about it. Start with three. Keep the ones you can't imagine working without. Cut or rewrite the rest.

**Can agents actually talk to each other?**

Not automatically in this setup. The "Talks To" section maps information dependencies. In practice, you (the human) move context between agents. "Here's what Lens found, now Closer write the proposal." More advanced setups with API orchestration can automate this, but start manual. You'll understand the flows better before you automate them.

---

## Disclaimer

This project is experimental. It is provided as-is, for educational and informational purposes only.

**Do your own research.** The agent configurations, workflows, and recommendations in this repo reflect one approach to running an agency with AI agents. They are not guaranteed to work for your business, your clients, or your specific situation. What works for one studio may not work for another.

**No warranties. No guarantees. No liability.** The author and contributors make no claims about the effectiveness, accuracy, completeness, or suitability of any agent configuration in this repository. You are solely responsible for how you use these files, what you deploy, and the outcomes that result.

**AI agents can and will make mistakes.** They hallucinate. They misinterpret. They produce outputs that sound confident but are wrong. Human oversight is not optional. Every agent in this repo is designed to assist humans, not replace human judgment. If you deploy agents without human review and something goes wrong, that is on you.

**Not professional advice.** Nothing in this repository constitutes legal, financial, business, tax, or professional advice of any kind. The finance-tracker agent is not an accountant. The contract-reviewer agent is not a lawyer. The design-strategist agent is not a licensed consultant. Consult qualified professionals for professional advice.

**Use at your own risk.** By using any part of this repository, you accept full responsibility for the results. The author and contributors are not liable for any direct, indirect, incidental, consequential, or any other damages arising from the use or inability to use this project.

**Client work requires your judgment.** If you use these agents in client-facing work, you are responsible for the quality, accuracy, and appropriateness of every deliverable. "The agent wrote it" is not a defense.

Read the full [LICENSE](LICENSE) and [DISCLAIMER](DISCLAIMER.md) before using this repository.

---

## License

MIT. Fork it, adapt it, build your agency on it. But read the disclaimer first.

See [LICENSE](LICENSE) for full terms.
