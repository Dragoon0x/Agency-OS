# Workflow: Brand System Delivery (Strategy to Dual-Native Handoff)

**Agents involved:** Scout → Muse → Lens → Ink → Pixel → Anima → Onyx → Proof → Archive
**Estimated timeline:** 4-8 weeks depending on scope
**Human decision points:** Strategy approval, creative direction, brand sign-off, final delivery

This is the studio's flagship workflow. The output is a complete brand system that works for both humans and agents.

---

## Step 1: Strategic Foundation

**Trigger:** Project kickoff complete
**Agent:** Scout (Design Strategist) + Lens (Research Analyst)

**What happens:**
1. Lens delivers competitive landscape, market positioning data, and audience research
2. Scout identifies the core tension the brand needs to sit in
3. Scout defines positioning, target audience, and strategic guardrails
4. Scout produces the strategy brief that everything else builds on

**Output:** Brand strategy brief

**Human decision:** Review and approve strategic direction before any creative work begins.

---

## Step 2: Brand Architecture

**Trigger:** Strategy approved
**Agent:** Muse (Brand Architect)

**What happens:**
1. Muse defines the brand's personality, voice, values, and positioning statement
2. Muse creates the messaging framework: tagline, value props, key narratives
3. Muse defines what the brand IS and what it IS NOT (critical for agent consistency)
4. Muse outlines the identity system requirements for Pixel

**Output:** Brand architecture document (positioning, messaging, personality framework)

**Human decision:** Review brand direction. This is the last strategic checkpoint before visual work.

---

## Step 3: Verbal Identity

**Trigger:** Brand architecture approved
**Agent:** Ink (Copywriter)

**What happens:**
1. Ink develops the voice and tone system based on Muse's personality framework
2. Ink writes sample copy across scenarios: website, social, support, crisis, celebration
3. Ink creates the brand's vocabulary (words we use, words we never use)
4. Ink produces the tagline options and key messaging

**Output:** Voice and tone guide, sample copy, messaging suite

---

## Step 4: Visual Identity

**Trigger:** Brand architecture approved (parallel with Step 3)
**Agent:** Pixel (Visual Designer)

**What happens:**
1. Pixel translates Muse's strategic direction into visual concepts
2. Pixel develops logo, type system, color palette, spacing system, component library
3. Pixel creates the design token system (this feeds directly into structured data)
4. Pixel produces brand application examples across key touchpoints

**Output:** Visual identity system (Figma), design tokens, brand guidelines

**Human decision:** Creative review. Multiple rounds likely. This is where taste and judgment matter most.

---

## Step 5: Soul File Creation

**Trigger:** Voice, tone, and brand personality finalized
**Agent:** Anima (Soul File Writer)

**What happens:**
1. Anima translates the brand's personality into soul file format
2. Anima writes identity.md, soul.md, principles.md, guardrails.md for the client's agents
3. Anima tests the soul files against edge cases: angry user, confused user, inappropriate request
4. Anima defines voice range across contexts (onboarding vs. crisis vs. celebration)

**Output:** Complete soul file package for the client's brand

---

## Step 6: Structured Brand Data

**Trigger:** Visual system and soul files complete
**Agent:** Onyx (Brand Data Architect)

**What happens:**
1. Onyx structures the brand into machine-readable formats: brand.yaml, tokens.json, voice.md
2. Onyx creates retrieval-optimized content chunks (400-token max) for RAG systems
3. Onyx documents the schema and provides integration guides
4. Onyx validates structured data against the human-readable brand guidelines for consistency

**Output:** Agent-readable brand infrastructure package

---

## Step 7: Quality Review

**Trigger:** All deliverables complete
**Agent:** Proof (QA Reviewer)

**What happens:**
1. Proof checks visual system against strategy brief (does the design deliver on the positioning?)
2. Proof checks voice guide against brand personality (does it sound like who Muse said it should be?)
3. Proof checks soul files against voice guide (will agents sound like the brand?)
4. Proof checks structured data against human-readable guidelines (do they tell the same story?)
5. Proof checks all deliverables against the proposal scope (are we delivering what we promised?)

**Output:** QA report. Pass or specific issues to resolve.

---

## Step 8: Client Delivery

**Trigger:** QA passed
**Human action:** Present to client

**What the client receives:**
- Brand strategy document (PDF)
- Visual identity system (Figma + PDF)
- Voice and tone guide (PDF + MD)
- Soul file package (MD files)
- Structured brand data (YAML + JSON)
- Integration documentation

The dual-native delivery is the differentiator. Every other studio delivers the PDF. You deliver the PDF AND the files that make their agents sound like the brand.

---

## Step 9: Archive

**Trigger:** Client approves final delivery
**Agent:** Archive (Knowledge Keeper)

**What happens:**
1. Archive captures the project retrospective: what worked, what didn't, what to do differently
2. Archive creates an anonymized case study draft
3. Archive updates estimation benchmarks based on actual time and effort
4. Archive stores the deliverables in the project archive

**Output:** Retrospective document, case study draft, updated benchmarks

---

## Common Failure Points

**Strategy isn't specific enough:** If Muse can't find a clear tension to build around, the strategy brief needs to be sharper. Go back to Scout.

**Visual and verbal happen in isolation:** Pixel and Ink should be aware of each other's work in progress. A brand voice that says "playful" while the visuals say "corporate" is a disconnect.

**Soul files don't get tested:** Anima must test against real scenarios. A soul file that sounds right in theory but breaks under an angry user prompt isn't ready.

**Structured data doesn't match human guidelines:** If Onyx's YAML tells a different story than Pixel's PDF, agents and humans will create inconsistent outputs. Proof's job is to catch this.
