# GitHub Pages Deployment Guide (gh-pages)

## 🚀 Quick Setup

Your website is now configured to deploy to GitHub Pages at:
**https://pingpong-games.github.io**

## 📋 Steps to Deploy

### 1. Install Dependencies

First, install the `gh-pages` package:

```bash
bun install
```

### 2. Deploy Your Site

Simply run the deploy command:

```bash
bun run deploy
```

This will:
- Build your site (`astro build`)
- Push the `dist` folder to the `gh-pages` branch
- Deploy automatically to GitHub Pages

### 3. Configure GitHub Pages (First Time Only)

1. Go to your repository: https://github.com/PingPong-Games/pingpong-games.github.io
2. Click **Settings** → **Pages** (in the left sidebar)
3. Under **Source**, select:
   - Branch: **gh-pages**
   - Folder: **/ (root)**
4. Click **Save**

## 🌐 Access Your Site

After the first deployment (takes 2-3 minutes), visit:
**https://pingpong-games.github.io**

## 🔄 Deploying Updates

Every time you want to publish changes:

```bash
bun run deploy
```

That's it! Your changes will be live in 2-3 minutes.

## 📝 Content Management Workflow

Since Keystatic CMS requires server-side capabilities, it only works locally:

1. **Edit content locally:**
   ```bash
   bun run dev
   # Visit http://localhost:4321/keystatic
   ```

2. **Make your changes** in the Keystatic interface (add games, write blog posts, etc.)

3. **Commit your changes:**
   ```bash
   git add .
   git commit -m "Update content"
   ```

4. **Deploy to production:**
   ```bash
   bun run deploy
   ```

Your content changes will be published to the live site!

## ⚙️ What Was Changed

- ✅ Updated `site.config.ts` with your GitHub Pages URL
- ✅ Changed Astro output from `hybrid` to `static`
- ✅ Removed Cloudflare adapter (not needed for static sites)
- ✅ Added `gh-pages` package to deploy directly from your machine
- ✅ Created `deploy` script in `package.json`
- ✅ Added `.nojekyll` file to prevent Jekyll processing

## 🛠️ Local Testing

Before deploying, you can test locally:

```bash
# Build the site
bun run build

# Preview the production build
bun run preview
```

## 📝 Notes

- **First deployment** may take 3-5 minutes
- Subsequent deployments are faster (1-2 minutes)
- If you see a 404 error, wait a few minutes and refresh
- **Keystatic CMS** (`/keystatic`) only works in local development mode. To update content:
  1. Run `bun run dev` locally
  2. Edit content at `http://localhost:4321/keystatic`
  3. Content is saved as files in your repository
  4. Commit and run `bun run deploy` to publish changes

## 🔒 Authentication

The `gh-pages` package uses your Git credentials to push to the `gh-pages` branch. Make sure you're authenticated with GitHub (you already are if you can push code).

## 💡 Troubleshooting

**Site not showing up?**
- Verify GitHub Pages source is set to `gh-pages` branch
- Wait 2-3 minutes for deployment to complete
- Check if the `gh-pages` branch was created in your repository

**Build failing?**
- Check the terminal output for error messages
- Ensure all dependencies are installed: `bun install`
- Test the build locally first: `bun run build`

**Permission denied?**
- Make sure you're authenticated with GitHub
- Check that you have write access to the repository

## 🎉 You're Done!

Your PingPong Games Studio website will be live at https://pingpong-games.github.io after running `bun run deploy`!

## 📝 Quick Command Reference

```bash
# Install dependencies
bun install

# Run locally
bun run dev

# Build locally
bun run build

# Deploy to GitHub Pages
bun run deploy
```

