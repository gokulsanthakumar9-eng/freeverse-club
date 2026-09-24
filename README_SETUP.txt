FREEVERSE CLUB — REAL FIREBASE SETUP

1. Firebase Console -> Authentication -> Sign-in method -> enable Email/Password.
2. Firebase Console -> Firestore Database -> Create database.
3. Firestore -> Rules -> paste firestore.rules from this package -> Publish.
4. Firebase Console -> Authentication -> Settings -> Authorized domains -> add:
   - localhost (for local testing)
   - gokulsanthakumar9-eng.github.io (for GitHub Pages)
5. Replace the index.html in your GitHub repository with freeverse_index_working.html and rename it to index.html.
6. Commit the change and wait for GitHub Pages to redeploy.
7. Test Register with a new account, then Sign Out and Sign In again.

What is real in this version:
- Firebase email/password registration and login
- Password reset email
- Persistent user profile stored in Firestore
- Optional public freelancer profile publishing
- Skill filtering
- Portfolio links/projects
- Authenticated contact messages stored in Firestore
- Inbox for received messages
- Event registration stored in Firestore
- Sign out and Firebase auth state handling
- No localStorage password/demo authentication fallback

Important:
The Firebase web API key in a browser app is not a password. Security comes from Firebase Authentication and Firestore Security Rules. Keep the rules published and do not put service-account/private keys in this HTML file.
