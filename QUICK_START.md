# 🚀 Quick Start Guide - Nirmal E-Profile Deployment

**Time Required**: 15 minutes (+ DNS propagation 15 min - 24 hours)

---

## 📥 What You Have

6 files ready to upload:
1. `index.html` - Main profile page
2. `manifest.json` - PWA configuration
3. `service-worker.js` - Offline support
4. `CNAME` - Custom domain pointer
5. `.gitignore` - Git configuration
6. `README.md` - Full documentation

---

## ⚡ Express Deploy (5 Steps)

### Step 1️⃣: Create GitHub Repo (2 min)

```
Go to: https://github.com/goldameesh
Click: "New" button
Name: nirmal-eprofile
Select: Public
Click: "Create repository"
```

### Step 2️⃣: Upload Files (2 min)

**Option A - Using GitHub Web Interface (Easiest):**

```
1. Go to your new repo: https://github.com/goldameesh/nirmal-eprofile
2. Click "Upload files" (above file list)
3. Drag and drop all 6 files
4. Scroll down, click "Commit changes"
5. Done! ✅
```

**Option B - Using Git (Terminal):**

```bash
cd path/to/nirmal-eprofile
git init
git add .
git commit -m "Initial: Nirmal e-profile"
git remote add origin https://github.com/goldameesh/nirmal-eprofile.git
git branch -M main
git push -u origin main
```

### Step 3️⃣: Enable GitHub Pages (1 min)

```
1. Go to repo → Settings → Pages
2. Source: "Deploy from a branch"
3. Select: "main" + "/ (root)"
4. Click: "Save"
5. Wait 1-2 minutes ⏳
```

✅ **Your site is live at:**  
**https://goldameesh.github.io/nirmal-eprofile/**

### Step 4️⃣: Configure Custom Domain - GoDaddy (3 min)

**Go to GoDaddy → My Products → basfoundry.co → Manage DNS**

**Add ONE record:**
- **Name**: `nirmal-computer`
- **Type**: `CNAME`
- **Points to**: `goldameesh.github.io`
- **TTL**: `3600`
- Click: **"Save"**

### Step 5️⃣: Configure in GitHub (1 min)

```
1. Repo → Settings → Pages
2. Custom domain: nirmal-computer.basfoundry.co
3. Click: "Save"
4. ✅ HTTPS enabled automatically
```

---

## ⏱️ Wait for DNS (15 min - 24 hours)

Check status: https://dnschecker.org/
- Enter: `nirmal-computer.basfoundry.co`
- Wait for green checkmarks ✅

**Your profile will be live at:**  
**https://nirmal-computer.basfoundry.co**

---

## 🎯 Test Your Profile

Once live, verify:

- [ ] Visit: https://nirmal-computer.basfoundry.co
- [ ] Click "📱 QR" - generates QR code
- [ ] Click "💬" - opens WhatsApp
- [ ] Click "📞" - initiates call
- [ ] Click "💾" - downloads vCard
- [ ] Refresh page - view counter increments
- [ ] Toggle between नेपाली & English
- [ ] Test offline mode (disable internet)

---

## 🔄 After Deployment

### Share Your Profile

**WhatsApp:**
```
Check out: https://nirmal-computer.basfoundry.co
All services, contact, & QR code! 🎯
```

**Email:**
```
Subject: Nirmal Computer E-Profile

Click here to view all our services:
https://nirmal-computer.basfoundry.co
```

**Social Media:**
```
📱 Nirmal Computer & Photocopy Center
🔗 https://nirmal-computer.basfoundry.co
📍 Kalanki, Kathmandu
📞 +977 9841631075
```

---

## 📊 Monitor Your Profile

### View Counter
- Visible at top: "👁️ Views: X"
- Tracks local device visits only (privacy-safe)

### Analytics
- Open DevTools (F12) → Application → LocalStorage
- Look for key: `nirmal_views`

---

## 🔧 Make Changes

Need to update profile text or services?

### Method 1: GitHub Web (Easy)
```
1. Go to repo → index.html
2. Click edit (pencil icon)
3. Make changes
4. Click "Commit changes"
5. Live in 30 seconds! 🚀
```

### Method 2: Local Git (Full Control)
```bash
# Edit files locally
# Then:
git add .
git commit -m "Updated services"
git push
```

---

## ❓ Common Questions

**Q: How long until custom domain works?**  
A: 15 minutes - 24 hours. Usually 1-2 hours.

**Q: Will profile work offline?**  
A: Yes! Shows contact, address, 12 services without internet.

**Q: Can I see how many views I got?**  
A: Yes! Each device tracks its own views in localStorage.

**Q: How do I change the colors?**  
A: Edit index.html and change hex codes:
- Blue: `#1E40AF` 
- Yellow: `#FFD700`

**Q: Does it require a server/database?**  
A: No! Pure static HTML. No backend needed.

**Q: Is the QR code real?**  
A: Yes! It points to your actual profile URL.

---

## 🆘 Troubleshooting

**Profile shows blank page:**
- Wait 2-5 minutes for GitHub to process
- Clear browser cache (Ctrl+Shift+Delete)
- Try Incognito/Private mode

**Custom domain not working:**
- Check DNS at: https://dnschecker.org/
- If pending: wait up to 24 hours
- If red X: verify GoDaddy DNS records are correct

**CNAME file didn't upload:**
- GitHub should auto-create it when you add custom domain
- Or manually add it to repo with content: `nirmal-computer.basfoundry.co`

**QR code doesn't scan:**
- Ensure domain is live first
- Check phone camera app has camera permission
- Try different QR scanner app

---

## 📚 Full Documentation

For detailed info, see:
- `README.md` - Complete feature guide
- `GODADDY_DNS_SETUP.md` - DNS configuration details
- Repository README in GitHub

---

## ✅ Deployment Checklist

- [ ] All 6 files uploaded to GitHub
- [ ] GitHub Pages enabled
- [ ] Repository is public
- [ ] Custom domain added to GitHub Settings
- [ ] DNS record (CNAME) added in GoDaddy
- [ ] DNS propagation verified (dnschecker.org)
- [ ] Profile accessible at custom domain
- [ ] HTTPS enabled (lock icon visible)
- [ ] QR code working
- [ ] View counter incrementing
- [ ] All buttons functional (call, WhatsApp, etc)
- [ ] Offline mode tested

---

## 🎉 Congratulations!

Your Nirmal Computer E-Profile is now live and shareable!

**Profile URL:** https://nirmal-computer.basfoundry.co  
**GitHub Repo:** https://github.com/goldameesh/nirmal-eprofile

**Start sharing:**
- QR code
- Profile link
- vCard file

---

**Need help?** Check the full README.md or contact GitHub/GoDaddy support.

**Last Updated**: April 2026
