# Offline Notes Lab

A beginner Progressive Web App (PWA) built with React, TypeScript, and Vite.
The app lets you create notes, stores them in the browser using localStorage,
and works fully offline using a service worker.

## Run locally

npm install
npm run dev

## Verify the build

npm run check
npm run build
npm run preview

## PWA test

1. Run npm run build then npm run preview.
2. Open the preview URL (http://localhost:4173).
3. Open DevTools → Application → Service Workers and confirm it shows
   "activated and is running".
4. Check the "Offline" box in the Service Workers panel.
5. Reload the page — the app still loads and displays all notes.
6. Create a new note while offline — it saves successfully.

This confirms the app shell is cached by the service worker and notes
persist via localStorage, satisfying the offline-first requirement.