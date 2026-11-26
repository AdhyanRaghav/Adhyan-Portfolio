# Adhyan Raghav — Portfolio

A simple, responsive portfolio built with plain HTML and CSS.

## Run locally on Zorin OS

From the extracted project folder:

```bash
cd public
python3 -m http.server 8000
```

Open `http://localhost:8000` in Firefox. Stop the server with `Ctrl+C`.

## Files

- `public/index.html` — all portfolio content
- `public/styles.css` — uploaded editorial design, with uniform project heading sizes
- `public/favicon.svg` — site icon
- `public/_headers` — basic security headers for Cloudflare Pages
- `public/Adhyan-Raghav-Resume.pdf` — your supplied résumé

## Publish using GitHub + Cloudflare Pages

1. Create a public GitHub repository, e.g. `adhyan-portfolio`.
2. From the project root, run:

```bash
git init
git add .
git commit -m "Add cybersecurity portfolio"
git branch -M main
git remote add origin https://github.com/AdhyanRaghav/adhyan-portfolio.git
git push -u origin main
```

3. In Cloudflare, open Workers & Pages and create a Pages project connected to that repository.
4. Choose `main` as the production branch.
5. Set build command to `exit 0` and output directory to `public`.
6. Deploy. Cloudflare gives you a `pages.dev` URL. Future pushes to `main` redeploy automatically.

## Updating content

Edit `public/index.html`. Before publishing, add direct GitHub repository links for the FIM and AI-gated secure-folder projects if those repositories are public.
