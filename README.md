# Postcards from Absurdistan

A personal blog. Built with Hugo, hosted on GitHub Pages.

---

## Setup

### Prerequisites
- [Hugo](https://gohugo.io/installation/) installed locally
- [Git](https://git-scm.com/) installed
- A GitHub account

### Local development

```bash
# Clone your repo
git clone https://github.com/Thiyaghessan/postcards-from-absurdistan.git
cd postcards-from-absurdistan

# Run local dev server (live reload)
hugo server -D

# Visit http://localhost:1313
```

### Writing a new post

```bash
hugo new content posts/my-post-title.md
```

This creates `content/posts/my-post-title.md`. Open it and edit:

```markdown
---
title: "My Post Title"
date: 2026-02-28
tags: ["singapore", "film", "macro"]
---

Your writing here...
```

Save the file. The dev server hot-reloads instantly.

### Publishing

```bash
git add .
git commit -m "new post: my post title"
git push
```

GitHub Actions builds and deploys automatically. Live in ~60 seconds.

---

## GitHub Pages setup (one-time)

1. Create a new repo on GitHub named `postcards-from-absurdistan` (or anything you like)
2. Push this folder to it
3. Go to repo **Settings → Pages**
4. Set Source to **GitHub Actions**
5. Update `baseURL` in `hugo.toml` to match your GitHub Pages URL

---

## Adding tags

Add any tags you want in the frontmatter of each post:

```markdown
tags: ["singapore", "film", "macro", "food", "observations"]
```

They appear automatically on the homepage, post pages, and the `/tags/` index.
