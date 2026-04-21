# Extractable Components

## NavBar
- Source: `index1.html`
- Category: layout
- Description: Top fixed navigation with logo, section links, and theme toggle.
- Extractable props: `activeSection` (string, default: "contact")
- Hardcoded: logo image source, text labels, icon names, glass classes

## HeroSection
- Source: `index1.html`
- Category: layout
- Description: Intro hero with floating visual elements, main headline, and CTAs.
- Extractable props: `headlineName` (string, default: "MANALI")
- Hardcoded: gradient style, float animation, CTA class styles

## SkillsGrid
- Source: `index1.html`
- Category: basic
- Description: Grid of skill cards with logos and hover states.
- Extractable props: `title` (string, default: "The Arsenal")
- Hardcoded: individual icon tokens and card classes

## ProjectCard
- Source: `index1.html`
- Category: basic
- Description: Media-first project showcase card with overlay and external-link affordance.
- Extractable props: `title` (string), `description` (string), `tag` (string), `imageUrl` (string)
- Hardcoded: glass shell style, hover transitions, overlay treatment

## ContactPanel
- Source: `index1.html`
- Category: layout
- Description: CTA + form container with glowing background blobs and social links.
- Extractable props: `heading` (string), `ctaLabel` (string)
- Hardcoded: blob effect layers, social icon set, spacing tokens
