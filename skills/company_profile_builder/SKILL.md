# Skill: company_profile_builder

## Description
The `company_profile_builder` is a core agentic skill designed for the Agentic Build Track (Unit 01). It autonomously extracts financial and operational data from dense SEC filings (e.g., 10-K, 20-F) and outputs structured data (`company.json`) to seed a company universe and build a Value-Capture Profit Pool Map. 

## Inputs
- **Filing Data:** Raw PDFs, Markdown, or text documents of annual reports (e.g., TSMC 20-F, ASML Annual Report, NVIDIA 10-K, ARM Filings).
- **Target Ticker/Company:** The primary entity for which data is being extracted.

## Outputs
- **Data Object:** `company.json`
- **Observability Artifact:** Local Markdown table logging success/failure rates.

## Evaluation Gates (Strict Enforcement)
This skill employs rigid validation checks before completing a run. 

### 1. Required-Sections Presence
The extracted data MUST conform exactly to `company.schema.json`. It must contain the following fields:
- `ticker` (string)
- `business_model` (enum: IDM, Fabless, Foundry, WFE, EDA, OSAT, IP)
- `gross_margin_percent` (number)
- `capex` (number)
- `citations` (object)

*Fail Condition:* Any missing or structurally invalid field will cause the pipeline to reject the extraction and prompt a retry.

### 2. Citations Presence
Accurate attribution is critical. The `citations` object MUST include the exact page number from the 10-K/20-F for the gross margin. 
- *Check:* Does the agent correctly cite the exact page number?
- *Fail Condition:* If the page number is omitted, vague (e.g., "Financials Section"), or hallucinated, the extraction fails immediately. Do not attempt to guess blended margins.

## Execution Workflow

1. **Intake:** Read the provided annual report or filing document.
2. **Extraction:** Navigate to the financial summary, MD&A, and consolidated statements to extract the core metrics (Gross Margin %, Capex) and identify the business model.
3. **Verification:** Check the document's page numbers corresponding to the extracted figures.
4. **Validation (Eval Gates):** 
   - Parse the extracted data against the JSON schema (`company.schema.json`).
   - Run the Citation Gate: ensure `gross_margin_page` is a specific string representing a real page number.
5. **JSON Generation:** Write the validated payload to `[ticker]_company.json`.
6. **Logging:** Append an entry to the local observability log (`extraction_logs.md`), recording:
   - Date/Time
   - Ticker
   - Required Sections Eval (Pass/Fail)
   - Citations Eval (Pass/Fail)
   - Reason for failure (if any)

## Schema Reference
See `company.schema.json` in this directory for the definitive data structure.
