# GitHub Pages Setup Guide

This guide will help you host your portfolio on GitHub Pages.

## Prerequisites
- GitHub account (free)
- Git installed on your computer
- Your portfolio files ready

## Step-by-Step Instructions

### Step 1: Create a GitHub Repository

1. Go to **https://github.com**
2. Click the **"+"** icon in the top right → **"New repository"**
3. Repository name: `ibrahim-portfolio` (or any name you prefer)
4. Description: "Personal Portfolio Website"
5. Make sure it's set to **Public**
6. **DO NOT** initialize with README, .gitignore, or license
7. Click **"Create repository"**

### Step 2: Initialize Git in Your Portfolio Folder

Open your terminal/command prompt in your portfolio folder (`c:\ibrahim-portfolio`) and run:

```bash
git init
git add .
git commit -m "Initial commit - Portfolio website"
```

### Step 3: Connect to GitHub and Push

```bash
git branch -M main
git remote add origin https://github.com/Aromoyeibm/ibrahim-portfolio.git
git push -u origin main
```

*(Note: Replace `Aromoyeibm` with your GitHub username and `ibrahim-portfolio` with your repository name)*

### Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (at the top of your repository)
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select **"Deploy from a branch"**
5. Branch: select **"main"**
6. Folder: select **"/(root)"**
7. Click **Save**

### Step 5: Access Your Live Portfolio

Your portfolio will be available at:
```
https://Aromoyeibm.github.io/ibrahim-portfolio/
```

*(Replace with your GitHub username and repository name)*

## Important Notes for Your Portfolio

### EmailJS Configuration
Your contact form uses EmailJS. After hosting on GitHub Pages, you'll need to:

1. Add your GitHub Pages URL to EmailJS's authorized domains
2. Go to EmailJS dashboard → **Add-ons** → **Authorized domains**
3. Add your GitHub Pages URL (e.g., `https://Aromoyeibm.github.io`)

### File Structure
Make sure your files are in the root directory:
```
ibrahim-portfolio/
├── index.html
├── styles.css
├── script.js
├── images/
│   ├── profile.jpg
│   ├── license.jpg
│   ├── project1-1.png
│   ├── project1-2.png
│   └── ... (all other images)
└── README.md
```

### Making Future Updates

Whenever you update your portfolio:

```bash
git add .
git commit -m "Description of changes"
git push
```

Your changes will go live within 1-2 minutes.

## Alternative: GitHub Desktop (GUI Method)

If you prefer using a graphical interface:

### Using GitHub Desktop App

1. **Download GitHub Desktop**: https://desktop.github.com/
2. **Install and sign in** with your GitHub account
3. **Add your portfolio folder**:
   - Click "File" → "Add Local Repository"
   - Navigate to `c:\ibrahim-portfolio`
   - Select the folder
4. **Publish to GitHub**:
   - Click "Publish repository"
   - Choose repository name: `ibrahim-portfolio`
   - Make it public
   - Click "Publish"
5. **Enable GitHub Pages** (same as Step 4 above)

## Troubleshooting

### Site Not Loading?
- Wait 1-2 minutes after enabling GitHub Pages
- Check the URL is correct (case-sensitive)
- Go to Settings → Pages to verify deployment status

### Images Not Showing?
- Check file paths are correct (e.g., `images/profile.jpg`)
- File names are case-sensitive on GitHub
- Make sure all images are committed and pushed

### Contact Form Not Working?
- Add your GitHub Pages URL to EmailJS authorized domains
- Verify all EmailJS credentials are set correctly

## Custom Domain (Optional)

Want to use your own domain?

1. In your repository Settings → Pages
2. Add your custom domain
3. Follow GitHub's instructions to verify it
4. Add a `CNAME` file with your domain name

## Security Tips

1. **Don't commit sensitive data** like EmailJS keys directly
2. Consider using environment variables (for future enhancements)
3. Keep your repository public for GitHub Pages (or upgrade to paid GitHub plan)

## Need Help?

- GitHub Pages Documentation: https://pages.github.com/
- GitHub Community: https://github.community/

---

**Your live portfolio will be accessible at:**
`https://Aromoyeibm.github.io/ibrahim-portfolio/` 
*(Remember to replace with your actual GitHub username)*

