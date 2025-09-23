
### Sales Streamlit Dashboard
A minimal, interactive dashboard for sales/finance data built with Streamlit, Plotly, Pandas, and DuckDB.[2][1]

### Features
- Upload an Excel workbook from the sidebar to load data into the app.[2]
- Expandable data preview with basic column configuration for Year.[2]
- KPI cards and gauges for key metrics (e.g., Accounts Receivable/Payable, Equity Ratio, Debt Equity, Current Ratio, stock days, delay).[2]
- Grouped bar chart of 2023 Sales by business unit and Scenario.[2]
- Monthly Budget vs Forecast line chart for 2023 (Software business unit).[2]
- Bar chart of Actual yearly totals by Account across years (non-Sales accounts).[2]

### Data input
- Expected file type: .xlsx read via Pandas with openpyxl in the environment.[1][2]
- Expected columns include: Account, business_unit, Currency, Year, Scenario, and monthly columns Jan–Dec.[3]
- Example rows include Sales and various expense accounts across business units like Software, Advertising, and Hardware.[3]

### Quickstart
1) Install dependencies from requirements.txt.[1]
2) Run the app with Streamlit.[2]

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

3) In the app sidebar, use “Choose a file” to upload the Excel data.[2]
4) Explore the data preview and the charts laid out in the two-row dashboard.[2]

### Tech stack
- Streamlit for the UI, layout, caching, and file upload.[1][2]
- Plotly (Express and Graph Objects) for indicators, gauges, bar, and line charts.[1][2]
- DuckDB SQL for in-memory unpivoting and aggregations over monthly columns.[1][2]
- Pandas for reading Excel and dataframe handling.[1][2]

### Project files
The repository includes the app, dependencies, and a sample dataset.[3][1][2]

```text
streamlit_app.py
requirements.txt
Financial-Data-Clean.xlsx
```
