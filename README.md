# Andrew Kelly, Nenagh Dentist — Website

A fast, accessible, SEO-optimised marketing website for a family dental practice in Nenagh,
Co. Tipperary. Built as a lightweight static site (HTML + CSS + vanilla JS) — no build step,
no framework lock-in, deploys anywhere in seconds.

## Pages
- `index.html` — Home
- `about.html` — About the practice
- `services.html` — Treatments (with anchor links per service)
- `contact.html` — Contact, opening hours, map & enquiry form

## Tech
- Semantic HTML5, mobile-first responsive CSS (custom design system in `css/styles.css`)
- Vanilla JS (`js/main.js`) — sticky header, mobile nav, scroll reveal, FAQ accordion, form UX
- Google Fonts: Fraunces (display) + Inter (body)
- `Dentist` schema.org JSON-LD, Open Graph tags, `sitemap.xml`, `robots.txt`
- Security headers + long-cache static assets via `vercel.json`

---

## 1) Preview locally
No Node or Python needed — a tiny PowerShell server is included:

```powershell
powershell -ExecutionPolicy Bypass -File serve.ps1
# then open http://localhost:8080
```

(Or just double-click `index.html` — it works over `file://` too.)

## 2) Deploy to Vercel (matches andrewkelly-dental.vercel.app)
1. Push this folder to a GitHub repo (or drag-and-drop into Vercel).
2. In Vercel: **New Project → Import** → framework preset **"Other"** (it's static).
3. Deploy. `vercel.json` handles clean URLs, caching and security headers automatically.
4. Set the production domain to `andrewkelly-dental.vercel.app` (or a custom domain).

> Alternative hosts: Netlify, Cloudflare Pages, or GitHub Pages all work — just upload the folder.

---

## ⚠️ Before you go live — client to confirm / replace
These items are placeholders or assumptions and **must be verified with the client**:

- [x] **Pricing** — intentionally not shown on the site. All services direct visitors to call 067 33755 for pricing (per project decision, July 2026). Do not add prices back.
- [ ] **Team names, roles, bios & photos** on `about.html` (currently placeholders).
- [ ] **Reviews** — the testimonials block is a *sample layout*. Embed real Google reviews (see below). Do not publish invented reviews.
- [ ] **Email address** — `hello@nenaghdentist.ie` is a placeholder on the contact page.
- [ ] **Medical card / PRSI (DTSS / Treatment Benefit)** — confirm exact scheme participation.
- [ ] **Opening hours** — verified Mon–Fri 9–5; confirm Saturday/emergency arrangements.
- [ ] **Real photography** — replace SVG "photo slots" (see `IMAGE-PROMPTS.md`).

## Wire up the contact form (required to receive enquiries)
The form is currently front-end only (shows a success message but sends nothing). Pick one:

**Formspree (easiest):**
1. Create a free form at formspree.io and copy your endpoint.
2. In `contact.html`, change the `<form>` tag to:
   ```html
   <form class="form" id="enquiry-form" action="https://formspree.io/f/XXXX" method="POST">
   ```
3. In `js/main.js`, remove the `e.preventDefault()` block (or let Formspree handle it via AJAX).

Alternatives: Netlify Forms (add `netlify` attribute), Getform, or Web3Forms.

## Add live Google reviews
Use a free widget (e.g. Elfsight, Trustindex, or Google's own place widget), or manually paste
2–3 real reviews into the testimonial cards in `index.html`, replacing the "Placeholder review"
text and the `P` avatar with the reviewer's initial.

---

## Maintenance checklist
- **Monthly:** check the contact form still delivers; scan for broken links.
- **Quarterly:** refresh any seasonal offers; add new Google reviews.
- **Twice a year:** review service prices & opening hours for accuracy.
- **Annually:** update the footer year (auto-updates via JS), review meta descriptions & photos.
- Keep an eye on Google Business Profile — it drives most local dental searches.

## SEO quick wins after launch
1. Claim/verify the **Google Business Profile** and match the name, address, phone (NAP) exactly to this site.
2. Submit `sitemap.xml` in Google Search Console.
3. Get listed consistently on Irish directories (goldenpages.ie, etc.) with identical NAP.
4. Encourage happy patients to leave Google reviews.
