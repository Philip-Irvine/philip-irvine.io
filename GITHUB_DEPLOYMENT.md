# GitHub Pages Deployment Guide

This website is optimized for GitHub Pages deployment. Follow these steps to deploy your personal website:

## Prerequisites

- A GitHub account
- Git installed on your local machine

## Step-by-Step Deployment

### 1. Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" button in the top right corner
3. Select "New repository"
4. Name your repository: `personal-website`
5. Make sure it's **Public** (required for free GitHub Pages)
6. **Do NOT** initialize with README (we already have one)
7. Click "Create repository"

### 2. Initialize Git and Push

Open your terminal in the project directory and run:

```bash
# Initialize Git repository
git init

# Add all files
git add .

# Make initial commit
git commit -m "Initial commit - Personal website"

# Add remote repository (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/personal-website.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" section in the left sidebar
4. Under "Build and deployment", select:
   - **Source**: Deploy from a branch
   - **Branch**: main
   - **Folder**: / (root)
5. Click "Save"

### 4. Wait for Deployment

- GitHub will build and deploy your site
- This usually takes 1-2 minutes
- You'll see a green checkmark when ready
- Your site will be available at: `https://YOUR_USERNAME.github.io/personal-website`

## Custom Domain (Optional)

If you want to use a custom domain:

1. In repository Settings > Pages, click "Add a domain"
2. Enter your domain (e.g., `philipirvine.com`)
3. Configure DNS settings as instructed by GitHub
4. Update the `homepage` field in `package.json` to your custom domain

## Updating Your Website

To make changes:

```bash
# Make your changes to the files

# Stage and commit changes
git add .
git commit -m "Update website content"

# Push to GitHub
git push origin main
```

GitHub Pages will automatically rebuild and deploy your changes.

## Important Notes

- **Repository must be public** for free GitHub Pages
- All file paths are relative and will work correctly on GitHub Pages
- The 404.html page will handle broken links gracefully
- The website is fully responsive and will work on all devices
- No build process required - it's pure HTML/CSS/JS

## Troubleshooting

If your site doesn't appear:

1. Check that the repository is public
2. Verify GitHub Pages is enabled in Settings
3. Wait a few minutes for deployment to complete
4. Check the "Pages" section for any error messages
5. Make sure your `index.html` is in the root directory

## Performance

This website is optimized for GitHub Pages:
- ✅ No build process required
- ✅ Static files only
- ✅ Fast loading times
- ✅ SEO friendly
- ✅ Mobile responsive

Your website is now ready for the world! 🚀
