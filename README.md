# Alertim Website

This repository contains the Alertim website, ready to be deployed on GitHub Pages.

## Project Structure

```
Alertim/
├── index.html          # Main entry point (redirects to Home.html)
├── Home.html           # Home page
├── Projects.html       # Projects page
├── Contact.html        # Contact page
├── Home/               # Images for Home page
├── Projects/           # Images for Projects page
└── Contact/            # Images for Contact page
```

## Setting Up GitHub Pages

### Prerequisites

- A GitHub account
- Git installed on your local machine

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name your repository (e.g., `alertim-website` or `alertim.github.io`)
   - **Note**: If you name it `yourusername.github.io`, it will be available at `https://yourusername.github.io`
   - Otherwise, it will be at `https://yourusername.github.io/repository-name`
5. Choose whether to make it public or private
6. **Do NOT** initialize with a README, .gitignore, or license (we already have these)
7. Click "Create repository"

### Step 2: Push Your Code to GitHub

Open a terminal in the project directory and run:

```bash
# Add all files to git
git add .

# Create your first commit
git commit -m "Initial commit: Alertim website"

# Rename branch to main (if needed)
git branch -M main

# Add your GitHub repository as remote (replace with your repository URL)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git

# Push to GitHub
git push -u origin main
```

**Replace `YOUR_USERNAME` and `YOUR_REPOSITORY_NAME` with your actual GitHub username and repository name.**

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** (in the repository navigation bar)
3. Scroll down to the **Pages** section in the left sidebar
4. Under **Source**, select:
   - **Branch**: `main` (or `master` if that's your default branch)
   - **Folder**: `/ (root)`
5. Click **Save**

### Step 4: Access Your Website

- GitHub will provide you with a URL like:
  - `https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME` (for regular repositories)
  - `https://YOUR_USERNAME.github.io` (if repository is named `YOUR_USERNAME.github.io`)

- It may take a few minutes for the site to be available after enabling Pages
- You can check the deployment status in the **Actions** tab

## Updating Your Website

To update your website:

```bash
# Make your changes to the HTML files or images

# Stage the changes
git add .

# Commit the changes
git commit -m "Description of your changes"

# Push to GitHub
git push
```

GitHub Pages will automatically rebuild your site when you push changes. It usually takes 1-2 minutes for updates to appear.

## Custom Domain (Optional)

If you want to use a custom domain:

1. Create a file named `CNAME` in the root directory
2. Add your domain name (e.g., `www.yourdomain.com`) to the file
3. Configure your DNS settings as instructed by GitHub
4. Commit and push the `CNAME` file

## Troubleshooting

### Site Not Loading

- Wait a few minutes after enabling Pages (first deployment can take up to 10 minutes)
- Check the **Actions** tab for any build errors
- Verify that `index.html` exists in the root directory
- Ensure all image paths are correct (relative paths should work)

### Images Not Showing

- Verify that image folders (Home/, Projects/, Contact/) are in the root directory
- Check that image paths in HTML files use relative paths (e.g., `Home/image.jpg`)
- Ensure image files are committed to the repository

### 404 Errors

- Make sure `index.html` exists in the root
- Verify that all HTML files (Home.html, Projects.html, Contact.html) are in the root directory
- Check that internal links use correct relative paths

## Local Testing

To test your website locally before pushing:

1. Use a simple HTTP server:
   ```bash
   # Python 3
   python3 -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   
   # Node.js (if you have http-server installed)
   npx http-server
   ```

2. Open your browser and go to `http://localhost:8000`

## Support

For more information about GitHub Pages, visit:
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Pages Guide](https://pages.github.com/)

