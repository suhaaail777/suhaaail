# GitHub Upload Guide

## Step 1: Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon (top right) → **New repository**
3. Repository name: `portfolio` (or any name you prefer)
4. Make it **Public** (for free hosting)
5. Check **Add a README file** (optional)
6. Click **Create repository**

## Step 2: Upload Your Files

### Method A: Web Upload (Easiest)

1. In your new repo, click **Add file** → **Upload files**
2. Drag and drop all files from `s:\projects\portofolio`
3. Wait for upload to complete
4. Add commit message: "Initial portfolio upload"
5. Click **Commit changes**

### Method B: Git Command Line

```bash
# Navigate to your portfolio folder
cd s:\projects\portofolio

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial portfolio upload"

# Connect to GitHub (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git

# Push to GitHub
git push -u origin main
```

## Step 3: Enable GitHub Pages (Free Hosting)

1. Go to your repository on GitHub
2. Click **Settings** (top right tab)
3. Scroll down to **Pages** section (left sidebar)
4. Under **Source**, select **Deploy from a branch**
5. Select **main** branch and **/ (root)** folder
6. Click **Save**
7. Wait 1-2 minutes for the site to deploy

## Step 4: Your Live URL

Your portfolio will be live at:
```
https://YOUR_USERNAME.github.io/portfolio/
```

## File Structure to Upload

```
portfolio/
├── index.html              (main page)
├── resume.html             (CV)
├── profile-photo.png       (your photo)
├── manifest.json
├── robots.txt
├── sitemap.xml
├── sw.js
├── animations-id-card.html
├── animations-stroke-fill.html
├── animations-symbol-decode.html
├── project-showcase.jpg    (rename the long filename!)
├── certificates/
│   ├── akai-certificate.html
│   ├── b777-certificate.html
│   ├── coreframe-certificate.html
│   ├── edappal-certificate.html
│   └── sevenify.html
└── .github/                (optional, for workflows)
```

## Quick Check Before Upload

✅ Files renamed (no spaces, lowercase)  
✅ `index.html` is your main page  
✅ All links work locally  
✅ Images display correctly  

## Troubleshooting

**Images not showing?**
- Check filenames match exactly (case-sensitive on GitHub)
- Use relative paths: `profile-photo.png` not `C:\path\photo.png`

**404 error?**
- Ensure `index.html` exists at root
- Check GitHub Pages is enabled in Settings

**Changes not updating?**
- GitHub Pages takes 1-2 minutes to refresh
- Hard refresh: `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)

## Need Help?

- GitHub Docs: [pages.github.com](https://pages.github.com)
- Video tutorial: Search "GitHub Pages tutorial" on YouTube
