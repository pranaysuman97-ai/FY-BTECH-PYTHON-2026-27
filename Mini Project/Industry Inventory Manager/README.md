# Stone Crusher Inventory & Fuel Management

A simple offline app to track materials, fuel purchases, machine fuel usage, and sales
for a small stone crusher business. Built with Python, Streamlit and SQLite.

## Files

- `app.py` — the whole application
- `requirements.txt` — dependencies
- `stone_crusher.db` — created automatically the first time you run the app

## Install

1. Install Python 3.9 or newer from python.org.
2. Open a terminal in this folder and run:

```bash
pip install -r requirements.txt
```

## Run

```bash
streamlit run app.py
```

The app opens in your browser at http://localhost:8501

## How to use

1. **Products & Inventory** — add each item you track (diesel in litres, spare parts in
   pieces, sand in tonnes...). Set a minimum stock level so you get a low-stock warning.
2. **Purchases** — record every bill. Stock goes up automatically.
3. **Usage / Fuel** — record fuel or material issued to a machine (crusher, JCB, truck,
   generator). Stock goes down automatically, and usage above available stock is blocked.
4. **Sales / Dispatch** — record material sold, with buyer, vehicle number and destination.
   Stock goes down automatically.
5. **Dashboard** — totals, low-stock alerts, current fuel stock, recent activity and a
   monthly usage chart.
6. **Reports** — filter by product and date range; shows total usage, average monthly and
   average daily usage, plus full history tables.

## Backup

All data lives in `stone_crusher.db`. Copy that single file to back up or move your data.
