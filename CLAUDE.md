# Portfolio Site - Context & Guide

**Owner:** Sakshi Vishnoi
**Theme:** Minimal Mistakes Jekyll
**Purpose:** Professional portfolio for engineering leaders and hiring managers
**Reading Time:** 5-10 minutes total

---

## Site Structure

```
├── _config.yml              # Theme config, author info, site settings
├── _data/navigation.yml     # Top menu (Home, Projects, About)
├── _pages/
│   ├── index.md            # Homepage - experience summary
│   ├── about.md            # Education, contact, tech stack
│   └── projects.md         # Projects overview
├── _projects/               # One file per company
│   ├── ninjacart.md        # 2019-2021
│   ├── shadowfax.md        # 2021-2022
│   └── gojek.md            # 2022-Present
└── Gemfile                  # Dependencies
```

---

## Content Principles

### Readability
- Break paragraphs into bullet points
- Use bold headers: **What I Did:**, **Impact:**, **Approach:**
- Add `---` between major sections
- Tech stack = one-liners only
- Keep metrics visible when mentioned (50% increase, 90% reduction)

### Length
- Company pages: 450-900 words
- Total site: readable in 5-10 minutes

### Company Page Template
```markdown
## Project Name

Brief 1-2 sentence description.

**Key Points:**
- Bullet 1
- Bullet 2

**Tech Stack:** Tool1, Tool2, Tool3

---
```

---

## Key Files

### _config.yml
```yaml
title: Sakshi Vishnoi
theme: minimal-mistakes-jekyll
minimal_mistakes_skin: "default"  # Options: air, aqua, contrast, dark, mint

author:
  name: "Sakshi Vishnoi"
  location: "Bengaluru, India"
  email: "vishsak09@gmail.com"
  links: [LinkedIn, GitHub]
```

### Front Matter
**Pages:**
```yaml
---
layout: single
title: Page Title
permalink: /url/
author_profile: true
---
```

**Projects:**
```yaml
---
layout: single
title: Company Name
period: YYYY-YYYY
---
```

---

## How to Update

### Add New Company
1. Create `_projects/company-name.md`
2. Update `_pages/projects.md` (add to list)
3. Update `_pages/index.md` (add to experience)
4. Follow template above (450-900 words)

### Edit Content
- Paragraphs >3-4 lines → break into bullets
- Always use section headers
- Keep tech stack as one-liners
- Separate sections with `---`

### Change Theme Color
Edit in `_config.yml`:
```yaml
minimal_mistakes_skin: "mint"  # or air, aqua, dark, etc.
```

---

## Local Development

```bash
bundle install
bundle exec jekyll serve
```
Visit: `http://localhost:4000`

Enable in GitHub: Settings → Pages → Source: main

Live at: `https://vishsak09.github.io`


## Quick Reference

**Contact:** `_config.yml` (author section) + `_pages/about.md`
**Navigation:** `_data/navigation.yml`
**Theme skin:** `_config.yml` → `minimal_mistakes_skin`
**Projects:** `_projects/*.md`
**Pages:** `_pages/*.md`
