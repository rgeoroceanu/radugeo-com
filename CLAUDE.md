# Radu Georoceanu - Professional Freelancing Website

## Project Overview

A professional website for Radu Georoceanu's freelancing software services, focused on **legacy modernization** and **AI integration**.

## Tech Stack

- **Framework:** Astro (static site generator)
- **Styling:** Tailwind CSS v4
- **Hosting:** Netlify (or GitHub Pages)
- **Languages:** Bilingual (English + German)

## Design Requirements

### Style Reference
- Reference site: https://uxcontinuum.com/
- **Theme:** Dark-first aesthetic (navy/dark backgrounds)
- **Accent color:** Teal (#14b8a6) - matches existing CV branding
- **Typography:** Clean, modern (Inter font family)
- **Animations:** Subtle hover effects, smooth transitions (not excessive)

### Design Principles
- Modern but minimalist
- Eye-catching with 1-2 tasteful animations
- Mobile-responsive
- Accessibility-conscious

## Site Structure

### Sections (Single-page design)
1. **Navigation** - Fixed top nav with language switcher, "Book a Call" CTA
2. **Hero** - Tagline, brief intro, primary CTA
3. **Pain Points** - 3 cards addressing client challenges
4. **Services** - 4 service cards (Legacy Modernization, AI Integration, Architecture Consulting, Full-Stack Dev)
5. **About/Credentials** - Stats, certifications, bio
6. **Testimonials** - 2 LinkedIn recommendations
7. **CTA Section** - Final call-to-action with booking link
8. **Footer** - Contact info, social links

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

## Assets Needed

- [ ] Professional photo (user will provide)
- [x] Favicon (create simple "RG" favicon)

## File Structure

```
radugeo-com/
├── public/
│   ├── images/
│   │   └── profile.jpg (to be provided)
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Hero.astro
│   │   ├── PainPoints.astro
│   │   ├── Services.astro
│   │   ├── About.astro
│   │   ├── Testimonials.astro
│   │   └── CTA.astro
│   ├── i18n/
│   │   └── translations.ts
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   ├── index.astro (English)
│   │   └── de/
│   │       └── index.astro (German)
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── package.json
├── tailwind.config.mjs
└── CLAUDE.md
```

## Development Commands

```bash
npm run dev      # Start dev server
npm run build    # Build for production
npm run preview  # Preview production build
```

## Deployment

Deploy to Netlify:
1. Connect GitHub repository
2. Build command: `npm run build`
3. Publish directory: `dist`
