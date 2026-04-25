# Retail Decision-Support Workflow: Supermarket Product-Line Priorities and Branch-Level Differences

## Project Overview
This project presents a reusable Python workflow for supermarket transaction analysis. The current notebook uses a sample supermarket Excel dataset as a demonstration case, but the same workflow is intended to be applicable to other structured retail transaction inputs such as POS exports, CSV sales reports, ERP extracts, or database outputs.

The main goal of the project is to support supermarket managers and branch managers in identifying product-line priorities, understanding sales and gross-income concentration, and recognising branch-level differences that may justify more localised operational strategies.

## Business Question and Target User
### Business Question
Which product lines should managers prioritise, and do different branches require different product-line strategies based on sales, income, concentration, and branch-level patterns?

### Target User
The main users of this workflow are supermarket managers and branch managers. A secondary audience includes retail analysts or business students interested in transaction-based decision support.

## Data Standard
The workflow is designed for structured retail transaction data.

### Required fields
- product category / product line
- branch / store identifier
- sales value
- income / profit-related value
- date

### Recommended fields
- quantity
- customer type
- payment method
- time of transaction
- rating / feedback
- city / location

### Optional fields
- promotion / discount
- inventory
- customer ID
- foot traffic
- supplier or cost details

### Supported file formats
- `.xlsx`
- `.csv`

## Current Demonstration Dataset
The current notebook uses a sample supermarket transaction dataset containing 1,000 records and 17 variables.

Key fields in the current sample include:
- `Product line`
- `Branch`
- `Total`
- `gross income`
- `Date`

**Source:** Kaggle supermarket sales dataset (used here as a sample demonstration input)  
**Accessed:** 2026-04-20

The current dataset is used as a sample input for demonstration. The workflow is intended to be reusable with other structured supermarket transaction datasets that contain comparable fields.

## Workflow Structure
The notebook follows a structured decision-support workflow:

1. Project introduction
2. Executive summary / quick summary
3. User guide and output navigation
4. Data standard and submission guide
5. Data loading and schema detection
6. Data cleaning and feature engineering
7. Core decision-support analysis
8. Extensible analysis design
9. Business insights and recommendations
10. Final summary / key takeaways
11. Limitations and future reuse

## Core Analysis Modules
The current sample activates the following main analytical modules:

- Sales Overview
- Product-Line Priority Analysis
- Sales and Income Quality Analysis
- Concentration Analysis
- Branch-Level Performance Analysis
- Customer Analysis
- Time Pattern Analysis
- Relationship / Correlation Analysis

## Key Findings
- `Food and beverages` is the strongest product line overall in both total sales and gross income.
- Sales and gross income are concentrated in a relatively small number of product lines.
- The strongest product lines are not identical across all branches.
- Branch-level results suggest that company-wide priorities are useful, but branch-level adjustment is still necessary.
- The current sample supports strongest decision-making insight through product-line, concentration, and branch-level analysis.

## How to Run
1. Download the repository files.
2. Make sure `supermarket_decision_support_analysis.ipynb` and `supermarket.xlsx` are in the same folder.
3. Open the notebook in Jupyter Notebook or JupyterLab.
4. Run the cells from top to bottom.

## Repository Contents
- `supermarket_decision_support_analysis.ipynb`
- `supermarket.xlsx`
- `README.md`

## Limitations and Future Reuse
This project uses a sample Excel file and a relatively short time period, so it should not be treated as a long-term forecasting tool. The current notebook is best understood as a reusable decision-support workflow demonstrated with one sample retail dataset.

In future work, the workflow could be extended with:
- longer time-series data
- richer inventory variables
- customer-level transaction records
- promotion or discount fields
- more direct integration with POS exports, ERP reports, database inputs, or dashboard tools
