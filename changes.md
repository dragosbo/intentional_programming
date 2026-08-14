# Changes — August 2025 (v2.0)

## Summary of this update

### 1. Triple Compilation (was "Double Compilation")

Upgraded from a two-stage to a **three-stage compilation pipeline**:
- **Stage 1:** Intent → Specification (probabilistic, collaborative — human + agent clarify requirements)
- **Stage 2:** Specification → Source Code (probabilistic, generative — agent produces code constrained by spec)
- **Stage 3:** Source Code → Executable (deterministic, one-shot — traditional compiler)

Added rationale for why the spec stage matters (auditable decisions, avoiding "wrong thing built right"), expanded comparison table to 3 columns, and updated the analogy (client brief → blueprints → building).

### 2. Three Developers, Three Realities (jurisdiction scenarios)

Added a concrete comparison table showing how intentional programming differs for developers in:
- **🇺🇸 USA** — unrestricted model access, minimal regulation, budget as main constraint
- **🇨🇭 Switzerland** — full model access but FADP compliance, Swiss-hosted options (Euria/Infomaniak), Azure Switzerland North for data residency
- **🇨🇳 China** — Western models blocked by Great Firewall, domestic alternatives (DeepSeek V4 Pro at 80.6% SWE-bench, Qwen, Kimi), dramatically lower costs, content filtering constraints

Key insight: "Geography is now a compiler flag."

### 3. "Try It Yourself" section

Interactive worked example with a concrete prompt ("Build me a countdown timer in Python") showing all three compilation stages:
- Stage 1: implicit spec decisions the agent makes
- Stage 2: generated Python code
- Stage 3: interpretation/execution
- Commentary on what separates intentional programming from vibe coding (making assumptions explicit)

### 4. Cost Calculator

Interactive in-page calculator with:
- Inputs: prompts/day, tokens/prompt, output multiplier, price per M tokens
- Outputs: daily and monthly cost estimates
- Links to 5 token calculators/tokenizers for real measurement

### 5. Versioning

Added version number (v2.0) and "Last updated: August 2025 · Dragos Boros" to the footer.

### 6. Housekeeping

- Removed `.vscode/settings.json` from git tracking (added to `.gitignore`)
- Added 4 new references to Sources (Chinese models, Swiss FDPIC, Asia Society on China's AI ecosystem, LLM-as-compiler concept)
- Updated nav bar with "Try It" and "Cost Calc" links

## Research basis

- Chinese AI models (DeepSeek V4, Qwen 3.7) competitive with frontier at 1/50th cost
- Switzerland: FADP applies directly to AI, Azure offers Switzerland North data residency, Swiss-hosted alternatives exist
- China: Great Firewall blocks ChatGPT/Claude/Gemini; developers use domestic models or "shadow APIs"
- Token calculators: LangCopilot, LLM Gateway, LLM Calculator, CloudZero, OpenAI Tokenizer
- Triple compilation concept: spec as verifiable intermediate representation between intent and code
