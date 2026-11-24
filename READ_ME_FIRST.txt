GM2R CORPORATE PORTAL — PUBLIC VIEWING FIX (24 NOV 2026)

The website opens in PUBLIC VIEWER MODE with no password popup.
Only clicking the UNLOCK EDITING navigation button shows the editor password form.

Two authorized Firebase Authentication editor accounts:
- gmrr.editor01@gmail.com
- gmrr.adm01@gmail.com

UPLOAD TO GITHUB PAGES
1. Extract this ZIP file on your computer.
2. Open https://github.com/gmrreditor01-hue/gm2r-website
3. Replace the existing index.html with the index.html inside this ZIP, and commit changes.
4. GitHub Settings > Pages: main branch, /(root). Check Actions for a green successful deployment.
5. Open https://gmrreditor01-hue.github.io/gm2r-website/ in a PRIVATE/INCOGNITO window.
6. You should see Home/KPI/Calendar/Leaderboard/Chart without any password prompt.
7. Click UNLOCK EDITING to test the password form.

FIREBASE: Uploading firestore.rules to GitHub DOES NOT apply Firestore rules.
Paste the contents of firestore.rules into Firebase Console > Firestore Database > Rules > Publish.
For each approved account, create a users/{Firebase Authentication UID} document in Firestore with
  email: corresponding Gmail (string)
  role: admin (string)
  active: true (boolean)
Both accounts must already exist in Firebase Authentication with Email/Password sign-in.
The passwords are not stored in the website files. The password-only UI tries the listed Firebase accounts.

IMPORTANT: The dashboard is PUBLIC-READ by design and may show employee data to anyone with a link.
Do not publish confidential employee information to the public portal.
The site may not synchronize until Firebase rules and admin records are configured.
Make a full backup from your existing data browser before updating.
