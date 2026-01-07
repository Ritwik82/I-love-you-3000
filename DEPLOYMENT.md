# 🚀 GitHub Deployment Guide for The Bard's Secret CTF

This guide will walk you through deploying your Shakespearean CTF challenge on GitHub and hosting it with GitHub Pages.

## 📋 Prerequisites

- A GitHub account (create one at https://github.com if you don't have one)
- Git installed on your computer
- Basic command line knowledge

---

## 🎯 Deployment Steps

### Option 1: Deploy via GitHub Web Interface (Easiest)

#### Step 1: Create a New Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the **+** icon in the top-right corner
3. Select **"New repository"**
4. Configure your repository:
   - **Repository name:** `shakespearean-ctf` (or your preferred name)
   - **Description:** "A Shakespearean-themed Capture The Flag challenge"
   - **Visibility:** Public (required for free GitHub Pages)
   - ✅ Check **"Add a README file"**
   - Click **"Create repository"**

#### Step 2: Upload the CTF Files

1. In your new repository, click **"Add file"** → **"Upload files"**
2. Drag and drop your `index.html` file
3. Click **"Commit changes"**
4. The README.md will be updated separately (or you can upload it too)

#### Step 3: Enable GitHub Pages

1. In your repository, click **"Settings"** (top menu)
2. Scroll down and click **"Pages"** in the left sidebar
3. Under **"Source"**, select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **"Save"**
5. Wait 1-2 minutes for deployment
6. Your CTF will be live at: `https://YOUR-USERNAME.github.io/shakespearean-ctf/`

---

### Option 2: Deploy via Command Line (Git)

#### Step 1: Initialize Local Repository

Open your terminal and navigate to your CTF folder:

```bash
# Navigate to where you saved the CTF files
cd path/to/your/ctf-folder

# Initialize Git repository
git init

# Add all files
git add index.html README.md

# Commit the files
git commit -m "Initial commit: Shakespearean CTF challenge"
```

#### Step 2: Create GitHub Repository

1. Go to [GitHub](https://github.com) and create a new repository (as described in Option 1)
2. **Important:** Do NOT initialize with README since you already have files

#### Step 3: Push to GitHub

```bash
# Add GitHub repository as remote
git remote add origin https://github.com/YOUR-USERNAME/shakespearean-ctf.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

#### Step 4: Enable GitHub Pages

Follow Step 3 from Option 1 above.

---

## 🔧 Using GitHub CLI (Alternative Method)

If you have GitHub CLI installed:

```bash
# Create repository directly from command line
gh repo create shakespearean-ctf --public --source=. --remote=origin --push

# Enable GitHub Pages
gh api repos/{owner}/{repo}/pages -X POST -f source[branch]=main -f source[path]=/
```

---

## ✅ Verify Deployment

1. Visit your GitHub Pages URL: `https://YOUR-USERNAME.github.io/shakespearean-ctf/`
2. The CTF challenge should load with the Shakespearean theme
3. Test all three stages to ensure functionality
4. Share the link with participants!

---

## 🎨 Customization After Deployment

### Update Files

**Via Web Interface:**
1. Navigate to the file in your repository
2. Click the **pencil icon** (Edit)
3. Make changes
4. Click **"Commit changes"**
5. GitHub Pages will auto-update in 1-2 minutes

**Via Git:**
```bash
# Make your changes to index.html
git add index.html
git commit -m "Update challenge difficulty"
git push origin main
```

---

## 📊 Monitor Your CTF

### View Repository Statistics

- Go to **Insights** → **Traffic** to see visitor stats
- Check **Stars** to see how popular your CTF becomes

### Share Your CTF

Share this URL format:
```
https://YOUR-USERNAME.github.io/shakespearean-ctf/
```

Example social media post:
> 🎭 Just created "The Bard's Secret" - a Shakespearean-themed CTF challenge!
> Test your cybersecurity skills with Base64, JavaScript, and Caesar ciphers.
> All wrapped in theatrical Elizabethan flair. 
> Play here: [your-github-pages-url]
> #CTF #Cybersecurity #Shakespeare

---

## 🐛 Troubleshooting

### GitHub Pages Not Loading?

1. **Check Settings:** Ensure GitHub Pages is enabled and set to `main` branch
2. **Wait Time:** Initial deployment can take 5-10 minutes
3. **Repository Visibility:** Must be Public for free GitHub Pages
4. **File Name:** Ensure your main file is named `index.html` (lowercase)

### 404 Error?

- Verify the URL format: `https://username.github.io/repository-name/`
- Check that `index.html` is in the root directory

### Changes Not Appearing?

- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Wait 1-2 minutes for GitHub Pages to rebuild
- Check GitHub Actions tab for deployment status

---

## 🔒 Security Considerations

### For CTF Creators:

- ✅ Flags are visible in source code (intentional for beginner CTFs)
- ✅ No backend = no server-side vulnerabilities
- ✅ Pure client-side = easy to host and maintain

### Want to Make It Harder?

1. **Obfuscate JavaScript:** Use tools like [JavaScript Obfuscator](https://obfuscator.io/)
2. **Hide in Network Requests:** Store flags in fake API responses
3. **Use Steganography:** Hide flags in images
4. **Add Cookie Challenges:** Store clues in browser cookies

---

## 📱 Mobile Testing

Your CTF is mobile-responsive! Test on:
- iOS Safari
- Android Chrome
- Different screen sizes

---

## 🎯 Next Steps

### Enhance Your CTF:

1. **Add Analytics:** Integrate Google Analytics to track completions
2. **Create Leaderboard:** Use GitHub Issues or external service
3. **Add More Stages:** Expand with XSS, SQL injection simulations
4. **Create Variations:** Make seasonal versions (Halloween, Christmas)
5. **Add Certificates:** Generate completion certificates

### Share in Communities:

- Reddit: r/netsec, r/cybersecurity, r/CTF
- Discord: CTF communities
- Twitter: #CTF #Cybersecurity
- LinkedIn: Professional network

---

## 📚 Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Basics Tutorial](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
- [Markdown Guide](https://www.markdownguide.org/) (for README formatting)

---

## 🎓 Example GitHub Repository Structure

```
shakespearean-ctf/
├── index.html          # Main CTF challenge page
├── README.md           # Solution guide and documentation
├── DEPLOYMENT.md       # This file
└── assets/             # (Optional) For images, CSS, etc.
    ├── images/
    └── styles/
```

---

## ✨ Success!

Once deployed, your CTF will be:
- ✅ Publicly accessible
- ✅ Free to host
- ✅ Easy to share
- ✅ Version controlled
- ✅ Professional looking

**Your CTF URL:** `https://YOUR-USERNAME.github.io/shakespearean-ctf/`

---

*"The web's the thing wherein we'll catch the conscience of the king!" - Hamlet (adapted)*

Happy hosting! 🎭🚀
