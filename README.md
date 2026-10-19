# Francis Amoah Nuako Portfolio (pcboss.me)

A lightweight, responsive, static academic/engineering portfolio. No dependencies, framework, build step, or database.

## Preview locally

Open `index.html` in a browser, or in Cursor's terminal:

```bash
python -m http.server 8080
```

Visit `http://localhost:8080`.

## Customize before launch

1. **LinkedIn:** The correct LinkedIn URL is not provided. In `index.html` search for `ADD YOUR VERIFIED LINKEDIN URL HERE` and uncomment the anchor with your real profile. Add the verified URL to the `sameAs` array in the JSON-LD block too.
2. **Projects:** Edit the four project cards under `id="work"`. Only make claims about work you actually performed. Add GitHub links for additional projects only after they are available publicly.
3. **Research and degree status:** MSc graduation is shown as *expected November 2026*, as supplied. Update once official.
4. **Social accounts:** GitHub `github.com/pcb2k18` and TikTok `@pcboss_dollar1` were supplied. Other social accounts can be added to the contact section.
5. **Contact:** Public email currently is `francisnuako@gmail.com`. The phone is intentionally not posted to avoid unwanted calls/spam.
6. **Images:** `og-preview.png` is the social-sharing image. Swap with a photo later if desired.
7. **Custom domain:** The website uses `https://pcboss.me/` as its canonical URL. Keep this if using the root domain.

## Deploy to Cloudflare Pages using GitHub

1. Create an empty GitHub repo, for example `pcb2k18/pcboss-portfolio`.
2. Upload **the contents of this folder** to that repository's root, or open the folder in Cursor and run:

   ```bash
   git init
   git add .
   git commit -m "Launch academic portfolio"
   git branch -M main
   git remote add origin https://github.com/pcb2k18/pcboss-portfolio.git
   git push -u origin main
   ```

   (Create the repository first, and authenticate to GitHub when prompted.)
3. Cloudflare Dashboard → **Workers & Pages** → **Create application** → **Pages** → **Import an existing Git repository** → select repo.
4. Set branch `main`; build command `exit 0` (or leave blank where accepted); build output directory `.` (repository root).
5. Deploy and visit the `.pages.dev` preview URL first.
6. Go to Pages project → **Custom domains** → **Set up a domain** → `pcboss.me`.
7. To connect the root/apex domain `pcboss.me`, Cloudflare requires your domain as a Cloudflare zone and appropriate Cloudflare nameservers. Follow the instructions shown in Cloudflare. Your registrar and current DNS hosting may affect the elapsed time.
8. When the domain is active, check the canonical site, email link, mobile menu, GitHub, TikTok, `https://pcboss.me/robots.txt`, and `https://pcboss.me/sitemap.xml`.

Official: https://developers.cloudflare.com/pages/framework-guides/deploy-anything/ and https://developers.cloudflare.com/pages/configuration/custom-domains/

## Search engine indexing

- The page includes a unique `<title>`, meta description, Open Graph tags, canonical URL, robots.txt, sitemap.xml, and Schema.org `ProfilePage`/`Person` data with known social links.
- Add `pcboss.me` as a Google Search Console property, verify domain ownership, and submit `https://pcboss.me/sitemap.xml`.
- Link to `https://pcboss.me/` from your real GitHub bio, TikTok bio, LinkedIn, and other appropriate profiles.
- Search visibility is **not instant** and backlinks do **not** guarantee rankings.

## Content integrity

For PhD outreach, ensure research achievements are verifiable and distinguish your contributions from reused code. Do not add hypothetical experiments, evaluation results, or unverified third-party repositories as your own work.
