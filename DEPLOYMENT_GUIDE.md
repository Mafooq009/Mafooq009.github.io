# Exact deployment steps

Your repository and DNS are already configured. The repository is:

`Mafooq009/Mafooq009.github.io`

The public website is:

`https://syedmafooqulhassan.com`

## 1. Download and extract the package

Download `syedmafooqulhassan_portfolio.zip` and extract it on your computer.

Open the extracted folder. You should see:

- `index.html`
- `styles.css`
- `script.js`
- `CNAME`
- `.nojekyll`
- `robots.txt`
- `sitemap.xml`
- `site.webmanifest`
- `README.md`
- `assets` folder

## 2. Upload everything to GitHub

1. Open GitHub.
2. Open the repository `Mafooq009.github.io`.
3. Select the **Code** tab.
4. Click **Add file**.
5. Click **Upload files**.
6. Open the extracted folder on your computer.
7. Select **all files and the assets folder inside it**.
8. Drag them into GitHub's upload area.
9. Do not upload the outer `syedmafooqulhassan_portfolio` folder itself.
10. In the commit-message box, enter:
   `Deploy complete academic portfolio`
11. Select **Commit directly to the main branch**.
12. Click **Commit changes**.

If GitHub asks whether to replace an existing `CNAME` or `README.md`, allow the replacement. The included `CNAME` contains the same custom domain.

## 3. Wait for deployment

1. Open the repository's **Actions** tab.
2. Wait for **pages build and deployment** to show a green check.
3. This normally takes around one to three minutes.
4. Open `https://syedmafooqulhassan.com`.
5. Use a private/incognito browser window or press `Ctrl + F5` if an older version is cached.

## 4. Enable HTTPS

Open:

**Repository → Settings → Pages**

When the certificate is ready, enable **Enforce HTTPS**.

GitHub may need several minutes and sometimes up to 24 hours before this option becomes available.

After HTTPS is enabled, use:

`https://syedmafooqulhassan.com`

## 5. Add your real photograph later

1. Rename your portrait to `profile.jpg`.
2. Open the repository.
3. Open the `assets` folder.
4. Select **Add file → Upload files**.
5. Upload `profile.jpg`.
6. Open `index.html` and click the pencil icon.
7. Replace:

`assets/profile-placeholder.svg`

with:

`assets/profile.jpg`

8. Commit the change to `main`.

## 6. Update the website later

Every commit to the `main` branch is automatically published because GitHub Pages is configured to deploy from:

- Branch: `main`
- Folder: `/(root)`

For text changes, open `index.html`, click the pencil icon, edit, and commit.

## Troubleshooting

### Website still shows the README or an old page

- Confirm `index.html` is in the repository root, not inside another folder.
- Open the **Actions** tab and confirm the deployment succeeded.
- Press `Ctrl + F5`.
- Try an incognito window.

### 404 error

- Confirm the repository name is exactly `Mafooq009.github.io`.
- Confirm Pages uses `main` and `/(root)`.
- Confirm the repository is public.
- Confirm `index.html` is at the root.

### Custom domain disappears

- Restore the root file named `CNAME`.
- Its only content must be:
  `syedmafooqulhassan.com`

### HTTPS is unavailable

- Do not change the DNS records.
- Wait for GitHub's certificate to be issued.
- Recheck **Settings → Pages** later.
