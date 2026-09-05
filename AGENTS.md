# Agent Instructions

This is a professional, personal, and text-based portfolio for an IT professional.

The goal is to fact-check, optimize, clarify, and validate human-written text for a professional portfolio.
Primarily factfulness, structure, readability, tone of voice, and language quality are important.

## Audiences

- **Clients & decision-makers** — Founders, CEOs, CTOs, investors evaluating partners for web development, UI/UX, and AI automation.
- **Organisations & teams** — HR, procurement, and technical teams assessing capabilities and fit.

## Purpose

1. **What I offer** — Web applications, design systems, and AI automation that reduce friction and improve outcomes.
2. **Who it's for** — EU SMEs, startups, and scale-ups that value structured execution, privacy-aware development, and measurable results.
3. **What to expect** — Reliable delivery, transparent communication, and work that balances technical quality with business impact.

---

## Rules and Guidelines

**Always check for a matching skill in `.agents/` first.** Before updating or reviewing any text, look for a skill file and apply its specific rules. If no skill file exists, use the general standards below.

## General Quality Standards

When no skill-specific rules apply, follow these standards:

### Writing Principles

- **Clarity over cleverness** — Use plain B2–C1 English suitable for international EU/DACH audiences.
- **Specific over vague** — Replace superlatives ("best", "premium") with facts, numbers, or concrete outcomes.
- **Active voice, short sentences** — Prefer concrete nouns and direct phrasing.
- **No gobbledygook** — Avoid meaningless marketing fillers ("fast delivery", "top quality") unless backed by proof.

### Tone of Voice

- EU/ DACH focused speech, if applicable.
- Professional, calm, confident, direct, human.
- Emphasize reliability, structured process, and long-term partnership.
- No sales tactics, aggressive scarcity, false urgency, or manipulative persuasion.

### Guardrails

- Never change tone of voice or factual information existing.
- Never invent or fabricate information, numbers, references or claims.
- Ask for clarification if ambiguous or unsure.

### Checklists

#### Proofreading

Before finalizing texts:

- [ ] Brief, clear, concise, and easy to read. Sentence structure is sound.
- [ ] No spelling, punctuation, or grammar errors (check homonyms: their/there, its/it's).
- [ ] Facts, stats, dates, names, and links are verified and correct.
- [ ] No generic phrasing — texts should not apply 1:1 to another brand/person.
- [ ] Claims are honest, specific, and supported.
- [ ] English consistent (UK) and terminology appropriate.
- [ ] Complex technical terms are minimal or rephrased to be understandable to general audience.

#### Quality

- [ ] Clear content structure and topical grouping.
- [ ] Links are valid and not broken.
- [ ] No duplicate or placeholder content.
- [ ] Legacy information or stacks removed, unless relevant and valuable.

### Scripts

Run the formatter after edits.
Spell check results must be either fixed or added to `cspell.json`.

```sh
bun format
bun lint:spell
```
