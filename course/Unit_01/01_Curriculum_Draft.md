# Unit 1: Foundations & Ecosystem

**Time Budget:** 5–8 hrs total

### A) Preview

- **Why it matters:** The semiconductor supply chain is the most complex, capital-intensive, and geopolitically sensitive manufacturing ecosystem on Earth. Before you can model the economics of AI or predict the next bullwhip cycle, you must map the physical realities of the industry—who designs, who builds, who tests, and who owns the IP.
- **Look-for:** 
  1. What is the fundamental difference between a Fabless model and an IDM model?
  2. How do gross margins serve as a proxy for a company's technological moat?
  3. Why does cyclicality (inventory bullwhips) occur in this specific industry?

### B) Core Learn

- **Semiconductor Focus**: 
  - Importance of semiconductors in modern technology.
  - Mapping the semiconductor supply chain (IP → EDA → WFE → Fabless → Foundry → OSAT).
  - Industry players and their roles (e.g., TSMC, ASML, NVIDIA, ARM).
  - Cyclical nature of semiconductors and market trends.
  - Basic economics and business models.
- **Financial Fluency (CFA Microdose)**: 
  - *FRA/Equity:* Analyze TSMC and ASML filings (understanding revenue models, depreciation, and capacity utilization).
  - *Econ:* Cyclicality, ASPs (Average Selling Prices), and FX exposure (NTD/EUR/USD).
  - *Ethics:* Research objectivity & sourcing standards.
- **Core Resource**: TSMC Annual Report (20-F), ASML Investor Day Presentations, Steve Blank's SC Ecosystem breakdown.
- **Case Study**: The TSMC (Foundry) vs. NVIDIA (Fabless) margin comparison.

### C) Agentic Build Track (1.5–2 hrs)

- **New Skill(s)**: `company_profile_builder`, `profit_pool_map_generator`
- **New Data Type(s)**: `company.json` (Ticker, Business Model, Gross Margin %, Capex), `segment.json`
- **Workflow Step**: Seed the initial company universe. Build a sandboxed AI workflow to autonomously extract financial/operational data from dense SEC filings.
- **Eval(s)**: 
  - *Required-sections presence:* Does the extracted JSON contain all mandatory schema fields?
  - *Citations presence:* Does the agent correctly cite the exact page number from the 10-K/20-F for the Gross Margin? (Fails if hallucinated).
- **UI/Observability**: Log extraction success/failure rates to a local markdown table.

### D) Build Artifact

- **Spec**: *Value-Capture Profit Pool Map* (A visual/data mapping of Gross Margin bands across the entire supply chain).
- **Inputs**: TSMC 20-F, ASML Annual Report, NVIDIA 10-K, ARM Filings.
- **Method**: Run the `company_profile_builder` skill against the raw PDFs, output the `company.json` files, and use the `profit_pool_map_generator` workflow to compile them into the final map.
- **Evidence**: ≥3 sources (10-K filings, Investor Decks, Industry Primers).

### E) Synthesize

- **200-word caption + 3 citations:** A concise summary explaining why value accrues at specific chokepoints in the supply chain (e.g., EUV lithography or leading-edge foundry).
- **Blog draft (prompt):** *"What I Learned About the Semiconductor Supply Chain: Why Gross Margins tell the story of technological moats."* (Autonomously drafted by the Content Director agent using the extracted JSON data).

### F) Reflect

- **Self-quiz (6 questions):** Test recall on Fabless vs. Foundry, WFE monopolies, and Margin vs. Volume models.
- **Gaps & next steps:** Identify missing data in the Profit Pool Map (e.g., private companies, emerging Chinese foundries).
- **Add 2 finance questions:** 
  1. How does TSMC's accelerated depreciation schedule impact its short-term Free Cash Flow?
  2. If the USD strengthens against the NTD, how does this impact TSMC's reported margins?
- **Add 1 agentic question:** Did my citation evaluation successfully catch the edge case where the model tried to guess a blended margin instead of extracting the exact figure?