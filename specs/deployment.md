# Deployment Guide

## GitHub Pages Deployment

This project is designed for GitHub Pages deployment with a custom domain.

### Feasibility Assessment

**Status: Excellent** - This static site project is perfectly suited for GitHub Pages deployment.

### Prerequisites

- GitHub account
- Domain ownership (`naic25.cassandev.live`)
- DNS management access

### Deployment Steps

#### 1. Create GitHub Repository

```bash
# Create a new repository on GitHub first, then:
git add .
git commit -m "Initial commit: Static site with PDF and video content"
git remote add origin https://github.com/yourusername/your-repo-name.git
git push -u origin main
```

#### 2. Enable GitHub Pages

1. Navigate to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Source", select **Deploy from a branch**
4. Choose **main** branch and **/ (root)** folder
5. Click **Save**

#### 3. Configure Custom Domain

The CNAME file is already configured with `naic25.cassandev.live`.

In GitHub Pages settings:
1. Go to **Settings** → **Pages**
2. Under "Custom domain", enter: `naic25.cassandev.live`
3. Enable **Enforce HTTPS**

#### 4. DNS Configuration

Configure your domain's DNS records to point to GitHub Pages:

**For apex domain:**
- **A records**: 
  - `185.199.108.153`
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`

**For subdomain:**
- **CNAME record**: `yourusername.github.io`

### Deployment Timeline

- Initial deployment: 1-2 minutes after enabling Pages
- Custom domain propagation: 10-15 minutes
- DNS propagation: Up to 24 hours (typically faster)

### Final Result

Site will be accessible at: `https://naic25.cassandev.live`

### File Structure

The deployment includes:
- `index.html` - Main page with PDF and video display
- `assets/` - Static assets (PDF, video, logo)
- `CNAME` - Custom domain configuration
- `.gitignore` - Git ignore rules