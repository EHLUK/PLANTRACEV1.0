# PlanTrace

**Planning intelligence for project delivery teams.**

Trace logic. Expose risk. Drive delivery.

---

## What is PlanTrace?

PlanTrace is a Primavera P6 XER programme analysis tool that lets Project Managers, Project Leads, Project Controls Managers and Directors interrogate a schedule without opening P6.

Upload a `.xer` file and immediately get:

- Executive Summary with risk assessment
- Critical path analysis
- Negative float and near-critical tracking
- Logic trace (predecessors and successors)
- Labour demand histograms
- Programme health checks
- WBS risk heatmap
- Milestone tracker
- Lookahead planner
- PM Action list
- Risk & Opportunity register
- Programme comparison (two XER revisions)
- PM Mode / Planner Mode toggle

---

## Deployment

### Streamlit Cloud (recommended)

1. Fork or push this repo to GitHub
2. Go to [share.streamlit.io](https://share.streamlit.io)
3. Connect the repo, set `app.py` as the main file
4. Deploy — dependencies install automatically from `requirements.txt`

### Local

```bash
pip install -r requirements.txt
streamlit run app.py
```

---

## How to export from Primavera P6

1. Open P6
2. File → Export
3. Select **Primavera P6 XER** format
4. Choose the project(s) to export
5. Save the `.xer` file
6. Upload to PlanTrace using the sidebar uploader

---

## Dependencies

| Package | Purpose |
|---|---|
| streamlit | Web framework |
| pandas | Data manipulation |
| plotly | Charts and Gantt views |
| networkx | Logic network graph |
| openpyxl / xlsxwriter | Excel export |
| python-docx | Word document export |
| xerparser | P6 XER file parsing |

---

## Pages

| Page | Description |
|---|---|
| Overview | KPI summary, PM Attention panel, Readiness Check, WBS Heatmap |
| Executive Summary | Plain-English narrative, Top 5 points, Recommended Actions, Word/Excel export |
| Programme | Activity Search, Lookahead, Milestones, Planning Notes |
| Logic | Logic Trace, Path to Selected Activity |
| Critical Path | Full critical path, near-critical, negative float |
| Labour | Weekly/monthly histograms, resource and WBS views |
| Health Check | 11 automated schedule quality checks |
| Comparison | Programme Movement, Risk & Opportunity Register |
| PM Actions | Auto-generated prioritised action list |
| Risk Register | Auto-generated risk and opportunity register |
| Reports | Export all data to Excel |

---

## Modes

**PM Mode** — Plain English descriptions, simplified tables, "What this means" boxes.

**Planner Mode** — Full technical detail: relationship types, lag, calendars, constraints, raw schedule fields.

Toggle in the sidebar.

---

*PlanTrace — No P6 licence required.*
