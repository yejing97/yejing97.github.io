# Academic Page Customization Checklist

## Essential Setup (Do First!)

- [ ] Update `_config.yml`:
  - [ ] Site title with your name
  - [ ] URL with your GitHub username
  - [ ] Author name and email
  - [ ] Professional bio
  - [ ] Institution/employer name

- [ ] Add profile picture:
  - [ ] Create professional headshot
  - [ ] Save as `/images/profile.png` (300x300px)
  - [ ] Verify `avatar: profile.png` in `_config.yml`

- [ ] Update homepage (`_pages/about.md`):
  - [ ] Replace research interests
  - [ ] Update professional background
  - [ ] Personalize about section

## Academic Profiles (Highly Recommended)

- [ ] Google Scholar link
- [ ] ORCID identifier
- [ ] GitHub profile link
- [ ] LinkedIn profile (optional)
- [ ] ArXiv profile (if applicable)

## Content Pages

### CV (`_pages/cv.md`)
- [ ] Add education details (degrees, institutions, years)
- [ ] Add work experience
- [ ] List technical and research skills
- [ ] List professional service roles

### Publications (`_publications/`)
- [ ] Remove placeholder publications
- [ ] Add your actual publications
- [ ] Include paper URLs and citations
- [ ] Organize by category (manuscripts, conferences, etc.)

### Talks (`_talks/`)
- [ ] Add conference presentations
- [ ] Add seminar talks
- [ ] Include dates and venues
- [ ] Link to slides if available

### Teaching (`_teaching/`)
- [ ] List courses taught
- [ ] Include terms and levels
- [ ] Add course descriptions

### Portfolio (`_portfolio/`)
- [ ] Add research projects
- [ ] Include datasets
- [ ] Add project descriptions and links

## Final Polish

- [ ] Add CV PDF to `/files/cv.pdf`
- [ ] Test site locally with `bundle exec jekyll serve`
- [ ] Check all links are working
- [ ] Verify contact information is correct
- [ ] Review mobile appearance
- [ ] Enable Google Scholar/academic profile links

## Publishing

- [ ] Push changes to GitHub
- [ ] Verify site updates at https://yejing97.github.io
- [ ] Monitor for any build errors in GitHub Actions

---

**Quick Start Example:**

After creating your profile, your homepage should look like:
1. Professional photo (left sidebar)
2. Your name and title
3. Your bio and research interests
4. Links to all your academic content
5. Easy navigation to Publications, CV, Talks, Teaching, etc.

