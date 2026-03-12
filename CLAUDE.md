# CLAUDE.md — Studio 9 Design & Supply Website

## Project Overview
Teaser/landing page for Studio 9 Design & Supply, an interior design studio and premium materials showroom in Fortitude Valley, Brisbane. Currently a static landing page hosted on GitHub Pages at s9d.com.au. Full WordPress site build planned on ArcHub theme.

## Brand Guidelines

### Colours
- Primary dark olive: #6E6F4E
- Secondary light olive: #9C9D72
- Background cream: #F4F0EF
- Faint olive (borders/accents): #C5C6A8
- Text dark: #3A3B2E
- White: #FAFAF8

### Fonts (Google Fonts)
- Display/headings: MuseoModerno (weights 300-600, including italic)
- Body/labels: Bebas Neue

### Logo
- Custom "9" mark: logo-9.jpg (olive green on cream)
- Text lockup: "STUDIO" in MuseoModerno + 9 mark + "DESIGN & SUPPLY" in Bebas Neue below

### Tagline
"The design & supply destination that delivers expert interior design, hands-on project management, and premium finishes — streamlining every stage of your construction project."

## Business Details
- **Name:** Studio 9 Design & Supply (formerly ASA Tiles)
- **Address:** Shop 9, 1000 Ann Street, Fortitude Valley QLD 4006
- **Phone:** 07 3257 4940
- **Email:** hello@studio9design.com.au
- **Services:** Interior Design, Project Management, Premium Finishes, Material Supply

## File Structure
```
/
├── index.html          # Landing/teaser page
├── logo-9.jpg          # Brand 9 mark (olive on cream)
├── CNAME               # GitHub Pages custom domain (s9d.com.au)
└── CLAUDE.md           # This file
```

## Technical Notes
- Static HTML/CSS only (no build tools, no JS framework)
- Hosted on GitHub Pages (repo: heyitsmeez/studio9-website)
- Custom domain: s9d.com.au (DNS via GoDaddy)
- The logo JPG uses `mix-blend-mode: multiply` to blend cream background with page
- Animations use CSS @keyframes (staggered fade-in/slide-up)
- Mailchimp form action URL still needs configuring (placeholder in HTML)
- Email addresses must not use Cloudflare email protection encoding

## Design Principles
- Clean, minimal, warm, premium aesthetic
- Generous white space
- Subtle grid texture background (olive at 4% opacity, 80px grid)
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
- Mobile-first responsive design
- Keep it as a single index.html file for now (no build step)
- Commit messages: imperative mood, concise
