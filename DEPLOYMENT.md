# GitHub Pages Deployment Guide

## 🚀 Quick Deployment Steps

### 1. Create GitHub Repository
1. Go to [GitHub.com](https://github.com)
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. **Important**: Name your repository exactly as `your-username.github.io`
   - Replace `your-username` with your actual GitHub username
   - Example: If your username is `neerajchaudhari`, name it `neerajchaudhari.github.io`
5. Make sure it's **Public**
6. Click "Create repository"

### 2. Upload Your Files
**Option A: Using GitHub Web Interface**
1. In your new repository, click "Add file" → "Upload files"
2. Drag and drop all files from your portfolio folder
3. Click "Commit changes"

**Option B: Using Git Commands (Recommended)**
```bash
# Add your GitHub repository as remote
git remote add origin https://github.com/your-username/your-username.github.io.git

# Push your code to GitHub
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages
1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" section (in the left sidebar)
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch
6. Click "Save"

### 4. Your Site is Live!
- Wait 1-2 minutes for GitHub to build your site
- Visit `https://your-username.github.io` to see your portfolio!

## 🔧 Customization Before Deployment

### Update GitHub Profile Link
In `index.html`, find this line:
```html
<a href="#" target="_blank" class="text-white hover:text-blue-200 transition-colors">
```
Replace `#` with your actual GitHub profile URL:
```html
<a href="https://github.com/your-username" target="_blank" class="text-white hover:text-blue-200 transition-colors">
```

### Update Project Repository Links
In the Projects section, update the GitHub repo links:
```html
<a href="https://github.com/your-username/project-name" class="inline-flex items-center text-blue-600 hover:text-blue-800 font-medium">
```

### Add Your Profile Picture
Replace the placeholder icon with your actual photo:
```html
<!-- Replace this placeholder -->
<div class="w-40 h-40 bg-white/20 rounded-full flex items-center justify-center">
    <svg class="w-20 h-20 text-white/60" fill="currentColor" viewBox="0 0 24 24">
        <path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"/>
    </svg>
</div>

<!-- With your actual image -->
<img src="your-photo.jpg" alt="Neeraj Chaudhari" class="w-40 h-40 rounded-full object-cover">
```

## 📁 Files Included
- `index.html` - Main portfolio website (Tailwind CSS version)
- `README.md` - Project documentation
- `.gitignore` - Git ignore file
- `DEPLOYMENT.md` - This deployment guide

## 🌐 Alternative Hosting Options

### Netlify (Drag & Drop)
1. Go to [netlify.com](https://netlify.com)
2. Drag your portfolio folder to the deploy area
3. Your site will be live instantly!

### Vercel
1. Go to [vercel.com](https://vercel.com)
2. Connect your GitHub repository
3. Deploy automatically on every push

## 🔍 Troubleshooting

### Site Not Loading?
- Check that your repository is named correctly: `username.github.io`
- Ensure the repository is public
- Wait 2-3 minutes for GitHub Pages to build
- Check the "Actions" tab in your repository for build status

### Styling Issues?
- Make sure all files are uploaded
- Check browser console for any errors
- Verify Tailwind CSS CDN is loading properly

### Need Help?
- Check GitHub Pages documentation
- Look at the "Actions" tab for build logs
- Ensure your `index.html` is in the root directory

## 🎉 Success!
Once deployed, your portfolio will be accessible at:
`https://your-username.github.io`

Share this URL with potential employers, add it to your resume, and start showcasing your data science skills! 