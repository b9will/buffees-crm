# Buffee's CRM

Lead pipeline & relationship tracker for Buffee's Coffee Corp.

## Setup

### 1. Google Sheet
The CRM reads/writes to a Google Sheet. The sheet should have these headers in Row 1:

```
id | name | contact | email | phone | type | stage | package | revenue | notes | followUp | createdAt
```

### 2. Google Cloud API Key
- Create a project at [console.cloud.google.com](https://console.cloud.google.com)
- Enable the **Google Sheets API**
- Create an API key restricted to Google Sheets API and your GitHub Pages domain

### 3. Deploy
- Push this repo to GitHub
- Enable GitHub Pages (Settings > Pages > Deploy from main branch)
- Access at `https://yourusername.github.io/buffees-crm`

### 4. Passwords
Default passwords are set in `index.html` under `CONFIG.SIMPLE_PASSWORDS`:
- `buffees2026`
- `heather2026`

Change these before deploying.

## Features
- Kanban pipeline view (Cold Lead > Contacted > Meeting Booked > Proposal Sent > Won)
- Table view with search and filtering
- Lead types: Gym, Event/Pop-up, Corporate, Other
- Package tier tracking with revenue estimates
- Follow-up date alerts (overdue / due soon)
- Timestamped activity notes per lead
- All data stored in Google Sheets (accessible from any device)
- Password-gated access
