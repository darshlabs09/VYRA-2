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
4. Log out and log in again. An "Admin" tab appears (only for you). Before that, Goals page > "Owner access" shows your User ID with a Copy button.

Admin tab shows all registered users, their plan and activity, Pro requests,
and lets you switch Pro on/off and export the list.
