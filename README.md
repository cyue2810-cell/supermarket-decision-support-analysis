# Product-Line Priorities and Branch-Level Differences: A Python Data Analysis Project for Supermarket Decision Support

## Project Overview
This project presents a reusable Python workflow for supermarket transaction analysis. The notebook uses a sample supermarket Excel dataset as a demonstration case, but the same workflow is intended to be applicable to other structured retail transaction inputs such as POS exports, CSV sales reports, ERP extracts, or database outputs.

The main goal of the project is to support supermarket managers and branch managers in identifying product-line priorities, understanding sales and gross-income concentration, and recognising branch-level differences that may justify more localised operational strategies.

## Business Question and Target User
### Business Question
Which product lines should supermarket managers prioritise, and do different branches require different product-line strategies based on sales and gross-income patterns?

### Target User
The main users of this workflow are supermarket managers and branch managers. A secondary audience includes retail analysts or business students interested in transaction-based decision support.

## Dataset
The project uses a supermarket transaction dataset containing 1,000 records and 17 variables. Key fields include:

- `Product line`
- `Branch`
- `Total`
- `gross income`
- `Date`

The current dataset is used as a sample input for demonstration. The workflow is intended to be reusable with other structured supermarket transaction datasets that contain comparable fields.

## Methods
The notebook follows a structured workflow:

1. Data loading
2. Initial inspection
3. Data cleaning and preparation
4. Product-line priority analysis
5. Sales and income concentration analysis
6. Branch-level difference analysis
7. Reusable workflow functions
8. Business insights and managerial recommendations

The analysis uses Python libraries such as `pandas` and `matplotlib`, together with reusable functions for category summaries, branch-level summaries, and top-n concentration analysis.

## Key Findings
- `Food and beverages` is the strongest product line overall in both total sales and gross income.
- `Sports and travel` and `Electronic accessories` also perform strongly across the main business indicators.
- Sales and gross income are meaningfully concentrated in a relatively small number of product lines.
- Branch-level analysis shows that total branch performance alone is not sufficient; product-line priorities differ across branches.
- The results support a combined strategy of company-wide product priorities and branch-level adjustment.

## How to Run
1. Download the repository files.
2. Make sure the notebook file and `supermarket.xlsx` are in the same folder.
3. Open the notebook in Jupyter Notebook or JupyterLab.
4. Run the cells from top to bottom.

## Limitations and Future Improvements
This project uses a sample Excel file and a relatively short time period, so it should not be treated as a long-term forecasting tool. In future work, the workflow could be extended with longer time-series data, richer inventory or customer-level variables, and more direct integration with POS exports, ERP reports, database inputs, or dashboard tools.
