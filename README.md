# License Inspection Dashboard

Single-file, offline dashboard for inspecting operational license CSV data.

## Overview

This project provides a browser-based dashboard in `index.html` with:

- KPI summary cards
- CSV import (file picker and drag-and-drop)
- Filtering and free-text search
- Priority queues (upcoming expiries and no-inspection records)
- Offline SVG charts
- CSV export of the current filtered table

No backend or build step is required.

## Getting started

1. Open `index.html` in a web browser.
2. Click **Load CSV** (or drag/drop a CSV file into the drop zone).
3. Use filters and table sorting to inspect records.
4. Click **Export current table to CSV** to download filtered results.

## Expected CSV columns

The dashboard expects these headers:

- `Business_Area`
- `Field_Team`
- `Management_Unit`
- `Licence_ID`
- `Tenure`
- `Registrant`
- `Licence_State`
- `Licence_Issued_Done_Date`
- `Licence_Substantial_Completion_Done_Date`
- `Licence_Current_Expiry_Date`
- `Logging_Started_Activity_Done_Any_Block_In_Licence`
- `First_HBS_Scale_Date`
- `Latest_HBS_Scale_Date`
- `First_Prework_Any_Type_Done_Date`
- `First_Inspection_Any_Type_Done_Date`
- `Latest_Inspection_Any_Type_Done_Date`
- `Latest_Inspection_Final_Done_Date`
- `Latest_Inspection_Obligations_Complete_Done_Date`
- `Count_Inspection_Any_Type_Done`
- `Days_Since_Latest_Inspection`
- `Days_Since_Latest_Prework_or_Inspection`

`Tenure` should contain the tenure/category value provided by your source licensing dataset.

## Project structure

- `index.html` — complete application (HTML, CSS, and JavaScript)
- `README.md` — project documentation
