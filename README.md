# PingPong Games Studio

<a href="https://astro.build/">![Astro](.github/images/astro-icon.png)</a>
<a href="https://tailwindcss.com/">![Tailwind](.github/images/tailwind-icon.png)</a>
<a href="https://alpinejs.dev/">![Alpine js](.github/images/alpine-icon.png)</a>

PingPong Games Studio website - spinning up wildly fun mobile games for iOS and Android!

Built with [Astro](https://astro.build), [Tailwind CSS](https://tailwindcss.com/), and [AlpineJS](https://alpinejs.dev/), this site showcases our mobile game portfolio and development expertise.

This project is based on the [Mizar template](https://github.com/majesticooss/mizar).

---

## 🎮 Our Games

- **[Hindu Bubbles](https://play.google.com/store/apps/details?id=com.eyogi.hindububbles)** - A spiritually-themed bubble shooter featuring Hindu mythology, the Dashavatara lives system, and mystical power-ups
- **[Merge Garden](https://mergegarden.top/)** - A relaxing merge puzzle game where players create beautiful gardens by combining plants and flowers

---

## 🚀 Quick Start

### Prerequisites

- [Bun](https://bun.sh/) (recommended) or Node.js 18+

### Development

1. **Install dependencies:**
   ```bash
   bun install
   ```

2. **Start the dev server:**
   ```bash
   bun run dev
   ```

3. **Open your browser:**
   Navigate to `http://localhost:4321`

### Build for Production

```bash
bun run build
```

The built site will be in the `dist/` directory.

### Preview Production Build

```bash
bun run preview
```

### Deploy to GitHub Pages

```bash
bun run deploy
```

This will build and deploy your site to GitHub Pages automatically. See `DEPLOYMENT.md` for full deployment instructions.

---

## 🛠️ Tech Stack

- **Framework:** [Astro](https://astro.build/) - Fast, content-focused static site generator
- **Styling:** [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- **Interactivity:** [AlpineJS](https://alpinejs.dev/) - Lightweight JavaScript framework
- **Animations:** [GSAP](https://greensock.com/gsap/) - Professional-grade animation library
- **CMS:** [Keystatic](https://keystatic.com/) - Git-based content management
- **Package Manager:** [Bun](https://bun.sh/) - Fast all-in-one JavaScript runtime

## ✨ Features

- ✅ **Game Portfolio** - Showcase mobile games with beautiful previews and descriptions
- ✅ **Blog/News System** - Share updates and articles about game development and Dharma
- ✅ **Dark Mode** - Automatic dark theme with smooth transitions
- ✅ **Responsive Design** - Optimized for mobile, tablet, and desktop
- ✅ **Smooth Animations** - GSAP-powered scroll effects and transitions
- ✅ **Content Management** - Keystatic CMS for easy content editing
- ✅ **SEO Optimized** - Meta tags, Open Graph, and sitemap generation
- ✅ **PWA Ready** - Progressive Web App capabilities

## 📝 Content Management

### Admin Dashboard

Access the Keystatic CMS at `/keystatic` to manage:
- Game entries and descriptions
- Blog posts and news articles
- About page content
- Navigation and site configuration

For more information, see the [Keystatic documentation](https://keystatic.com/docs/introduction).

### Adding a New Game

1. Navigate to `/keystatic/collections/games`
2. Click "Create entry"
3. Fill in game details (title, description, tags, cover image)
4. Add game link and assets to `src/assets/games/[game-name]/`
5. Save and the game will appear on the homepage and games page

---

## 📁 Project Structure

```
/
├── public/              # Static assets (favicon, logo, etc.)
├── src/
│   ├── assets/          # Images, videos, and other assets
│   │   ├── games/       # Game cover images and assets
│   │   ├── pages/       # Page-specific assets
│   │   └── posts/       # Blog post assets
│   ├── components/      # Reusable Astro components
│   ├── content/         # Content collections (games, posts, pages)
│   │   ├── games/       # Game entries
│   │   ├── posts/       # Blog posts
│   │   └── pages/       # Static pages
│   ├── layouts/         # Page layout templates
│   ├── lib/             # Utility functions and helpers
│   └── pages/           # File-based routing
└── keystatic.config.ts  # CMS configuration
```

---

## 🌐 Deployment

The site is configured to deploy to **GitHub Pages** using the `gh-pages` package.

**Quick Deploy:**
```bash
bun run deploy
```

For detailed deployment instructions, see [DEPLOYMENT.md](./DEPLOYMENT.md).

**Alternative hosting platforms:**
- Netlify
- Vercel
- Cloudflare Pages

---

## 📄 License

Built using the [Mizar template](https://github.com/majesticooss/mizar) by [Majestico](https://majestico.co).

---

<p align="center">Made with ❤️ by PingPong Games Studio</p>
