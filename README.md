# Adult ESL AI Bridge/ICAPS Student Success Dashboard

This is an aggregate, class-level dashboard prototype for an adult education AI Bridge/ICAPS program.

The dashboard is designed for administrator review through GitHub Pages without publishing individual student information.

## Important Privacy Note

This public dashboard should not include:

- Student names
- Student ID numbers
- Individual attendance records
- Individual course progress records
- Student-level risk indicators
- Teacher notes
- Support needs
- Raw student data
- Private Excel workbooks

Only aggregate class-level results should be displayed.

## Current Status

The values in the current dashboard are illustrative preview placeholders only.

They are not official program results and should be replaced with verified aggregate results before publication.

## Files

- `index.html` - the GitHub Pages dashboard file
- `dashboard-summary.json` - aggregate class-level results exported from the private Excel tracker; upload this only after reviewing it
- `excel-to-dashboard-export.html` - local browser tool for creating `dashboard-summary.json`
- `vendor/jszip.min.js` - local spreadsheet-reading library used by the export tool
- `README.md` - this project description

The private Excel Student Success Tracker should not be published to GitHub Pages when it contains real student information.

## Beginner Update Workflow

1. Open `excel-to-dashboard-export.html` in your browser.
2. Click Choose Excel File.
3. Select the private Excel Student Success Tracker from your computer.
4. Click Generate Dashboard Summary.
5. Review the aggregate preview.
6. Download `dashboard-summary.json`.
7. Upload `dashboard-summary.json` to the same GitHub repository as `index.html`.

The Excel file is processed in the browser. It is not uploaded by the export tool.

The export tool uses the local `vendor/jszip.min.js` file to read `.xlsx` files. Because that library is included in this project folder, the export tool can work offline as long as `excel-to-dashboard-export.html` and the `vendor` folder stay together.

## Dashboard Sections

The dashboard displays aggregate results for:

- Participation and Persistence
- Google AI Essentials
- Digital Readiness Growth
- Workforce Preparation
- Northstar Digital Literacy
- Program Highlights

## Dashboard Measures and Privacy Approach

Participation and Persistence displays total students started, Bridge attendance, Bridge completion, ICAPS attendance, and ICAPS completion as class-level counts and averages.

Google AI Essentials displays average courses completed at the midpoint, average courses completed at the end, and the number of students earning the Google AI Essentials certificate. Course progress and certificate attainment are separate outcomes.

Digital Readiness Growth displays baseline average, follow-up average, and average growth from the existing Digital Readiness Tracker. The public dashboard should not include student-level assessment results.

Workforce Preparation displays resume and cover letter completion counts only.

Northstar Digital Literacy displays the number of students earning at least one Northstar certificate and the total number of Northstar certificates earned by the class. It should not rank students or show individual certificate totals.

Program Highlights is an editable narrative section for two or three verified accomplishments. Planned activities should not be presented as completed.

## Reporting Notes

Bridge and ICAPS are reported separately while representing one continuous 12-week program.

Google AI Essentials course progress and certificate attainment are reported separately.

Digital readiness results should come from the existing Digital Readiness Tracker as summary results, not from new student-level assessments.

Northstar Digital Literacy is reported as voluntary achievement, using class-level certificate totals only.

## Dashboard Data Source

The public dashboard reads aggregate results from `dashboard-summary.json`.

If no verified JSON file has been uploaded yet, the dashboard displays Not Yet Reported instead of sample results.
