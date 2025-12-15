# ⚡ Quick Reference Card

## 📋 File Locations

| What | Where | Edit |
|------|-------|------|
| Site Title & URL | `_config.yml` | Lines 12-20 |
| Author Info | `_config.yml` | Lines 24-45 |
| Homepage | `_pages/about.md` | All |
| CV | `_pages/cv.md` | All |
| Navigation Menu | `_data/navigation.yml` | All |
| Profile Photo | `/images/profile.png` | New file |
| Publications | `_publications/` | Add files |
| Talks | `_talks/` | Add files |
| Teaching | `_teaching/` | Add files |
| PDFs & Files | `/files/` | Add files |

## 🚀 Commands

### Test Locally
```bash
cd yejing97.github.io
bundle exec jekyll serve
# Visit http://localhost:4000
```

### Deploy to GitHub
```bash
git add .
git commit -m "Update academic profile"
git push
```

### Check Status
```bash
git status
```

## 🎯 10-Minute Setup

### 1. Open `_config.yml` and update:
```yaml
title: "Jing Ye | Academic Homepage"
name: "Jing Ye"
email: "your.email@university.edu"
employer: "Your University"
bio: "Your professional description"
github: "yejing97"
```

### 2. Add profile photo:
- Save as `/images/profile.png` (300x300px)

### 3. Edit homepage (`_pages/about.md`):
Replace sections with your information

### 4. Edit CV (`_pages/cv.md`):
Fill in education, experience, skills

### 5. Push changes:
```bash
git add .
git commit -m "Setup academic profile"
git push
```

## 📖 Documentation Files

1. **README_ACADEMIC_SETUP.md** ← START HERE
2. **SETUP_COMPLETE.md** → Detailed overview
3. **ACADEMIC_PAGE_SETUP.md** → Full guide
4. **SETUP_CHECKLIST.md** → Checklist format
5. **PUBLICATIONS_GUIDE.md** → How to add papers

## 🎨 Customization

### Change Site Theme
In `_config.yml`, line 13:
```yaml
site_theme: "default"  # or "air"
```

### Add Academic Profiles
In `_config.yml`:
```yaml
googlescholar: "https://scholar.google.com/citations?user=XXXXX"
orcid: "https://orcid.org/0000-0000-0000-0000"
arxiv: "https://arxiv.org/a/your-profile"
```

### Add Blog Post
Create file: `_posts/2024-12-15-title.md`
```markdown
---
title: "Blog Title"
date: 2024-12-15
categories: blog
---

Your content here
```

### Add Publication
Create file: `_publications/2024-12-15-short-title.md`
```markdown
---
title: "Full Paper Title"
collection: publications
category: manuscripts
date: 2024-12-15
venue: "Journal Name"
paperurl: "https://link.to.paper"
---

Your content here
```

## 🔗 Key URLs

- Your website: `https://yejing97.github.io`
- GitHub repo: `https://github.com/yejing97/yejing97.github.io`
- Edit online: GitHub web interface
- View changes: Takes 1-2 minutes after push

## ✅ Common Tasks

| Task | Steps |
|------|-------|
| Update name | `_config.yml` line 16 |
| Update email | `_config.yml` line 34 |
| Change homepage | Edit `_pages/about.md` |
| Add publication | Create in `_publications/` |
| Upload PDF | Add to `/files/` |
| Add Google Scholar | `_config.yml` line 46 |
| Change menu order | Edit `_data/navigation.yml` |
| Add blog post | Create in `_posts/` |
| Update CV | Edit `_pages/cv.md` |
| Add photo | Save `/images/profile.png` |

## 📚 Publication Format

```markdown
---
title: "Your Paper"
collection: publications
category: manuscripts
date: 2024-12-15
venue: "Journal Name"
paperurl: "link"
citation: "Your Name et al. (2024)"
---
```

## 🏗️ Directory Quick View

```
yejing97.github.io/
├── _config.yml ..................... Site config
├── _pages/
│   ├── about.md .................... Homepage
│   ├── cv.md ....................... Curriculum Vitae
│   └── publications.html ........... Publications page
├── _publications/ .................. Add papers here
├── _talks/ ......................... Add talks here
├── _teaching/ ...................... Add courses here
├── _portfolio/ ..................... Add projects here
├── _data/
│   └── navigation.yml .............. Menu
├── images/
│   └── profile.png ................. Your photo
├── files/ .......................... PDFs & docs
└── (Documentation files)
```

## 🎯 Priority Actions

```
Right now:
1. Read README_ACADEMIC_SETUP.md
2. Update _config.yml
3. Add profile photo

This week:
4. Edit homepage
5. Fill in CV
6. Add first publication

Later:
7. Add talks
8. Add teaching
9. Add projects
```

## 💡 Tips & Tricks

- **Photo size:** 300x300 pixels PNG or JPG
- **Citations:** Use format in PUBLICATIONS_GUIDE.md
- **Links:** Use relative paths `/publication/YYYY-MM-DD-title`
- **PDFs:** Upload to `/files/` and link in publications
- **Google Scholar:** Add your profile ID for auto-linking
- **Test first:** Always test locally before pushing
- **Commit messages:** Use descriptive messages
- **Update often:** Add new papers as published

## 🆘 Troubleshooting

| Problem | Solution |
|---------|----------|
| Site won't build | Check Jekyll errors in terminal |
| Changes not showing | Wait 1-2 min, hard refresh browser |
| Photo not appearing | Check filename is `profile.png` in `/images/` |
| Links broken | Use paths like `/publication/title` |
| Menu items missing | Check `_data/navigation.yml` |
| Publication not showing | Check `permalink` is unique |

## 📞 Resources

- **GitHub Pages:** https://pages.github.com
- **Jekyll:** https://jekyllrb.com
- **Academic Pages:** https://academicpages.github.io
- **Markdown Guide:** https://markdown.guide
- **YAML Syntax:** https://yaml.org

---

**Quick Summary:**
- Edit files in text editor or GitHub web interface
- Commit and push changes to GitHub
- Site updates automatically in 1-2 minutes
- Test locally with `bundle exec jekyll serve`

**Ready to start?** Begin with README_ACADEMIC_SETUP.md!
