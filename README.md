# S&P 500 Stock Segmentation (RFM + Risk/Return)

**Student:** Haritha Shavina Thillainathan (20836733)
**Module:** 6BUIS017W – CRM and CM with Business Intelligence
**Final notebook:** `CWK1_SP500_Analysis.ipynb`

## Study details
- Study period: 1 Jan 2021 – 31 Dec 2024 (end date excluded)
- Observation date: 31 December 2024
- Constituent list retrieved: 24/11/2026 (Wikipedia); prices downloaded 24/11/2026 (Yahoo Finance via yfinance)
- Shares retained: 486 of 503 (17 excluded, reasons in `outputs/share_selection_log.csv`)

## Repository contents
- `snapshots/` – the saved input data from the 24/11/2026 run: `sp500_tickers.csv`, `market_data_raw_2021_2024.csv.gz`, `acquisition_metadata.json`, `download_log.csv`, `download_retry_log.csv`
- `outputs/` – result tables and run records (see Key outputs)
- `requirements.txt` – package versions

## How to run
1. Open `CWK1_SP500_Analysis.ipynb` in Google Colab.
2. **To reproduce the reported results:** upload the files from `snapshots/` into `/content/CWK1_outputs/` (create the folder if needed). The notebook reuses saved files when it finds them.
3. **To download fresh data instead:** run without uploading anything. Live data will differ from the reported results.
4. Run All. All files are written to `/content/CWK1_outputs/` (Colab) or `cwk1_outputs/` (local). Colab deletes these when the session ends, so download what you need.

## Key outputs
- `share_features_and_assignments.csv` – features plus four cluster labels
- `share_selection_log.csv` – inclusion and exclusion reasons
- `weekly_return_pair_correlations.csv` – return correlation summary used in 3.2.3
- `run_details.json` and `package_versions.csv` – full settings and package versions
