# Module 3: The "SemiClaw" Agent (Modern Agentic Build Track) - Resources

## Core Build Assets
- **JSON Schema Specification:** 
  - *Link:* [json-schema.org](https://json-schema.org/)
  - *Why:* Defining the strict `company.json` output structure enforcing fields like Ticker, Primary Business Model, TTM CapEx, etc.

- **OpenClaw Documentation:**
  - *Link:* [OpenClaw GitHub / Docs](https://github.com/openclaw/openclaw)
  - *Why:* Guides on building local tools and AgentSkills for the `company_profile_builder` function.

## Tooling Built for the Curriculum
- **SEC Edgar Search Tool (`edgar_search/search.py`):**
  - *Why:* Replaces fragile web scraping with programmatic fetching of SEC filings natively in the workspace. We teach this modern tool-building approach.

- **PDF Parsing Libraries:**
  - *Link:* [PyMuPDF (fitz)](https://pymupdf.readthedocs.io/en/latest/) or `pdfplumber`
  - *Why:* Text extraction from dense SEC filing PDFs before passing context to the LLM.

## LLM API Documentation
- **Anthropic / OpenAI API Docs on Structured Outputs:**
  - *Why:* Crucial for guaranteeing JSON formatting and enforcing citations (the "Eval" component: returning exact page numbers for Gross Margin metrics).
