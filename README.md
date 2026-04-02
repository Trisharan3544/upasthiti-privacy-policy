# Upasthiti Privacy Policy Website

This repository contains the privacy policy and terms of service for the Upasthiti mobile application, hosted on GitHub Pages.

## 📁 Repository Structure

```
upasthiti-privacy-policy/
├── index.html          # Privacy Policy page
├── terms.html          # Terms of Service page
├── landing.html        # App Landing page
├── css/
│   └── style.css       # Custom CSS with purple theme
├── images/
│   ├── logo.png        # App logo (add your logo here)
│   └── favicon.png     # Favicon (add your favicon here)
└── README.md           # This file
```

## 🎨 Design Features

- **Purple Theme**: Matches your app's #6200EE color scheme
- **Responsive Design**: Works on all devices (mobile, tablet, desktop)
- **Modern UI**: Clean, professional design with Material Design principles
- **Accessibility**: Screen reader friendly and high contrast support
- **Fast Loading**: Optimized for quick loading times

## 🚀 Setup Instructions

1. **Create GitHub Repository**:
   - Repository name: `upasthiti-privacy-policy`
   - Make it public
   - Add README file

2. **Upload Files**:
   - Upload all files from this folder to your repository
   - Add your app logo to `images/logo.png`
   - Add favicon to `images/favicon.png`

3. **Enable GitHub Pages**:
   - Go to repository Settings
   - Scroll to "Pages" section
   - Source: Deploy from a branch
   - Branch: main
   - Folder: / (root)
   - Click "Save"

4. **Your URLs will be**:
   - Privacy Policy: `https://[your-username].github.io/upasthiti-privacy-policy/`
   - Terms of Service: `https://[your-username].github.io/upasthiti-privacy-policy/terms.html`

## 📱 App Integration

Update your Android app with these URLs:

```java
// In PrivacyPolicyActivity.java
private static final String PRIVACY_POLICY_URL = "https://[your-username].github.io/upasthiti-privacy-policy/";

// In TermsAndConditionsActivity.java
private static final String TERMS_URL = "https://[your-username].github.io/upasthiti-privacy-policy/terms.html";
```

## 🎯 Features

- ✅ **Mobile-First Design**: Optimized for mobile devices
- ✅ **Purple Theme**: Matches your app's branding
- ✅ **Fast Loading**: Optimized CSS and HTML
- ✅ **SEO Friendly**: Proper meta tags and structure
- ✅ **Accessibility**: Screen reader support
- ✅ **Print Friendly**: Clean print styles
- ✅ **Dark Mode Support**: Automatic dark mode detection

## 🔧 Customization

### Colors
The CSS uses CSS variables for easy customization:
```css
:root {
    --primary-purple: #6200EE;
    --secondary-purple: #BB86FC;
    /* ... other colors */
}
```

### Content
Edit the HTML files to update:
- Privacy policy content
- Terms of service content
- Contact information
- App branding

## 📞 Support

If you need help with setup or customization, contact:
- **Email**: teamupasthiti@gmail.com
- **App**: Available in the app settings

## 📄 License

This privacy policy website is part of the Upasthiti project. All rights reserved.
