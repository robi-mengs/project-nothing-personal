# Data Analysis

## [`privacy_protection.ipynb`](https://colab.research.google.com/drive/1-ssAXLpjf9C04apXQY-AMap8Ym3hp9oT#scrollTo=MDphAmN8cQ5Q)

This notebook analyzes the strategic risk of exposing a startup's innovation
roadmap through sequential patent searches and proposes a differential
privacy-based mitigation strategy. It:

- Simulates a high-risk search evolution pattern (e.g., from "blockchain" to
  "HIPAA compliant blockchain auth").
- Generates synthetic patent data to safely model real-world competitive
  dynamics.
- Implements a privacy-preserving transformation using the Laplace mechanism (ε
  = 1.0) to generalize search terms and add statistical noise.
- Quantifies the trade-off between **intelligence retention** and **competitive
  risk reduction**.
- Demonstrates through visual and numerical evidence that privacy protection
  hides project intent while preserving ~85% of market insight value.
    
**The synthetic patent dataset**: used in this project is generated
programmatically to ensure legal compliance, ethical integrity, and
reproducibility avoiding the use of real USPTO data, which may contain sensitive
information or be subject to usage restrictions. It simulates a realistic yet
entirely fictional set of U.S. patent records over a six-month period, including
plausible patent numbers, application and grant dates, technology categories
(e.g., “blockchain healthcare,” “AI medical diagnosis”), filing entity types
(e.g., startups, big tech), and auto-generated abstracts.

For clarity and modularity, the data generation logic is implemented in a
dedicated notebook named
[`synthetic_uspto_data_generator.ipynb`](./1_datasets/synthetic_uspto_data_generator.ipynb),
while the core privacy analysis—including risk simulation and differential
privacy—is contained in
[`privacy_protection.ipynb`](./4_data_analysis/privacy_protection.ipynb). The
resulting dataset is saved as `synthetic_uspto_data.raw.csv` for transparency
and reuse. No external datasets are used; all data is synthetically generated
for analytical demonstration. The focus is on **strategic insight**, **risk
modeling**, and **privacy-aware research design** data cleaning or exploratory
profiling.
