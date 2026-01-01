# URL Update Instructions

## ⚠️ IMPORTANT: Update URLs After Hosting

After you host your privacy policy website on GitHub Pages, you **MUST** update the URLs in your app code.

## 📝 Files to Update

### 1. PrivacyPolicyActivity.java

**File:** `app/src/main/java/com/shu/upasthiti/PrivacyPolicyActivity.java`

**Line 18:** Replace `YOUR_USERNAME` with your actual GitHub username:

```java
// BEFORE:
private static final String PRIVACY_POLICY_URL = "https://YOUR_USERNAME.github.io/upasthiti-privacy-policy/";

// AFTER (example):
private static final String PRIVACY_POLICY_URL = "https://johndoe.github.io/upasthiti-privacy-policy/";
```

### 2. TermsAndConditionsActivity.java

**File:** `app/src/main/java/com/shu/upasthiti/TermsAndConditionsActivity.java`

**Line 17:** Replace `YOUR_USERNAME` with your actual GitHub username:

```java
// BEFORE:
private static final String TERMS_URL = "https://YOUR_USERNAME.github.io/upasthiti-privacy-policy/terms.html";

// AFTER (example):
private static final String TERMS_URL = "https://johndoe.github.io/upasthiti-privacy-policy/terms.html";
```

## 🔍 How to Find Your GitHub Username

1. Go to GitHub.com
2. Sign in to your account
3. Your username is in the top right corner (or in your profile URL)
4. Example: If your profile URL is `https://github.com/johndoe`, then `johndoe` is your username

## ✅ After Updating

1. **Test the URLs** in a browser to make sure they work
2. **Build and test** the app to verify WebView loads correctly
3. **Test offline fallback** by disabling internet and checking if text version shows

## 📱 Example URLs

After hosting, your URLs will look like:
- Privacy Policy: `https://yourusername.github.io/upasthiti-privacy-policy/`
- Terms: `https://yourusername.github.io/upasthiti-privacy-policy/terms.html`

Replace `yourusername` with your actual GitHub username.

---

**Note:** The app will automatically fall back to the offline text version if:
- Internet is not available
- WebView fails to load
- URL is incorrect or site is down

This ensures users can always read the Privacy Policy and Terms even offline.

