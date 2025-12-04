# Dataset Documentation

## USPTO Open Patent Data

### Source and Collection Method

The dataset the are used in this project originates from the **United States
Patent and Trademark Office (USPTO) Open Patent Data**, a publicly available
repository of U.S. patents and published patent applications. It is classified
as **secondary data** originally collected by the USPTO for legal and
administrative purposes and repurposed here for research on innovation equity.
The data is **public**, structured in standardized formats (XML, bulk text, and
via APIs), and updated regularly through official USPTO channels such as the
[Patent Public Search](https://www.uspto.gov/patents/search) platform and the
[Bulk Data Storage System](https://bulkdata.uspto.gov/).

### Data Content and Types

The dataset contains both **structured** and **semi-structured** records,
including:

- **Quantitative (discrete)**: Patent counts, application/filing dates, CPC/USPC
  classification codes
- **Qualitative (nominal)**: Inventor names, assignee organizations, countries
  of residence, legal status
- **Temporal**: Time-stamped events (filing, publication, grant dates), making
  it a rich **time series** resource
- **Textual (unstructured)**: Abstracts, claims, and full descriptions, ideal
  for NLP-based topic modeling

All files are retained in their original form (e.g.,
`uspto_patents_2024.raw.zip`) to preserve data integrity, per project
guidelines. Processed subsets such as cleaned inventor-location mappings or
filtered entry-level technology domains will be saved as new files (e.g.,
`uspto_inventors_underrepresented_2024.csv`).

## Relevance to Research Question

This dataset directly supports the investigation:  
> *“How can privacy-preserving technologies like differential privacy create a
> fairer innovation ecosystem by providing underrepresented inventors with
> market intelligence and idea protection without compromising their
> intellectual property?”*

While USPTO data does not include explicit demographic identifiers (e.g., race,
gender), it provides **proxy indicators**, such as name etymology, geographic
location, and institutional affiliation that, when handled responsibly, can
reveal disparities in innovation access. The public nature of patent disclosures
also creates a tension: inventors must reveal technical details to secure
rights, yet this exposure may disadvantage those without legal or commercial
safeguards.

By applying **differential privacy** to aggregated patent trends (e.g.,
“emerging AI subfields by region”), this project aims to generate equitable
market intelligence that protects individual strategies especially for
independent or underrepresented inventors while preserving utility for
early-stage innovation support.

## Ethical and Quality Considerations

- **Privacy**: Raw inventor names/addresses are sensitive; all analyses will use
  anonymized or aggregated views.
- **Bias**: Geographic and institutional proxies may not fully capture
  underrepresentation; limitations will be documented.
- **Completeness**: USPTO data is highly complete for granted patents but may
  lag for recent applications.
- **Timeliness**: Data is updated quarterly; our snapshot reflects filings
  through Q3 2024.

This dataset was chosen because it offers a transparent, large-scale, and
legally grounded window into the U.S. innovation system making it ideal for
prototyping fair, privacy-aware intelligence tools.
