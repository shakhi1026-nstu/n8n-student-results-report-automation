# n8n-student-results-report-automation
An n8n workflow that reads student marks From CSV , validates and cleans the data, generates summary statistics and emails the report via Gmail.
## What it does
1. Reads a CSV file of student marks
2. Extracts the data from the file
3. Validates makes and classifies each record as **Pass / Fail / Missing / Invalid**
4. Remove duplicate records
5. Generates statistical summaries
6. Builds a text report and saves it to a '.txt' file
7. Sends the report by email using Gmail.
## Tool used 
- n8n (local installation on windows)
- JavaScript (code nodes)
- Gmail integration
- CSV / text files
  
## Workflow Overview
> Screenshot will be added in `/images`

## Sample Input

| Name | Marks |
|------|-------|
| Student A | 78 |
| Student B | 35 |
| Student C | |

## Sample Output
Total students: [ ]
Pass: [ ]
Fail: [ ]
Missing: [ ]
Invalid: [ ]
Average marks: [ ]
## How to Run

1. Install n8n locally
2. Import `workflow.json` from this repository
3. Connect your own Gmail credentials in n8n
4. Add your own sample CSV file and update the file path
5. Click **Execute Workflow**

## Limitations

- Runs manually on a local machine
- Works only with the specific CSV format used here
- Pass mark and validation rules are fixed in the workflow

## Future Improvements

- Add a scheduled trigger
- Support more CSV formats
- Add charts to the report
- Connect with the AI Student Report Analyzer

## Author

Fatema Yeasmin Shakhi | Statistics student @ NSTU 
