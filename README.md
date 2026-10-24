# Daily Routine Tracker

A simple, private app to track your daily routine:

- **Sleep**: enter the time you fell asleep and woke up, sleep hours are calculated for you (works past midnight).
- **Food**: add as many meals as you like per day (breakfast, lunch, snack, evening meal, dinner), with calories and protein. Daily totals are added up.
- **Weight**: log it daily and see the change.
- **Daily photo**: take or choose one photo a day, then compare any two days on the Progress tab.
- **History** and **Insights**: all your days, averages, weekday patterns and charts against your own goals.

There is no server and no account. It is plain HTML, CSS and JavaScript.

## Run it

Just open `index.html` in a browser (double-click it). Works best in Chrome, Edge, Safari or Firefox.

To use it on your phone like an app, put the folder on any static host (see below), open the link on the phone, and choose **Add to Home Screen**.

## Put it on GitHub (free hosting with GitHub Pages)

1. Create a new repository on GitHub and upload everything in this folder.
2. In the repository, go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then save.
4. After a minute your app is live at `https://<your-username>.github.io/<repository-name>/`.

## Where your data is stored

Entries and photos are saved in the browser on the device you use (localStorage), so they stay private and need no internet. That also means:

- Data is **per browser and per device**. Your phone and laptop do not share entries.
- Clearing site data deletes it.
- Photos are shrunk to about 480 px to save space. Browsers allow roughly 5 MB, which is around 100 to 150 photos.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest`, `icon-*.png`, `icon.svg` | Phone install details and icons |
| `sw.js` | Lets the app open offline |
| `excel/Daily_Routine_Tracker.xlsx` | The original Excel version with auto sleep hours and a dashboard |

## Change the look

Colours live in the `:root` block at the top of the `<style>` in `index.html`. Edit those values and everything follows, including dark mode.
