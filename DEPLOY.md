# 🚀 Netlify Deployment Guide

This guide will walk you through deploying the InAmigos Foundation webpage on **Netlify** — completely free, no credit card needed.

---

## ✅ Prerequisites

Before you start, make sure you have:

- [ ] A **GitHub account** — [github.com](https://github.com)
- [ ] A **Netlify account** — [netlify.com](https://netlify.com) (sign up free with GitHub)
- [ ] Your project files uploaded to a **GitHub repository**

---

## 📤 Step 1 — Upload Files to GitHub

If you haven't already pushed your code:

### Option A — Using GitHub Website (No Terminal Needed)

1. Go to [github.com](https://github.com) and log in
2. Click the **"+"** icon → **New repository**
3. Name it: `inamigos-awareness`
4. Set it to **Public**
5. Click **Create repository**
6. On the next page, click **"uploading an existing file"**
7. Drag and drop your `index.html` and `README.md`
8. Scroll down → click **Commit changes**

### Option B — Using Git Terminal

```bash
# Initialize git in your project folder
git init

# Add all files
git add .

# First commit
git commit -m "feat: Add InAmigos Foundation NGO awareness webpage"

# Connect to your GitHub repo (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/inamigos-awareness.git

# Push to GitHub
git branch -M main
git push -u origin main
```

---

## 🌐 Step 2 — Deploy on Netlify

### Method 1 — Netlify + GitHub (Recommended — Auto-deploys on every push!)

1. Go to **[app.netlify.com](https://app.netlify.com)**
2. Click **"Add new site"** → **"Import an existing project"**
3. Click **"Deploy with GitHub"**
4. Authorize Netlify to access your GitHub
5. Search for and select your repo: `inamigos-awareness`
6. Configure build settings:

   | Setting | Value |
   |---|---|
   | Branch to deploy | `main` |
   | Base directory | *(leave empty)* |
   | Build command | *(leave empty)* |
   | Publish directory | `.` or *(leave empty)* |

7. Click **"Deploy site"** 🎉

> Netlify will assign a random URL like `https://random-name-12345.netlify.app`

---

### Method 2 — Netlify Drag & Drop (Fastest — 30 seconds!)

1. Go to **[app.netlify.com/drop](https://app.netlify.com/drop)**
2. Simply **drag and drop your project folder** onto the page
3. Netlify auto-deploys it instantly
4. You get a live URL immediately!

> ⚠️ Note: Drag & Drop doesn't auto-update when you push changes. Use Method 1 for automatic updates.

---

## 🔗 Step 3 — Set a Custom Site Name

After deployment, your site has a random name. To customize it:

1. Go to **Site settings** → **General** → **Site details**
2. Click **"Change site name"**
3. Enter something like: `inamigos-foundation` or `inAmigos-ngo`
4. Your new URL: `https://inamigos-foundation.netlify.app`
5. Update the live demo link in your `README.md`!

---

## ⚙️ Step 4 — Verify Deployment

Once deployed, check:

- [ ] ✅ Site loads correctly at your Netlify URL
- [ ] ✅ All sections visible (Hero, About, Projects, etc.)
- [ ] ✅ Images load (Unsplash CDN images)
- [ ] ✅ Animations work on scroll
- [ ] ✅ Mobile view looks good (check in browser DevTools → toggle device toolbar)
- [ ] ✅ Contact form button works

---

## 🔄 Step 5 — Auto-Deploy on Changes (If using Method 1)

Every time you push a change to GitHub, Netlify automatically rebuilds and deploys:

```bash
# Make your changes in index.html, then:
git add .
git commit -m "fix: Update project description"
git push
# Netlify auto-detects the push and redeploys in ~30 seconds!
```

---

## 🛠️ Troubleshooting

| Problem | Solution |
|---|---|
| Site shows blank page | Make sure your file is named exactly `index.html` |
| Images not loading | You're offline — Unsplash images need internet connection |
| Old version showing | Go to Netlify dashboard → Deploys → Trigger deploy |
| Custom domain needed | Netlify → Site settings → Domain management → Add custom domain |
| Build failed | Check that there's no `netlify.toml` with wrong settings |

---

## 🌍 Optional — Custom Domain

If you have your own domain (e.g., `inamigosprathip.in`):

1. Go to **Site settings** → **Domain management**
2. Click **"Add custom domain"**
3. Enter your domain name
4. Follow DNS configuration instructions from Netlify
5. Netlify provides **free HTTPS/SSL** automatically!

---

## 📸 After Deployment — Submission Checklist

- [ ] 🔗 Copy your Netlify live URL
- [ ] 📸 Take screenshots of the deployed site
- [ ] 📁 Upload source code + screenshots to your drive folder
- [ ] 📱 Post on LinkedIn with your live site link
- [ ] 🏷️ Add hashtags: `#InAmigos` `#WebDevelopment` `#NGO` `#Netlify`
- [ ] 🔖 Tag InAmigos Foundation on LinkedIn

---

## 📞 Help

If you get stuck, feel free to:
- Check [Netlify Docs](https://docs.netlify.com)
- Ask in the InAmigos intern group

---

*Happy deploying! 🚀 — Built by Prathip T for InAmigos Foundation Web Dev Internship Task 1*
