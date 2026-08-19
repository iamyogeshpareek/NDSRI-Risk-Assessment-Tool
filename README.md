# NDSRI Risk Screening Tool

An interactive, browser-based decision-support tool for **nitrosamine drug substance-related impurity (NDSRI) risk assessment** - built around two current regulatory frameworks used across the pharmaceutical industry.

![status](https://img.shields.io/badge/status-portfolio_project-orange)
![stack](https://img.shields.io/badge/stack-HTML%2FCSS%2FJS-black)
![license](https://img.shields.io/badge/use-educational%2Fscreening_aid-teal)

---

## What it does

### 1. Process Risk Assessment
A weighted checklist based on **ICH M7(R2) Annex 2** root-cause factors — secondary/tertiary amines, nitrosating agents, reaction pH, recycled solvents, excipient nitrite potential, and API-class precedent (sartans, metformin, ranitidine-class, rifamycins). Produces a **Low / Medium / High** process-risk verdict with recommended next steps: standard risk review vs. confirmatory LC-MS/MS or GC-MS testing.

### 2. CPCA Structural Categorization
A simplified, educational implementation of the **FDA/EMA Carcinogenic Potency Categorization Approach (CPCA)** (Cross, Ponting *et al.*; FDA 2023 nitrosamine guidance). Walks through the core structural descriptors -

- alpha-hydrogen availability
- cyclic vs. acyclic nitrogen context
- branching/steric hindrance at the alpha-carbon
- conjugated electron-withdrawing groups
- beta-heteroatom substitution

— and returns an indicative **potency category (1–5)** with the corresponding **Acceptable Intake limit (18–1,500 ng/day)**.

---

## Why this exists

CPCA-based assessment is currently available through enterprise tools such as Lhasa's **Derek Nexus**, and FDA has also released an open-source reference implementation (**Featurize-Nitrosamines**, Kruhlak *et al.*, 2024). This project doesn't propose new science — it's a from-scratch implementation of the published CPCA logic, built to make the reasoning process transparent and accessible for students, small labs, and QA/regulatory teams without access to licensed software.

Built as a portfolio project by an M.Pharm (Pharmaceutical Analysis) graduate (currently pursuing PhD) working on AQbD-based analytical method development and a review article on NDSRIs covering FDA, EMA, and ICH M7(R2) frameworks.

---

## Tech

Single-file HTML/CSS/JS. No backend, no dependencies, fully client-side - open `index.html` in any browser.

---

## Disclaimer

This tool is a **screening and training aid only**. It is not validated software and does not replace expert structural review, read-across assessment, (Q)SAR tooling, or regulatory submission-grade evaluation. Category and risk outputs should be independently verified before use in any real risk assessment or filing.

---

## References

- ICH M7(R2) — *Assessment and Control of DNA Reactive (Mutagenic) Impurities in Pharmaceuticals to Limit Potential Carcinogenic Risk*
- FDA (2023) — *Control of Nitrosamine Impurities in Human Drugs*, guidance for industry
- Cross, K.P., Ponting, D.J. *et al.* — development of the Carcinogenic Potency Categorization Approach (CPCA)
- Kruhlak, N.L. *et al.* (2024) — *Limits for N-Nitrosamine Impurities in Pharmaceuticals: Development and Application of the CPCA*, Regulatory Toxicology and Pharmacology
