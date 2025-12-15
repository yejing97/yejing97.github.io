# Academic Personal Page Setup Guide

Welcome! Your academic personal website has been configured with a professional template. Here's what has been set up and what you need to customize next.

## ✅ Completed Setup

### 1. **Site Configuration** (`_config.yml`)
- Site title updated to "Jing Ye | Academic Homepage"
- Site URL: `https://yejing97.github.io`
- Repository: `yejing97/yejing97.github.io`
- Author name, email, and GitHub profile configured

### 2. **Homepage** (`_pages/about.md`)
- Professional academic homepage created
- Sections included:
  - About Me
  - Research Interests
  - Professional Background
  - Navigation links to key pages

### 3. **Curriculum Vitae** (`_pages/cv.md`)
- Education section with template entries
- Work experience section with professional roles
- Skills section for technical and professional skills
- Automated displays of publications, talks, and teaching
- Service and leadership section

### 4. **Publications Page** (`_pages/publications.html`)
- Professional publications listing
- Link to Google Scholar (when configured)
- Organized by publication category
- Example publication updated with proper structure

### 5. **Navigation Menu** (`_data/navigation.yml`)
- Optimized menu structure:
  - Home
  - Publications
  - Talks
  - Teaching
  - CV
  - Blog Posts
  - Portfolio

## 📝 Next Steps: What You Need to Customize

### Priority 1: Personal Information

1. **Update `_config.yml` with your details:**
   ```yaml
   title: "Your Name | Academic Homepage"
   name: &name "Your Full Name"
   
   author:
     bio: "Your professional bio"
     location: "Your location"
     employer: "Your institution/company"
     email: "your.email@institution.edu"
   ```

2. **Add your academic profiles** (in `_config.yml`):
   - `googlescholar`: Link to your Google Scholar profile
   - `orcid`: Your ORCID identifier
   - `arxiv`: Your ArXiv profile (if applicable)
   - `github`: Your GitHub username
   - `linkedin`: Your LinkedIn profile
   - Other relevant academic profiles

3. **Replace social media links:**
   - Twitter, LinkedIn, Instagram, etc. (leave blank if not applicable)

### Priority 2: Homepage Content (`_pages/about.md`)

Replace placeholder text with:
- Your actual research interests and areas
- Your background and expertise
- Your research goals and impact
- Personal touch and professional summary

### Priority 3: CV Content (`_pages/cv.md`)

Fill in your actual information:
- **Education**: Your degrees, institutions, years
- **Work experience**: Jobs, institutions, supervisors
- **Skills**: Technical, research, and professional skills
- Service and leadership roles

### Priority 4: Profile Picture

1. Add your professional photo:
   - Place image at `/images/profile.png` (or `.jpg`)
   - Size: 300x300 pixels recommended
   - File name should match `avatar` in `_config.yml`

### Priority 5: Publications

1. **Add your publications** to `_publications/` directory:
   - Copy the existing template file
   - Update the filename with date (YYYY-MM-DD-short-title.md)
   - Fill in proper metadata (title, venue, date, authors, links)
   - Add paper URL and preprint links

2. **Publication frontmatter example:**
   ```markdown
   ---
   title: "Your Paper Title"
   collection: publications
   category: manuscripts  # or conferences, books
   permalink: /publication/2024-01-01-paper-title
   excerpt: 'Brief description of your work'
   date: 2024-01-01
   venue: 'Journal or Conference Name'
   paperurl: 'https://link-to-your-paper.pdf'
   citation: 'Your Name, et al. (2024). "Title" Journal/Conference'
   ---
   ```

### Priority 6: Talks and Presentations

1. Add talks to `_talks/` directory with similar structure
2. Include conference presentations, seminars, and keynotes
3. Optionally add slides and video links

### Priority 7: Teaching

1. Add courses to `_teaching/` directory
2. Include course number, term, level, and description

### Priority 8: PDF Files

Place important documents in `/files/`:
- CV (PDF)
- Research papers
- Presentation slides
- Any other academic documents

These will be accessible at: `https://yejing97.github.io/files/filename.pdf`

## 🚀 Local Testing

To preview your site locally:

```bash
# Install dependencies (first time only)
bundle install

# Start Jekyll server
bundle exec jekyll serve

# Visit http://localhost:4000 in your browser
```

## 📚 Publishing Changes

Once you've made edits:

```bash
git add .
git commit -m "Update academic profile with personal information"
git push
```

GitHub Pages will automatically rebuild your site. Changes typically appear within 1-2 minutes.

## 🎨 Additional Customization Options

### Themes
- Site theme options: "default" or "air" (modify in `_config.yml`)

### Blog Posts
- Add posts to `_pages/year-archive.html`
- Blog posts go in `_posts/` directory

### Portfolio Projects
- Add project showcases to `_portfolio/` directory
- Display with images and descriptions

### Contact Page
- You can add a contact section to your homepage or create dedicated page

## 📖 Resources

- **Academic Pages**: https://academicpages.github.io/
- **Jekyll Documentation**: https://jekyllrb.com/
- **Markdown Guide**: https://www.markdownguide.org/
- **YAML Syntax**: https://yaml.org/start.html

## ✨ Tips for Success

1. **Keep it updated**: Regularly update your publications, talks, and CV
2. **Use consistent formatting**: Follow the templates for all publications
3. **Add descriptions**: Include meaningful excerpts for each publication
4. **Professional photo**: Use a clear, professional headshot
5. **Contact info**: Make it easy for people to reach out for collaboration
6. **Search optimization**: Google Scholar and ArXiv links help with discoverability

---

**Enjoy your new academic website!** This template provides a professional, maintainable platform for showcasing your research and academic work.
