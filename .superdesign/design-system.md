# Manali Cinematic Portfolio Design System

## Product Context
- Product: Single-page cinematic portfolio
- Audience: Recruiters, clients, collaborators
- Primary goals: Showcase brand, skills, project highlights, and contact CTA

## Core Visual Direction
- Style: Dark cinematic, glassmorphism, neon-accented gradients
- Mood: Premium, futuristic, creator-focused
- Visual rhythm: High-contrast hero, card-based sections, soft animated motion

## Color Tokens
```css
:root {
  --bg-dark: #05070a;
  --bg-light: #f8fafc;
  --accent-cyan: #22d3ee;
  --accent-purple: #a855f7;
  --accent-pink: #ec4899;
}
```

- Base background: `#05070a`
- Primary text on dark: `#ffffff`
- Secondary text on dark: Tailwind `text-gray-400` / `text-gray-500`
- Accent sequence: cyan -> purple -> pink

## Typography
- Display font: `Cabinet Grotesk` (bold headlines)
- Body font: `Satoshi` (UI/body copy)
- Headline style: Extra bold, tight tracking, large responsive scale

## Surfaces & Effects
- Shared glass style:
```css
.glass {
  background: rgba(255, 255, 255, 0.03);
  backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.1);
}
```
- Glow utility:
```css
.glow-cyan {
  box-shadow: 0 0 20px rgba(34, 211, 238, 0.2);
}
```

## Spacing & Layout
- Section vertical spacing: `py-32`
- Container width: `max-w-7xl` (or `max-w-4xl` for contact)
- Core grid patterns:
  - About: `grid-cols-1 lg:grid-cols-2`
  - Skills: `grid-cols-2 md:grid-cols-3 lg:grid-cols-6`
  - Projects: `grid-cols-1 md:grid-cols-2`

## Motion
- Floating ornaments via custom keyframes (`float`)
- Hero scroll parallax via GSAP + ScrollTrigger
- Section entrance: fade + upward translate

## Component Conventions
- Navigation: fixed top bar with pill glass menu
- CTA buttons: rounded-full/rounded-2xl with hover scale
- Project cards: image-led cards with overlay badges and hover reveal icon
- Contact panel: large glass container with blurred accent blobs

## Interaction Patterns
- Smooth anchor scrolling by document class `scroll-smooth`
- Theme toggle in nav (dark/light class toggling)
- Hover-driven visual feedback (borders, glow, opacity, scale)

## Accessibility Notes
- Ensure icon-only links have `aria-label` in future iterations
- Preserve text/background contrast when enabling light mode
- Keep animations subtle and optional for reduced motion support in future
