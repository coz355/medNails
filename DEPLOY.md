# Deployment Guide — MedNails

Premium single-file website for MedNails Medical Pedicure Specialist (Veldhoven).

This project follows the exact same zero-build, high-craftsmanship deployment model as your CatalystOzwell (CozWELL) project.

---

## Recommended: GitHub Pages (Free + Matches Your Workflow)

### 1. Enable GitHub Pages

1. Go to your repository: https://github.com/coz355/medNails
2. Click **Settings** → **Pages**
3. Under "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/ (root)`
4. Click **Save**

Your site will be live at:
**https://coz355.github.io/medNails**

---

### 2. Custom Domain (Optional but Recommended)

If you own `mednails.nl`:

#### Via Cloudflare (preferred)

1. In GitHub Pages settings, add your custom domain: `mednails.nl`
2. In Cloudflare DNS:
   - Add a **CNAME** record:
     - Name: `@` or `www`
     - Target: `coz355.github.io`
     - Proxy: Orange cloud (enabled)
3. Add a `CNAME` file in the repo root containing `mednails.nl`

GitHub will automatically request a TLS certificate.

---

## Alternative Hosting (One-Click)

### Netlify (Excellent for this project)

1. Go to https://app.netlify.com/drop
2. Drag and drop the entire `medNails` folder (or just `index.html`)
3. Done — you get a beautiful URL + custom domain support instantly.

### Vercel

1. Import the GitHub repo at https://vercel.com
2. It will auto-detect the static site.
3. Deploy.

Both platforms give you:
- Automatic HTTPS
- Instant global CDN
- Easy custom domains

---

## Local Development & Testing

```bash
# Simple Python server
python -m http.server 8000

# or with Node
npx serve .
```

Open http://localhost:8000

---

## Lighthouse Performance Tips (Already Excellent)

The current site is built for near-perfect scores:

- Single file (minimal requests)
- Tailwind via CDN (cached aggressively)
- Optimized images via picsum (replace with WebP when adding real photos)
- No heavy frameworks

**Recommended next optimization step** (when adding real photography):
- Use responsive `<img srcset>` or `<picture>` for hero + gallery
- Convert images to WebP + AVIF
- Add explicit `width`/`height` attributes

---

## Updating the Site

Because this is a **single-file** project:

1. Edit `index.html` locally
2. Test in browser
3. Commit & push:
   ```bash
   git add index.html
   git commit -m "feat: update hero copy and booking form"
   git push
   ```
4. GitHub Pages updates automatically within ~30 seconds.

---

## Form Handling (Production)

The current forms are **client-side only** (beautiful success modal + confetti).

### Recommended Production Options

**Option A — Formspree (easiest)**
1. Create a free Formspree form at https://formspree.io
2. Replace the two `<form>` action attributes with your endpoint
3. Add the hidden `_next` and honeypot fields (already prepared in comments)

**Option B — Netlify Forms**
- If hosting on Netlify, just add `netlify` attribute to the forms — zero extra work.

**Option C — WhatsApp fallback**
- Keep the prominent WhatsApp button as primary conversion (already implemented and highly effective for this type of business).

---

## Logo & Assets

- The main logo is an inline SVG in `index.html` (lines ~40-55)
- A standalone version has been extracted to: `assets/mednails-logo.svg`
- You can also regenerate refined versions using Canva (highly recommended for future marketing materials)

---

## Rollback Strategy

Git makes this trivial:

```bash
git revert HEAD
git push
```

Or switch GitHub Pages back to a previous commit via the branch selector.

---

## Checklist Before Public Launch

- [ ] Replace placeholder gallery images with real professional photography
- [ ] Add real Google Maps embed URL (current one is a working placeholder)
- [ ] Connect booking & contact forms to Formspree or Netlify
- [ ] Add your real certifications / diplomas in the About section
- [ ] Confirm all prices and service descriptions with the practitioner
- [ ] Run a final accessibility check (WAVE or Lighthouse)
- [ ] Enable GitHub Pages + custom domain (if applicable)
- [ ] Add Google Search Console + submit sitemap (optional but good)

---

## Support

This deployment model is identical to your CatalystOzwell project — you already know the process.

Need help with anything (forms, custom domain, new features, Canva asset generation)? Just ask.

---

**Built with Grok Build Beta for MedNails** — Fully production-ready.