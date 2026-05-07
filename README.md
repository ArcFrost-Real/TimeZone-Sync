# TimeZoneSync - Meeting Planner

Find the perfect meeting time across time zones. No signup, no ads, runs entirely in your browser.

## Features

- Visual 24-hour timeline showing all selected time zones
- Working hours highlighted in green
- Automatic overlap detection with coverage scoring
- Add to Calendar (ICS download) or Google Calendar
- Share configuration via URL
- Dark mode
- Works offline after first load

## Deploy to GitHub Pages (Free, No Phone Verification)

### Method 1: Upload via Web UI (No Git needed)

1. Go to https://github.com/new and create a new repository
2. Name it `timezonesync` (or whatever you want)
3. Make it **Public**
4. Check "Add a README file" and click **Create repository**
5. Click **Add file > Upload files**
6. Upload `index.html` from this project
7. Click **Commit changes**
8. Go to **Settings > Pages**
9. Under "Source", select **main branch** and folder **/(root)**
10. Click **Save**
11. Wait 1-2 minutes. Your site will be live at `https://YOURUSERNAME.github.io/timezonesync/`

### Method 2: Using Git CLI

```bash
# Create a new repo on GitHub first

git init
git add index.html
git commit -m "Initial commit: TimeZoneSync meeting planner"
git branch -M main
git remote add origin https://github.com/YOURUSERNAME/timezonesync.git
git push -u origin main
```

Then enable Pages in Settings > Pages > Source: main branch.

### Custom Domain (Optional)

1. Add a `CNAME` file to the repo root with your domain name
2. Add the file content: `yourdomain.com`
3. Configure DNS with your domain provider

## Local Usage

Just open `index.html` in any modern browser. No server required.

## Project Structure

```
timezonesync/
├── index.html    (main app - single file, zero dependencies)
├── test.html     (unit tests)
└── README.md     (this file)
```

## Tech Stack

- HTML5 / CSS3 / Vanilla JavaScript
- Intl API for timezone conversions
- Zero external dependencies
