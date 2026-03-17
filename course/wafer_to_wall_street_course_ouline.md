# From Wafer to Wall Street: Unified Curriculum

### Integrating Semiconductor Mastery, Financial Fluency, and Agentic System Development

> This unified curriculum merges the semiconductor self-training program with financial fluency (CFA-inspired) **and** an agentic system build track. Each unit produces domain artifacts _and_ the skills, workflows, and evals to reproduce them.

---

## 🧭 Program Subtitle

**From Wafer to Wall Street: Understanding Technology, Capital, and Power in the Global Chip Economy**

---

## ⚙️ Three-Track Integration

| Track                       | What Learners Gain                                                                       |
| --------------------------- | ---------------------------------------------------------------------------------------- |
| **Domain Track**            | Semiconductor industry mastery                                                           |
| **Financial Fluency Track** | Capital markets literacy (CFA-inspired)                                                  |
| **Agentic Build Track**     | Skills-as-files, workflow orchestration, artifact-first storage, eval-driven reliability |

**End-of-course statement:**

> "I built a sandboxed agentic research system with skills-as-files, workflow orchestration, artifact-first storage, and eval-driven reliability—then used it to produce semiconductor investment artifacts end-to-end."

---

## 💡 Time Budget (per week)

- Preview: 45–60 min
- Core Learn: 2–3 hrs (semiconductor + financial microdose)
- **Agentic Build Track**: 1.5–2 hrs
- Synthesize: 60–90 min
- Reflect: 20 min

---

# 🧩 Module-by-Module Unified Outline

---

## Module 1: Semiconductor Industry Overview

### Unit 1 — Foundations & Ecosystem

**Semiconductor Focus**: 
- Importance of semiconductors in modern technology
- Mapping the semiconductor supply chain 
- Industry players and their roles (IDMs, foundries, fabless companies) 
- Cyclical nature of semiconductors and market trends
- Basic economics and business models

**Financial Fluency**:

- FRA/Equity: Analyze TSMC/ASML filings (revenue models, utilization)
- Econ: Cyclicality, ASPs, FX exposure (NTD/EUR/USD)
- Ethics: Research objectivity & sourcing standards

**Artifact**: Value-Capture Profit Pool Map (gross margin bands by stage)

**Agentic Build Track**:

- **Skills**: `company_profile_builder`, `profit_pool_map_generator`
- **Data Types**: `company.json`, `segment.json`
- **Workflow**: "seed company universe"
- **Evals**: required-sections + citations presence

**Signals**: WFE billings, foundry utilization, FX trends

**Blog Prompt**: "What I Learned About the Semiconductor Supply Chain"

---

## Module 2: Manufacturing & Supply Chain Analysis

### Unit 2 — Manufacturing Process (FE/BE)

**Semiconductor Focus**:
- Silicon wafer production and prep
- Front-end processes (photolithography, etching, doping)
- Back-end processes (packaging, testing)
- Manufacturing challenges, yield management, and bottlenecks
- Moore’s Law: history, current status, and future projections

**Financial Fluency**:

- FRA: Cost stack of fabs/equipment, capex vs. expense
- QM: Yield math, learning curves, sensitivity analysis

**Artifact**: Toy cost stack for a 5-nm wafer run

**Agentic Build Track**:

- **Skills**: `node_economics_model`
- **Data Types**: `node_assumptions.json`
- **Workflow**: "run model → publish artifact"
- **Evals**: unit sanity + recompute formulas

**Signals**: Wafer pricing, resist/chemical prices, tool lead times

**Blog Prompt**: "Inside the Chipmaking Process: From Sand to Silicon"

---

### Unit 3 — Resilience & Geopolitics

**Semiconductor Focus**:
- Geopolitical chokepoints (Taiwan, South Korea, rare earths)
- Regional strategies (CHIPS Act, EU Chips Act, China’s drive, India/ASEAN)
- Corporate mitigation (China+1, diversification, vertical integration)
- Supply chain transparency challenges  
- Case studies: COVID shortages, Huawei sanctions, US–China tech war

**Financial Fluency**:

- Econ: Trade/tariffs, FX impacts, supply chain finance
- CorpFin: Working capital under stress

**Artifact**: Risk-to-P&L Heat Map (regional exposure, mitigation costs)

**Agentic Build Track**:

- **Skills**: `policy_event_tracker`, `risk_to_pnl_heatmap`
- **Data Types**: `policy_event.json`
- **Workflow**: weekly policy refresh
- **Evals**: event date normalization

**Signals**: Export control changes, subsidy terms, insurance premiums

