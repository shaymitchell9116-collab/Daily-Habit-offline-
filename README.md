# Habitly — Daily Habit Tracker

A responsive daily habit tracker designed around the uploaded UI reference.

## Features
- Add, edit, and delete your own habits
- Choose a category, emoji, colour, and reminder time
- Mark habits complete for today
- Daily completion count and progress bar
- Browser notifications for scheduled reminders
- Saves habits in the browser using localStorage
- Responsive layout for phones and desktop

## Publish with GitHub Pages
1. Create a new repository on GitHub (for example, `habit-tracker`).
2. Upload `index.html` to the root of the repository.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then save.
6. Wait for GitHub to publish the site. Your website URL will appear in the Pages section.

## Important reminder limitation
This is a static website, so browser reminders work while the website is open in a browser tab. Notifications require HTTPS (GitHub Pages provides HTTPS) and permission from the user. If the browser is closed or the device stops the page in the background, reminders may not fire. Reliable reminders while the site is fully closed require a push-notification service and a backend/ push subscription setup.

## Data
Habits are stored locally in the browser on the device where you use the site. Clearing browser site data or switching devices will not transfer your habits.


## Offline / installable app update
This version is a Progressive Web App (PWA). After uploading these files to the same GitHub Pages repository and opening the site once while online, the service worker caches the app shell. On later visits, the app can open offline. Habits continue to be stored in browser localStorage on this device.

On Android Chrome, open the site and use the **Install app** prompt/button if shown, or browser menu → **Install app** / **Add to Home screen**.

Important: the first visit must be online so the app can be cached. Browser notifications are not guaranteed while the app is fully closed; reliable scheduled background notifications require push notifications plus a server-side push service. Offline use does not sync data between devices.
