# Station Guard Installation Report Generator

Zero-cost GitHub Pages tool for Station Satcom.

## Hosting
Upload these files to the root of the `ESET` branch and enable GitHub Pages from branch `/root`:

- `index.html`
- `assets/station-guard-logo.png`
- `assets/station-satcom-logo.png`

## Output
The tool generates one Station Satcom formatted Excel report with:

- Installation Report
- Validation Audit
- Run Summary

The report columns are:

- CUSTOMER NAME
- VESSEL NAME
- DEVICE NAME
- SERIAL NUMBER
- INSTALLATION DATE

Installation Date is exported in `DD-MM-YYYY HH:MM` format.

## Notes
- No server
- No database
- No paid hosting
- Browser-based processing
- CSV/XLSX recommended for production accuracy
