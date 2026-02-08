# 🚀 Deployment Guide

## GitHub Pages Setup

### Quick Start (5 minutes)

1. **Create a GitHub repository**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Word Nexus puzzle game"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/word-nexus.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click **Settings** → **Pages** (in the left sidebar)
   - Under "Source", select **main** branch
   - Click **Save**

3. **Access your game**
   - Your game will be live at: `https://YOUR_USERNAME.github.io/word-nexus/`
   - It may take 1-2 minutes for the site to build and deploy

### Custom Domain (Optional)

If you own a custom domain:

1. **Create CNAME file**
   ```bash
   echo "yourdomain.com" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push
   ```

2. **Configure DNS**
   - Add a CNAME record pointing to `YOUR_USERNAME.github.io`
   - Or add A records pointing to GitHub Pages IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```

3. **Update GitHub Settings**
   - Go to Settings → Pages
   - Enter your custom domain
   - Check "Enforce HTTPS"

## Alternative Deployment Options

### Netlify

1. Push your code to GitHub
2. Go to [Netlify](https://netlify.com)
3. Click "Add new site" → "Import an existing project"
4. Connect your GitHub repository
5. Deploy settings:
   - Build command: (leave empty)
   - Publish directory: `/`
6. Click "Deploy site"

### Vercel

1. Push your code to GitHub
2. Go to [Vercel](https://vercel.com)
3. Click "Import Project"
4. Select your repository
5. Click "Deploy"

### Cloudflare Pages

1. Push your code to GitHub
2. Go to [Cloudflare Pages](https://pages.cloudflare.com)
3. Click "Create a project"
4. Connect your GitHub repository
5. Build settings:
   - Build command: (leave empty)
   - Build output directory: `/`
6. Click "Save and Deploy"

## Local Testing

Before deploying, test locally:

```bash
# Option 1: Python
python -m http.server 8000

# Option 2: Node.js
npx http-server

# Option 3: PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## Troubleshooting

### GitHub Pages not showing
- Wait 2-3 minutes after enabling Pages
- Check that your repository is public (or you have GitHub Pro for private repos)
- Verify the branch is set to "main" in Pages settings

### 404 Error
- Ensure `index.html` exists in the root directory
- Check that `.nojekyll` file exists (bypasses Jekyll processing)

### Styles not loading
- Open browser console (F12) to check for errors
- Verify all files are committed and pushed
- Clear browser cache

### Custom domain not working
- DNS changes can take up to 48 hours to propagate
- Verify CNAME record is correct: `dig yourdomain.com`
- Check GitHub Pages settings shows your domain

## Performance Optimization

The game is already optimized, but for even better performance:

1. **Enable Cloudflare** (free CDN)
   - Speeds up global load times
   - Free SSL certificate
   - DDoS protection

2. **Compress assets**
   - GitHub Pages serves files with gzip compression automatically

3. **Monitor uptime**
   - Use [UptimeRobot](https://uptimerobot.com) for free monitoring

## Analytics (Optional)

Add Google Analytics or Plausible to track visitors:

```html
<!-- Add before </head> in index.html -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR-ID');
</script>
```

## Updates

To update your deployed game:

```bash
# Make changes to index.html or other files
git add .
git commit -m "Update: describe your changes"
git push
```

Changes will go live automatically within 1-2 minutes.

---

Need help? [Open an issue](https://github.com/YOUR_USERNAME/word-nexus/issues)
