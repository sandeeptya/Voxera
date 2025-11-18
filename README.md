# Voxera — Upgraded Static Starter (v2)

This package contains a single-file, production-capable front-end for Voxera with:
- Prime-like hero + carousel
- Search
- Continue Watching (localStorage)
- Watch history (localStorage)
- Client-side login (local, no passwords stored on server)
- Admin panel to add films locally and export/import JSON for permanent updates
- Embedded Gumroad modal player
- Responsive layout

Files:
- index.html — drop into your public GitHub repo root (replaces existing file)
- README.md — this file

How to add a film (quick):
1. Upload your thumbnail PNG to the repo (Add file → Upload files). After upload, click it and copy the 'Raw' URL.
2. Upload your film to Gumroad and copy the slug (the part after /l/ in the product URL).
3. Edit index.html in GitHub: find the films array near the top and replace the sample object or use the Admin UI to add films locally and then Export JSON to paste into the films array in the file for permanence.

Admin notes:
- Admin is protected by a simple client-side password (voxera-admin-2025). Change it by editing index.html locally before uploading if you want.
- Admin additions are stored locally (browser) until you paste exported JSON back into index.html for repository-level permanence.
- To make changes globally for all visitors, you must commit changes to index.html in the repo.

Deploy:
1. Create a **public** GitHub repository (or use yours).
2. Upload index.html to the repository root.
3. Settings → Pages → Deploy from a branch → main → / (root). Save.
4. Wait ~30–60s. Open https://<username>.github.io/<repo>/

If you want I can also:
- Pre-generate 8 demo thumbnails and include them in a ZIP for direct upload to your repo
- Automate a script to rewrite index.html with new films (CLI guidance)
