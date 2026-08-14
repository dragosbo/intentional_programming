# Changes — v2.0 (August 2025)

## This session's updates

### 1. README rewrite — reflections on what this project is

- **Document or web app?** The HTML file is both. It started as a static article but now contains interactive widgets (audio player, cost calculator, game). That blurriness is itself a feature of intentional programming — you don't decide the category upfront; you express intent and the artifact becomes what it needs to be.
- **README vs specification:** Added a comparison table showing the different roles (forward-looking spec vs present-tense README), and noted that they blur in a project where the artifact *is* the content.
- Updated the Mermaid diagram to reflect the full iterative workflow through Kiro.
- Added version number (v2.0) to the header.
- Noted that the entire workflow is itself an instance of the triple compilation.

### 2. Triple Compilation (upgraded from "double")

Rewrote the compilation section with three stages:
- **Stage 1:** Intent → Specification (collaborative, exploratory)
- **Stage 2:** Specification → Source Code (generative, constrained by spec)
- **Stage 3:** Source Code → Executable (deterministic, traditional)

Key argument: jumping from intent directly to code skips the most critical artifact — the specification. Making the spec explicit creates an auditable trail of *why* decisions were made.

### 3. Three Developers, Three Realities

Jurisdiction comparison table (US / Switzerland / China):
- US: unrestricted access, budget as main constraint
- Switzerland: full access + FADP compliance, Azure Switzerland North, Swiss-hosted alternatives
- China: Great Firewall blocks Western models; DeepSeek V4 Pro (80.6% SWE-bench) competitive at 1/50th cost; shadow APIs exist but carry legal risk

Insight: "Geography is now a compiler flag."

### 4. Try It Yourself

Worked example: "Build me a countdown timer in Python" traced through all three compilation stages with generated code, implicit spec decisions, and commentary.

### 5. Cost Calculator

Interactive widget with formula: (prompts × tokens × multiplier × price) ÷ 1M = daily cost. Links to 5 token calculators/tokenizers.

### 6. Versioning

Footer now shows: v2.0 · Last updated: August 2025 · Dragos Boros

### 7. Housekeeping

- Removed `.vscode/settings.json` from git tracking
- Added 4 new references (Chinese models, Swiss FDPIC, Asia Society, LLM-as-compiler)
- Nav bar updated with new section links
