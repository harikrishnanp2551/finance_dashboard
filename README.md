
### Sales Streamlit Dashboard
A minimal, interactive dashboard for sales/finance data built with Streamlit, Plotly, Pandas, and DuckDB

Access the dashboard at : https://harikrishnanp2551-finance-dashboard-streamlit-app-dfaquo.streamlit.app/

### Features
- Upload an Excel workbook from the sidebar to load data into the app.
- Expandable data preview with basic column configuration for Year.
- KPI cards and gauges for key metrics (e.g., Accounts Receivable/Payable, Equity Ratio, Debt Equity, Current Ratio, stock days, delay).
- Grouped bar chart of 2023 Sales by business unit and Scenario.
- Monthly Budget vs Forecast line chart for 2023 (Software business unit).
- Bar chart of Actual yearly totals by Account across years (non-Sales accounts).

### Data input
- Expected file type: .xlsx read via Pandas with openpyxl in the environment.
- Expected columns include: Account, business_unit, Currency, Year, Scenario, and monthly columns Jan–Dec.
- Example rows include Sales and various expense accounts across business units like Software, Advertising, and Hardware.

### Quickstart
1) Install dependencies from requirements.txt.
2) Run the app with Streamlit.

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

3) In the app sidebar, use “Choose a file” to upload the Excel data.
4) Explore the data preview and the charts laid out in the two-row dashboard.

### Tech stack
- Streamlit for the UI, layout, caching, and file upload.
- Plotly (Express and Graph Objects) for indicators, gauges, bar, and line charts.
- DuckDB SQL for in-memory unpivoting and aggregations over monthly columns.
- Pandas for reading Excel and dataframe handling.

### Project files
The repository includes the app, dependencies, and a sample dataset.

```text
streamlit_app.py
requirements.txt
Financial-Data-Clean.xlsx
```
