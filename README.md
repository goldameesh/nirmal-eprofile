# Nirmal Computer & Photocopy Center - E-Profile

A professional, mobile-first digital e-profile for Nirmal Computer & Photocopy Center in Kathmandu, Nepal.

## ✨ Features

- **Bilingual Support**: Nepali & English with toggle
- **View Counter**: Tracks profile views using localStorage
- **Offline Mode**: Basic information accessible without internet
- **Functional QR Code**: Generate scannable QR codes pointing to the profile
- **vCard Download**: Contact information in .vcf format for easy import
- **Responsive Design**: Works seamlessly on all devices
- **PWA Ready**: Can be installed as an app on mobile devices
- **Royal Blue + Yellow Gradient**: Premium color scheme (#1E40AF + #FFD700)
- **Fast Loading**: Optimized for slow internet connections
- **No Backend Required**: Static HTML - pure front-end

## 📁 File Structure

```
nirmal-eprofile/
├── index.html           # Main profile page
├── manifest.json        # PWA manifest
├── service-worker.js    # Offline support
├── CNAME               # Custom domain configuration
├── .gitignore          # Git ignore rules
└── README.md           # This file
```

## 🚀 Deployment Instructions

### Step 1: Create GitHub Repository

1. Go to https://github.com/goldameesh
2. Click **"New"** to create a new repository
3. **Repository name**: `nirmal-eprofile`
4. Select **"Public"**
5. Click **"Create repository"**

### Step 2: Initialize Local Git & Push Files

Open terminal/command prompt and run:

```bash
# Navigate to the project directory (where you have the files)
cd nirmal-eprofile

# Initialize git
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial commit: Nirmal Computer e-profile"

# Add remote origin (replace with your repo URL)
git remote add origin https://github.com/goldameesh/nirmal-eprofile.git

# Push to main branch
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository: https://github.com/goldameesh/nirmal-eprofile
2. Click **"Settings"** (top right)
3. Click **"Pages"** (left sidebar)
4. Under **"Source"**, select **"Deploy from a branch"**
5. Select **"main"** branch
6. Select **"/ (root)"** folder
7. Click **"Save"**

**Wait 1-2 minutes** - Your site is now live at: `https://goldameesh.github.io/nirmal-eprofile/`

### Step 4: Configure Custom Domain (GoDaddy)

#### 4.1 Get GitHub Pages IP Addresses

GitHub Pages uses these IP addresses:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

#### 4.2 Configure DNS in GoDaddy

1. **Log in to GoDaddy**: https://www.godaddy.com/
2. Go to **"My Products"** → **"Manage"** (for basfoundry.co)
3. Click **"Manage DNS"**
4. Under **"Records"**, add/update:

**For A Records (root domain):**
- **Name**: `@` or leave blank
- **Type**: `A`
- **Points to**: `185.199.108.153`
- Click **"Add Another"** and repeat for:
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`

**For CNAME Record (subdomain):**
- **Name**: `nirmal-computer`
- **Type**: `CNAME`
- **Points to**: `goldameesh.github.io`
- **TTL**: 3600 (1 hour)

**Click "Save All"**

#### 4.3 Wait for DNS Propagation

DNS changes take 15 minutes to 24 hours (usually 1-2 hours). You can check status at:
- https://dnschecker.org/

#### 4.4 Configure in GitHub Repository

1. Go back to repository **Settings** → **Pages**
2. Under **"Custom domain"**, enter: `nirmal-computer.basfoundry.co`
3. Click **"Save"**
4. ✅ GitHub will automatically verify and enable HTTPS

### Step 5: Verify Deployment

Once DNS propagates (check after 15-30 minutes):

- **Visit**: https://nirmal-computer.basfoundry.co
- **Scan QR code**: Opens the profile
- **View counter**: Increments on each visit
- **Offline mode**: Test by disabling internet

## 🔧 Features Explained

### View Counter
- **How it works**: Uses browser localStorage (local to each device)
- **What it tracks**: Number of times the page is visited from that device
- **Privacy**: No data sent to servers, completely local
- **Visible**: Top right corner "👁️ Views: X"

### QR Code
- **Function**: Click "📱 QR" button to generate
- **Target**: Points to `nirmal-computer.basfoundry.co`
- **Scanning**: Works with any standard QR code scanner
- **Color**: Royal Blue (#1E40AF) for better scannability

### Offline Mode
- **Automatically enables**: When internet is unavailable
- **Shows**: Contact info, address, 12 services list
- **Banner**: Orange "📡 Offline Mode" appears at top
- **Service Worker**: Caches essential data on first visit

### vCard Download
- **Button**: "💾" in action bar
- **Format**: .vcf file (universal contact format)
- **Import**: Works with Contacts, WhatsApp, Gmail, Outlook, etc.
- **Includes**: All phone numbers, address, services list

## 📱 Mobile Installation

Users can install this as an app on their phone:

1. **iOS**: 
   - Open in Safari
   - Tap Share → Add to Home Screen
   
2. **Android**:
   - Open in Chrome
   - Tap Menu (3 dots) → "Install app" or "Add to Home Screen"

## 🔒 Security

- ✅ **HTTPS**: Automatically enabled by GitHub Pages
- ✅ **No server-side code**: Pure static HTML
- ✅ **No data collection**: All tracking is local
- ✅ **No cookies**: Uses localStorage only
- ✅ **No third-party integrations**: Only QR library from CDN

## 📊 Analytics

View counter data is stored in browser localStorage:
- **Key**: `nirmal_views`
- **Access**: Open browser DevTools → Application → LocalStorage
- **Clear**: Browser "Clear browsing data"

## 🎨 Color Scheme

- **Primary Blue**: `#1E40AF` (Royal Blue)
- **Primary Yellow**: `#FFD700` (Smiley Yellow)
- **Gradient**: Diagonal from top-left to bottom-right
- **Text**: Contrasting colors for readability
- **Hover Effects**: Subtle shadows and color transitions

## 🌐 Supported Browsers

- ✅ Chrome/Edge (Latest)
- ✅ Firefox (Latest)
- ✅ Safari (iOS 12+)
- ✅ Samsung Internet
- ✅ All modern mobile browsers

## 🚨 Troubleshooting

### QR Code not working
- Ensure your domain is properly configured
- Check DNS propagation: https://dnschecker.org/
- Clear browser cache and reload

### Custom domain not working
- **DNS Propagation**: Can take up to 24 hours
- **Check CNAME**: Verify `nirmal-computer` points to `goldameesh.github.io`
- **Check A Records**: All 4 GitHub IP addresses should be present

### View counter not working
- Check if localStorage is enabled in browser
- Private/Incognito mode might not persist data
- Clear browser data and refresh

### Offline mode not available
- Service Worker requires HTTPS
- Check browser console for errors
- Refresh page after enabling offline mode

## 📞 Contact Support

**Nirmal Computer & Photocopy Center**
- 📱 +977 9841631075 (Nirmal Maharjan)
- 📱 +977 9841331396 (Nilkeshor Maharjan)
- 📍 Kalanki, Kathmandu, Nepal

## 📄 License

This project is created for Nirmal Computer & Photocopy Center. All rights reserved.

## ✅ Deployment Checklist

- [ ] GitHub repository created (`nirmal-eprofile`)
- [ ] All files pushed to GitHub
- [ ] GitHub Pages enabled
- [ ] Custom domain added to GitHub Settings
- [ ] DNS records configured in GoDaddy:
  - [ ] A records added (all 4 IPs)
  - [ ] CNAME record for `nirmal-computer` pointing to `goldameesh.github.io`
- [ ] DNS propagation verified (test at https://dnschecker.org/)
- [ ] HTTPS enabled (automatic)
- [ ] Profile accessible at `https://nirmal-computer.basfoundry.co`
- [ ] QR code tested and working
- [ ] View counter displaying correctly
- [ ] vCard download functioning
- [ ] Offline mode tested
- [ ] Mobile installation working

---

**Last Updated**: April 2026  
**Version**: 1.0 - Final Production Release
