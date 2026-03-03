# System Architecture

1. User submits lead data into Google Sheet.
2. Apps Script scans unprocessed rows.
3. Script constructs structured LLM prompt.
4. Lead data is sent to LLM API.
5. Model returns structured JSON output.
6. Script parses JSON.
7. Spreadsheet is updated with:
   - Score
   - Priority
   - Category
   - Suggested reply
   - Timestamp
   - Status flag
