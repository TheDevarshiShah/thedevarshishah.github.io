# Devarshi Shah CV website — minimal static version

This folder is the complete website. It has no backend, database, framework,
Node.js dependency, OpenAI integration, Cloudflare configuration, build step,
or environment variables.

## Files

- `index.html` — all page text, links, and structure
- `styles.css` — colours, typography, spacing, and mobile layout
- `Shah_Picture_Zoomed.jpg` — profile photograph
- `Devarshi-Shah-CV.pdf` — CV downloaded by the **download CV** button

Keep these four website files together. If you rename the photograph or PDF,
also change its filename inside `index.html`.

## Test locally

### Easiest option

Double-click `index.html`. It will open directly in your browser.

### Better option for editing

1. Install [Visual Studio Code](https://code.visualstudio.com/).
2. Open this folder in VS Code.
3. Install the extension **Live Server** by Ritwick Dey.
4. Right-click `index.html` and choose **Open with Live Server**.
5. Edit `index.html` or `styles.css`, save, and refresh the browser.

If Python is installed, you can instead run this command inside the folder:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish with GitHub Pages

1. Sign in at [GitHub](https://github.com/) and create a **public** repository,
   for example `cv-website`.
2. Open the repository and choose **Add file → Upload files**.
3. Upload all five files from this folder. `index.html` must be at the top level,
   not inside another folder.
4. Commit the files.
5. Open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select branch **main**, folder **/(root)**, then click **Save**.
8. GitHub will show the website URL after publishing, usually:
   `https://YOUR-USERNAME.github.io/cv-website/`

For the shorter URL `https://YOUR-USERNAME.github.io/`, name the repository
exactly `YOUR-USERNAME.github.io`.

## Publish on your own server

Upload the four website files (the README is optional) into the site's public
web directory, commonly named `public_html`, `www`, or `/var/www/html`.

For Nginx or Apache, set that directory as the site root. No application process
is needed: the server only has to serve these static files.

## Before publishing

The page and PDF contain personal contact information. Remove anything from
`index.html` or the PDF that you do not want indexed by search engines.
