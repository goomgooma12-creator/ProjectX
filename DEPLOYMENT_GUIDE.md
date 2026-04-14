# 🚀 Deploy to Vercel via GitHub — Step by Step Guide
## Mike Ronald Lakra | Bajaj Life AI Chatbot

---

## 📁 Your Project Structure

```
bajaj-life-chatbot/           ← Your GitHub repository name
├── api/
│   └── chat.js               ← Gemini AI serverless function (AUTO-DEPLOYED by Vercel)
├── public/
│   └── index.html            ← Your complete website with AI chatbot
├── vercel.json               ← Vercel configuration
├── package.json              ← Project config
└── DEPLOYMENT_GUIDE.md       ← This file
```

---

## STEP 1 — Get Your FREE Gemini API Key

1. Go to: **https://aistudio.google.com/app/apikey**
2. Sign in with your Google account
3. Click **"Create API Key"**
4. Copy the key — it looks like: `AIzaSyXXXXXXXXXXXXXXXXXXX`
5. Save it somewhere safe — you'll need it in Step 4

**FREE TIER:** 15 requests/minute, 1 million tokens/day = handles hundreds of users daily!

---

## STEP 2 — Create GitHub Repository

### Option A: Using GitHub Website (Easiest)
1. Go to **https://github.com** — Sign in or create free account
2. Click **"+"** → **"New repository"**
3. Repository name: `bajaj-life-chatbot` (or any name)
4. Set to **Public** (required for free Vercel)
5. Click **"Create repository"**

### Option B: Using GitHub Desktop App
1. Download: **https://desktop.github.com**
2. Sign in → File → New Repository
3. Name it `bajaj-life-chatbot`
4. Click "Create Repository"

---

## STEP 3 — Upload Your Files to GitHub

### Method A: Drag & Drop on GitHub Website
1. Open your new repository on GitHub
2. Click **"uploading an existing file"** link
3. **Drag all 5 files/folders** from your computer:
   - `api/` folder (contains `chat.js`)
   - `public/` folder (contains `index.html`)
   - `vercel.json`
   - `package.json`
4. Write commit message: `Initial deployment`
5. Click **"Commit changes"**

⚠️ **IMPORTANT:** Keep the folder structure exactly as shown!
- `api/chat.js` must be in an `api` folder
- `public/index.html` must be in a `public` folder

### Method B: Using GitHub Desktop
1. Open GitHub Desktop → Your repository
2. Copy all files into the repository folder on your computer
3. GitHub Desktop will show all new files
4. Write summary: "Initial commit"
5. Click **"Commit to main"**
6. Click **"Push origin"**

---

## STEP 4 — Deploy on Vercel

1. Go to **https://vercel.com** — Sign up FREE with your GitHub account
2. Click **"Add New Project"**
3. Click **"Import"** next to your `bajaj-life-chatbot` repository
4. Vercel auto-detects settings — **DON'T change anything**
5. Scroll down to **"Environment Variables"**
6. Click **"Add"** and enter:
   - **Name:** `GEMINI_API_KEY`
   - **Value:** `AIzaSyXXXXXXXXXX` (your key from Step 1)
7. Click **"Deploy"** ✅

**Wait 1-2 minutes** for deployment to complete.

---

## STEP 5 — Your Live Website! 🎉

After deployment, Vercel gives you a URL like:
```
https://bajaj-life-chatbot.vercel.app
```

**Your chatbot is now live!** The `/api/chat` endpoint is automatically created.

### Test it:
1. Open your Vercel URL in browser
2. Click the **AI Assistant** button (floating avatar)
3. Type: "AWG Second Income kya hai?"
4. You should get a detailed Gemini AI response! ✅

---

## STEP 6 — Add Custom Domain (Optional)

### To use your own domain (e.g., mikeronald.com):
1. In Vercel Dashboard → Your Project → **"Settings"** → **"Domains"**
2. Click **"Add"** → Enter your domain: `mikeronald.com`
3. Vercel shows DNS records to add
4. Go to your domain registrar (GoDaddy/Hostinger etc.)
5. Add the DNS records Vercel shows you
6. Wait 24-48 hours for DNS propagation
7. Done! Your chatbot is now on your custom domain ✅

---

## 🔄 How to Update Your Website

Whenever you want to update:
1. Edit files on your computer
2. Upload to GitHub (drag & drop or GitHub Desktop)
3. **Vercel automatically redeploys within 60 seconds!** 🚀

---

## ❓ Troubleshooting

### "Chat not working" / "API Error"
- Check Vercel Dashboard → Your Project → **"Functions"** tab
- Click on `api/chat` → Check logs for errors
- Make sure `GEMINI_API_KEY` is set in Environment Variables

### "404 on /api/chat"
- Make sure file is at exactly `api/chat.js` (not `API/chat.js`)
- Check `vercel.json` is in root folder

### "Gemini API quota exceeded"
- Free tier: 15 requests/minute
- Go to Google AI Studio → Increase limits
- Or upgrade to paid Gemini API (very cheap)

### "Website not showing"
- Make sure `public/index.html` exists
- Check `vercel.json` routing configuration

---

## 📊 What Gets Deployed

| File | What it does |
|------|-------------|
| `api/chat.js` | Gemini AI brain — handles all chat requests |
| `public/index.html` | Your complete website with chatbot UI |
| `vercel.json` | Routes `/api/chat` to function, everything else to `public/` |
| `package.json` | Tells Vercel it's a Node.js project |

---

## 🌐 Final URLs

After deployment:
- **Website:** `https://your-project.vercel.app`
- **AI API:** `https://your-project.vercel.app/api/chat`
- **Health:** `https://your-project.vercel.app/api/chat` (POST only)

The `index.html` already has `/api/chat` as the API URL — Vercel handles routing automatically. **No changes needed!**

---

## 💰 Cost

| Service | Cost |
|---------|------|
| Vercel Hosting | **FREE** (Hobby plan) |
| Gemini API | **FREE** (1M tokens/day) |
| GitHub | **FREE** |
| Custom Domain | ₹500-1000/year (optional) |

**Total: ₹0/month** for running your AI chatbot! 🎉

---

## 📞 Need Help?

**Mike Ronald Lakra**
- WhatsApp: +91 93821 81126
- IC Code: ABLIC1003446377
- Unit: JK Millenium, Kolkata
