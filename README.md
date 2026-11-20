# reset. — updated web app

## Included in this update
- Black-and-orange visual refresh
- Animated XP reward feedback and level-up overlay
- Monthly habit calendar with per-day completion details
- Editable profile: name, age, height, weight, fitness goal and water target
- Existing editable calorie and macro targets
- Progress photo comparison wipe slider
- Barcode lookup through the free Open Food Facts API, with camera scanning where the browser supports BarcodeDetector and manual barcode entry fallback
- Meal-photo capture/review workflow with editable nutrition estimates
- Local-first storage retained for habits, food, meals, weight and progress photos

## Important AI limitation
This build does **not** yet include a trained on-device food-recognition model. The meal-photo screen captures a photo and lets you enter/review identified foods and macros; it does not claim to automatically recognise foods. Integrating a real on-device model is a separate next step and requires selecting and packaging a browser-compatible model that can run within iPhone Safari memory limits.

## Publish/update on GitHub Pages
1. Unzip this archive.
2. Open your existing GitHub repository.
3. Upload and replace `index.html`, `manifest.webmanifest`, and `sw.js` in the repository root (the files inside the `reset_app` folder).
4. Commit the changes.
5. Open the GitHub Pages site in Safari. If the old version remains, close the installed web app, open the site in Safari, refresh, then reopen it from the Home Screen.

## Data and privacy
- Habits, nutrition, meals, profile and weight use browser localStorage.
- Progress photos remain in IndexedDB on the same device/browser.
- Barcode lookup sends the barcode to Open Food Facts to retrieve public product data.
- Meal photos are not uploaded by this starter workflow.
- Clearing Safari website data may erase locally stored app data. Export/backup and cross-device sync are not included.
- The app remains a web app/PWA; no native iOS project is required.
