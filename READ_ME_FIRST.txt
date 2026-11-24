GM2R CORPORATE PORTAL — WEBSITE PACKAGE

Website source: index.html
Firebase database security rules: firestore.rules

GITHUB PAGES:
1. Extract this ZIP on your computer (GitHub Pages does not automatically extract ZIP files).
2. Open https://github.com/gmrreditor01-hue/gm2r-website
3. Replace the repository root index.html with the extracted index.html (do not upload an index (1).html).
4. Keep Settings > Pages set to Deploy from a branch, main, /(root).
5. Check Actions for successful deployment; then refresh https://gmrreditor01-hue.github.io/gm2r-website/

FIREBASE:
The HTML uses Firebase project gm2r-official-portal. For secure editor access, the matching Firestore rules must be published in Firebase Console > Firestore Database > Rules. The admin user document under users/{Firebase Authentication UID} must contain email (string), role = admin (string), active = true (boolean). The Firebase Authentication account must use Email/Password sign-in. Do not upload private credentials or secret keys to GitHub.

IMPORTANT:
- The ZIP is a delivery package, not a file you upload directly as a working website to GitHub Pages.
- This package has not been tested against your live Firebase project. A valid ZIP does not resolve missing Firestore admin approval or incorrect rules.
- Back up existing company data before publishing or restoring cloud records.
- Public viewing means company information synced to portalData can be accessible to anyone with the website link.
