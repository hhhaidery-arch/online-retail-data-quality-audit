# Online Retail Data Quality Audit

**Exploratory Data Quality Investigation | Python · Pandas · NumPy · Matplotlib**

## Overview

This project investigates data quality issues in an Online Retail transactional dataset. The objective is to identify missing values, duplicate records, unusual quantities, zero-price transactions, and suspicious transaction patterns before downstream business analysis.

## Dataset at a Glance

| Metric | Finding |
|---|---:|
| Original records | 541,909 |
| Records after removing exact duplicates | 536,641 |
| Missing `CustomerID` values | 135,080 |
| Missing `Description` values | 1,454 |
| Negative-quantity records | 10,624 |
| Zero-unit-price records | 2,515 |

## Key Findings

- Investigated cancellation-prefixed invoices and negative-quantity records.
- Identified 1,179 positive-quantity records with zero unit prices.
- Identified 1,336 negative-quantity, zero-price records without a `C` invoice prefix.
- Found that these 1,336 records were associated with the United Kingdom and had missing customer identifiers.
- Reviewed extreme quantities, high unit prices, unusual descriptions, and date completeness.

## Tools

- Python
- Pandas
- NumPy
- Jupyter Notebook
- Matplotlib

## Audit Conclusion

The exploratory investigation identified several data-quality risks that may affect revenue analysis, customer analysis, and reporting. Unusual records require contextual interpretation before they are removed or reclassified.

The next stages are to document cleaning decisions, validate the cleaned dataset, perform business analysis, and build an interactive Power BI dashboard.

## Project Status

**Current stage:** Exploratory data quality audit.

Cleaning, final validation, SQL analysis, and dashboard development are planned next steps.
