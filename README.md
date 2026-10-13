# Board Meeting Workbench (BMWB)

A lightweight, browser-based project for preparing board meeting packs and company secretary review drafts using structured company data. The app consolidates company details, director records, meeting information, and related-party inputs into a single working interface for generating professional draft documents.

## Overview

This project is designed to streamline the preparation of:

- Board meeting notices
- Agenda drafts
- Attendance summaries
- Director and related-party checklists
- Company secretarial review templates
- Email and document-ready content for internal review

It is built as a static HTML application, which means there is no install step or build pipeline required for day-to-day use.

## Features

- Single-page interface for board-meeting preparation
- Data entry and review for company-level and meeting-level facts
- Director / KMP tracking with appointment, independence, and chairperson status
- Related-party and agenda validation sections
- Draft generation for notice, agenda, and meeting communication content
- Excel-backed input support through structured workbook files
- Browser-based output for quick review and documentation

## Project Structure

```text
BMWB/
├── index.html              # Main application interface
├── Company.xlsx           # Company register / master data
├── Directors.xlsx         # Director and key management personnel data
├── Meetings.xlsx          # Meeting details and event metadata
├── RelatedParties.xlsx    # Related-party and disclosure records
├── agenda-draft.doc       # Agenda draft output
├── attendance-draft.doc   # Attendance summary draft output
├── notice-draft.doc       # Notice draft output
├── email-draft.eml        # Email draft artifact
├── agenda-email-draft.eml # Agenda email draft artifact
├── outlook-draft.eml      # Outlook-ready draft message
├── README.md              # Project documentation
```

## Getting Started

### Option 1: Open directly in browser

1. Navigate to the project folder.
2. Open `index.html` in a modern browser.
3. Use the interface to populate or review data and generate drafts.

### Option 2: Run a local HTTP server

If you prefer serving the app locally:

```bash
cd "c:\RAO\ICSI WEB SERIES\02 - 12-09-2026 - Automation for CompanySecretaries -- Develop your ownApps with AI, No Coding Needed\BMWB"
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## Data Inputs

The app expects structured spreadsheet data to support company secretarial drafting. The following files are included as examples or working templates:

- `Company.xlsx` – company information such as incorporation details, registered address, corporate identity, and contact facts
- `Directors.xlsx` – details of directors, roles, appointment dates, independent status, and chairperson information
- `Meetings.xlsx` – meeting schedule and board meeting metadata
- `RelatedParties.xlsx` – related-party and disclosure tracking data

## Typical Workflow

1. Review or update the company and director workbook data.
2. Load the relevant sheets through the app interface.
3. Validate required fields, statuses, and meeting attributes.
4. Generate the relevant draft notice, attendance, or agenda output.
5. Export or forward the generated document/email content for review.

## Intended Use

This project is intended for internal drafting and review workflows in a company secretarial or governance context. It helps reduce manual effort when preparing board-related communications and formal records.

## Notes

- This application is static and client-side; no backend or database is required.
- It is best suited for browser-based drafting and validation rather than enterprise-scale workflow automation.
- It should be used with clean, validated spreadsheet data for best document quality.

## License

This project does not currently declare a formal license. If you intend to publish or share the repository publicly, add a suitable license before GitHub release.

## Suggested Next Steps

- Add a `.gitignore` file for temporary files and generated artifacts
- Add an explicit project license
- Add a screenshot or sample generated output to the repository
- Optionally convert the workflow into a fuller app if broader automation is required
