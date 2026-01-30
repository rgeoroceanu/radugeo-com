# Radu Georoceanu - Professional Freelancing Website

## Project Overview

A professional website for Radu Georoceanu's freelancing software services, focused on **legacy modernization** and **AI integration**.

## Tech Stack

- **Framework:** Astro (static site generator)
- **Styling:** Tailwind CSS v4
- **Hosting:** GitHub Pages (custom domain: radugeo.com)
- **Languages:** Bilingual (English + German) with auto-detection
- **CI/CD:** GitHub Actions (auto-deploy on push to main)

## Design Requirements

### Style Reference
- Reference site: https://uxcontinuum.com/
- **Theme:** Dark-first aesthetic (navy/dark backgrounds)
- **Accent color:** Teal (#14b8a6) - matches existing CV branding
- **Typography:** Clean, modern (Inter font family)
- **Animations:** Subtle hover effects, smooth transitions, floating orb in hero

### Design Principles
- Modern but minimalist
- Eye-catching with tasteful animations
- Mobile-responsive (hamburger menu on mobile)
- Accessibility-conscious (focus-visible, ARIA labels, semantic HTML)

## Site Structure

### Sections (Single-page design)
1. **Navigation** - Fixed glass-effect top nav with language switcher, "Book a Call" CTA, mobile menu
2. **Hero** - Tagline, brief intro, primary CTA, quick stats (10+ years, 15+ clients, 3 certifications)
3. **Pain Points** - 3 cards addressing client challenges (legacy systems, talent shortage, tech debt)
4. **Services** - 4 service cards (Legacy Modernization, AI Integration, Architecture Consulting, Full-Stack Dev)
5. **About/Credentials** - Profile photo, bio, stats, certifications, tech stack tags
6. **Testimonials** - 2 LinkedIn recommendations with LinkedIn link
7. **CTA Section** - Final call-to-action with booking link, email, phone
8. **Footer** - Logo, location, LinkedIn, email, copyright, Impressum/Privacy links

### Additional Pages
- **Impressum** (`/impressum` and `/de/impressum`) - Legal notice required by German law (TMG §5)
- **Privacy Policy** (`/privacy` and `/de/datenschutz`) - GDPR/DSGVO compliant privacy policy

### Legal / GDPR Compliance
- **Impressum** contains: name, address, contact, USt-IdNr, responsible person
- **Privacy Policy** covers: data controller info, Google Analytics (with IP anonymization), Google Fonts, Google Calendar, cookies, user rights (DSGVO Art. 15-21), right to complain to supervisory authority
- **Cookie consent** would be needed if Google Analytics is active (future enhancement)
- Footer links to both pages from all pages

### Features
- **Auto language detection:** Detects browser language on first visit, redirects to /de for German users
- **Language switcher:** Manual EN/DE toggle, saves preference in localStorage
- **SEO:** hreflang tags, Open Graph meta, semantic HTML, descriptive alt texts
- **Performance:** WebP images with PNG fallback, lazy loading, optimized assets

## Content

### Positioning
- **Title:** Legacy Modernization Expert
- **Tagline:** "I help companies modernize legacy systems, accelerate development, and integrate AI"
- **Target audience:** Companies with legacy systems, technical debt, or needing senior talent

### Pain Points to Address
1. Legacy systems holding back business growth
2. Difficulty finding senior talent (expensive, slow onboarding)
3. Technical debt piling up (quick fixes accumulated over years)

### Services
1. **Legacy Modernization** - Transform outdated systems, microservices, clean code
2. **AI Integration** - OpenAI APIs, ML pipelines, practical AI implementation
3. **Architecture Consulting** - System design, tech choices, scalability (iSAQB certified)
4. **Full-Stack Development** - Java, Spring Boot, React/Angular, cloud infrastructure

### Credentials
- 10+ years freelance experience (since 2014)
- AWS Certified Solutions Architect - Associate (2023)
- iSAQB Certified Professional for Software Architecture (2023)
- Certified Vaadin 24 Developer (2023)
- M.Sc. Information Technology (University of Stuttgart)

### Notable Clients/Industries
- Atruvia AG (Banking)
- Ippen Digital (Media - 3rd largest in Germany)
- Oncochain Solutions (Healthcare)
- Sweap.io (Event Management)
- BMW Motorrad (via Considion)
- DLR German Aerospace Center (Galileo satellite system)

### Testimonials

**Matthias Heicke (Sweap):**
> "Standout freelancer... expertise in Java and Vaadin with remarkable speed... exceptional proficiency in understanding complex requirements... analytical mindset for bug detection and resolution"

**Thomas Reiners:**
> "Very focused approach with rapid completion of deliverables... maintained high quality standards... would sign up for the next project again"

## Contact & Links

- **Booking:** https://calendar.app.google/5aJYvSXHJigk6raE9 (Google Calendar)
- **Email:** contact@radugeo.com
- **Phone:** +49 176 588 30284
- **LinkedIn:** https://www.linkedin.com/in/rgeoroceanu
- **Location:** Munich, Germany

## Assets

- [x] Logo (RG monogram - teal/silver 3D, transparent background)
- [x] Profile photo (in About section)
- [x] Favicon (derived from logo)

### Optimized Image Files (in public/)
| File | Purpose | Format |
|------|---------|--------|
| logo-nav.webp / .png | Navigation logo | WebP + PNG fallback |
| logo-footer.webp / .png | Footer logo | WebP + PNG fallback |
| profile.webp / .png | About section photo | WebP + PNG fallback |
| favicon.ico / .png | Browser tab icon | ICO + PNG |

## File Structure

```
radugeo-com/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions deploy workflow
├── public/
│   ├── CNAME                   # Custom domain for GitHub Pages
│   ├── favicon.ico
│   ├── favicon.png
│   ├── logo-nav.png
│   ├── logo-nav.webp
│   ├── logo-footer.png
│   ├── logo-footer.webp
│   ├── profile.png
│   └── profile.webp
├── src/
│   ├── components/
│   │   ├── Hero.astro
│   │   ├── PainPoints.astro
│   │   ├── Services.astro
│   │   ├── About.astro
│   │   ├── Testimonials.astro
│   │   └── CTA.astro
│   ├── i18n/
│   │   └── translations.ts    # EN/DE translations + helpers
│   ├── layouts/
│   │   └── Layout.astro       # Main layout (nav, footer, scripts)
│   ├── pages/
│   │   ├── index.astro        # English homepage
│   │   ├── impressum.astro    # Impressum (EN)
│   │   ├── privacy.astro      # Privacy Policy (EN)
│   │   └── de/
│   │       ├── index.astro    # German homepage
│   │       ├── impressum.astro # Impressum (DE)
│   │       └── datenschutz.astro # Datenschutzerklärung (DE)
│   └── styles/
│       └── global.css         # Tailwind + custom theme + animations
├── astro.config.mjs
├── package.json
├── tsconfig.json
└── CLAUDE.md
```

## Development Commands

```bash
npm run dev      # Start dev server (http://localhost:4321)
npm run build    # Build for production (output: dist/)
npm run preview  # Preview production build
```

## Deployment

### GitHub Pages (with custom domain radugeo.com)

**GitHub repo:** github.com/rgeoroceanu/radugeo-com

**Automatic deployment:** Push to `main` triggers GitHub Actions → builds → deploys to GitHub Pages.

**DNS (Squarespace):**

A records (root domain):
- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

CNAME record (www):
- www → rgeoroceanu.github.io

**GitHub repo settings:**
1. Settings → Pages → Source: GitHub Actions
2. Settings → Pages → Custom domain: radugeo.com
3. Settings → Pages → Enforce HTTPS: enabled