**Blog Prompt**: "How Geopolitics Shapes the Semiconductor Supply Chain"

---

## Module 3: Innovation & Hardware Evaluation

### Unit 4 — Technology Evaluation Frameworks

**Semiconductor Focus**:
- Metrics and benchmarking methodologies
- Cost analysis and economic viability
- Technology readiness levels (TRLs)
- Risk assessment frameworks
- Intellectual property considerations

**Financial Fluency**:

- CorpFin: WACC, NPV/IRR, cost of capital for new nodes
- Equity: ROIC spread and growth analysis

**Artifact**: Technology Adoption Investment Memo (NPV + TRL)

**Agentic Build Track**:

- **Skills**: `investment_memo_builder`, `assumptions_table_generator`
- **Data Types**: `memo_schema.json`
- **Workflow**: "draft → validate → finalize"
- **Evals**: memo rubric

**Signals**: EUV order mix, co-investment structures

---

### Unit 5 — Hardware Innovation Cycles

**Semiconductor Focus**:
- Innovation S-curves in semiconductors
- Disruptive vs sustaining innovations
- Technology adoption lifecycles
- Case studies (EUV adoption, FinFET transition, Intel Itanium failure)
- Identifying promising technologies early

**Financial Fluency**:

- CorpFin: Real options, operating leverage
- Equity: Cyclical valuation patterns

**Artifact**: Capex Flow Map → ROIC Bridge

**Agentic Build Track**:

- **Skills**: `capex_flow_map`, `roic_bridge`
- **Data Types**: `capex_event.json`
- **Workflow**: ingest capex events
- **Evals**: narrative consistency checks

**Signals**: Fab pricing frameworks, utilization rates

---

## Module 4: Semiconductor Technology Deep Dive

### Unit 6 — Advanced Process Technologies

**Semiconductor Focus**:
- Advanced node scaling (5nm, 3nm, 2nm)
- Alternative scaling (chiplets, 3D stacking)
- New materials (GaN, SiC)
- Advanced lithography (EUV, High-NA EUV)
- Process variation and reliability

**Financial Fluency**:

- FRA: Depreciation impact on margins
- QM: Yield vs time regression, cost per transistor

**Artifact**: Node Economics Model (yield, cost/mm²)

**Agentic Build Track**:

- **Skills**: `yield_regression`, `table_extraction_quality`
- **Data Types**: `table_meta.json`
- **Workflow**: extract → score → index tables
- **Evals**: extraction accuracy gates

**Signals**: High-NA EUV installs, wafer starts

---

### Unit 7 — Emerging Trends & Challenges

**Semiconductor Focus**:
- Power and thermal constraints
- Interconnect and packaging innovations
- Memory-centric architectures
- Heterogeneous integration
- Quantum effects at advanced nodes

**Financial Fluency**:

- FRA/CorpFin: HBM pricing, cash conversion, supply bottlenecks
- Equity: Value capture shifts in advanced packaging

**Artifact**: Bottleneck Profit Transfer Analysis

**Agentic Build Track**:

- **Skills**: `bottleneck_profit_transfer`
- **Data Types**: `constraint_signal.json`
- **Workflow**: constraint tracker update
- **Evals**: "bottleneck story" checks

**Signals**: Substrate constraints, TSV yields, OSAT capacity

---

## Module 5: Silicon for AI and Computing

### Unit 8 — GPU Architecture & Alternatives

**Semiconductor Focus**:
- GPU architecture fundamentals
- NVIDIA’s dominance and ecosystem
- Supply-demand dynamics in AI accelerators
- Custom silicon vs general-purpose approaches
- Emerging alternatives (Graphcore, Cerebras, Tenstorrent)

**Financial Fluency**:

- Equity: Platform moat (CUDA), margin analysis
- CorpFin: Capex intensity, supplier prepayments

**Artifact**: AI Accelerator Value Chain Profit Pool

**Agentic Build Track**:

- **Skills**: `accelerator_value_chain_profit_pool`
- **Data Types**: `moat_analysis.json`
- **Workflow**: retrieve notes → generate view
- **Evals**: required-fields + citations

**Signals**: Foundry allocation, cloud prepay disclosures

---

### Unit 9 — Essential Chip Categories

**Semiconductor Focus**:
- Networking chips & interconnects
- Memory technologies (DRAM, NAND, HBM)
- Microcontrollers for edge AI
- Power management ICs
- FPGAs and reconfigurable computing

**Financial Fluency**:

- FRA: Segment reporting for diversified vendors
- Equity: SOTP analysis

**Artifact**: Data Center BOM-to-Margin Sensitivity

**Agentic Build Track**:

