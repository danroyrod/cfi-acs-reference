# GitHub Pages Deployment Guide

This guide will walk you through deploying your CFI ACS Reference Tool to GitHub Pages.

## 📋 Prerequisites

- GitHub account (free at github.com)
- Your prepared files (already done!)

## 🚀 Step-by-Step Deployment

### 1. Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **"+"** button in the top right corner
3. Select **"New repository"**
4. Fill in the details:
   - **Repository name**: `cfi-acs-reference` (or your preferred name)
   - **Description**: "Interactive CFI ACS reference tool for flight instructor candidates"
   - **Visibility**: Public (required for free GitHub Pages)
   - **Initialize**: Don't check any boxes (we'll upload files manually)
5. Click **"Create repository"**

### 2. Upload Files

#### Option A: Web Interface (Easiest)
1. In your new repository, click **"uploading an existing file"**
2. Drag and drop these files:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `README.md`
3. Add commit message: "Initial commit - CFI ACS Reference Tool"
4. Click **"Commit changes"**

#### Option B: Git Command Line (Advanced)
```bash
# Clone your repository
git clone https://github.com/YOUR_USERNAME/cfi-acs-reference.git
cd cfi-acs-reference

# Copy your files to the repository folder
# (Copy index.html, manifest.json, sw.js, README.md)

# Add and commit files
git add .
git commit -m "Initial commit - CFI ACS Reference Tool"
git push origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click the **"Settings"** tab
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select **"Deploy from a branch"**
5. Choose **"main"** branch and **"/ (root)"** folder
6. Click **"Save"**

### 4. Access Your Live Site

1. GitHub will show you the URL (usually takes 1-2 minutes)
2. Your site will be available at: `https://YOUR_USERNAME.github.io/cfi-acs-reference`
3. Bookmark this URL!

## 🎨 Optional: Add Icons (Recommended)

To make your app look more professional, add these icon files:

1. **Create icons** (192x192 and 512x512 pixels):
   - Use an aviation-themed icon or airplane symbol
   - Save as `icon-192.png` and `icon-512.png`

2. **Create favicons**:
   - `favicon-32x32.png` (32x32 pixels)
   - `favicon-16x16.png` (16x16 pixels)
   - `apple-touch-icon.png` (180x180 pixels)

3. **Upload to repository** (same process as above)

## 📱 PWA Features

Your app is already configured as a Progressive Web App (PWA):

- **Installable**: Users can "Add to Home Screen" on mobile
- **Offline Ready**: Works without internet after first load
- **App-like**: Full-screen experience on mobile devices

## 🔄 Updating Your App

To update your app:

1. **Edit files locally** (modify `index.html`, etc.)
2. **Upload new versions** to GitHub
3. **Changes go live automatically** (may take 1-2 minutes)

## 🌐 Custom Domain (Optional)

To use a custom domain (like `cfiacs.com`):

1. **Buy a domain** from any registrar
2. **Add CNAME file** to your repository:
   - Create file named `CNAME` (no extension)
   - Add your domain: `yourdomain.com`
3. **Configure DNS** at your domain registrar:
   - Add CNAME record pointing to `YOUR_USERNAME.github.io`

## 📊 Analytics (Optional)

To track usage:

1. **Google Analytics**: Add tracking code to `index.html`
2. **GitHub Insights**: View traffic in repository settings

## 🛠️ Troubleshooting

### Site Not Loading
- Wait 2-3 minutes after enabling Pages
- Check repository is public
- Verify files are in root directory

### PWA Not Working
- Ensure `manifest.json` is accessible
- Check service worker registration in browser console
- Verify HTTPS (GitHub Pages provides this automatically)

### Mobile Issues
- Test on actual devices
- Check viewport meta tag
- Verify touch interactions work

## 🎉 Success!

Once deployed, your CFI ACS Reference Tool will be:
- ✅ **Live on the web** for anyone to use
- ✅ **Mobile-friendly** and installable
- ✅ **Searchable** on Google
- ✅ **Shareable** with other CFI candidates
- ✅ **Always up-to-date** with your latest changes

## 📞 Support

If you run into issues:
1. Check GitHub Pages documentation
2. Verify all files are uploaded correctly
3. Test locally first (open `index.html` in browser)

**Happy flying!** ✈️
