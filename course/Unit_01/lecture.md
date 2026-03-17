# Unit 1: Foundations & Ecosystem - Complete Lecture Guide

## Introduction
Welcome to Unit 1 of the SemiClaw Curriculum. In this unit, we build our domain expertise in semiconductors, align it with financial analysis principles, and deploy modern AI agents to automate data extraction and synthesis. This is the foundation of our course.

---

## Module 1: Semiconductor Industry Overview

### 1. The Silicon Primer (Domain Track)
**Objective:** Map the global supply chain, understand distinct business models, and identify where the leverage lies.

The semiconductor industry isn't just one business; it's an interdependent global supply chain. 
- **Business Models:** 
  - **Fabless (e.g., NVIDIA, AMD):** They design the chips but don't manufacture them. 
  - **Foundry (e.g., TSMC):** They manufacture chips designed by others. 
  - **IDM (e.g., Intel):** Integrated Device Manufacturers do both design and manufacturing.
  - **OSAT:** Outsourced Semiconductor Assembly and Test companies package the chips.
  - **EDA/IP (e.g., ARM, Synopsys):** Provide the software and intellectual property blocks to design chips.

- **Monopolies & Duopolies:** Power is concentrated. ASML is the sole provider of EUV Lithography machines. TSMC dominates leading-edge logic manufacturing. ARM dominates mobile and increasingly data-center IP. NVIDIA has a near-monopoly on data-center compute for AI.
- **Cyclicality:** The industry is famously cyclical, driven by inventory bullwhips, long lead times for new fabs, and macroeconomic demand. 

### 2. The Money Flow (Financial Fluency Track)
**Objective:** Analyze how different business models capture value differently.

Understanding the "physics" of the supply chain allows us to understand the "math" of the financial statements.
- **Gross Margins as a Moat Proxy:** A company's gross margin often reflects its pricing power and technological moat. This is why NVIDIA's margins are significantly higher than TSMC's, which are higher than Foxconn's.
- **Capex Intensity:** Building a cutting-edge fab costs over $20 billion. This massive capital expenditure (Capex) creates immense barriers to entry but also results in heavy depreciation schedules that impact free cash flow.
- **Revenue Models:** 
  - ARM licenses IP and collects royalties.
  - TSMC sells processed silicon wafers.
  - ASML sells complex lithography tools.
  - NVIDIA sells finished chips and systems.

### 3. The "SemiClaw" Agent (Modern Agentic Build Track)
**Objective:** Build a sandboxed AI workflow to autonomously extract financial and operational data from dense SEC filings.

We are moving away from fragile web scrapers and moving toward robust, agentic workflows.
- **The Modern Approach:** Instead of parsing HTML, we feed our agent SEC filings and enforce a strict JSON schema (`company.json`).
- **Data Points:** We extract the Ticker, Primary Business Model, TTM CapEx, Gross Margin %, Next-Gen Node Dependency, and Top 3 Customers.
- **Evaluation:** The critical piece is the *Eval*. The agent must accurately cite the exact page number from the 10-K where it found the data. Hallucinated data fails the eval. We will be building the `company_profile_builder` skill to handle this.

### 4. Synthesis & Content Engine (The Flywheel)
**Objective:** Build a content flywheel that synthesizes our extracted data into high-value outputs.

Once we have structured, verified data, we deploy a Content Director agent. This agent takes the `company.json` data and autonomously drafts deeply researched essays and X threads (e.g., *"What I Learned About the Semiconductor Supply Chain: Why Gross Margins tell the story of technological moats."*).

---

## Conclusion
By the end of this unit, you will not only understand the players and the financials of the semiconductor industry but also possess a working AI agent capable of extracting and synthesizing this data automatically.