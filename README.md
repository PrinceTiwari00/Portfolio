# Prince Tiwari — Portfolio

A single-page personal portfolio website for **Prince Tiwari** — web developer,
IT support &amp; management accountant based in Hetauda, Nepal.

Built as a fast, dependency-free static site: plain HTML, CSS and vanilla JS.
No build step, no framework, no tracking.

---

## Run it locally

Any static server works. For example:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

Or just open `index.html` in a browser.

## Deploy

The site is fully static, so it drops straight onto:

- **GitHub Pages** — Settings → Pages → deploy from this branch, folder `/` (root)
- **Netlify / Vercel / Cloudflare Pages** — no build command, publish directory `.`
- **Any shared host** — upload `index.html`, `styles.css`, `script.js` and `assets/`

---

## Files

```
index.html                      # all page content & markup
styles.css                      # design tokens, layout, components, responsive rules
script.js                       # theme toggle, mobile nav, scroll reveal, counters, form
assets/profile.jpg              # profile photograph (600×600)
assets/Prince-Tiwari-CV.pdf     # downloadable CV
```

## Features

- **Dark & light themes** with system-preference detection and a saved choice (`localStorage`).
- **Fully responsive** — mobile-first navigation, fluid type, no horizontal scroll.
- **Accessible** — skip link, visible focus rings, ARIA labels, keyboard-operable menu
  (closes on `Esc`), semantic landmarks, respects `prefers-reduced-motion`.
- **Motion, restrained** — scroll-reveal, animated counters and skill bars that trigger
  once via `IntersectionObserver`.
- **Working contact form** — validates inline, then hands off a pre-filled message to
  the visitor's mail client (a static site can't send mail on its own).
- **SEO-ready** — descriptive title, meta description, Open Graph and Twitter card tags,
  inline SVG favicon.

## Content sources

Copy was written from the supplied CV and résumé:

- **Email:** `princet6ye@gmail.com` (the résumé PDF also lists `aaaaaq865@gmail.com`)
- **Phone:** +977 974 666 0285
- **Current address:** Piple, Hetauda Sub-Metropolitan City, Makwanpur
- **Permanent address:** Kanutole, Gaur Municipality, Rautahat
- **Roles:** Internal Management Accountant @ Zenith Secondary School (Dec 2023 – now),
  Web Designer &amp; Developer (remote/freelance), IT Support Officer @ Chandra Jyoti
  Awasiya School (3 years)
- **Education:** BCA (ongoing), Diploma in Computer Training @ Unihub (Oct 2020)
- **Languages:** Nepali, English

## Things to update

1. **Work section** — the three cards are representative project types, not named client
   engagements. Replace with real project titles, links and screenshots as they become
   available (`#work` in `index.html`).
2. **Skill percentages** in the bars (`#skills`) are illustrative — adjust to taste.
3. **Social links** — none were supplied, so none are shown. Add a LinkedIn/GitHub block
   in the contact section if wanted.
4. **Contact form** — for real inbox delivery with no mail-client handoff, point it at a
   form service (Formspree, Netlify Forms, etc.) and remove the `mailto:` submit handler
   in `script.js`.
5. **Open Graph image** — `og:image` uses a relative path; set it to the full URL of the
   deployed site for correct social previews.

## Privacy note

The citizenship certificate images supplied with the CV were **not** used anywhere on
this site. Identity documents like that should not be published publicly.

---

© Prince Tiwari. Built with care in Nepal.
