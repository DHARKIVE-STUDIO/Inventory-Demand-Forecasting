# Inventory Demand Forecasting

Built with AI assistance. The sales data is simulated (one store, 30 products, 156 weeks, 2023 to 2025) because no real store file was available. Results describe the simulation, not a real store.

## What is in this folder
- `data/sales_raw.csv`: simulated raw sales. This is the only input.
- `inventory_forecast_simple.ipynb`: the full analysis. Cleaning, EDA, six forecasting methods, reorder simulation and results.
- `outputs/business_report.docx`: the business report (problem, data, results, products at risk, limitations, next steps).
- `outputs/`: forecasts, reorder table, accuracy and cost tables, and charts. Written by the notebook when it runs.
- `data/sales_clean.csv`: cleaned data. Written by the notebook when it runs.
- `data/RAW_DATA_NOTE.txt`: how the raw file was made.

## How to run
1. `pip install -r requirements.txt`
2. Keep `data/sales_raw.csv` in the `data/` folder.
3. Open `inventory_forecast_simple.ipynb` and run all cells top to bottom.

## Notes
- Demand in the reorder simulation is recorded sales. Stockouts hide some demand, so those results favour low stock levels.
- Margin (30%) and carrying cost (25%) are assumptions. Replace them with real figures before using the buffer results.
