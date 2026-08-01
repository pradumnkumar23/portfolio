# Your Name — Portfolio Website

A single-page, static portfolio website for a Salesforce Developer — built with plain HTML, CSS, and JavaScript (no build step, no dependencies, no framework).

**Live site:** _add your GitHub Pages URL here after deploying, e.g. `https://yourusername.github.io/portfolio`_

## Sections

- **Hero** — animated node-network background
- **About** — short bio and quick facts
- **Skills** — categorized skill list with proficiency bars
- **Certifications** — Salesforce certification cards
- **Projects** — project cards with tags
- **Experience** — job history timeline
- **Resume** — upload/preview/download a resume PDF
- **Contact** — email and social links

## Editing your content

Open `index.html` and search for the section near the top of the `<script>` tag marked:

```
EDIT YOUR CONTENT HERE
```

You'll find plain JavaScript arrays for `SKILLS`, `CERTS`, `PROJECTS`, and `EXPERIENCE` — edit the text inside these to update the site. No HTML/CSS knowledge is required for basic content changes.

Also update by hand, directly in the HTML:
- Your name (appears in `<title>`, the nav brand, and the hero heading)
- The hero tagline and About paragraphs
- The email address and social links in the Contact section

## Adding a permanent, downloadable resume

The built-in "Upload Resume" button only works for the current visitor's browser session — it can't make a file visible to everyone, since this is a static site with no server.

To make your resume permanently downloadable by anyone who visits:

1. Add your resume file to this folder, e.g. `resume.pdf`.
2. In `index.html`, find this line in the Resume section:
   ```html
   <a class="btn btn-solid" id="resume-download-btn" href="#" download="resume.pdf" style="pointer-events:none; opacity:0.4;">Download PDF</a>
   ```
3. Replace it with:
   ```html
   <a class="btn btn-solid" href="resume.pdf" download="resume.pdf">Download PDF</a>
   ```

## Deploying with GitHub Pages

See the step-by-step guide provided alongside this file, or follow these commands:

```bash
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/portfolio.git
git push -u origin main
```

Then enable GitHub Pages in your repository's **Settings → Pages** tab, selecting the `main` branch and `/ (root)` folder as the source.

## Tech stack

- HTML5, CSS3 (custom properties, no framework)
- Vanilla JavaScript (no dependencies)
- Google Fonts: Fraunces, Manrope, JetBrains Mono

## License

This is your personal project — use, modify, and deploy it however you like.
