# 🚀 GitHub Pages Setup Guide

This guide will walk you through publishing SongDrop on GitHub Pages, step by step.

---

## Prerequisites

- A GitHub account (create one at [github.com](https://github.com/signup) if you don't have one)
- The SongDrop files from this project

---

## 📝 Step 1: Create a New Repository

1. **Go to GitHub** and sign in
2. **Click the "+" icon** in the top-right corner
3. **Select "New repository"**

---

## ⚙️ Step 2: Configure Your Repository

Fill in the following details:

### **Repository Name**
```
songdrop
```
- This will be part of your URL: `https://yourusername.github.io/songdrop/`
- Use lowercase, no spaces (use hyphens if needed)

### **Description** (optional but recommended)
```
🎵 Share music, personally. A beautiful retro-styled music sharing app.
```

### **Visibility**
- ✅ **Public** — Choose this so GitHub Pages works (free tier)
- ❌ Private — Requires GitHub Pro for Pages hosting

### **Initialize Repository**
- ✅ Check "Add a README file" — **UNCHECK THIS** (we're providing our own)
- ❌ Add .gitignore — **Leave as "None"**
- ✅ Choose a license — **Select "MIT License"**

### **Click "Create repository"**

---

## 📤 Step 3: Upload Your Files

You now have two options:

### **Option A: Upload via GitHub Website** (Easiest)

1. On your new repository page, click **"uploading an existing file"** (in the Quick Setup section)
2. **Drag and drop** or **choose** these files:
   - `index.html`
   - `README.md`
   - `SETUP.md` (this file)
   - Any other files you have

3. **Scroll down** to the "Commit changes" section
4. **Commit message:** 
   ```
   Initial commit: Add SongDrop application
   ```
5. **Click "Commit changes"**

### **Option B: Upload via Git Command Line** (For developers)

```bash
# Navigate to where you saved the SongDrop files
cd /path/to/songdrop

# Initialize git repository
git init

# Add all files
git add .

# Make your first commit
git commit -m "Initial commit: Add SongDrop application"

# Add GitHub as remote (replace 'yourusername')
git remote add origin https://github.com/yourusername/songdrop.git

# Push to GitHub
git branch -M main
git push -u origin main
```

---

## 🌐 Step 4: Enable GitHub Pages

1. **Go to your repository** on GitHub
2. **Click "Settings"** (top menu, far right)
3. **Scroll down** and click **"Pages"** in the left sidebar
4. Under **"Source"**, select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
5. **Click "Save"**

---

## ⏳ Step 5: Wait for Deployment

- GitHub will take **30-60 seconds** to build and deploy your site
- A **blue banner** will appear saying "Your site is ready to be published"
- Refresh the page after a minute
- The banner will turn **green** with your live URL

---

## 🎉 Step 6: Visit Your Site

Your app is now live at:
```
https://yourusername.github.io/songdrop/
```

**Replace `yourusername` with your actual GitHub username!**

---

## 📝 Step 7: Update README Links (Important!)

Your README.md has placeholder URLs. Update them:

1. **Go to your repository**
2. **Click on `README.md`**
3. **Click the pencil icon** (Edit this file)
4. **Find and replace** all instances of:
   ```
   yourusername
   ```
   with your actual GitHub username
   
5. **Scroll down** and click **"Commit changes"**

---

## 🎨 Optional: Add a Custom Domain

Want to use your own domain instead of `username.github.io`?

1. **Buy a domain** (from Namecheap, Google Domains, etc.)
2. **In GitHub:** Settings → Pages → Custom domain
3. **Enter your domain** (e.g., `songdrop.app`)
4. **In your domain registrar**, add these DNS records:

   **For apex domain (songdrop.app):**
   ```
   A     @     185.199.108.153
   A     @     185.199.109.153
   A     @     185.199.110.153
   A     @     185.199.111.153
   ```

   **For subdomain (www.songdrop.app):**
   ```
   CNAME     www     yourusername.github.io
   ```

5. **Wait 24-48 hours** for DNS propagation
6. **Enable "Enforce HTTPS"** in GitHub Pages settings

---

## 🔧 Updating Your Site

### Via GitHub Website:
1. Click the file you want to edit
2. Click the pencil icon
3. Make changes
4. Scroll down and click "Commit changes"
5. Wait ~1 minute for changes to go live

### Via Git:
```bash
# Make your changes to index.html or other files

# Stage changes
git add .

# Commit with a descriptive message
git commit -m "Add new iPod color option"

# Push to GitHub
git push
```

Changes go live in about 1 minute.

---

## 📊 Optional: Add Analytics

Want to track visitors? Add Google Analytics or Plausible:

1. **Get your tracking code**
2. **Edit `index.html`**
3. **Add the tracking script** before `</head>`
4. **Commit and push**

---

## 🐛 Troubleshooting

### Site not loading?
- Wait 2-3 minutes after enabling Pages
- Check Settings → Pages for error messages
- Make sure your repository is Public
- Verify `index.html` is in the root directory

### 404 Error?
- Ensure the file is named `index.html` (lowercase)
- Check the branch is set to `main` in Pages settings
- Visit the full URL: `https://yourusername.github.io/songdrop/`

### Links not working?
- Update the `yourusername` placeholders in README.md
- Update the meta tags in `index.html` with your actual URL

### Changes not appearing?
- Clear your browser cache (Cmd/Ctrl + Shift + R)
- Wait 1-2 minutes for GitHub to rebuild
- Check if commit went through in repository

---

## 🎓 Learning Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
- [Markdown Guide](https://www.markdownguide.org/)

---

## 🎉 You're Done!

Your SongDrop app is now live and ready to share with the world!

**Next steps:**
- Share your app with friends
- Add screenshots to the README
- Customize colors and themes
- Star the original repo if you found it helpful

**Questions?** Open an issue in the repository!

---

**Made with 🎵 and ✨**
