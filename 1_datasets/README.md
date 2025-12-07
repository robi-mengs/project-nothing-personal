# Dataset Documentation

## Synthetic Patent Data (Not Real USPTO Data)

### Source and Rationale for Synthetic Data

This project **does not use real USPTO patent data**. Instead, it relies
entirely on **synthetic, artificially generated data** that mimics the
structure, patterns, and statistical properties of real patent records. This
approach was adopted for the following reasons:

- **Legal compliance**: Real USPTO data is subject to usage restrictions, API
  rate limits, and terms of service that may prohibit certain types of automated
  analysis or redistribution.
- **Privacy protection**: Actual patent filings contain personally identifiable
  information (e.g., inventor names, addresses), which poses ethical risks if
  used without explicit consent.
- **Research safety**: Using synthetic data eliminates the risk of inadvertently
  revealing real inventors’ strategies or exposing sensitive innovation
  trajectories.
- **Educational clarity**: A controlled, reproducible dataset allows the core
  concept—**privacy-preserving market intelligence**—to be demonstrated without
  confounding real-world noise or legal ambiguity.

The synthetic dataset used in this project is generated programmatically within
the analysis notebook:
[privacy_protection.ipynb](../4_data_analysis/privacy_protection.ipynb) ensuring
full transparency and reproducibility.

For reference, the complete data generation logic (including timeline setup,
patent record synthesis , and CSV export) is included in **Section 2: The Legal
& Safe Approach** of the notebook. Should you need the standalone code snippet
for educational or auditing purposes, it is also available in the repository
under
[synthetic_USPTO_data_generator.ipynb](./synthetic_USPTO_data_generator.ipynb).

### Data Content and Structure

The synthetic dataset includes realistic but entirely fictional records with the
following fields:

- **Patent number**: Formatted like real USPTO IDs (e.g., `US2022999890`)
- **Application and grant dates**: Simulated across a 6-month window
- **Technology category**: Drawn from common innovation domains (e.g.,
  “blockchain healthcare”, “AI medical diagnosis”)
- **Filing entity type**: Categorized as `startup`, `big_tech`, `pharma_giant`,
  etc.
- **Abstract**: Auto-generated placeholder text reflecting the technology
  category

This data is **structured** (tabular), **temporal** (time-stamped), and includes
**categorical** and **text-like** fields to support demonstration of privacy
techniques.

### Relevance to Research Question

This synthetic dataset directly supports the investigation:  
> *“How can privacy-preserving technologies like differential privacy create a
> fairer innovation ecosystem by providing underrepresented inventors with
> market intelligence and idea protection without compromising their
> intellectual property?”*

While no real demographic data is used, the simulation models how **search
behavior** not identity can expose strategic intent. The focus is on the
**process** of research, not specific inventors. By showing how even generic
search patterns (e.g., “blockchain” → “HIPAA-compliant auth”) reveal a roadmap,
the project demonstrates why **privacy-aware tools** are essential for equitable
participation in innovation especially for solo inventors or small teams without
legal shields.

### Ethical and Methodological Integrity

- **No real individuals or entities are represented**.
- **No actual patent data was accessed, stored, or modified**.
- **All outputs are for educational and methodological demonstration only**.
- The synthetic approach aligns with best practices used by institutions like
  Apple, Google, and the NIH when prototyping privacy-sensitive systems.

This strategy ensures full compliance with data ethics principles while still
delivering actionable insights into how differential privacy can protect
early-stage innovators.

[← Back to Project Overview](../README.md)
