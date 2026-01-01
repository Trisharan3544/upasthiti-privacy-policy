# Privacy Policy Website Hosting Guide

## 🚀 Quick Setup on GitHub Pages (Free & Easy)

### Step 1: Create GitHub Repository

1. **Go to GitHub.com** and sign in to your account
2. **Click the "+" icon** in the top right → **"New repository"**
3. **Repository Settings:**
   - **Repository name:** `upasthiti-privacy-policy`
   - **Description:** `Privacy Policy and Terms of Service for Upasthiti App`
   - **Visibility:** Select **Public** (required for free GitHub Pages)
   - ⚠️ **DO NOT** check "Add README" (we'll upload our files)
   - ⚠️ **DO NOT** add .gitignore or license (we'll add our own)
4. **Click "Create repository"**

---

### Step 2: Upload Files to GitHub

#### Option A: Using GitHub Web Interface (Easiest)

1. **In your new repository**, click **"uploading an existing file"**
2. **Drag and drop** all files from `privacy-policy-website/` folder:
   - `index.html`
   - `terms.html`
   - `README.md`
   - `css/` folder (with `style.css` inside)
   - `images/` folder (with logo files)
3. **Scroll down** and click **"Commit changes"**
4. **Wait for files to upload**

#### Option B: Using Git Command Line (For Advanced Users)

```bash
# Navigate to your project folder
cd C:\Users\admin\Desktop\UPASTHITI\Upasthiti\privacy-policy-website

# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Privacy Policy and Terms of Service"

# Add remote repository (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/upasthiti-privacy-policy.git

# Push to GitHub
git branch -M main
git push -u origin main
```

---

### Step 3: Enable GitHub Pages

1. **Go to your repository** on GitHub
2. **Click "Settings"** tab (at the top of the repository)
3. **Scroll down** to **"Pages"** section (in the left sidebar)
4. **Under "Source":**
   - Select **"Deploy from a branch"**
   - **Branch:** Select `main`
   - **Folder:** Select `/ (root)`
5. **Click "Save"**
6. **Wait 1-2 minutes** for GitHub to build your site
7. **Your site will be live at:**
   - Privacy Policy: `https://YOUR_USERNAME.github.io/upasthiti-privacy-policy/`
   - Terms of Service: `https://YOUR_USERNAME.github.io/upasthiti-privacy-policy/terms.html`

---

### Step 4: Verify Your Site

1. **Click the link** GitHub provides after enabling Pages
2. **Test both pages:**
   - Privacy Policy loads correctly
   - Terms of Service loads correctly
   - CSS styling works
   - Images display properly
3. **Test on mobile** (if possible)

---

### Step 5: Update Your App with URLs

Once you have your GitHub Pages URL, update your app:

#### Update Privacy Policy URL in App:

**File:** `app/src/main/java/com/shu/upasthiti/PrivacyPolicyActivity.java`

Add a method to open the web version:
```java
// Add this constant at the top of the class
private static final String PRIVACY_POLICY_URL = "https://YOUR_USERNAME.github.io/upasthiti-privacy-policy/";

// Add this method to open web version
private void openPrivacyPolicyWeb() {
    Intent intent = new Intent(Intent.ACTION_VIEW);
    intent.setData(Uri.parse(PRIVACY_POLICY_URL));
    startActivity(intent);
}
```

#### Update Terms & Conditions URL in App:

**File:** `app/src/main/java/com/shu/upasthiti/TermsAndConditionsActivity.java`

Add a method to open the web version:
```java
// Add this constant at the top of the class
private static final String TERMS_URL = "https://YOUR_USERNAME.github.io/upasthiti-privacy-policy/terms.html";

// Add this method to open web version
private void openTermsWeb() {
    Intent intent = new Intent(Intent.ACTION_VIEW);
    intent.setData(Uri.parse(TERMS_URL));
    startActivity(intent);
}
```

---

### Step 6: Add URL to Play Console

When you submit to Google Play Store:

1. **Go to Google Play Console**
2. **Select your app**
3. **Go to "Store presence" > "Store listing"**
4. **Scroll to "Privacy Policy" section**
5. **Enter your URL:** `https://YOUR_USERNAME.github.io/upasthiti-privacy-policy/`
6. **Save**

---

## ✅ Checklist

- [ ] GitHub repository created
- [ ] All files uploaded to GitHub
- [ ] GitHub Pages enabled
- [ ] Site is live and accessible
- [ ] Privacy Policy page loads correctly
- [ ] Terms of Service page loads correctly
- [ ] CSS styling works
- [ ] Images display properly
- [ ] Mobile responsive works
- [ ] URLs saved for Play Console

---

## 🔧 Troubleshooting

### Site Not Loading?
- Wait 2-5 minutes after enabling Pages
- Check if repository is **Public** (required for free Pages)
- Verify branch is `main` and folder is `/ (root)`
- Check repository settings → Pages section

### CSS Not Loading?
- Verify `css/style.css` file is in the `css/` folder
- Check file paths in HTML (should be `css/style.css`)
- Clear browser cache and reload

### Images Not Showing?
- Verify `images/` folder contains logo files
- Check file paths in HTML
- Ensure image files are uploaded to GitHub

---

## 📝 Example URLs

After setup, your URLs will look like:
- **Privacy Policy:** `https://yourusername.github.io/upasthiti-privacy-policy/`
- **Terms of Service:** `https://yourusername.github.io/upasthiti-privacy-policy/terms.html`

Replace `yourusername` with your actual GitHub username.

---

## 🎯 Next Steps After Hosting

1. ✅ Test URLs in browser
2. ✅ Update app with URLs (optional - for web view)
3. ✅ Add URL to Play Console when submitting
4. ✅ Share URL in app settings if needed

---

## 💡 Tips

- **Free Forever:** GitHub Pages is free for public repositories
- **Custom Domain:** You can add a custom domain later if needed
- **Auto Updates:** Any changes you push to GitHub will automatically update the website
- **HTTPS:** GitHub Pages automatically provides HTTPS security

---

## 📞 Need Help?

If you encounter any issues:
1. Check GitHub Pages documentation: https://docs.github.com/en/pages
2. Verify all files are uploaded correctly
3. Ensure repository is Public
4. Wait a few minutes for changes to propagate

---

**Ready to host?** Follow the steps above and you'll have your privacy policy website live in minutes! 🚀

