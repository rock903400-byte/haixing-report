# AGENTS.md

Static HTML report served via GitHub Pages. No build step, no dependencies.

## Deployment

Push to `master` → GitHub Pages auto-deploys to https://rock903400-byte.github.io/haixing-report/

## Content

`index.html` = 海星社理事會報告 (board report for elderly readers). Edit directly.

## Key Constraints

- **Target audience**: elderly board members reading on mobile phones
- **Design**: large fonts (18px+ body), single-column mobile-first, high contrast, no animations
- **Language**: Traditional Chinese; avoid English abbreviations and harsh/warning tone

## Data Verification

Source data lives in parent workspace `C:\Users\user\Desktop\穿透\下載工具\`:
- `exported_data.csv` — financial data (逾期, 放款, 業務費用)
- `資料庫.xlsx` — 社員數, 股金, 貸放比, 儲蓄率 (NOT in CSV)
- `verify_data.py` — run `python verify_data.py` after any data changes

**Important**: 貸放比 values come from `資料庫.xlsx`, not computed from CSV. Do not recalculate.
