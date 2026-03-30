# GitHub Setup Instructions

## 📦 What You Have

A complete TFT Team Builder project ready for GitHub, including:

- ✅ `index.html` - Single-file app (with TFT logo, Sets 14-17)
- ✅ `README.md` - Professional project documentation
- ✅ `CONTRIBUTING.md` - Contribution guidelines
- ✅ `LICENSE` - MIT License
- ✅ `.gitignore` - Git configuration

---

## 🚀 Push to GitHub (5 Minutes)

### Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. **Repository name**: `tft-team-builder`
3. **Description**: `Offline-first Team Fight Tactics team builder`
4. **Public** or **Private**: Choose (Public recommended)
5. **Initialize repository**: Leave unchecked (we'll push existing files)
6. Click **Create repository**

### Step 2: Copy Repository URL

After creating, you'll see:
```
https://github.com/yourusername/tft-team-builder.git
```

Copy this URL.

### Step 3: Initialize Git and Push

```bash
# Navigate to your project folder
cd /path/to/tft-team-builder

# Initialize git
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: Add TFT Team Builder

- Single-file offline app
- Supports Sets 14-17
- TFT logo and branding
- Team builder, meta list, set browser
- iPhone web app ready"

# Add remote repository
git remote add origin https://github.com/yourusername/tft-team-builder.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Done!** Your project is now on GitHub. 🎉

---

## 📋 Verify Your GitHub Repo

Check your GitHub repository:
1. Go to `https://github.com/yourusername/tft-team-builder`
2. Verify these files are showing:
   - ✅ index.html
   - ✅ README.md
   - ✅ CONTRIBUTING.md
   - ✅ LICENSE
   - ✅ .gitignore

3. You should see the **README displayed** on the main page
4. **Green "Code" button** with clone options

---

## ⭐ Optional: Make Your Repo Stand Out

### Add GitHub Topics
1. Go to your repository **Settings**
2. Scroll to **Repository topics**
3. Add these topics:
   - `tft`
   - `team-fight-tactics`
   - `team-builder`
   - `offline-app`
   - `web-app`
   - `game-tools`

### Add a Repository Description
1. Go to **About** (gear icon, top right)
2. Add description: `Offline TFT team builder - Works anywhere, no internet needed`
3. Add website URL if deployed
4. Check **Releases** box if you'll publish versions

### Pin Important Files
GitHub will automatically show:
- README.md (in main view)
- LICENSE (recognizes MIT License)
- CONTRIBUTING.md (shows to contributors)

---

## 🔄 Update Your Repository

### After Making Changes Locally

```bash
# Check what changed
git status

# Add changes
git add .

# Commit with meaningful message
git commit -m "Update: Add Set 17 champions"

# Push to GitHub
git push origin main
```

### Good Commit Messages
```bash
# Examples of good commit messages:
git commit -m "Add: Set 16 meta compositions"
git commit -m "Fix: Trait synergy calculation"
git commit -m "Update: Improve mobile responsiveness"
git commit -m "Docs: Update README with new features"
```

---

## 📈 Growing Your Repository

### Get Stars ⭐
- Share on Reddit (r/teamfighttactics, r/leagueoflegends)
- Share on Discord servers
- Share on Twitter/X
- Add to awesome lists

### Example Tweet
```
🎮 Just released TFT Team Builder - An offline team composition builder 
that works without internet. Build teams anywhere, anytime!

📥 Runs in browser, saves locally
📱 Works on iPhone as web app
⚡ Zero dependencies
📖 Open source & MIT licensed

Check it out: github.com/yourusername/tft-team-builder
```

### Add to Awesome Lists
Submit your project to:
- [Awesome TFT](https://github.com/topics/tft)
- [Awesome Gaming](https://github.com/topics/game-tools)
- [Awesome Tools](https://github.com/sindresorhus/awesome)

---

## 🚀 Deploy Your App

Even better than GitHub: Deploy it online!

### Option 1: GitHub Pages (Free)
```bash
# In your GitHub repo Settings → Pages
# Set to deploy from "main" branch
# Your app will be available at:
# https://yourusername.github.io/tft-team-builder
```

### Option 2: Vercel (Recommended)
```bash
# 1. Go to vercel.com
# 2. Connect your GitHub repo
# 3. Deploy (automatically!)
# 4. Get URL like: tft-team-builder.vercel.app
```

### Option 3: Netlify
```bash
# 1. Go to netlify.com
# 2. Connect your GitHub repo
# 3. Deploy (automatically!)
# 4. Get free URL
```

---

## 🔐 Security & Best Practices

### Enable GitHub Security Features
1. Go to **Settings** → **Security & analysis**
2. Enable:
   - ✅ Dependabot alerts (if applicable)
   - ✅ Secret scanning (if applicable)

### Protect Main Branch (Optional)
1. **Settings** → **Branches**
2. Add rule for "main"
3. Require pull request reviews
4. Dismiss stale PR approvals

### Add GitHub Actions (Optional)
Create `.github/workflows/` for:
- Automated testing
- Code quality checks
- Deploy notifications

---

## 📞 Managing Issues & Discussions

### Enable Issues
- ✅ Enabled by default
- Users can report bugs
- Request features
- Ask questions

### Set Up Issue Templates
Create `.github/ISSUE_TEMPLATE/`:

**bug_report.md**
```markdown
---
name: Bug Report
about: Report a bug
---

## Description
[Describe the bug]

## Steps to Reproduce
[How to reproduce]

## Browser & OS
[Browser and operating system]

## Expected vs Actual
[What should happen vs what happened]
```

**feature_request.md**
```markdown
---
name: Feature Request
about: Suggest an enhancement
---

## Description
[Describe the feature]

## Why?
[Why would this be useful?]

## Alternatives
[Alternative approaches?]
```

---

## 🎯 GitHub Profile Tips

### Add to Your Profile
1. Go to `github.com/yourusername`
2. Pin your TFT Team Builder repo
3. It will show as your top project

### Write a Good Bio
```
Game developer | TFT enthusiast | Open source contributor
Passionate about gaming tools and offline-first apps 🎮
```

---

## 📊 Track Progress

### GitHub Insights
Visit `github.com/yourusername/tft-team-builder/insights` to see:
- Traffic & views
- Repository contributors
- Traffic sources
- Clone statistics

### Watch for Issues
Visit `github.com/yourusername/tft-team-builder/issues` to see:
- Bug reports from users
- Feature requests
- Discussions

---

## 🆘 If Something Goes Wrong

### "Everything is messed up"
```bash
# Reset local repo to GitHub
git fetch origin
git reset --hard origin/main
```

### "I pushed the wrong code"
```bash
# Revert last commit
git revert HEAD
git push origin main
```

### "I need to undo everything"
```bash
# Go back to a previous commit
git log  # Find the commit hash
git reset --hard <commit-hash>
git push origin main --force-with-lease
```

---

## ✅ Checklist: Ready for GitHub?

Before pushing, make sure:

- [ ] `index.html` works correctly
- [ ] `README.md` looks good
- [ ] `CONTRIBUTING.md` is clear
- [ ] `LICENSE` is included
- [ ] `.gitignore` is set up
- [ ] No sensitive data in files
- [ ] All links work properly
- [ ] File structure is clean
- [ ] No unnecessary files

---

## 🎉 You're Live!

Your TFT Team Builder is now on GitHub! 🚀

### Next Steps:
1. ⭐ Share the repo with friends
2. 📢 Post on social media
3. 🐛 Wait for feedback/issues
4. 🔄 Continue improving
5. 📈 Watch it grow!

---

## 💡 Pro Tips

- **Update regularly** - Keep meta data fresh
- **Engage with issues** - Respond to bug reports
- **Merge PRs** - Accept community contributions
- **Release updates** - Create GitHub releases
- **Write good docs** - Help users understand
- **Ask for feedback** - Get community input

---

## 🤝 Community Features

### Badges for Your README
```markdown
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/yourusername/tft-team-builder.svg)](https://github.com/yourusername/tft-team-builder)
[![Version](https://img.shields.io/badge/Version-2.0-blue.svg)](#)
```

### Discussion Board
Enable **Discussions** in Settings:
- Users can ask questions
- Share tips & strategies
- Suggest features
- Community help

---

## 📚 Resources

- [GitHub Docs](https://docs.github.com)
- [Git Guide](https://git-scm.com/doc)
- [Writing README](https://guides.github.com/features/wikis/)
- [Open Source Guide](https://opensource.guide)

---

## 🎊 Final Notes

You now have:
- ✅ A professional GitHub repository
- ✅ Complete documentation
- ✅ Clear contribution guidelines
- ✅ MIT licensed open source project
- ✅ Ready to share with the world

**Go forth and share your TFT Team Builder!** 🎮⚔️

---

<div align="center">

**Questions? Open an issue on your GitHub repository!**

Made with ❤️ for the TFT Community

</div>
