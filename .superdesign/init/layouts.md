# Shared Layout Components

There are no separate layout component files in the current repository. Layout is authored directly within static page files.

## Main layout source
- Source file: `index1.html`
- Layout areas included:
  - Fixed top navigation
  - Full-page hero
  - Section stack (`about`, `skills`, `projects`, `contact`)
  - Footer

```html
<!-- Layout excerpt from index1.html -->
<div id="root-container" class="min-h-screen bg-[#05070a] text-white transition-colors duration-500 selection:bg-cyan-500/30 selection:text-cyan-200">
  <nav id="main-nav" class="fixed top-0 left-0 w-full z-50 px-6 md:px-12 py-6 flex items-center justify-between">
    <!-- ... -->
  </nav>

  <section id="hero" class="relative min-h-screen flex flex-col items-center justify-center px-6 overflow-hidden">
    <!-- ... -->
  </section>

  <section id="about" class="py-32 px-6 md:px-24">
    <!-- ... -->
  </section>

  <section id="skills" class="py-32 bg-white/5">
    <!-- ... -->
  </section>

  <section id="projects" class="py-32 px-6">
    <!-- ... -->
  </section>

  <section id="contact" class="py-32 px-6">
    <!-- ... -->
  </section>

  <footer class="py-12 px-6 border-t border-white/5 flex flex-col md:flex-row justify-between items-center gap-6">
    <!-- ... -->
  </footer>
</div>
```
