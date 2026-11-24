# Print Ops – PWA Version (Ready for APK)

This folder contains a Progressive Web App version of your Print Sampling + Printer Maintenance app.

## Files
- `index.html` – Main app
- `manifest.json` – PWA configuration
- `sw.js` – Service Worker (basic offline support for the app shell)
- `icons/` – Put your app icons here

---

## Step 1: Add Icons (Required for good APK)

You need two PNG icons:

1. **icon-192.png** (192×192 pixels)
2. **icon-512.png** (512×512 pixels)

### Easy ways to create icons:
- Go to → https://favicon.io/favicon-generator/  
  or https://www.pwabuilder.com/imageGenerator  
  or https://icon.kitchen/

- Use text “PO” or a printer emoji, dark blue background (#0f172a), white icon.
- Download the 192 and 512 sizes.
- Place both files inside the `icons` folder:
  ```
  icons/icon-192.png
  icons/icon-512.png
  ```

---

## Step 2: Host the App (Important)

PWABuilder needs a public HTTPS URL.

### Easiest free hosting options:

**Option A – Netlify Drop (Recommended, no account needed for quick test)**
1. Go to https://app.netlify.com/drop
2. Drag the entire `print-app-pwa` folder
3. You will get a link like `https://random-name.netlify.app`

**Option B – GitHub Pages / Vercel / Cloudflare Pages** (also free)

---

## Step 3: Generate APK using PWABuilder

1. Open → **https://www.pwabuilder.com/**
2. Paste your hosted app URL (from Step 2)
3. Click **Start**
4. Wait for the score to appear
5. Click **Package For Stores**
6. Choose **Android**
7. Click **Generate**
8. Download the **Android package**

You will get:
- An `.apk` file (for direct install)
- Or a bundle for Play Store

### Install the APK on phone:
1. Transfer the `.apk` file to your Android phone
2. Open it → Allow “Install from unknown sources” if asked
3. Install

---

## Step 4: Test “Add to Home Screen” (Optional)

Even without APK, after hosting:

- **Android Chrome**: Open the site → Menu → “Install app” or “Add to Home screen”
- **iPhone Safari**: Share button → “Add to Home Screen”

It will open like a real app (full screen, no browser bar).

---

## Notes

- The app still needs internet for Google Apps Script (data + photos).
- Service Worker caches the app shell so it opens faster.
- After generating APK, you can share the same APK with Manager, Sampling Department and Maintenance team.

---

Need help with any step? Just tell me where you got stuck.
