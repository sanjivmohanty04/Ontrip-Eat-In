# Ontrip Eat-In

A restaurant table booking app for Indian and Thai/International restaurants across Thailand.

## Live Site
https://YOUR-USERNAME.github.io/ontrip-eatin/

---

## Setup Instructions

### Step 1 — Google Apps Script (Save bookings to Google Sheet)

1. Go to https://script.google.com → **New Project**
2. Delete all code → paste contents of `Code.gs`
3. Click **Deploy → New deployment**
4. Click the ⚙️ gear → select **Web app**
5. Set:
   - Execute as: **Me**
   - Who has access: **Anyone**
6. Click **Deploy** → **Authorize access** → allow all permissions
7. Copy the **Web app URL**

### Step 2 — Add URL to the app

Open `index.html` and find this line near the top of the `<script>` section:

```js
var APPS_SCRIPT_URL = "YOUR_APPS_SCRIPT_URL_HERE";
```

Replace `YOUR_APPS_SCRIPT_URL_HERE` with your copied URL. Example:

```js
var APPS_SCRIPT_URL = "https://script.google.com/macros/s/AKfycbx.../exec";
```

Save the file.

### Step 3 — Host on GitHub Pages

1. Go to https://github.com → **New repository**
2. Name it: `ontrip-eatin`
3. Set to **Public** → click **Create repository**
4. Upload `index.html` (drag and drop into the repository page)
5. Go to **Settings → Pages**
6. Under **Source**, select **Deploy from a branch**
7. Branch: **main** | Folder: **/ (root)** → click **Save**
8. Wait ~60 seconds → your site is live at:
   `https://YOUR-USERNAME.github.io/ontrip-eatin/`

---

## Files

| File | Purpose |
|------|---------|
| `index.html` | The complete app (upload this to GitHub) |
| `Code.gs` | Google Apps Script (paste into script.google.com) |

---

## Features
- 36 restaurants across Bangkok, Phuket, Chiang Mai, Pattaya, Koh Samui, Hua Hin
- Filter by city, cuisine type, and category (Indian / Thai-International)
- Live search
- Table booking form with confirmation
- Bookings auto-saved to Google Sheets
- Google Maps links for every restaurant
- Fully mobile responsive
