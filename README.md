# Ibnu Fachrian — Portfolio Website

This is a **static website**: it uses plain HTML, CSS, and vanilla JavaScript. It does **not** use React, TypeScript, Tailwind, Node.js, a database, or a server.

## Project structure

```text
ibnu-fachrian-portfolio-self-hosted/
├── index.html     # Page content and SEO metadata
├── styles.css     # Design, responsive layout, print styles
├── script.js      # Menu, filters, case-study modal, animations
├── netlify.toml   # Optional Netlify configuration
└── README.md      # This guide
```

## Dependencies and services

- No `npm install`, build command, API key, environment variable, paid service, database, or backend is required.
- No local image asset is required. The portrait shown is deliberately a CSS placeholder, so replace it with your own image when ready.
- Typography uses **Plus Jakarta Sans** from the Google Fonts CDN. This needs no key or account. If Google Fonts is unavailable to a visitor, the browser uses its local fallback font automatically.
- The “Print / Save as PDF” CV button opens the browser print dialog; choose **Save as PDF** to create the PDF locally.

## Run locally

Because this is a static site, you can double-click `index.html` to inspect it. For the closest local-server behavior, run one of these commands inside this folder:

```bash
# Node.js 18+
npx serve .

# Python 3
python -m http.server 8080
```

Then open the local URL shown by the command (usually `http://localhost:3000` or `http://localhost:8080`). No installation is required when using a free hosting provider.

## Deploy for free — Netlify (recommended)

1. Create a free account at [netlify.com](https://www.netlify.com/).
2. Unzip this package.
3. In Netlify, select **Add new site → Deploy manually**.
4. Drag the **contents of this folder** (the folder that contains `index.html`) into the upload area.
5. Netlify gives you a public `*.netlify.app` URL. You can change the site name later in Site configuration.

There is no build setting: publish the root folder and leave the build command empty.

## Deploy for free — GitHub Pages

1. Create a new GitHub repository, for example `ibnu-portfolio`.
2. Upload all files from this folder to the repository root — `index.html` must stay at the top level.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
5. Your site will be available at `https://YOUR-USERNAME.github.io/ibnu-portfolio/`.

## Deploy for free — Cloudflare Pages

1. Create an account at [pages.cloudflare.com](https://pages.cloudflare.com/).
2. Create a project and connect the GitHub repository above, or use **Direct Upload**.
3. For a Git repository deployment, use no framework preset and leave the build command empty.
4. Set the output directory to `.` (the project root), then deploy.

## Content updates

- **Portrait:** replace the CSS placeholder in `index.html` (search for `Photo placeholder`) with an image element pointing to your own file.
- **Email/social links:** search for `your.email@example.com`, `LinkedIn URL`, `Instagram URL`, and `WhatsApp URL` in `index.html`.
- **Portfolio:** project copy is in `index.html`; matching modal case-study text is in `script.js`.
- **CV:** update the Digital CV section in `index.html`; its printed version automatically follows the screen content.

After any update, upload the edited files again or push them to your connected GitHub repository. The live site will refresh automatically.