- **Skills**: `dc_bom_margin_sensitivity`
- **Data Types**: `bom_item.json`
- **Workflow**: compute sensitivity
- **Evals**: math cross-check

**Signals**: DRAM/HBM pricing, lead times

---

### Unit 10 — AI Chip Landscape

**Semiconductor Focus**: 
- Training vs inference architectures
- Domain-specific accelerators
- Edge AI silicon requirements
- Performance/watt trade-offs
- AI supply-demand crunch (TSMC capacity, HBM shortages)

**Financial Fluency**:

- Econ/Equity: Scarcity pricing, tiered allocation
- PM: Scenario analysis and capacity constraints

**Artifact**: Capacity-Constrained Pricing Model

**Agentic Build Track**:

- **Skills**: `capacity_constrained_pricing_model`
- **Data Types**: `capacity_assumptions.json`
- **Workflow**: schedule weekly run
- **Evals**: assumption transparency

**Signals**: HBM supply, foundry capacity, ASP trends

---

## Module 6: Future Computing Paradigms

### Unit 11 — Beyond Traditional Computing

**Semiconductor Focus**:
- Neuromorphic, photonic, analog, in-memory, probabilistic computing
- Early-stage supply chain signals (research hubs, CAPEX trends, patents)

**Financial Fluency**:

- CorpFin: R&D option valuation, funding runway
- QM: Early-signal scoring models

**Artifact**: Feasibility-to-Finance Matrix

**Agentic Build Track**:

- **Skills**: `feasibility_to_finance_matrix`
- **Data Types**: `early_signal.json`
- **Workflow**: score + publish matrix
- **Evals**: evidence weighting

**Signals**: Pilot lines, strategic partnerships

---

### Unit 12 — Beyond Silicon

**Semiconductor Focus**:
- Quantum computing
- Post-silicon materials (CNTs, 2D materials)
- Spintronics, molecular computing
- Exotic supply chain considerations

**Financial Fluency**:

- Equity: Venture-style economics, grants as non-dilutive capital
- Ethics: Tech vs investable milestone communication

**Artifact**: Evidence-Weighted Roadmap + Capital Needs Ladder

**Agentic Build Track**:

- **Skills**: `evidence_weighted_roadmap`
- **Data Types**: `roadmap_claim.json`
- **Workflow**: ingest patents/papers
- **Evals**: claim-to-citation integrity

**Signals**: Government funding, patents, consortium activity

---

## Module 7: AI Industry Landscape

### Unit 13 — AI Development Pipeline

**Semiconductor Focus**:
- Data collection and preparation
- Model development & training infra
- Inference deployment strategies
- MLOps lifecycle
- AI hardware–software co-design

**Financial Fluency**:

- CorpFin: TCO of AI infra, depreciation schedules
- FRA: Revenue recognition for AI services

**Artifact**: Infra TCO-to-Pricing Ladder

**Agentic Build Track**:

- **Skills**: `ai_infra_tco_ladder`
- **Data Types**: `tco_inputs.json`
- **Workflow**: compute + publish ladder
- **Evals**: decomposition completeness

**Signals**: Cloud capex, utilization rates

---

### Unit 14 — AI Application Domains

**Semiconductor Focus**:
- LLMs and generative AI
- Robotics and autonomous systems
- AI for scientific discovery
- Industry-specific AI applications
- AI-driven semiconductor demand

**Financial Fluency**:

- Econ/PM: Adoption S-curves, TAM/SAM/SOM analysis
- Equity: Revenue mix forecasting

**Artifact**: AI Demand–Supply Flywheel Model

**Agentic Build Track**:

- **Skills**: `demand_supply_flywheel_model`
- **Data Types**: `scenario.json`
- **Workflow**: scenario generator
- **Evals**: scenario completeness

**Signals**: AI inference cost trends, data center expansion

---

## Module 8: Investment & Strategy

### Unit 15 — Technology Assessment for Investment

**Semiconductor Focus**:
- Metrics for assessment
- Due diligence frameworks
- Red flags & risk indicators
- Cost estimation methodologies
- ROI models

**Financial Fluency**:

- FRA/CorpFin/Equity: Mini DCF, ROIC vs WACC, comps, precedents
- PM: Portfolio weighting logic

**Artifact**: Investment Memo with Sensitivity Analysis

**Agentic Build Track**:

- **Skills**: `investment_memo_with_sensitivity`
- **Data Types**: `sensitivity.json`
- **Workflow**: memo pipeline (retrieve → compute → draft → validate)
- **Evals**: "numbers verified" gate

**Signals**: TSMC Arizona capex updates, yield ramp

