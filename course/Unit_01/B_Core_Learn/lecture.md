# Unit 1: Foundations & Ecosystem - Complete Lecture Guide

## Introduction
Welcome to Unit 1 of the SemiClaw Curriculum. In this unit, we build our domain expertise in semiconductors, align it with financial analysis principles, and deploy modern AI agents to automate data extraction and synthesis. This is the foundation of our course.

---

## A) Preview
**Why it matters:** The semiconductor supply chain is the most complex, capital-intensive, and geopolitically sensitive manufacturing ecosystem on Earth. Before you can model the economics of AI or predict the next bullwhip cycle, you must map the physical realities of the industry—who designs, who builds, who tests, and who owns the IP.

**Look-for:** 
1. What is the fundamental difference between a Fabless model and an IDM model?
2. How do gross margins serve as a proxy for a company's technological moat?
3. Why does cyclicality (inventory bullwhips) occur in this specific industry?

---

## B) Core Learn (Domain & Financial Fluency)
**Semiconductor Focus:**
The semiconductor industry isn't just one business; it's an interdependent global supply chain. 
- **Business Models:** 
  - **Fabless (e.g., NVIDIA, AMD):** Design chips but don't manufacture them. 
  - **Foundry (e.g., TSMC):** Manufacture chips designed by others. 
  - **IDM (e.g., Intel):** Integrated Device Manufacturers do both.
  - **OSAT:** Outsourced Semiconductor Assembly and Test.
  - **EDA/IP (e.g., ARM, Synopsys):** Software and IP blocks for design.
- **Monopolies & Duopolies:** ASML is the sole provider of EUV Lithography machines. TSMC dominates leading-edge logic. NVIDIA commands data-center compute.
- **Cyclicality:** Driven by inventory bullwhips, massive capital requirements, and macroeconomic demand.

**Financial Fluency (CFA Microdose):**
Understanding the "physics" of the supply chain enables understanding the "math" of the financial statements.
- **Gross Margins as a Moat Proxy:** A company's gross margin often reflects its pricing power. NVIDIA's margins are significantly higher than TSMC's, which are higher than Foxconn's.
- **Capex Intensity:** Building a cutting-edge fab costs over $20 billion. This massive Capex creates huge barriers to entry but results in heavy depreciation schedules that impact Free Cash Flow (FCF).
- **Revenue Models & FX Exposure:** ARM licenses IP (royalties); TSMC sells processed silicon wafers (exposed to NTD/USD fluctuations); ASML sells complex lithography tools.

---

## C) Agentic Build Track
**Objective:** Build a sandboxed AI workflow to autonomously extract financial and operational data from dense SEC filings.

We are moving away from fragile web scrapers and moving toward robust, agentic workflows.
- **The Modern Approach:** Instead of parsing HTML, we feed our agent SEC filings and enforce a strict JSON schema (`company.json`).
- **Data Points:** Extract Ticker, Primary Business Model, TTM CapEx, Gross Margin %, Next-Gen Node Dependency, and Top 3 Customers.
- **Evaluation:** The critical piece is the *Eval*. The agent must accurately cite the exact page number from the 10-K/20-F where it found the data. Hallucinated data fails the eval. We will be building the `company_profile_builder` skill.

---

## D) Build Artifact
**Objective:** The Value-Capture Profit Pool Map.
By passing the TSMC 20-F, ASML Annual Report, NVIDIA 10-K, and ARM Filings through our new agentic workflow, we will output verified `company.json` structures. Using the `profit_pool_map_generator` skill, we compile these into a visual mapping of Gross Margin bands across the entire supply chain.

---

## E) Synthesize & F) Reflect
**Synthesis:** We deploy a Content Director agent to draft deeply researched essays based on our extracted structured data. (e.g., *"What I Learned About the Semiconductor Supply Chain: Why Gross Margins tell the story of technological moats."*)

**Reflection:** You will test your recall on the Fabless vs. Foundry models and audit your agent's citation evaluations to ensure complete accuracy.

---

**Conclusion:** By the end of this unit, you will understand the players and financials of the semiconductor industry, and possess a working AI agent capable of extracting and synthesizing this data automatically.