# Excellent Mind Tutorial Centre — Fee & Payment Dashboard

A self-contained student management dashboard built for a private tutorial centre, covering student enrollment, fee tracking, payments, expenses, receipts, and reporting.

**Live Demo:** https://elijahbonny23-byte.github.io/tutorial-centre-dashboard/

## Features

- **Student enrollment** — track name, exam type (JAMB/WAEC/NECO/IJMB/POST-UTME/GCE), department, and total fees
- **Payment recording** — log payments by method (cash, transfer, POS, other) against each student
- **Expense tracking** — log day-to-day operating expenses
- **Live dashboard** — fees expected, amount paid, outstanding balances, and net cash position, updating automatically
- **Printable receipts** — generate a formatted, print-ready payment receipt for any transaction
- **Reports** — summarized views across students, payments, and expenses for a selected date range
- **Secure login** — password-protected access with salted, SHA-256 hashed credentials (no plaintext storage) and an in-app password change flow
- **Native Excel export** — a dependency-free `.xlsx` export engine built from scratch (workbook/sheet XML, zip packaging, byte-level encoding) for student, payment, expense, and financial summary reports — no spreadsheet library required
- **Backup & restore** — export all records to a JSON file and restore them on any device, plus configurable auto-backup to a local folder (where supported by the browser) with a settings panel to manage backup frequency and retention
- **Offline-first** — runs entirely in the browser with no server or internet connection required

## Tech

Built with React, bundled into a single HTML file using esbuild so it runs directly in any browser with zero setup or install. Data persists locally via the browser's `localStorage`, and the Excel export pipeline is implemented natively in JavaScript without any third-party spreadsheet library.

## Running it

No installation needed — download `excellent-mind-app-offline.html` and open it in any browser.

## Notes

This project was built using AI-assisted development (Claude) to accelerate implementation, with the data model, feature set, and UX directed throughout the build.
