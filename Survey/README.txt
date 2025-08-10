Colorful NC II Survey - Instructions

1. Unzip the package.
2. Edit firebase-config.js with your Firebase Web App config.
   - Enable Cloud Firestore and Authentication (Email/Password) in Firebase Console.

3. (Optional) Deploy Google Apps Script and set config.json.appsScriptUrl.

4. Test locally using a simple server:
   python -m http.server 8000
   visit http://localhost:8000

5. To deploy to Firebase Hosting:
   npm install -g firebase-tools
   firebase login
   firebase init hosting
   # set public directory to the folder containing these files
   firebase deploy

6. Admin: go to Admin page to create an admin account (uses Firebase Auth).
7. Edit questions: open questions.json and modify text/options. Redeploy after changes.

Security note: For production, secure Firestore rules to restrict reading/writing to authorized users as needed.
