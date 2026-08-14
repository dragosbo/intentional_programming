# Changes — August 2025

## New sections added to intentional-programming.html

### 1. "Where the work runs — and what it costs" (`#infra`)

Covers the three execution loci of intentional programming:
- **Local** — models on your machine (Ollama, LM Studio), zero cost per token, limited capability
- **Dedicated server** — self-hosted GPU, predictable costs, data stays in your perimeter
- **Cloud API** — frontier models, pay-per-token, maximum capability

Includes:
- Cost comparison table across all three loci (hardware, per-token, subscription, electricity, rate limits)
- Note on the 1,200× cost decline in LLM inference (2020–2025)
- Jurisdiction & sovereignty callout: EU AI Act, data residency laws, sanctions, subscription tier limitations
- Guidance on when local-only is viable vs. when cloud access is needed

### 2. "The double compilation" (`#compilation`)

Frames intentional programming as a two-stage compilation pipeline:
- **Stage 1** (probabilistic, iterative): intent → source code via reasoning agent
- **Stage 2** (deterministic, one-shot): source code → executable via traditional compiler

Includes:
- Equation-style visualization of the full pipeline
- Comparison table of properties (determinism, iteration, cost model, failure modes)
- Architect/construction analogy
- Discussion of why source code remains the intermediate representation
- Note on the two-pass compiler pattern resurfacing in AI code generation

### 3. Expanded Sources section

Added 6 new references:
- o-mega.ai — LLM inference cost trends
- SitePoint — local vs cloud AI coding performance
- InfoWorld — two-pass compiler in AI code generation
- SelfLabs — the intent → executable pipeline
- EU AI Act — regulatory framework
- Prediction Guard — self-hosted vs cloud deployment guide

### 4. Navigation updated

Added "Infrastructure" and "Double Compilation" links to the sticky nav bar.

## Research basis

Content informed by web research into:
- LLM inference pricing (2020–2026 cost curves)
- Local vs cloud deployment trade-offs (privacy, latency, cost, capability)
- EU AI Act and data sovereignty regulations
- Two-pass compiler patterns applied to AI code generation
- The "intent → source → binary" compilation pipeline concept
