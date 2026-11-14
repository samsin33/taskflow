# Taskflow — Personal Task Manager

A lightweight, responsive task manager with a dashboard, task editor, status filters, and monthly calendar. It uses plain HTML, CSS, and JavaScript — no dependencies or build step required.

## Run locally

1. Download and unzip the project.
2. Open `index.html` in a modern browser.

For a local development server, you can also run:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Deploy to GitHub

1. Create a new repository on GitHub.
2. Extract this ZIP file.
3. Upload `index.html`, `styles.css`, `app.js`, and `README.md` to the repository root (or push them with Git).
4. Commit the files.

## Deploy to Vercel

1. Sign in at <https://vercel.com> and choose **Add New → Project**.
2. Import your GitHub repository.
3. Vercel should detect this as a static site. If it asks for settings:
   - Framework Preset: **Other**
   - Build Command: leave blank
   - Output Directory: `.`
   - Install Command: leave blank
4. Click **Deploy**.

Every push to the connected GitHub branch will trigger a new deployment.

## Features

- Create, edit, complete, reopen, and delete tasks
- Due dates, priority, category, and optional descriptions
- Dashboard with total, completed, pending, due-today, and overdue counts
- Completion percentage and progress visualization
- Monthly calendar with task markers and selected-day agenda
- Search, sort, and status filters
- Responsive desktop and mobile layout

## Data and privacy

Tasks are stored in your browser's `localStorage`. They remain available in the same browser on the same device after refresh or restart, but they are **not synced to other devices** and are not automatically backed up to GitHub or Vercel. Clearing browser data can remove them.

This first version does not include user accounts, a server, or cloud database. For multi-device access and secure backups, connect a backend such as Supabase or Firebase in a future version.

## Project structure

```text
taskflow-manager/
├── index.html
├── styles.css
├── app.js
└── README.md
```
