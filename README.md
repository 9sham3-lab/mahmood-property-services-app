# Mahmood Property Services app

Jobs, customers, quotes, invoices, expenses, pricing, calculators and the kitchen planner in one app.
It runs in the phone's browser and can be installed on the home screen like a normal app.

## What is in this folder

| File | What it is |
|---|---|
| `index.html` | The whole app (all the code is in this one file) |
| `manifest.webmanifest` | Tells the phone this can be installed, and gives its name and colours |
| `sw.js` | Lets the app open quickly and work without a signal |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` | The home screen icons (your logo's house) |
| `README.md` | These instructions |

Keep all of these files together in the same place, with exactly these names (all lowercase).

## Put it on GitHub and turn it into a phone app

You need a free GitHub account (github.com). This works from a computer or from a phone browser.

### 1. Create the repository
1. Sign in to GitHub and tap **+** then **New repository**.
2. Name it something simple, for example `mahmood-app`.
3. Choose **Public**. (GitHub Pages is free for public repositories. The repository only holds the app, never your customers or invoices.)
4. Tick **Add a README file** if you like, then tap **Create repository**.

### 2. Upload the files
1. In the repository, tap **Add file** then **Upload files**.
2. Select every file from this folder (`index.html`, `manifest.webmanifest`, `sw.js`, the four `.png` icons and `README.md`).
3. Scroll down and tap **Commit changes**.

Do **not** upload `Mahmood-data-backup-PRIVATE.json`. That file contains your customers and invoices. It is only for your own phone.

### 3. Switch on GitHub Pages
1. In the repository, open **Settings**, then **Pages** in the left menu.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Set **Branch** to `main` and the folder to `/ (root)`, then tap **Save**.
4. Wait one or two minutes and refresh the page. A green box shows your address, which looks like
   `https://YOUR-USERNAME.github.io/mahmood-app/`

### 4. Install it on your phone
**Android (Chrome):** open your address in Chrome, tap the three dots menu, then **Install app** (or **Add to Home screen**). Open it from the new icon.

**iPhone (Safari):** open your address in Safari, tap the Share button, then **Add to Home Screen**.

Open the app once while you have a signal. After that it also works without one.

## Bring your existing data across

Your current information is in the Claude version. It has been saved into `Mahmood-data-backup-PRIVATE.json`.

1. Get that file onto your phone (email it to yourself, or put it in Google Drive).
2. Open the installed app, then **Home**, then scroll to **Back up your data**.
3. Tap **Restore from a backup**, choose the file, and tap **Restore from a backup** again to confirm.
4. Check your customers, jobs and invoices are there, then delete the backup file from email and Drive.

## Looking after your data

- Everything you enter is stored **on your phone only**. Nothing is sent to GitHub or anywhere else.
- Use **Home > Save a backup file** about once a month, and keep the file somewhere safe. If the phone is lost, reset, or the browser data is cleared, restoring that file brings everything back.
- Always open the app from the same icon or address, so you see the same data.
- The Claude version and this version are separate. Changes made in one do not appear in the other.

## Things that work better as an installed app

- **Save as PDF** saves the invoice to your downloads, and **Share PDF** sends it straight to WhatsApp or email.
- **Expenses** can take a receipt photo with the camera (allow the camera when asked).
- **Backups** and the **CSV** export save as normal downloads.

## Updating the app later

Replace `index.html` in the repository: open the file, tap the pencil to edit, or use **Add file > Upload files** with the same name to overwrite it, then **Commit changes**. The phone picks up the new version the next time you open the app. Close it and open it a second time if you do not see the change straight away.

## If something goes wrong

- **Page not found:** wait a few minutes after switching on Pages. Check the file is called `index.html` and sits at the top level of the repository, not inside a folder.
- **No Install option:** use Chrome on Android (or Safari on iPhone) and open the full `https://` address.
- **Blank or old version:** close the app completely and open it again.
- **PDF will not save:** open the app once with a signal so it can finish loading its PDF tool, then try again.

## Optional: a real Android app file (.apk)

If you ever want to list it in the Google Play Store, the free tool at pwabuilder.com can wrap this web app into an Android package. You paste in your GitHub Pages address. Installing from the home screen as above is simpler for your own use.
