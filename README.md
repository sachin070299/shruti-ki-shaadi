# Shruti ki Shaadi – Shopping List – Setup (one time, ~10 min)

## 1. Create the repo
1. On GitHub, create a new repository, e.g. `shruti-ki-shaadi` (Public is simplest for free GitHub Pages).
2. Upload `index.html` and `data.txt` to it.
3. Go to **Settings → Pages → Branch: main / (root) → Save**.
   After about a minute your page is live at `https://YOUR-USERNAME.github.io/shruti-ki-shaadi/`

## 2. Create the "family access key" (so people can save)
GitHub Pages is read-only by itself, so the page saves changes using a GitHub token.
1. GitHub → your photo → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**
2. Expiration: until after the wedding (e.g. 90 days)
3. Repository access: **Only select repositories** → pick `shruti-ki-shaadi`
4. Permissions → Repository permissions → **Contents: Read and write**
5. Generate, then copy the token (starts with `github_pat_…`).

## 3. Share with the family
1. Open the page, tap ⚙, enter your name and paste the token, then Save.
2. Tap **🔗 Copy share link** and send that link in the family WhatsApp group.
3. When someone opens the link, the key is saved on their phone. They only need to enter their name once.

Without the key, anyone can still **view** the list but can't edit it.

## Safety notes
- **Never** paste the token inside `index.html` or any file in the repo (GitHub will auto-disable it).
- Only share the link with family. If it leaks, delete the token on GitHub and create a new one.
- Every change is saved as a commit, so you have full history and can restore anything from GitHub.

## Customise
- The page title is set in `CONFIG.title` at the top of the `<script>` in `index.html`.
- You can add new functions (e.g. Mehendi, Haldi) and categories right from the "Add Item" form (choose ➕ Add new…).

## Already included
- 56 ready items for Lagan & Shadi (puja samaan, bartan, electronics, furniture, bedding, kapde, jewellery, shringar, decoration, mithai, gifts…). Edit or delete any of them from the page.
- Set the wedding date in ⚙ Settings to show a "days to go" countdown for everyone.