---

### Unit 16 — Future-Proofing Strategies

**Semiconductor Focus**:
- Roadmapping & scenario planning
- Strategies for resilience in volatile supply chains
- Balancing innovation vs practical implementation
- Building durable competitive advantages

**Financial Fluency**:

- PM/Econ: Scenario & Monte Carlo modeling
- QM: Range-based outcomes and risk distributions

**Artifact**: Contingency Capital Map (winners/losers under disruption)

**Agentic Build Track**:

- **Skills**: `scenario_monte_carlo`
- **Data Types**: `distribution.json`
- **Workflow**: scheduled scenario recompute
- **Evals**: distribution sanity + tail risks

**Signals**: Subsidy allocations, fab build timelines

---

# 🧮 CFA Domain → Semiconductor Topic Quick Reference

| CFA Domain | Where Integrated        | Application                                   |
| ---------- | ----------------------- | --------------------------------------------- |
| FRA        | Units 1–2, 6–9, 13      | Cost stacks, depreciation, segment reporting  |
| CorpFin    | Units 3–6, 10–11, 15–16 | WACC, NPV, real options, scenario modeling    |
| Equity     | Units 1, 5, 8–10, 15    | Valuation, moats, SOTP, profit pools          |
| Econ       | Units 1, 3, 10, 14, 16  | Cyclicality, trade, pricing, adoption curves  |
| QM         | Units 2, 6, 10, 16      | Yield regressions, sensitivities, Monte Carlo |
| PM         | Units 10, 14–16         | Scenario and risk analysis                    |
| Ethics     | Units 1, 12             | Research and communication standards          |

---

# 🧰 Artifacts Accumulated Across the Program

1. Value Chain Profit Pool Map
2. Node Economics Sheet
3. Bottleneck Profit Transfer Tracker
4. AI Infra TCO Ladder
5. Investment Memo + Sensitivity Analysis
6. Scenario Capital Map

---

# 🤖 Agentic Capabilities Accumulated

| Category         | Count | Examples                                                                                |
| ---------------- | ----- | --------------------------------------------------------------------------------------- |
| **Skills**       | 20+   | `profit_pool_map_generator`, `node_economics_model`, `investment_memo_with_sensitivity` |
| **Workflows**    | 16    | Seed universe, weekly refresh, memo pipeline, scenario recompute                        |
| **Data Schemas** | 16+   | `company.json`, `policy_event.json`, `sensitivity.json`                                 |
| **Evals**        | 30+   | Citation checks, math cross-checks, rubric gates, distribution sanity                   |

---

# ✅ Final Project

Choose:

- **Technology-centric** → Emerging semiconductor technology
- **Supply-chain-centric** → Chokepoint or geopolitical dynamic

Required components:

1. **Domain Artifact** (profit pool, investment memo, scenario model)
2. **Skill(s)** that can reproduce the artifact
3. **Workflow** to automate refresh
4. **Eval suite** to validate correctness
5. **Finance appendix** (assumptions table, valuation/ROI model, scenario tree)

---

# 📋 Unit Template

```markdown
## Unit {{N}} — {{Title}}

**Time Budget:** 5–8 hrs total

### A) Preview

- Why it matters: {{summary}}
- Look-for: {{3 guiding questions}}

### B) Core Learn

- **Semiconductor Focus**: {{topic details}}
- **Financial Fluency (CFA Microdose)**: {{domain + concept}}
- **Core Resource**: {{source/link}}
- **Case Study**: {{company/example}}
- **Stretch (optional)**: {{additional reading}}

### C) Agentic Build Track (1.5–2 hrs)

- **New Skill(s)**: {{1–3 markdown skills added/updated}}
- **New Data Type(s)**: {{1 JSON schema + optional DB table}}
- **Workflow Step**: {{1 workflow added/updated}}
- **Eval(s)**: {{1–2 regression tests}}
- **UI/Observability**: {{1 tiny improvement}}

### D) Build Artifact

- Spec: {{artifact name}}
- Inputs: {{datasets, filings, references}}
- Method: {{how built—run via skill + workflow}}
- Evidence: ≥3 sources (tech + finance)

### E) Synthesize

- 200-word caption + 3 citations
- Blog draft (prompt: {{prompt}})

### F) Reflect

- Self-quiz (6 questions)
- Gaps & next steps
- Add 2 finance questions (e.g., "What WACC did I assume?")
- Add 1 agentic question (e.g., "Did my eval catch the edge case?")
```

---

**End of Document**

_Unified Outline — Semiconductor mastery + Financial fluency + Agentic system development_

_Last updated: 2026-01-27_
