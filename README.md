# MedNails — Medical Pedicure Specialist

**Premium bilingual website for MedNails**  
A high-end, modern, clinical-beauty website for a certified medical pedicure practice in Veldhoven, Netherlands.

**Live Demo:** https://coz355.github.io/medNails (after enabling GitHub Pages)

---

## Features

- **Fully bilingual** — English + Nederlands with instant language switcher (🇬🇧 / 🇳🇱)
- **Single-file architecture** — One beautiful, self-contained `index.html` (Tailwind via CDN)
- **Premium medical-beauty aesthetic** — Deep teal (#0F766E) + soft rose (#F9A8D4) on warm off-white
- **Custom vector logo** — Stylized medical cross + elegant foot & caring hands illustration
- **Complete conversion-focused experience**
  - Hero with strong CTAs
  - 6 premium services with pricing
  - 8 Preventive Care tips (exactly matching professional medical pedicure standards)
  - Elegant masonry gallery with lightbox
  - 4 realistic testimonials
  - Dual forms: General Inquiry + Appointment Booking (fully functional client-side with success modal + confetti)
- **Quick contact actions**: Direct Call, WhatsApp (pre-filled), Instagram
- **Embedded location** for Blekkehei 4, 5508 TC Veldhoven
- **Mobile-first** with smooth hamburger menu and high-end micro-interactions
- **Production-ready** — WCAG-friendly, fast, deployable anywhere

---

## Tech Stack

- Tailwind CSS 3.4+ (via CDN — zero build step)
- Vanilla JavaScript (bilingual system, forms, gallery lightbox, confetti)
- Fully responsive, accessible, SEO-optimized single file

---

## Project Structure

```
medNails/
├── index.html          # The complete website (single file)
├── README.md           # This file
├── DEPLOY.md           # Deployment instructions
├── assets/
│   └── mednails-logo.svg   # Standalone logo
└── .git/
```

---

## Quick Start (Local)

1. Clone the repository:
   ```bash
   git clone https://github.com/coz355/medNails.git
   cd medNails
   ```

2. Open `index.html` directly in any modern browser.

Or serve it locally:
```bash
npx serve .
# or
python -m http.server 8000
```

---

## Business Details (used in the site)

- **Name**: MedNails
- **Tagline**: Medical Pedicure Specialist
- **Address**: Blekkehei 4, 5508 TC Veldhoven, Netherlands
- **Phone / WhatsApp**: 06 5751 0971
- **Instagram**: https://www.instagram.com/mednails.nl/

---

## Customization

The entire site is contained in `index.html`.

- All text is managed via a `translations` JavaScript object (easy to extend languages).
- Services, testimonials, and preventive tips are defined as clean data arrays.
- The custom logo is an inline SVG (also extracted to `assets/mednails-logo.svg`).
- Colors, typography, and spacing follow a clear design system at the top of the `<style>` block.

To change prices, services, or copy: edit the JavaScript data arrays near the top of the `<script>` section.

---

## Deployment

See [DEPLOY.md](./DEPLOY.md) for instructions on:
- GitHub Pages (recommended — free & matches your other projects)
- Netlify / Vercel (one-click)
- Custom domain + Cloudflare

---

## Built With

This website was designed and built with **Grok Build Beta** for MedNails.

**Built with Grok Build Beta for MedNails – Fully customizable**

---

## License

For personal and commercial use by MedNails.  
Feel free to adapt the design system and code for future projects.

---

**Need help?**  
Contact the practice directly via WhatsApp or phone. For website edits, reach out to your developer.

---

*Professional. Calm. Trustworthy. Medical-grade.*