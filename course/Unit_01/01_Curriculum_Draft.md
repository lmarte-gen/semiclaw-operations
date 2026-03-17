# Unit 1: Foundations & Ecosystem
## Module 1: Semiconductor Industry Overview

### 1. The Silicon Primer (Domain Track)
- **Objective:** Map the global supply chain, understand distinct business models, and identify where the leverage lies.
- **Key Concepts:**
  - Fabless vs. Foundry vs. IDM vs. OSAT vs. EDA/IP.
  - The Monopolies & Duopolies (ASML in EUV Lithography, TSMC in Leading Edge Logic, ARM in IP, NVDA in Datacenter Compute).
  - The Cyclicality of Silicon (Inventory cycles, bullwhips, lead times).
- **Core Assets:** TSMC Annual Report (20-F), ASML Investor Day Presentations.

### 2. The Money Flow (Financial Fluency Track)
- **Objective:** Analyze how different business models capture value differently (CFA FRA/Equity applied).
- **Key Concepts:**
  - **Gross Margins** as a proxy for technological moat (Why NVDA > TSMC > Foxconn).
  - **Capex Intensity:** Why cutting-edge foundries cost $20B to build (depreciation schedules vs. free cash flow).
  - **Revenue Models:** Licensing/Royalties (ARM) vs. Wafer Sales (TSMC) vs. Tool Sales (ASML) vs. Chip Sales (NVDA).
- **The Domain Artifact:** *Value-Capture Profit Pool Map* (A visual mapping of Gross Margin bands across the entire supply chain).

### 3. The "SemiClaw" Agent (Modern Agentic Build Track)
- **Objective:** Build a sandboxed AI workflow to autonomously extract financial and operational data from dense SEC filings and investor decks.
- **The Old Way (Deprecated):** Writing fragile Python web scrapers to parse Yahoo Finance HTML.
- **The Modern Way (What we teach):** 
  - **Define the Schema:** Create a strict JSON schema (`company.json`) enforcing fields like: Ticker, Primary Business Model, TTM CapEx, Gross Margin %, Next-Gen Node Dependency, Top 3 Customers.
  - **Build the Skill:** Create the `company_profile_builder` Tool (an MCP/OpenClaw-compatible function).
  - **Write the Eval:** Ensure the agent correctly cites the exact page number from the 10-K where it found the Gross Margin. (If it hallucinates a margin without a citation, the eval fails).
- **The Workflow:** Feed the agent a PDF of a 10-K, run the skill, output verified structured data into the repository.

### 4. Synthesis & Content Engine (The Flywheel)
- **Output Artifact:** A deeply researched essay and X thread summarizing the findings.
- **Example Prompt:** *"What I Learned About the Semiconductor Supply Chain: Why Gross Margins tell the story of technological moats."* (Drafted autonomously by the Content Director agent using the extracted `company.json` data).