# Drill Log app

Daily task tracker with 1–10 scores, streaks and a calendar. Plain HTML, CSS and JavaScript, hosted on GitHub Pages and installable on Android.

This repo holds no personal data. Your tasks and log are stored only in your phone's browser.

## Setup

1. **Upload:** create a new **public** repository (repo), for example `drill-log-app`, and upload every file in this folder, including `.nojekyll`.
2. **Pages:** *Settings > Pages*, Source: *Deploy from a branch*, branch `main`, folder `/ (root)`, Save.
   After a minute or two the app is live at `https://<your-username>.github.io/drill-log-app/`.
3. **Install:** open that address in Chrome on your phone, tap the ⋮ menu, then *Add to Home screen* or *Install app*.
4. **Load your tasks:** download `tasks.json` from your private reminders repo to your phone, then in the app open *Tasks > Import task list* and pick it.

## How scoring works

- Score = what you did ÷ target × 10, capped at 10. Target 20 push-ups and you do 10, the score is 5.
- A day counts toward a streak when its score reaches the streak rule (default 5/10, change it in the Tasks tab).
- Each task has its own streak. The big number at the top is the overall streak, using the average score of the day.
- Days a task is not scheduled never break its streak.

## Good to know

- Use **Download backup** in the Tasks tab every week or two. Clearing Chrome's site data erases the log.
- After changing tasks in the app, tap **Copy reminder file** and paste it over `tasks.json` in the reminders repo.
