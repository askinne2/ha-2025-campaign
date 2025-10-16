# GitHub Pages Deployment Guide
## Hispanic Alliance Campaign Mini-Site

This guide will help you deploy the Hispanic Alliance 15th Anniversary Campaign site to GitHub Pages.

---

## 📋 Pre-Deployment Checklist

Before deploying, verify:

- [x] All HTML files are present and working
  - `index.html`
  - `campaign-strategy.html`
  - `campaign-calendar.html`
- [x] Shared CSS stylesheet exists
  - `assets/css/styles.css`
- [x] Navigation works between pages
- [x] README.md is complete
- [x] .gitignore is in place

---

## 🚀 Deployment Steps

### Option 1: Deploy from Root Directory (Recommended)

#### Step 1: Create GitHub Repository

1. Go to [GitHub.com](https://github.com)
2. Click the **+** icon → **New repository**
3. Repository name: `ha-2025-campaign` (or your preferred name)
4. Description: "Hispanic Alliance 15th Anniversary Campaign Planning Resources"
5. Choose **Public** (for GitHub Pages to work with free account)
6. **Do NOT** initialize with README (we have one already)
7. Click **Create repository**

#### Step 2: Push Files to GitHub

```bash
# Navigate to your project folder
cd "/Users/andrewskinner/Library/CloudStorage/Dropbox/Creative Cloud Files/0-HA-CC/2025/4 - 2025 EOY/2025 HA EOY Overview"

# Initialize git repository
git init

# Add all campaign site files
git add index.html
git add campaign-strategy.html
git add campaign-calendar.html
git add assets/
git add README.md
git add .gitignore
git add DEPLOYMENT_GUIDE.md

# Commit files
git commit -m "Initial commit: HA 15th Anniversary Campaign site"

# Add remote repository (replace with your actual repository URL)
git remote add origin https://github.com/YOUR-USERNAME/ha-2025-campaign.git

# Push to GitHub
git branch -M main
git push -u origin main
```

#### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (gear icon)
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes for deployment

#### Step 4: Access Your Site

Your site will be available at:
```
https://YOUR-USERNAME.github.io/ha-2025-campaign/
```

---

### Option 2: Deploy from /docs Directory

If you prefer to keep the site in a `/docs` folder:

#### Step 1: Organize Files

```bash
# Create docs directory
mkdir docs

# Move site files to docs
mv index.html docs/
mv campaign-strategy.html docs/
mv campaign-calendar.html docs/
mv assets docs/

# Keep README.md in root
# Keep .gitignore in root
```

#### Step 2: Update Links (if needed)

All links in the HTML files use relative paths, so they'll work fine in `/docs`.

#### Step 3: Push to GitHub

```bash
git init
git add docs/
git add README.md
git add .gitignore
git commit -m "Initial commit: HA campaign site in /docs"
git remote add origin https://github.com/YOUR-USERNAME/ha-2025-campaign.git
git branch -M main
git push -u origin main
```

#### Step 4: Configure GitHub Pages

1. Go to Settings → Pages
2. Select:
   - Branch: `main`
   - Folder: `/docs`
3. Click **Save**

---

## 🔧 Troubleshooting

### Links Not Working

**Problem:** Navigation links show 404 errors

**Solution:** 
- Verify all files are in the same directory structure
- Check that file names match exactly (case-sensitive)
- Make sure you're using relative paths (no `/` at the beginning)

### CSS Not Loading

**Problem:** Pages appear unstyled

**Solution:**
- Verify `assets/css/styles.css` exists
- Check that the path in HTML files is: `href="assets/css/styles.css"`
- Clear browser cache and hard reload (Cmd+Shift+R or Ctrl+Shift+R)

### Site Not Deploying

**Problem:** GitHub Pages shows error or site doesn't appear

**Solution:**
- Wait 2-5 minutes (deployment can take time)
- Check Actions tab for build errors
- Verify repository is Public
- Make sure you selected the correct branch and folder

---

## 📱 Testing Your Deployment

After deployment, test these features:

### Desktop Testing
- [ ] Navigate to all three pages (Home, Strategy, Calendar)
- [ ] Click navigation links - verify they work
- [ ] Check that CSS loads properly
- [ ] Verify colors match HA branding
- [ ] Test print preview (Cmd/Ctrl + P)

### Mobile Testing
- [ ] Visit site on phone/tablet
- [ ] Check hamburger menu works
- [ ] Verify navigation cards stack vertically
- [ ] Test touch targets are large enough
- [ ] Check calendar tables scroll if needed

### Accessibility Testing
- [ ] Navigate using keyboard only (Tab key)
- [ ] Test screen reader (VoiceOver on Mac, NVDA on Windows)
- [ ] Verify sufficient color contrast
- [ ] Check skip-to-content link works

---

## 🎨 Customization After Deployment

### Update Repository URL in README

1. Edit `README.md`
2. Find `[Your GitHub Pages URL will go here]`
3. Replace with actual URL: `https://YOUR-USERNAME.github.io/ha-2025-campaign/`
4. Commit and push changes:
   ```bash
   git add README.md
   git commit -m "Update README with live site URL"
   git push
   ```

### Add Custom Domain (Optional)

If you have a custom domain:

1. Go to Settings → Pages
2. Under "Custom domain", enter: `campaign.hispanicalliancesc.com` (example)
3. Click Save
4. Add CNAME record with your DNS provider
5. Wait for DNS propagation (can take 24-48 hours)

---

## 📊 Analytics (Optional)

To track site usage, add Google Analytics:

1. Get tracking code from Google Analytics
2. Add before closing `</head>` tag in all three HTML files
3. Commit and push changes

---

## 🔄 Updating the Site

When you need to update content:

```bash
# Make your changes to HTML/CSS files

# Stage changes
git add .

# Commit with descriptive message
git commit -m "Update campaign deadlines"

# Push to GitHub
git push

# Site will auto-update within 1-2 minutes
```

---

## 📧 Support

**For deployment issues:** Contact your technical team or GitHub support

**For campaign content updates:** Contact Development Team

**For design changes:** Contact Marketing/Communications

---

## ✅ Post-Deployment Checklist

After successful deployment:

- [ ] Site is live and accessible
- [ ] All navigation works
- [ ] Mobile responsive confirmed
- [ ] Shared with development team
- [ ] Shared with board members (if applicable)
- [ ] URL added to campaign materials
- [ ] Bookmarked for easy access

---

## 🎉 You're Done!

Your Hispanic Alliance Campaign site is now live and ready to support your team through the Quinceañera campaign!

**Share the URL:**
- Email to development team
- Include in board packet
- Bookmark for quick reference
- Add to campaign planning docs

**Need Help?** Refer to GitHub Pages documentation: https://docs.github.com/en/pages

---

*Last updated: October 2025*

