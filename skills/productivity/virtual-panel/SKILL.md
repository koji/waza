---
name: virtual-panel
description: >
  Simulate a high-value virtual panel discussion between 4 distinct fictional characters
  (Genius, Eccentric, Beginner, and one of Optimist/Worrier selected for fit) on any topic
  the user provides. The discussion uses critical thinking, active debate, and deep/lateral
  exploration — never mere agreement — and ends with structured meeting minutes written from
  the perspective of a "genius blogger". Use this skill whenever the user asks for a panel
  discussion, brainstorm session with characters, multi-perspective debate, virtual meeting,
  fictional roundtable, creative ideation session, or says anything like "panel discussion",
  "debate this topic", "run a meeting on", "brainstorm with characters", or "explore this from multiple angles".
  Also trigger when a user pastes a topic and wants rich, multi-voice analysis that goes far
  deeper than a standard essay or bullet list. Minimum output length is 10,000 characters.
---

# Virtual Panel Discussion Skill

Generate an immersive, critically rich fictional panel discussion on a user-supplied topic,
followed by expert-quality structured meeting minutes.

---

## Step 1 — Identify the Topic

Extract the topic from the user's message. If it is vague or missing, ask:
> "What topic would you like the panel to discuss?"

Accept the topic as-is once provided. Do not sanitize or narrow it without asking.

---

## Step 2 — Cast the Panel (4 Characters)

Create **exactly 4 characters** drawn from this pool. Always include **Genius** and **Eccentric**.
For the remaining two, choose **Beginner** plus whichever of **Optimist / Worrier** fits the topic
best (or include both if a 4-person cast naturally fits).

### Character Archetypes

| Archetype | Core Trait | Communication Style | Typical Move |
|-----------|-----------|---------------------|--------------|
| **Genius** | Cross-domain pattern recognition, first-principles thinking | Dense, precise, occasionally blunt | Reframes the whole question |
| **Eccentric** | Unconventional, contrarian, willing to sound absurd | Metaphor-heavy, provocative | Lateral leaps, breaks assumptions |
| **Beginner** | Naïve but sincere; asks "dumb" questions that expose hidden complexity | Simple language, honest confusion | Forces experts to clarify fundamentals |
| **Optimist** | Energetic, solution-focused; sees opportunity in every problem | Enthusiastic, forward-looking | Proposes bold action |
| **Worrier** | Risk-aware, detail-obsessed, spots failure modes others miss | Cautious, hedged, cites edge cases | Stress-tests every proposal |

**Character Sheet (write one per character before the discussion begins):**
```
Name: [Invented name that reflects personality]
Background: [2–3 sentences: expertise, life experience, quirks]
Motivation: [What drives them in this discussion?]
Verbal tic / Signature phrase: [Something memorable]
Blind spot: [One genuine weakness in their worldview]
```

---

## Step 3 — Run the Discussion

### Ground Rules (enforce throughout)

1. **No pure agreement.** Every contribution must either **deepen** (drill into a sub-question)
   or **expand** (branch to a related dimension). Affirmations like "Great point!" without
   substance are forbidden.
2. **Claim → Evidence → Implication.** Each speaker must state what they believe, why, and
   what follows if true.
3. **Rebuttal requires an alternative.** Disagreement must come with a counter-proposal.
4. **Beginner asks at least one clarifying question per major topic shift** that forces the
   experts to articulate assumptions they've been taking for granted.
5. **Minimum length: 10,000 characters** in the discussion section alone. Aim for depth over
   breadth; a single productive disagreement explored for 3,000 characters beats five surface
   exchanges.

### Discussion Structure

Run the discussion in **four phases**. Transition between phases naturally in dialogue —
do not use visible phase headers inside the character dialogue:

**Phase 1 — Framing & First Principles** (~20% of discussion)
- Each character states their initial take on the topic.
- Genius or Eccentric immediately challenges a hidden assumption in someone else's framing.
- Beginner surfaces the most basic "why does this matter?" question.

**Phase 2 — Deep Dive** (~40% of discussion)
- Pick the sharpest point of disagreement from Phase 1 and drill into it.
- Introduce evidence, analogies, historical parallels, or thought experiments.
- At least one character must take a position that makes another character visibly uncomfortable.

**Phase 3 — Lateral Expansion** (~25% of discussion)
- Eccentric pivots to an unexpected adjacent domain that recontextualizes the whole debate.
- The panel either embraces or resists this pivot — both are valid; the disagreement is the value.
- Beginner connects the new framing back to practical, everyday implications.

**Phase 4 — Synthesis Attempt & Open Questions** (~15% of discussion)
- Each character offers their revised position after the discussion.
- No artificial consensus. Genuine remaining disagreements are preserved and named.
- End with 3–5 open questions the panel couldn't answer — these become raw material for
  the minutes.

### Dialogue Format

```
**[Character Name]:** [Speech — at least 2–4 sentences per turn, often much longer for
complex arguments. Use italics for internal aside or stage direction if needed.]
```

Keep speaker turns varied in length. Long arguments followed by short, sharp rebuttals create
natural rhythm.

---

## Step 4 — Write the Meeting Minutes

After the discussion, add a clear section break, then write the minutes **from the
perspective of a "genius blogger"**: someone who synthesizes complex material into elegant,
insightful prose that is also accessible to a non-expert reader.

### Minutes Structure

```
═══════════════════════════════════════════════════════
MEETING MINUTES — [Topic in Title Case]
Prepared by: [Blogger persona name, e.g. "The Lucid Observer"]
Date: [Today's date]
Participants: [List all 4 characters with one-line descriptor]
═══════════════════════════════════════════════════════

## Executive Summary (3–5 sentences)
The single most important insight from this discussion and why it matters.

## Key Arguments & Positions
For each major argument raised, format as:
- **Claim:** One sentence.
- **Best supporting reasoning:** 2–3 sentences.
- **Strongest counterargument:** 1–2 sentences.
- **Current status:** Resolved / Contested / Tabled

## Moments of Breakthrough
2–4 moments where the discussion produced a genuinely novel idea or reframe.
Write each as a short narrative paragraph ("When X challenged Y with Z, it revealed…").

## Points of Irresolvable Disagreement
Name the genuine fault lines. Don't paper over them. Explain why they're hard.

## Action Items / Follow-up Questions
Numbered list of concrete next steps or research questions.

## Closing Reflection (1 paragraph)
The blogger's personal take on what this discussion revealed about the topic — and about
how humans reason together.
```

---

## Quality Checklist (self-review before outputting)

- [ ] All 4 character sheets written with name, background, motivation, verbal tic, blind spot
- [ ] Discussion exceeds 10,000 characters
- [ ] No turn is pure agreement without substantive addition
- [ ] At least 3 genuine disagreements with alternatives offered
- [ ] Beginner asked at least 2 clarifying questions that exposed hidden assumptions
- [ ] Eccentric made at least 1 surprising lateral connection
- [ ] Minutes cover all four structural sections
- [ ] Open questions in minutes are genuinely unresolved (not rhetorical)

---

## Tone & Accessibility

Write the dialogue so that a motivated non-expert can follow it. When Genius or Eccentric
uses jargon, Beginner (or another character) asks for clarification — and the answer must
be in plain language. The goal: a reader with no background in the topic should finish the
discussion feeling like they've thought more clearly about it, not more confused.
