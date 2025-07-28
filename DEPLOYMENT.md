# 🚀 HealTale Deployment Guide

## Quick Start Commands

### 1. Start Development Server
```bash
npm run dev
# Opens at http://localhost:8000
```

### 2. Build for Production
```bash
npm run build
```

### 3. Deploy to Vercel (Recommended)
```bash
npm install -g vercel
vercel --prod
```

### 4. Deploy to Netlify
```bash
npm install -g netlify-cli
netlify deploy --prod --dir=out
```

## 📦 GitHub Repository Setup

### Step 1: Create Repository
```bash
# Initialize git
git init
git add .
git commit -m "Initial HealTale website with complete features"

# Add remote (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/healtale-website.git
git branch -M main
git push -u origin main
```

### Step 2: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Source: **Deploy from a branch**
4. Branch: **main**
5. Folder: **/ (root)**

## 🌐 Live Deployment Options

### Option 1: Vercel (Recommended)
1. Go to [vercel.com](https://vercel.com)
2. Import from GitHub
3. Select your repository
4. Deploy automatically

### Option 2: Netlify
1. Go to [netlify.com](https://netlify.com)
2. Drag and drop your project folder
3. Or connect to GitHub for auto-deploy

### Option 3: GitHub Pages
1. Push to GitHub
2. Enable Pages in repository settings
3. Site will be at: `https://YOUR_USERNAME.github.io/healtale-website`

## 📁 Required Files Checklist
✅ `src/app/layout.tsx` - Root layout with fonts
✅ `src/app/page.tsx` - Main page
✅ All components created
✅ `package.json` - Dependencies configured
✅ `next.config.ts` - Next.js config
✅ `tailwind.config.js` - Styling configured

## 🎯 Environment Variables
No environment variables required - the site works out of the box!

## 📧 Email Configuration
The contact email `taleheal@gmail.com` is hardcoded and ready to use.

## 🖼️ Adding Images Later
1. Create `public/images/` folder
2. Add images following naming conventions in IMAGE_GUIDE.md
3. Update component image paths
4. Redeploy

## 🚀 One-Command Deployment
```bash
# Full deployment pipeline
npm run build && vercel --prod
```

Your HealTale website is ready to publish! 🎉
