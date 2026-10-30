# VYRA - Food, Diet & Workout Tracker

## Files

- `index.html` - the app
- `firebase-config.js` - Firebase keys
- `firestore.rules` - security rules (publish in Firebase Console)

## Deploy

1. Upload `index.html` and `firebase-config.js` to GitHub Pages (same folder).
2. Firebase Console > Firestore Database > Rules > paste `firestore.rules` > Publish.
3. Firebase Console > Authentication > Settings > Authorized domains > add `darshlabs09.github.io`.

## Make yourself admin (only you)

1. Open the site, sign up / log in with YOUR account.
2. Firebase Console > Authentication > Users > copy your User UID.
3. Firestore Database > Start collection `admins` > Document ID = your UID > add field `enabled` (boolean) = true.
4. Log out and log in again.