# Station Guard IBIS Daily Installation Generator

Zero-cost GitHub Pages version for Station Satcom.

## Purpose
Combines two ESET reports into a Station Satcom branded IBIS-ready Excel/CSV output:

1. Device Information / Serial Number report
2. ESET Installation Date report

## Hosting
Upload these files to the `ESET` branch root of the GitHub repository and enable GitHub Pages from that branch.

Required files:

- `index.html`
- `assets/station-guard-logo.png`
- `assets/station-satcom-logo.png`

## Cost
No server, no database, no API, no paid hosting. Runs locally in the user's browser.

## Supported inputs
- CSV
- XLSX
- XLS
- Simple ESET table PDF extraction, when text tables are readable

For production accuracy, scheduled CSV/XLSX export from ESET is recommended.

## Output sheets
- IBIS Ready
- Validation Audit
- Data Quality Review
- Run Summary

## ICCID rule
- Use valid globally unique ESET serial number.
- If serial is blank, placeholder, VMware/virtual, duplicated, missing, or multiple serials exist, generate ICCID from `Vessel_Computer`.
- ICCID removes spaces and hyphens. Underscore separator is retained.
- Collision after cleaning goes to Data Quality Review.
