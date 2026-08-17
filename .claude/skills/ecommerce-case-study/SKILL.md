---
name: ecommerce-case-study
description: Use whenever working on the E-Commerce Marketing & Sales case study (Datasets/Case_Study data, the notebook at "E-commerce Case Study/ecommerce_case_study_1.ipynb", the 10 business questions on acquisition/retention/RFM/cohorts/CLV/seasonality). Triggers on mentions of this case study, its business questions, RFM segmentation, cohort retention, or the Online_Sales/CustomersData/Discount_Coupon/Marketing_Spend/Tax_amount files.
---

# E-Commerce Case Study

Before doing anything else, read these two files in full. They contain
everything already derived about this dataset (schema, data quirks, the
Invoice Value formula, notebook conventions, file locations), so there is no
need to re-explore the raw CSVs/Excel files from scratch:

1. `Datasets/Case_Study/Scope_Document.md`: problem statement, the 10 business
   questions verbatim, submission and evaluation criteria.
2. `Datasets/Case_Study/Knowledge_Base.md`: verified data dictionary, known
   data quirks (category mismatches, coupon edge cases), the core Invoice
   Value formula, and the notebook structure/formatting conventions the user
   expects (markdown header, then motive cell, then code cell; seaborn-only
   charts; no inline comments; Gemini-generated insight cells).

## Working conventions to follow

- The deliverable notebook lives at `E-commerce Case Study/ecommerce_case_study_1.ipynb`.
- The Gemini/Google AI Studio key lives in `E-commerce Case Study/.env` as
  `GOOGLE_API_KEY`. Load it with `python-dotenv` and `os.getenv`; never
  hardcode or print it. `.env.example` in the same folder is the safe
  template to reference instead.
- Final submission is a PDF export of the fully executed notebook. See
  `Scope_Document.md` for the exact submission rules: PDF only, under 20MB,
  no more than 50 pages, and no Colab links.
- If the Knowledge Base doc is missing information you need (e.g. a new data
  quirk discovered mid-analysis), update `Knowledge_Base.md` rather than only
  fixing it inline — keep it authoritative for future sessions.
