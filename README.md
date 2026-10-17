# Oli Evaluation Dashboard

## Run on Windows / VS Code
1. Extract this folder.
2. Open it in VS Code.
3. Open Terminal in this folder.
4. Install dependencies:
   ```powershell
   python -m pip install -r requirements.txt
   ```
5. Start the dashboard:
   ```powershell
   python -m streamlit run app.py
   ```
6. Open the local URL Streamlit prints (usually http://localhost:8501).

Or double-click `run_dashboard.bat`.

## Features
- Summary metrics: total, passed, failed, average score
- Pass/fail and per-case score charts
- Search and filter by result and fixture type
- Detailed tool-routing and safety checks per case
- CSV and JSON report downloads

## Important
This dashboard scores the transcript fixtures supplied in `transcripts.json`. It does not call Oli or run live model tests. The package contains one conversation-reconstructed fixture and synthetic demonstration fixtures. Replace synthetic fixtures with real exported transcripts before claiming real-world evaluation results.
