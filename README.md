# Git-Buddy

A Chrome extension that provides helpful Git-related functionality.

## Project Structure

```
Git-Buddy/
├── manifest.json          # Extension configuration file
├── hello.html            # Popup HTML file
├── popup.js              # Popup JavaScript logic
├── hello_extensions.png  # Extension icon
└── README.md             # This file
```

## Installation & Development Setup

### Prerequisites

- **Google Chrome Browser** (version 88 or later recommended)
- **Basic knowledge of Chrome DevTools** (helpful but not required)

### Step-by-Step Installation Guide

#### 1. Download/Clone the Project

If you haven't already, download or clone this project to your local machine:

```bash
git clone <repository-url>
cd Git-Buddy
```

#### 2. Open Chrome Extensions Page

1. Open **Google Chrome** on your computer
2. In the address bar, type: `chrome://extensions/`
3. Press **Enter**

**Alternative method:**
- Click the **three-dot menu** (⋮) in the top-right corner of Chrome
- Go to **More tools** → **Extensions**

#### 3. Enable Developer Mode

1. In the top-right corner of the Extensions page, find the **"Developer mode"** toggle
2. **Turn ON** the Developer mode toggle
3. You should see additional options appear below

#### 4. Load the Extension

1. Click the **"Load unpacked"** button that appears after enabling Developer mode
2. In the file picker dialog, navigate to your **Git-Buddy project folder**
3. **Select the folder** (not individual files) and click **"Select Folder"**
4. Chrome will load your extension and display it in the extensions list

#### 5. Verify Installation

1. Look for **"Hello Extensions"** in your extensions list
2. You should see the extension icon in your Chrome toolbar (top-right area)
3. The extension status should show **"Enabled"**

### Testing the Extension

#### Basic Functionality Test

1. **Click the extension icon** in your Chrome toolbar
2. A popup should appear with the message: **"Hello Extensions of the World!"**
3. **Right-click the extension icon** and select **"Inspect popup"** to open DevTools
4. Check the **Console tab** in DevTools - you should see: **"This is a popup!"**

#### Troubleshooting Common Issues

**Extension not appearing in toolbar:**
- Check if the extension is enabled in `chrome://extensions/`
- Try refreshing the page you're on
- Restart Chrome if necessary

**Popup not working:**
- Check the Console in DevTools for JavaScript errors
- Verify all files are in the correct location
- Ensure the manifest.json references the correct HTML file

**Extension disappears after Chrome restart:**
- This is normal for development mode extensions
- You'll need to reload it using "Load unpacked" again

### Development Workflow

#### Making Changes

1. **Edit your files** (HTML, CSS, JavaScript) in your preferred code editor
2. **Save the files**
3. **Go back to `chrome://extensions/`**
4. **Click the refresh/reload button** (🔄) on your extension card
5. **Test your changes** by clicking the extension icon

#### Hot Reload (Recommended)

For a better development experience, you can use the **"Reload"** button instead of manually refreshing:

1. Make changes to your code
2. Save the files
3. Click the **🔄 Reload button** on your extension in `chrome://extensions/`
4. Test immediately - no need to close/reopen popups

### File Descriptions

- **`manifest.json`**: Defines the extension's properties, permissions, and behavior
- **`hello.html`**: The popup interface that appears when clicking the extension icon
- **`popup.js`**: JavaScript logic for the popup functionality
- **`hello_extensions.png`**: Icon displayed in the Chrome toolbar

### Next Steps

Once you're comfortable with the basic setup:

1. **Modify the HTML** in `hello.html` to change the popup content
2. **Add functionality** in `popup.js` for your Git-related features
3. **Update the manifest.json** to add permissions or background scripts as needed
4. **Customize the icon** by replacing `hello_extensions.png`

### Publishing (Optional)

When you're ready to distribute your extension:

1. **Package the extension** using Chrome's "Pack extension" feature
2. **Submit to Chrome Web Store** for public distribution
3. **Or distribute the .crx file** directly to users (requires manual installation)

### Support & Resources

- **Chrome Extensions Documentation**: [developer.chrome.com/docs/extensions/](https://developer.chrome.com/docs/extensions/)
- **Manifest V3 Guide**: [developer.chrome.com/docs/extensions/mv3/intro/](https://developer.chrome.com/docs/extensions/mv3/intro/)
- **Chrome DevTools**: [developer.chrome.com/docs/devtools/](https://developer.chrome.com/docs/devtools/)

---

**Note**: This extension is currently in development mode. For production use, consider publishing to the Chrome Web Store or implementing proper security measures.