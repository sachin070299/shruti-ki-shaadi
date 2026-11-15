# Shruti ki Shaadi – Shopping List

No keys and no passwords for anyone. Family members just open the link and type their name once.
The page lives on GitHub Pages. The list is saved in **your Google Drive** through a small free Google script.

## One-time setup (only you, ~5 minutes)

### 1. Make the Google script
1. Open **script.google.com** (on a computer, or in Chrome with "Desktop site" on), signed in with your Google account.
2. Click **New project**. Delete what's there and paste everything from `Code.gs`. Click 💾 Save.
3. Click **Deploy → New deployment** → ⚙ next to "Select type" → **Web app**.
   - Execute as: **Me**
   - Who has access: **Anyone**
4. Click **Deploy** → **Authorize access** → choose your account.
   Google will say "Google hasn't verified this app". That's normal for your own script: click **Advanced → Go to … (unsafe) → Allow**.
5. Copy the **Web app URL** (it ends with `/exec`).

### 2. Put the URL in the page
1. On GitHub, open `index.html` → ✏️ Edit.
2. Near the top, find `apiUrl:   "",` and paste the URL between the quotes:
   `apiUrl:   "https://script.google.com/macros/s/…/exec",`
3. **Commit changes**. Wait about 1 minute.

### 3. Share
Send the normal page link (`https://YOUR-USERNAME.github.io/shruti-ki-shaadi/`) in the family WhatsApp group. Done.

## Your existing items
Keep your current `data.txt` in the repo. The first time the page opens, it copies those items into the online list automatically. After that, everything is saved in Google Drive (`shruti-ki-shaadi-data.txt`), and `data.txt` is only a fallback copy.

## Good to know
- Anyone with the link can edit, so share it only in the family.
- Backups: a copy is saved in the Drive folder **"Shruti ki Shaadi backups"** every 10 changes. Anyone can also tap ⚙ → **Download backup**.
- If you ever change `Code.gs`, use **Deploy → Manage deployments → ✏️ → Version: New version → Deploy**, so the URL stays the same.
- You can delete the old GitHub token now. It's no longer used.
