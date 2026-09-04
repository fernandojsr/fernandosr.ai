# Fernando Sanchez-Rodriguez — Portfolio

Personal portfolio site for Fernando Sanchez-Rodriguez, Digital Transformation & Operations professional.

**Live site:** [fernandosr.com](https://fernandosr.com)

## About

This site showcases 25+ years of experience across Mexico, Portugal, and Germany in Digital Transformation, Operations, and Change Management. It includes project case studies, Google Career Certificate capstone projects (Data Analytics, UX Design, AI Essentials, Business Intelligence), professional credentials, and testimonials.

## Tech Stack

- **Structure:** Single-page HTML (`index.html`)
- **Styling:** Custom CSS — dark navy/gold design system, Cormorant Garamond + DM Sans typography
- **Languages:** Trilingual switcher (EN / ES / DE) via a custom `CONTENT_MAP` / `TRANSLATIONS` architecture
- **Hosting:** GitHub Pages
- **Domain:** Custom domain via Namecheap, DNS pointed to GitHub Pages
- **Analytics:** Google Analytics 4 (GA4) with custom event tracking, visualized via a Looker Studio dashboard
- **SEO:** Indexed via Google Search Console, `sitemap.xml` included

## Features

- Responsive, mobile-tested layout
- Six project case study cards with PDF lightbox viewers (with mobile "Open in New Tab" fallback)
- Applied Practice section featuring Google Career Certificate capstone projects
- Video and image gallery lightboxes
- Credly badge integration for verified credentials
- Contact form via Formspree
- GA4 event tracking on key CTAs: CV downloads, case study views, video views, gallery opens, and LinkedIn clicks

## Project Structure

```
/
├── index.html          # Main site (formerly home.html)
├── CNAME                # Custom domain config for GitHub Pages
├── sitemap.xml           # SEO sitemap for Google Search Console
├── case-studies/         # PDF case study files
└── images/                # Site imagery, project photos
```

## Analytics Setup

- **GA4 Measurement ID:** `G-YRZ1B7EZJ0`
- Custom events tracked: `cv_download`, `connect_click`, `watch_video`, `view_case_study`, `view_gallery` (each tagged with a `project` parameter where relevant)
- Dashboard: Looker Studio, connected live to GA4, tracking users, traffic sources, engagement, and per-project interaction breakdowns

## Notes for Future Edits

- **Translation system:** Any new text element must be explicitly registered in the `CONTENT_MAP` in the `<script>` block, or it will not translate and will silently display in English regardless of selected language.
- The `<script>` block must remain inside `<body>`, before `</html>` — moving it outside this location breaks the language switcher.
- Always test responsive/mobile layout after structural changes (hamburger menu, grid overflow, and testimonial readability have been recurring trouble spots).

## Contact

Reach out via the site's contact form or [LinkedIn](https://www.linkedin.com/in/fs-creative/).
