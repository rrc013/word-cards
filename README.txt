WORD CARDS - setup steps
========================

What's in this folder
- index.html .............. the game
- manifest.webmanifest .... tells Android it's an installable app (name, icon, colors)
- sw.js ................... lets the app work with no internet once installed
- icons/ .................. app icons
- fonts/ .................. the early-reader font (Andika, free OFL license)

STEP 1 - Put it online with GitHub Pages (free, about 10 minutes, use a computer)
1. Unzip this file on your computer.
2. Go to github.com and create a free account if you don't have one.
3. Click "+" (top right) > "New repository". Name it: word-cards
   Set it to Public, then click "Create repository".
4. On the next page click "uploading an existing file".
   Drag in EVERYTHING from the unzipped folder (index.html, manifest.webmanifest,
   sw.js, README.txt, and the icons and fonts folders). Click "Commit changes".
5. Go to the repository's Settings > Pages.
   Under "Branch" choose "main" and "/ (root)", then Save.
6. Wait 1-2 minutes. Your app will be live at:
   https://YOUR-GITHUB-NAME.github.io/word-cards/

STEP 2 - Install it on the Android phone
1. Open that link in Chrome on the phone.
2. Tap the three-dot menu > "Install app" (or "Add to Home screen").
3. The Word Cards icon appears with her other apps and opens full screen.
   It keeps working without internet after the first open.

OPTIONAL - Get an actual APK file
1. Go to pwabuilder.com and paste your GitHub Pages link.
2. Click "Package for stores" > Android > "Generate Package".
3. Download the zip. Inside is an .apk file you can copy to the phone and open
   to install (Android will ask you to allow installs from that source).
Note: Step 2 already gives you a real app icon and offline play, so most
people never need the APK.

Updating the app later
When you get a new zip, upload just index.html and sw.js to GitHub (Add file >
Upload files > Commit changes). Same names replace the old files automatically.

Changing words later
Open index.html in a text editor and find the list starting with "const WORDS = [".
Each word looks like: ['big','The elephant is big!','🐘'],
(word, sentence, picture). Upload the changed index.html to GitHub again.
