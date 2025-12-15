# Guide to Adding Publications

This guide shows you how to add your publications to your academic website.

## Publication File Structure

Publications are stored in the `_publications/` directory. Each publication is a separate markdown file.

### Filename Format

```
YYYY-MM-DD-short-title.md
```

**Examples:**
- `2024-06-15-machine-learning-applications.md`
- `2023-11-20-neural-networks-survey.md`
- `2024-03-01-climate-modeling.md`

Use the **first publication date** or **acceptance date** for the date prefix.

## Publication Metadata (Frontmatter)

Every publication file starts with YAML frontmatter between `---` markers:

```markdown
---
title: "Full Title of Your Paper"
collection: publications
category: manuscripts
permalink: /publication/YYYY-MM-DD-short-title
excerpt: 'One or two sentence summary of the paper'
date: YYYY-MM-DD
venue: 'Journal Name or Conference Name'
authors: 'You, Co-Author One, Co-Author Two'
doi: '10.1234/example.doi'
paperurl: 'https://example.com/paper.pdf'
arxivurl: 'https://arxiv.org/abs/XXXX.XXXXX'
bibtexurl: 'https://example.com/bibtex.bib'
citation: 'Your Name, et al. (Year). "Paper Title." <i>Journal/Conference</i>. Volume(Issue). DOI or pages.'
---
```

## Field Descriptions

### Required Fields

| Field | Description | Example |
|-------|-------------|---------|
| `title` | Full paper title | "Machine Learning for Climate Prediction" |
| `collection` | Always use "publications" | publications |
| `category` | Type of publication | manuscripts, conferences, books |
| `permalink` | URL slug for the paper page | /publication/2024-06-15-ml-climate |
| `date` | Publication date | 2024-06-15 |
| `venue` | Journal or conference name | "Nature Machine Intelligence" |

### Optional Fields

| Field | Description | Example |
|-------|-------------|---------|
| `excerpt` | Brief summary (appears in lists) | "This paper presents a novel approach..." |
| `authors` | Co-authors | "Smith, Jane; Doe, John" |
| `doi` | Digital Object Identifier | "10.1234/example" |
| `paperurl` | Link to full PDF | "https://example.com/paper.pdf" |
| `arxivurl` | ArXiv link | "https://arxiv.org/abs/2406.12345" |
| `bibtexurl` | Link to BibTeX citation | "https://example.com/cite.bib" |
| `slides` | Link to presentation slides | "https://example.com/slides.pdf" |
| `video` | Link to talk video | "https://youtube.com/watch?v=xxxxx" |

### Publication Categories

Choose one of these for the `category` field:

- `manuscripts` - Journal articles
- `conferences` - Conference papers
- `books` - Books or book chapters
- (You can add custom categories in `_config.yml`)

## Complete Example

### File: `_publications/2024-06-15-neural-climate.md`

```markdown
---
title: "Deep Neural Networks for Global Climate Pattern Recognition"
collection: publications
category: manuscripts
permalink: /publication/2024-06-15-neural-climate
excerpt: 'This study demonstrates how convolutional neural networks can effectively identify complex climate patterns from satellite imagery with 94% accuracy.'
date: 2024-06-15
venue: 'Nature Climate Change'
authors: 'You, Jane Smith, John Doe'
doi: '10.1038/s41558-024-02000-z'
paperurl: 'https://www.nature.com/articles/s41558-024-02000-z'
arxivurl: 'https://arxiv.org/abs/2406.12345'
bibtexurl: 'https://github.com/yourname/site/files/climate_nn.bib'
citation: 'You, et al. (2024). "Deep neural networks for global climate pattern recognition." <i>Nature Climate Change</i>. 14(6), 489-495. https://doi.org/10.1038/s41558-024-02000-z'
---

## Summary

This paper presents a novel deep learning framework for analyzing global climate patterns using satellite data. We employ a customized convolutional neural network architecture specifically designed for multi-spectral climate data.

## Key Findings

- Achieved 94% accuracy in identifying El Niño patterns
- 47% faster processing compared to traditional methods
- Successfully applied to 30 years of historical climate data
- Model generalizes well to unseen geographic regions

## Methodology

We utilized:
- 10 years of MODIS satellite data
- PyTorch implementation
- GPU acceleration for training
- Cross-validation across 5 geographic regions

## Impact

This work has been cited by 42 subsequent papers in climate science and machine learning communities. The code has been made publicly available at [GitHub](https://github.com/yourname/climate-nn).

## Related Work

See also our other papers on [climate modeling](/publication/2023-11-20-climate-baseline) and [machine learning applications](/publication/2024-03-01-ml-survey).
```

## Publication Body Content

After the frontmatter, add content that will appear on the publication's detail page:

```markdown
## Introduction

Introduce the research problem and context.

## Literature Review

Summarize relevant prior work.

## Methodology

Describe your approach and methods.

## Results

Present your findings.

## Discussion

Interpret the results and implications.

## Limitations

Discuss any limitations.

## Future Work

What's next?

## References

List key citations.
```

## Adding Local PDF Files

If you have PDF files, place them in the `/files/` directory:

```
/files/
  ├── paper1.pdf
  ├── paper2.pdf
  └── slides_talk_2024.pdf
```

Then reference them in your publication:

```markdown
paperurl: 'https://yejing97.github.io/files/paper1.pdf'
```

## Citation Format Tips

Use this format for citations:

**Journal Articles:**
```
Your Name, Co-Author. (Year). "Title." <i>Journal Name</i>. Volume(Issue), pages. DOI.
```

**Conference Papers:**
```
Your Name, Co-Author. (Year). "Title." <i>Conference Name Proceedings</i>, pages. DOI.
```

**Books:**
```
Your Name. (Year). <i>Book Title</i>. Publisher. DOI or URL.
```

## Batch Adding Publications

To quickly add multiple publications:

1. Organize your publication list (title, date, venue, URL)
2. Create one markdown file per publication
3. Copy the frontmatter template and fill in details
4. Commit and push to GitHub

The site will automatically:
- Generate a publications list page
- Create individual pages for each paper
- Add to CV automatically
- Make searchable by search engines

## Organizing by Category

Publications are automatically grouped by category. Configure categories in `_config.yml`:

```yaml
publication_category:
  manuscripts:
    title: 'Journal Articles'
  conferences:
    title: 'Conference Papers'
  books:
    title: 'Books'
```

## Linking Between Publications

You can link between related publications:

```markdown
See also: [Related Paper Title](/publication/YYYY-MM-DD-short-title)
```

## Getting BibTeX Citations

Most journals provide BibTeX format:
1. Visit the journal article page
2. Look for "Export" or "Cite" option
3. Select "BibTeX"
4. Copy and save to `/files/yourname_YEAR.bib`

## Preprints on ArXiv

For papers on ArXiv before journal publication:

1. Set `arxivurl` to the ArXiv link
2. Keep `paperurl` pointing to final published version
3. Update `date` to journal publication date (not ArXiv date)
4. Both links will display on the paper page

## Publishing Schedule

- **Preprint**: Add to site immediately (with arxivurl)
- **Published**: Update with final venue and DOI
- **In Press**: Include publication date when known
- **Under Review**: Optional to include (mark clearly if doing so)

---

**Tips:**
- Keep the excerpt brief and compelling
- Always include the original publication date
- Link to publicly available versions when possible
- Update citations in your CV to match

