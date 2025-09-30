# Online Fun Service — Firebase Multi-page App (ZIP)

This package contains a multi-page static app that uses Firebase (Realtime Database, Auth, Storage) to implement a demo of the Online Fun Service.

## Files included
- index.html
- register.html
- login.html
- user-dashboard.html
- model-dashboard.html
- call.html
- chat.html
- admin-login.html
- admin-dashboard.html
- firebase.rules
- firebase.json

## Quick setup
1. Create a Firebase project in the Firebase console.
2. Enable Authentication (Email/Password). For production, use Phone Auth.
3. Create a Realtime Database and Storage bucket.
4. Replace the placeholder `firebaseConfig` values in each HTML file with your Firebase project's config.
5. (Optional) Adjust `firebase.rules` and deploy rules via Firebase console or CLI.
6. Deploy:
   - Using Firebase Hosting: `firebase init` (choose Hosting) then `firebase deploy --only hosting`
   - Or upload files to any static host, but ensure Firebase Realtime DB and Auth are configured.

## Notes
- This is a front-end-only scaffold. Payments are simulated. For secure payments integrate Stripe/Razorpay via Cloud Functions.
- WebRTC signaling uses Realtime Database; for production use TURN servers (coturn) for reliability.
- Create an admin by registering a user and setting `/users/{uid}/role = 'admin'` in Realtime DB.

Admin contact in app: onlinefunservice365@gmail.com

