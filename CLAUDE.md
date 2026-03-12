# CLAUDE.md — Studio 9 Design & Supply Website

## Project Overview
Teaser/landing page for Studio 9 Design & Supply, an interior design studio and premium materials showroom in Fortitude Valley, Brisbane. Currently a static landing page hosted on GitHub Pages at s9d.com.au. Full WordPress site build planned on ArcHub theme.

## Brand Guidelines

### Colours
- Primary dark olive: `#6E6F4E` (CSS var: `--olive-dark`)
- Secondary light olive: `#9C9D72` (`--olive-light`)
- Background cream: `#F4F0EF` (`--cream`)
- Faint olive (borders/accents): `#C5C6A8` (`--olive-faint`)
- Olive wash: `#E8E6DB` (`--olive-wash`)
- Text dark: `#3A3B2E` (`--text-dark`)
- White: `#FAFAF8` (`--white`)

### Fonts (Google Fonts)
- Display/headings: MuseoModerno (weights 300–600, including italic) — `--font-display`
- Body/labels: Bebas Neue — `--font-heading`

### Logo
- Custom "9" mark: `logo-9.jpg` (olive green on cream)
- Text lockup: "STUDIO" in MuseoModerno + 9 mark image + "DESIGN & SUPPLY" in Bebas Neue below
- The logo JPG uses `mix-blend-mode: multiply` to blend the cream background with the page

### Tagline
"The design & supply destination that delivers expert interior design, hands-on project management, and premium finishes — streamlining every stage of your construction project."

## Business Details
- **Name:** Studio 9 Design & Supply (formerly ASA Tiles)
- **Address:** Shop 9, 1000 Ann Street, Fortitude Valley QLD 4006
- **Phone:** 07 3257 4940
- **Email:** hello@s9d.com.au
- **Domain:** s9d.com.au
- **Services:** Interior Design, Project Management, Premium Finishes, Material Supply

## File Structure
```
/
├── index.html          # Landing/teaser page (all HTML, CSS, and JS in one file)
├── logo-9.jpg          # Brand 9 mark (olive on cream, ~34 KB)
├── CNAME               # GitHub Pages custom domain (s9d.com.au)
└── CLAUDE.md           # This file
```

## Technical Notes
- **Static HTML/CSS/JS** — no build tools, no framework, everything in `index.html`
- **Hosted on GitHub Pages** — repo: `heyitsmeez/studio9-website`, branch: `master`
- **Custom domain:** s9d.com.au (DNS via GoDaddy, CNAME file in repo root)
- **Google Fonts** loaded via `<link>` tags with `preconnect` for performance
- **CSS custom properties** defined in `:root` for all colours and font families
- **Animations** use CSS `@keyframes` with staggered `animation-delay` values (0.3s–2.6s) for a sequenced page reveal
- **Background texture:** subtle 80px grid using CSS `linear-gradient` at 4% olive opacity, applied via `body::before`
- **Watermark:** giant "9" character positioned bottom-right at 4% olive opacity
- **Inline `<script>`** at the bottom handles Mailchimp form submission with a fallback that shows a success message when no Mailchimp URL is configured
- **OG meta tags** present for social sharing (og:title, og:description, og:type, og:url)
- Email addresses must not use Cloudflare email protection encoding — use plain `mailto:` links

### Pending TODOs (found in code)
- Mailchimp form action URL still needs configuring (currently placeholder `YOUR_MAILCHIMP_FORM_ACTION_URL`)
- Instagram social link URL needs updating (currently `#`)

## Page Structure (index.html)
1. **Decorative border frame** — fixed-position with CSS corner accents
2. **Background watermark** — giant "9" character, decorative only (`aria-hidden`)
3. **Logo lockup** — "STUDIO" + 9 mark image + "Design & Supply" subtitle
4. **Divider** — horizontal olive line
5. **Tagline** — brand tagline paragraph
6. **Coming Soon badge** — olive pill/badge
7. **Enquiry CTA** — directs visitors to email hello@s9d.com.au
8. **Email signup form** — Mailchimp integration (pending configuration)
9. **Services list** — four service items with dot separators
10. **Footer** — address, phone, email, Instagram link

## Design Principles
- Clean, minimal, warm, premium aesthetic
- Generous white space
- Subtle grid texture background
- Decorative border frame with corner accents
- Staggered reveal animations on page load
- This is a design studio, NOT a tile shop — position accordingly

## Key Stakeholders
- Dean Short — Showroom Manager (budget approval)
- Bella Fischer — Interior Designer / Design Consultant (content, design assets)
- Ewan Monro — IT/PM (you're talking to him via Claude Code)

## Conventions
- Australian English spelling
- Use semantic HTML
- Mobile-first responsive design (breakpoint at 600px)
- Keep it as a single `index.html` file for now (no build step)
- All CSS is inline in `<style>` within `<head>`
- All JS is inline in `<script>` at bottom of `<body>`
- Commit messages: imperative mood, concise
- Default branch: `master`
