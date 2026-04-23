# A+ Agent Directory - Deployment Guide

## 🚀 Quick Deploy to Vercel

### Method 1: Vercel Web UI (Easiest - 2 Minutes)

1. **Go to Vercel**
   - Visit: https://vercel.com
   - Click "Sign Up" (use GitHub, GitLab, or email)

2. **Create New Project**
   - Click "Add New..." → "Project"
   - Click "Browse" or drag-and-drop this folder

3. **Configure**
   - Project Name: `aplusagent` (or whatever you want)
   - Framework Preset: Leave as "Other"
   - Root Directory: `./`
   - Click "Deploy"

4. **Wait ~30 seconds**
   - Your site will be live at: `https://aplusagent-[random].vercel.app`

5. **Add Custom Domain**
   - Go to Project Settings → Domains
   - Add: `aplusagent.ai`
   - Follow DNS instructions (see below)

---

### Method 2: Vercel CLI (For Developers)

```bash
# Install Vercel CLI
npm install -g vercel

# Navigate to your project folder
cd /path/to/project

# Deploy
vercel

# Follow prompts:
# - Link to existing project? N
# - Project name? aplusagent
# - Directory? ./
# - Override settings? N

# Production deploy
vercel --prod
```

---

## 🌐 Custom Domain Setup (aplusagent.ai)

### Step 1: Add Domain in Vercel
1. Go to your project → Settings → Domains
2. Enter: `aplusagent.ai`
3. Click "Add"

### Step 2: Update DNS (At Unstoppable Domains or wherever you bought it)

Vercel will show you one of these options:

**Option A: A Record (Recommended)**
```
Type: A
Name: @
Value: 76.76.21.21
```

**Option B: CNAME Record**
```
Type: CNAME
Name: @
Value: cname.vercel-dns.com
```

**For www subdomain:**
```
Type: CNAME
Name: www
Value: cname.vercel-dns.com
```

### Step 3: Wait for DNS Propagation
- Usually takes 5-60 minutes
- Check status: https://dnschecker.org

---

## ✅ After Deployment

Your site will be live at:
- **Vercel URL:** https://aplusagent-[random].vercel.app
- **Custom Domain:** https://aplusagent.ai (after DNS setup)

### Features You Get:
✅ Auto HTTPS/SSL certificate
✅ Global CDN (fast worldwide)
✅ 99.99% uptime
✅ Automatic deployments
✅ Free bandwidth
✅ Analytics (optional)

---

## 🔄 Updating Your Site

### Method 1: Vercel Web UI
1. Go to your project in Vercel
2. Click "Deployments"
3. Upload new `index.html`
4. Site updates automatically

### Method 2: Git Integration (Recommended)
1. Connect GitHub repo to Vercel
2. Push changes to GitHub
3. Vercel auto-deploys on every push

---

## 📊 Optional: Add Analytics

Vercel provides free analytics:
1. Go to Project → Analytics
2. Enable "Web Analytics"
3. Track visitors, page views, performance

---

## 🛠️ Troubleshooting

**Problem: Domain not working after 1 hour**
- Check DNS propagation: https://dnschecker.org
- Verify DNS records match Vercel's instructions exactly
- Try clearing browser cache

**Problem: SSL certificate error**
- Wait 24 hours after DNS setup
- Vercel auto-provisions SSL certificates
- Check domain is properly verified in Vercel

**Problem: Site not updating**
- Clear browser cache (Ctrl+Shift+R)
- Check deployment status in Vercel dashboard
- Wait 30-60 seconds for CDN to update globally

---

## 💡 Pro Tips

1. **Enable automatic deployments** by connecting GitHub
2. **Use environment variables** for API keys (if you add backend later)
3. **Set up preview deployments** for testing changes
4. **Add redirects** in vercel.json for SEO

---

## 📧 Support

- Vercel Docs: https://vercel.com/docs
- Vercel Support: https://vercel.com/support
- Community: https://github.com/vercel/vercel/discussions

---

## 🎉 You're Done!

Your AI Agent Directory is now live and globally distributed. No servers to maintain, no downtime worries.

Next steps:
1. Add more agents to your directory
2. Set up Google Analytics (optional)
3. Submit to Google Search Console for SEO
4. Start promoting on Twitter, Reddit, ProductHunt
