# Movement Library

A static, mobile-friendly exercise library created from a 23-page scan of rehab exercise handouts. Includes 88 exercise entries, full-page reference images, category search, saved routines, a stretch timer, and local workout history.

## Publish with GitHub Pages

1. Create a **public** GitHub repository named `movement-library`.
2. Upload the **contents** of this folder to the repository root (including the `reference` folder).
3. Open **Settings → Pages** and under **Build and deployment**, choose **Deploy from a branch**.
4. Select `main` and `/ (root)`, then save.
5. After deployment, visit `https://YOUR-USERNAME.github.io/movement-library/`.
6. On iPhone, open the site in Safari, tap Share, and select **Add to Home Screen**.

No accounts, API keys, database, or paid hosting needed. Progress is saved to the browser's localStorage, not synchronized between devices. Export history from the History tab before clearing browser data.

## Accuracy notes

This app contains a manually curated index of exercise titles, grouped by scanned page. Some source pages contain overlapping exercise names, faint text, and handwritten edits. Doses shown in cards are broad handout-level summaries, **not** verified individualized prescriptions. Always review the full reference page before performing a movement. The thumbnails display entire pages rather than individual cropped exercises. This app is informational and not medical advice.

## Run locally

From the project folder: `python -m http.server 8000`, then open `http://localhost:8000`.

## Psoas and hip-flexor additions
Six gentle mobility/relaxation exercises were added under **Psoas & Hip Flexor**. They are new suggestions, not transcriptions of the scanned handouts. Stretching cannot selectively “release” the psoas; avoid forcing motion or provoking radiating pain, tingling, or numbness. Seek individualized advice from a physical therapist if symptoms persist.

## Illustrated exercise demonstrations
Six psoas/hip-flexor exercises now have original simplified SVG positioning sketches and three-step movement guides. Other exercises retain the scanned reference handout images. Illustrations are schematic and should not be treated as clinical demonstrations.


## Guided workouts (v4)

Open **My routine** and tap **Start guided workout**. Follow each exercise using its original scan or available schematic, run a single-hold countdown, mark completed, and move backward/forward. The last step saves the session to device-local history. Closing without finishing does not save. Timers do not automatically advance because repetition counts and stretch holds differ.

**Visuals:** The six added psoas exercises have schematic positioning guides. Exercises transcribed from the 23-page handout show their source page; dedicated photos and videos for all movements have not been added. Do not mistake full-page source scans for individual demonstrations.


## Version 5: running and hamstring programs

16 new exercises (110 total) and 5 one-tap guided programs, including a dynamic pre-run warm-up and a tight-hamstring mobility/strength program. Programs use the same guided player and completion history. These new exercises are general additions, not transcriptions from the scanned handouts. Pre-run warm-ups are dynamic; longer holds are better after running or in separate sessions. If radiating nerve symptoms occur, stop and seek individualized assessment.

## Running day and recovery programs (v6)
Three new guided programs: After Run, Rest Day, and Running Day. Running Day includes a pause for the run between warm-up and recovery movements; use Next when ready. These are general suggestions added to the scanned exercise library.

**Fix:** Corrected exercise-data loading so the app can render the library and programs correctly.


## Version 7: Weekly calendar
Open the **Calendar** tab to assign any of the eight guided programs to individual dates, mark them completed, navigate weeks, and view planned/completed totals and weekly consistency. **Fill empty days with suggested plan** populates a sample schedule without overwriting existing selections. Everything stays in browser localStorage under `movement-calendar-v7`; export in History currently backs up routines and workout history only, not calendar plans. Browser storage is not synchronized across devices.

## Version 8: portable workout backups

Under **History**, use **Export full backup** to download a JSON file with your routine, completed workouts, and weekly calendar. On another device, open the same app and choose **Import backup**. Import replaces the existing saved data on that device, so export a copy first. Data is stored locally and does not automatically sync.

When you start a workout from a calendar day and check off every exercise before finishing, that day is automatically marked complete. Partial sessions remain in History but do not automatically mark the calendar day complete.
