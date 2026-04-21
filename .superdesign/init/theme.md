# Theme Sources

## Primary style source
- `index1.html` (embedded `<style>` block + Tailwind utility classes)

```css
@import url('https://api.fontshare.com/v2/css?f[]=cabinet-grotesk@800,700,400&f[]=satoshi@700,500,400&display=swap');

:root {
  --bg-dark: #05070a;
  --bg-light: #f8fafc;
  --accent-cyan: #22d3ee;
  --accent-purple: #a855f7;
  --accent-pink: #ec4899;
}

body {
  font-family: 'Satoshi', sans-serif;
  overflow-x: hidden;
}

.font-display {
  font-family: 'Cabinet Grotesk', sans-serif;
}

.glass {
  background: rgba(255, 255, 255, 0.03);
  backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.1);
}

.glass-light {
  background: rgba(0, 0, 0, 0.03);
  backdrop-filter: blur(12px);
  border: 1px solid rgba(0, 0, 0, 0.1);
}

.glow-cyan {
  box-shadow: 0 0 20px rgba(34, 211, 238, 0.2);
}

.text-glow {
  text-shadow: 0 0 10px rgba(34, 211, 238, 0.5);
}

@keyframes float {
  0%, 100% { transform: translateY(0px) rotate(0deg); }
  50% { transform: translateY(-20px) rotate(5deg); }
}

.animate-float {
  animation: float 6s ease-in-out infinite;
}

.animate-float-delayed {
  animation: float 8s ease-in-out infinite 1s;
}

@keyframes scroll-dot {
  0% { transform: translateY(0); opacity: 1; }
  100% { transform: translateY(12px); opacity: 0; }
}

.scroll-dot {
  animation: scroll-dot 1.5s infinite;
}

canvas#three-canvas {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1;
  pointer-events: none;
}

.theme-transition {
  transition: background-color 0.5s ease, color 0.5s ease;
}
```

## Tailwind config
- Dedicated `tailwind.config.*` file: Not present
- Tailwind usage source: CDN (`https://cdn.tailwindcss.com`)
