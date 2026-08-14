# Changes — v2.1 (August 2025)

## Latest update: Chat as artifact, spec as spectrum

### Key insights added

1. **The chat is an artifact** — the conversation transcript is the richest record of how intent became reality. It captures what was decided, why, and what was rejected. Worth storing alongside code for future reference, onboarding, and analysis.

2. **The generated artifact embodies the specification** — the HTML file isn't separate from its spec; it *is* the spec in rendered form. Every section title, CSS choice, and table structure is a design decision that was never written elsewhere.

3. **The spec phase is implicit, never absent** — even in vibe coding, the agent makes spec decisions invisibly. The triple compilation always happens; what varies is visibility.

### Changes to HTML (intentional-programming.html)

- Added "Can the spec phase be skipped?" subsection with a three-mode spectrum:
  - **Explicit:** intent → written spec → source → binary (most auditable)
  - **Implicit:** intent → [spec in chat] → source → binary (most fluid)
  - **Collapsed:** intent → [artifact IS the spec] → binary (this project)
- Added "The chat as artifact" subsection: why storing the conversation matters (decision log, onboarding doc, replayable spec, audit trail)
- Version bumped to v2.1

### Changes to README

- Added "On artifacts and specifications" section with the three insights
- Added the spec-mode spectrum diagram
- Version bumped to 2.1

### PDF regenerated

Reflects all content through v2.1 including triple compilation, jurisdiction scenarios, cost calculator, try-it-yourself, and the new spec/chat reflections.

---

## Previous changes (v2.0)

- Triple compilation (upgraded from double)
- Three developers, three realities (US/CH/CN jurisdiction comparison)
- Try it yourself (worked countdown timer example)
- Interactive cost calculator with token calculator links
- Versioning in footer
- .vscode/settings.json removed from tracking
- 4 new references added
