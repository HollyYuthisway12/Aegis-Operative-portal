AEGIS INITIATIVE — GM EDITOR / GITHUB PAGES KIT
===============================================

FILES
  index.html          The player login and portal
  player.js           Player portal logic
  style.css           Shared AEGIS styling
  campaign-data.json  The player-visible campaign content
  gm-editor.html      The separate GM editing interface
  gm-editor.js        GM editing logic

SETUP (FIRST TIME)
1. Download and unzip the AEGIS GM kit.
2. In your GitHub repository:
   https://github.com/HollyYuthisway12/Aegis-Operative-portal
   upload index.html, player.js, style.css, campaign-data.json.
   If asked, replace the old index.html. Keep these four files in the root.
3. Your published site remains:
   https://hollyyuthisway12.github.io/Aegis-Operative-portal/
4. Keep gm-editor.html and gm-editor.js privately on your computer.
   They are NOT needed by players, and should NOT be uploaded to GitHub.

EDITING BEFORE EACH SESSION
1. To run the editor locally, place gm-editor.html, gm-editor.js,
   style.css and a copy of campaign-data.json in the same folder.
2. Open gm-editor.html in a browser. Click IMPORT JSON and choose the
   latest campaign-data.json from your GitHub repo or computer.
   Browsers normally prevent local HTML from fetching other local files,
   so use IMPORT JSON rather than LOAD PUBLISHED DATA when offline.
3. Edit schedule, messages, personnel, bulletins and missions.
   Click SAVE RECORD after editing each record.
4. Click EXPORT CAMPAIGN-DATA.JSON.
5. Upload that newly downloaded campaign-data.json to the GitHub repo
   root, replacing the existing version, then COMMIT CHANGES.
6. After GitHub Pages publishes the change, players refresh their page.
   You do not need to replace index.html every session.

IMPORTANT
- This is an export/upload editor, not one-click GitHub publishing.
- Login is fictional and doesn't verify identities. The editor's local
  drafts are stored in that browser; export backups regularly.
- GitHub Pages content is PUBLIC, including raw JSON. Never store
  secret GM plots, player secrets, or real passwords in the JSON,
  even if a mission is marked unpublished.
- Player read/archive state stays on their device and browser only.
- Changes don't appear live until GitHub Pages deploys and players refresh.
- This kit replaces the previous single-file portal; its prior local
  message-read history is not carried over.
- Test with a local web server or GitHub Pages. Opening index.html as a
  file:// page can prevent campaign-data.json from loading.

LOCAL PREVIEW (OPTIONAL)
If Python is installed, from this folder run:
  python -m http.server 8000
Then open:
  http://localhost:8000/index.html
  http://localhost:8000/gm-editor.html
Do not expose the local server to the internet.
