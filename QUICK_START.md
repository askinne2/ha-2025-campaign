# 🚀 Quick Start Guide
## Get Your Campaign Site Live in 15 Minutes

---

## ⏱️ 15-Minute Deployment

### Step 1: Test Locally (3 minutes)

```bash
# Navigate to your folder
cd "/Users/andrewskinner/Library/CloudStorage/Dropbox/Creative Cloud Files/0-HA-CC/2025/4 - 2025 EOY/2025 HA EOY Overview"

# Open the site
open index.html
```

**Quick Check:**
- ✅ Landing page loads
- ✅ Click "Campaign Strategy" → page loads
- ✅ Click "Campaign Calendar" → page loads
- ✅ Click "Home" → returns to landing page
- ✅ Resize browser → mobile menu appears

---

### Step 2: Create GitHub Repository (2 minutes)

1. Go to https://github.com/new
2. Repository name: `ha-2025-campaign`
3. Make it **Public**
4. **Don't** initialize with README
5. Click **Create repository**

---

### Step 3: Push Your Files (5 minutes)

Copy and paste these commands:

```bash
# Initialize git
git init

# Add campaign files only
git add index.html campaign-strategy.html campaign-calendar.html
git add assets/ README.md .gitignore
git add DEPLOYMENT_GUIDE.md PROJECT_SUMMARY.md QUICK_START.md

# Commit
git commit -m "Initial commit: HA 15th Anniversary Campaign site"

# Add your repository (REPLACE with your actual URL)
git remote add origin https://github.com/YOUR-USERNAME/ha-2025-campaign.git

# Push
git branch -M main
git push -u origin main
```

**Replace `YOUR-USERNAME` with your actual GitHub username!**

---

### Step 4: Enable GitHub Pages (2 minutes)

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in left sidebar)
3. Under "Source":
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait 2 minutes

---

### Step 5: Visit Your Live Site! (1 minute)

Your site is now live at:
```
https://YOUR-USERNAME.github.io/ha-2025-campaign/
```

**Test it:**
- Visit the URL
- Try on your phone
- Share with your team

---

## 🎯 What You Get

### 3 Pages, All Connected

```
Landing Page (index.html)
    ├─→ Campaign Strategy
    └─→ Campaign Calendar
```

### Every Page Has:
- ✅ Navigation bar (sticky at top)
- ✅ Hispanic Alliance branding
- ✅ Mobile-responsive
- ✅ Print-friendly

---

## 📱 Quick Mobile Test

1. Visit site on your phone
2. Tap the ☰ menu icon (top right)
3. Menu appears
4. Tap "Campaign Strategy"
5. Page loads
6. Navigation still works

**If this works, you're 100% ready! ✅**

---

## 🖨️ Quick Print Test

1. Open any page
2. Press Cmd+P (Mac) or Ctrl+P (Windows)
3. Check print preview
4. Navigation should hide automatically
5. Content should look clean

---

## 🔗 Share With Your Team

**Email Template:**

```
Subject: New Campaign Planning Site - Live Now!

Hi team,

Our 15th Anniversary Campaign planning site is now live:

https://YOUR-USERNAME.github.io/ha-2025-campaign/

Quick links:
• Campaign Strategy: [URL]/campaign-strategy.html
• Campaign Calendar: [URL]/campaign-calendar.html

The site is mobile-friendly and print-friendly.
Bookmark it for easy access!

Questions? Reply to this email.

Thanks!
```

---

## ⚡ Common Quick Fixes

### "My site shows 404"
- Wait 2-3 more minutes
- Make sure repository is Public
- Check Settings → Pages is enabled

### "CSS not loading"
- Hard refresh: Cmd+Shift+R (Mac) or Ctrl+Shift+R (Windows)
- Check that `assets/css/styles.css` exists in your repository

### "Navigation doesn't work"
- Make sure all files are in root directory
- Check file names match exactly (case-sensitive)

---

## 📞 Need Help?

**Stuck?** 
- Check `DEPLOYMENT_GUIDE.md` for detailed troubleshooting
- Review `PROJECT_SUMMARY.md` for complete documentation
- Contact your IT/web team

**Everything working?** 
🎉 Congratulations! Your site is live and ready to use!

---

## 🔄 Making Updates Later

When you need to update content:

```bash
# Edit your HTML files

# Then push changes:
git add .
git commit -m "Update campaign dates"
git push

# Site updates automatically in 1-2 minutes
```

---

## ✅ Quick Success Checklist

After deployment, verify:

- [ ] Site loads at GitHub Pages URL
- [ ] All three pages accessible
- [ ] Navigation works between pages
- [ ] Mobile view works (test on phone)
- [ ] Shared URL with development team
- [ ] Bookmarked for quick access

---

**That's it! You're live! 🚀**

*Total time: ~15 minutes*  
*Difficulty: Easy*  
*Result: Professional campaign planning site!*

