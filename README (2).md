# Velez Control Systems — Website

Product website for the VCS-SYS1 Intelligent High-Current Power Controller.

Hosted via GitHub Pages at [velezcontrol.com](https://velezcontrol.com) (or `yourusername.github.io/velezcontrol`).

## Setup

### 1. Create the repo

```bash
git init
git add .
git commit -m "Initial site launch"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/velezcontrol.git
git push -u origin main
```

### 2. Enable GitHub Pages

1. Go to **Settings → Pages** in the repo
2. Under **Source**, select **Deploy from a branch**
3. Select **main** branch, **/ (root)** folder
4. Click **Save**
5. Your site will be live at `https://YOUR_USERNAME.github.io/velezcontrol/` within a minute

### 3. Custom domain (optional)

1. Buy `velezcontrol.com` on [Namecheap](https://namecheap.com) (~$10/year)
2. In Namecheap DNS, add these records:
   - **A Record** → `185.199.108.153`
   - **A Record** → `185.199.109.153`
   - **A Record** → `185.199.110.153`
   - **A Record** → `185.199.111.153`
   - **CNAME** `www` → `YOUR_USERNAME.github.io`
3. In GitHub repo **Settings → Pages → Custom domain**, enter `velezcontrol.com`
4. Check **Enforce HTTPS**
5. Wait 10-30 minutes for DNS propagation

### 4. Adding Stripe payments (when ready)

1. Create a [Stripe](https://stripe.com) account
2. Go to **Products → Add Product** → set name "VCS-SYS1" and price $49
3. Click **Create Payment Link**
4. Copy the link URL
5. Replace the "Notify me" button `href` in `index.html` with your Stripe link

## File structure

```
index.html    — Main product page (single file, no dependencies)
CNAME         — Custom domain config (created by GitHub when you set domain)
README.md     — This file
```

## Updating the site

Edit `index.html`, commit, push. GitHub Pages deploys automatically within ~60 seconds.

## License

Website content © 2026 Velez Control Systems. All rights reserved.
