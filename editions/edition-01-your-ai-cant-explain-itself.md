# Edition #01 — Your AI Can't Explain Itself. Your Pipeline Is Why.

> Published 2026-07-29 · [Read on LinkedIn](https://www.linkedin.com/pulse/your-ai-cant-explain-itself-pipeline-why-shashwat-saxena-qdepc/) · [Subscribe](https://www.linkedin.com/newsletters/7488207829871304704/)

## TL;DR

- The **EU AI Act's transparency rules** are now enforceable — fines up to €15M or 3% of global turnover, and regulators can demand model access or recall AI systems.
- You cannot explain a model's decision if you can't trace the data that shaped it. **Explainability starts in the pipeline, not the model.**
- 2026 research is converging on the same conclusion: provenance, lineage, and workflow replay are becoming the *minimum* enterprise standard.

## The three research shifts (July 2026)

1. **Model-level → system-level explainability.** The question is no longer "do we have explainability?" but "which transparency capability do we need for which risk?" For LLMs in workflows: which documents and retrieved passages drove the answer. For agents: why that tool, that memory, that plan.

2. **Provenance as minimum enterprise standard.** Citation grounding, retrieval perturbation testing, tool-call lineage, memory provenance, workflow replay — all *data engineering* problems. Lineage is the foundation of trust.

3. **Mechanistic interpretability is scaling.** Automated circuit discovery now reaches ~100B-parameter models with tractable compute — but only helps teams whose data infrastructure supports the tracing.

## The practitioner's checklist

- [ ] **Lineage first** — column-level lineage from source to feature store. When model reasoning shifts, locate the broken upstream table same-day, no labels needed.
- [ ] **Provenance for RAG** — every generated answer carries its retrieval trail. (In production this cut manual review by 40% and made every output auditable.)
- [ ] **Watch silent imputation** — a silent `fillna(0)` in the silver layer hides broken data from the model *and* from your explanations.

## Sources

- [From Explainability to Control: The 2026 Executive View of AI Interpretability (UST Insights)](https://www.ust.com/en/insights/ai-interpretability-explainability-2026-executive-view)
- [LLMs for Explainable AI: A Comprehensive Survey (arXiv)](https://arxiv.org/pdf/2504.00125)
- [Explainability of Large Language Models: Opportunities and Challenges toward Generating Trustworthy Explanations (arXiv)](https://arxiv.org/pdf/2510.17256)
- [LLM Research Papers: The 2026 List — Sebastian Raschka](https://magazine.sebastianraschka.com/p/llm-research-papers-2026-part1)
