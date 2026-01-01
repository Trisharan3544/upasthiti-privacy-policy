# Account Deletion Link Setup

## 🔗 Adding Account Deletion Link to Privacy Policy & Terms Pages

The Privacy Policy and Terms of Service pages now include a "Delete Account" link in the footer that directs users to the account deletion page.

## 📝 Configuration

### ⚠️ IMPORTANT: Update URLs in HTML Files

**You MUST replace `your-username` with your actual GitHub username in the HTML files:**

### Files to Update:
1. `index.html` - Line 549 (footer link)
2. `terms.html` - Line 468 (footer link)

**Find and replace:**
- `https://your-username.github.io/upasthiti-account-deletion/`

**With your actual URL:**
- `https://[YOUR-ACTUAL-USERNAME].github.io/upasthiti-account-deletion/`

### Step 2: Optional - Update Config File

You can also update **`js/config.js`** to override the HTML URL:

```javascript
const CONFIG = {
    // Account Deletion URL (update with your GitHub username)
    ACCOUNT_DELETION_URL: 'https://your-username.github.io/upasthiti-account-deletion/',
    
    // Contact Email
    CONTACT_EMAIL: 'teamupasthiti@gmail.com'
};
```

**Note**: The HTML files have default URLs that work immediately. The config.js file can override them if you prefer centralized configuration.

**Example:**
If your GitHub username is `johnsmith`, update to:
```javascript
ACCOUNT_DELETION_URL: 'https://johnsmith.github.io/upasthiti-account-deletion/',
```

## ✅ What's Included

### Footer Links

Both **Privacy Policy** (`index.html`) and **Terms of Service** (`terms.html`) now have:

- Privacy Policy link
- Terms of Service link
- **Delete Account link** (new) - Links to account deletion page

### Features

- **Centralized Configuration**: Update URL in one place (`js/config.js`)
- **Automatic Updates**: Both pages use the same URL
- **External Link**: Opens in new tab (`target="_blank"`)
- **Security**: Uses `rel="noopener noreferrer"` for security
- **Accessible**: Users can access account deletion from any page

## 🔍 Testing

After updating the URL:

1. Open Privacy Policy page
2. Scroll to footer
3. Click "Delete Account" - should open account deletion page
4. Open Terms of Service page
5. Scroll to footer
6. Click "Delete Account" - should open account deletion page
7. Verify both links work correctly

## 📱 User Flow

Users can now access account deletion from:

1. **Privacy Policy Page** → Footer → "Delete Account"
2. **Terms of Service Page** → Footer → "Delete Account"
3. **Account Deletion Page** → Direct access

This ensures users can easily find and access the account deletion page from any legal document page.

## 📞 Need Help?

If you need assistance:
- **Email**: teamupasthiti@gmail.com
- Check your GitHub Pages repository settings
- Verify your account deletion repository is public and deployed

---

**Note**: Make sure your account deletion repository is deployed and accessible before updating this URL.

