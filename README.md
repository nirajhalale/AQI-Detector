# AirScope — Professional AQI Dashboard

## Files
- `app.py` — Streamlit front end/dashboard
- `aqi_backend.py` — your original AQI logic, made importable by removing the command-line loop
- `requirements.txt` — Python dependencies

## Run locally
1. Install Python 3.10 or newer.
2. Open a terminal in this folder.
3. Run:
   ```bash
   python -m pip install -r requirements.txt
   streamlit run app.py
   ```
4. A browser tab should open with the dashboard.

## Data notes
The backend tries live Open-Meteo data first, then `aqi_real_data.csv`, then simulated demo data. If demo data is used, the dashboard displays a warning. If you have `aqi_real_data.csv`, put it in this same folder.

## Important
The existing AQI interpolation and forecasting model are retained from the supplied script. Treat forecasts as educational estimates, not official health or emergency guidance.
