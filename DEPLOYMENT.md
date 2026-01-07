
```md
<!-- DEPLOYMENT.md -->
# 🚀 GitHub Deployment Guide for The Bard's Secret CTF (LNMIIT Edition)

This guide walks you through deploying your Shakespearean CTF challenge on GitHub and hosting it with GitHub Pages.

## 📋 Prerequisites

- GitHub account
- Git installed
- Basic command line usage (CMD / PowerShell / terminal)

---

## 🎯 Deployment Steps

### Option 1: Deploy via GitHub Web (Easiest)

#### Step 1: Create Repository

1. Go to <https://github.com> and log in.
2. Click the **+** in the top-right → **New repository**.
3. Set:
   - **Name:** `shakespearean-ctf-lnm` (or similar).
   - **Public** repo.
4. Click **Create repository**.

#### Step 2: Upload Files

1. In the repo, click **Add file** → **Upload files**.
2. Upload:
   - `index.html`
   - `README.md`
   - `DEPLOYMENT.md`
3. Click **Commit changes**.

#### Step 3: Enable GitHub Pages

1. Go to **Settings** → **Pages**.
2. **Source:**  
   - Branch: `main`  
   - Folder: `/ (root)`
3. Click **Save**.
4. Wait 1–2 minutes.

Your CTF will be live at:

```text
https://YOUR-USERNAME.github.io/shakespearean-ctf-lnm/
