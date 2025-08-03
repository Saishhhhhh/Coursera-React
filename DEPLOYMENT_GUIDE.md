# GitHub Pages Deployment Guide

## 🚀 **Quick Fix for Blank White Screen**

### **Step 1: Update Repository Settings**

1. Go to your GitHub repository
2. Click on **Settings** tab
3. Scroll down to **Pages** section
4. Under **Source**, select **Deploy from a branch**
5. Choose **gh-pages** branch (or **main** if using GitHub Actions)
6. Click **Save**

### **Step 2: Deploy Using GitHub Actions (Recommended)**

The `.github/workflows/deploy.yml` file has been created. This will automatically deploy your app when you push to main branch.

1. **Push your changes** to the main branch
2. **Check Actions tab** in your repository
3. **Wait for deployment** to complete
4. **Visit your site** at: `https://saishhhhhh.github.io/Coursera-React/`

### **Step 3: Manual Deployment (Alternative)**

If you prefer manual deployment:

```bash
# Install gh-pages if not already installed
npm install --save-dev gh-pages

# Build the project
npm run build

# Deploy to GitHub Pages
npm run deploy
```

## 🔧 **Configuration Files Updated**

### **vite.config.js**
- ✅ Base path set to `/Coursera-React/`
- ✅ Build configuration optimized
- ✅ Development server settings

### **index.html**
- ✅ SPA routing script added
- ✅ Proper meta tags
- ✅ Title updated to "Paradise Nursery"

### **404.html**
- ✅ Created for GitHub Pages routing
- ✅ Handles SPA navigation properly

### **GitHub Actions**
- ✅ Automated deployment workflow
- ✅ Builds and deploys on push to main

## 🐛 **Common Issues & Solutions**

### **Blank White Screen**
- **Cause**: Incorrect base path or missing routing
- **Solution**: Updated vite.config.js with correct base path

### **404 Errors on Refresh**
- **Cause**: GitHub Pages doesn't support client-side routing
- **Solution**: Added 404.html and SPA routing script

### **Assets Not Loading**
- **Cause**: Incorrect asset paths
- **Solution**: Base path configured correctly

## 📋 **Deployment Checklist**

Before deploying, ensure:

- [ ] **Repository name** matches the base path in vite.config.js
- [ ] **GitHub Pages** is enabled in repository settings
- [ ] **gh-pages branch** is selected as source (or GitHub Actions)
- [ ] **All files** are committed and pushed
- [ ] **Build completes** without errors

## 🔍 **Testing Your Deployment**

1. **Wait 2-5 minutes** after deployment
2. **Clear browser cache** (Ctrl+F5 or Cmd+Shift+R)
3. **Test all functionality**:
   - Landing page loads
   - Navigation works
   - Cart functionality works
   - Responsive design works

## 📞 **If Still Having Issues**

1. **Check GitHub Actions** for build errors
2. **Verify repository name** matches base path
3. **Clear browser cache** and try incognito mode
4. **Check browser console** for JavaScript errors
5. **Verify all assets** are loading correctly

## 🎯 **Expected Result**

After successful deployment, your site should:
- ✅ Load without blank white screen
- ✅ Display the Paradise Nursery landing page
- ✅ Allow navigation between pages
- ✅ Have working cart functionality
- ✅ Be responsive on all devices

**Your site URL**: `https://saishhhhhh.github.io/Coursera-React/` 