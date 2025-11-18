# Voxera — Static OTT Starter

This ZIP contains a ready-to-deploy, single-branch static site for GitHub Pages.

Files:
- index.html — the main site. Drop into the root of your public GitHub repo.
- film-template.html — a simple film page template you can copy and customize per film.
- README.md — this file.

How to deploy:
1. Create a **public** GitHub repository.
2. Upload the files to the repository root (Add file → Upload files).
3. Go to **Settings → Pages** and set the source to **main** branch, **/ (root)** folder.
4. Wait ~30–60s and open: `https://<github-username>.github.io/<repo-name>/`

How to use:
- To show thumbnails, upload your PNG/JPG into the repo (Add file → Upload files). After upload, click the file and copy the **Raw** URL (raw.githubusercontent.com/...). Use that URL as the `thumb` value for a film in the `films` array in `index.html`.
- For streaming, upload your film on Gumroad, copy the product slug (the part after `gumroad.com/l/`), and paste it into the `films` array as the `gumroad` value for that film.
- Example film object format:
  {id:'film1', title:'My Film', year:2025, gumroad:'abc123', thumb:'https://raw.githubusercontent.com/USERNAME/REPO/main/assets/thumb1.png'}

Notes:
- Public-domain films: set Gumroad product price to free.
- Your images hosted on GitHub raw URLs are public and accessible to everyone.
- If you want me to auto-generate pre-filled film entries or upload a starter set of thumbnails, say so and I will prepare them.

