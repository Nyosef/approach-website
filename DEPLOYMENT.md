# GitHub Pages Deployment Guide

## Step 1: Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon (top right) → "New repository"
3. Repository name: `approach-website` (or your preferred name)
4. Set to **Public** (required for free GitHub Pages)
5. **Don't** check "Add a README file" (we already have one)
6. Click "Create repository"

## Step 2: Push Your Code

After creating the repository, GitHub will show you commands. Run these in your terminal:

```bash
git remote add origin https://github.com/YOUR_USERNAME/approach-website.git
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch
6. Leave folder as "/ (root)"
7. Click "Save"

## Step 4: Access Your Live Site

Your website will be available at:
```
https://YOUR_USERNAME.github.io/approach-website
```

**Note:** It may take 5-10 minutes for the site to go live after enabling Pages.

## Step 5: Custom Domain (Optional)

If you want to use a custom domain:
1. In Pages settings, add your domain in "Custom domain"
2. Update your domain's DNS settings to point to GitHub Pages
3. Enable "Enforce HTTPS" after DNS propagates

## Troubleshooting

- **Site not loading?** Wait 10 minutes and try again
- **404 error?** Make sure `index.html` is in the root directory
- **Changes not showing?** It can take a few minutes for updates to deploy

## Making Updates

To update your site:
1. Edit files locally
2. Commit changes: `git add . && git commit -m "Update message"`
3. Push: `git push origin main`
4. Changes will automatically deploy to your live site

Your professional Approach App landing page is ready to go live! 🚀