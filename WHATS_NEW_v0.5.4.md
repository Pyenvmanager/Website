
# What's New in PyEnvManager v0.5.4

## 🐛 Important Fixes/Features

### More Accurate Security Scanning

Added Detection and scanning for system python

**What this means for you:**
- Security scan results are now more reliable
- Better understanding of actual risk levels in your environments
- More accurate compliance reporting

### Virtual Environment Creation Now Works Reliably

Fixed an issue where creating virtual environments (venv) would sometimes fail, especially with Python installations from the Microsoft Store.

**What this means for you:**
- venv creation works smoothly every time
- No more "command not recognized" errors
- Better support for different Python installation types

### Cleaner Environment Selection

When creating a new virtual environment, you might have seen the same Python version listed twice in the dropdown. This has been fixed!

**What this means for you:**
- Cleaner, easier-to-read Python version selector
- No more duplicate entries
- Faster environment creation workflow

## ✨ New Features

### Quick Access to Environment Folders

We've added convenient buttons throughout the app so you can quickly jump to your environment folders in your file explorer.

**Where you'll find it:**

📋 **In the Environment List**  
Look for the small folder icon next to each environment's path - click it to open that environment's folder instantly.

📂 **In Environment Details**  
A prominent "Open Directory" button appears next to the installation path, making it easy to browse your environment's files.

🚀 **In Scan Results**  
After running an automated scan, use the "Open Results Folder" button to quickly view your generated reports and SBOM files.

**Why it's useful:**
- Quickly access environment files without navigating manually
- View scan results and exports with one click
- Faster debugging and file management

## 💡 Tips

- Use the new directory buttons to quickly verify environment contents
- After automated scans, click "Open Results Folder" to explore detailed reports
- Create venvs with confidence - the path resolution issues are fixed!

The installer will automatically update your existing installation while preserving all your environments and settings.

## 🔄 Upgrading from Previous Versions

Simply download and install the new version - all your existing:
- ✅ Environments will continue to work
- ✅ Scan history is preserved
- ✅ Settings remain unchanged
- ✅ Package data is kept


## 🙏 Thank You

Thank you to all users who provided feedback and feature requests and as usually, special thanks to [vmiengineering](https://github.com/vmiengineering)
