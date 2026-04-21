# Page Dependency Trees

## / (Expanded Portfolio)
Entry: `index.html`
Dependencies:
- `index.html` (self-contained)
  - inline `<style>` block
  - external script CDN: Tailwind, Iconify, Three.js, GSAP, ScrollTrigger
  - inline `<script>` block for matrix, Three.js scene, and animations

## /index1.html (Cinematic 3D Portfolio)
Entry: `index1.html`
Dependencies:
- `index1.html` (self-contained)
  - inline `<style>` block
  - external script CDN: Tailwind, Iconify, GSAP, ScrollTrigger
  - inline `<script>` block for theme toggle + section motion

## Key Notes
- No local component/module imports yet
- No framework page-level composition yet
- Best migration target is to split `index1.html` sections into reusable components
