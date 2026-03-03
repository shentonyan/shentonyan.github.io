# shentonyan.github.io

Personal website and blog of Shenton(Shentao) Yan, hosted on GitHub Pages.

🌐 **Live site:** [https://shentonyan.github.io](https://shentonyan.github.io)

---

## How to edit this site

> **Important:** This `README.md` file is **not** used to generate any page on the website.
> It is only shown here on GitHub as a repository overview.

### Edit the homepage

To update the homepage content, edit **[`index.md`](./index.md)**.
After you push your changes, GitHub Actions will automatically rebuild and redeploy the site.

### Write a new blog post

Create a new file in the **[`_posts/`](./_posts/)** folder following the naming convention:

```
_posts/YYYY-MM-DD-title-of-post.md
```

Add front matter at the top of the file:

```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD
tags: [tag1, tag2]
---

Your post content here...
```

### Dark mode

The site supports **dark / light mode** switching. A 🌙 / ☀️ toggle button is displayed in the top-right navigation bar. The selected preference is saved in the browser and will persist across page loads.

---

## Project structure

| Path | Description |
|------|-------------|
| `index.md` | **Homepage content** – edit this to update the homepage |
| `_posts/` | Blog posts (Markdown files) |
| `_layouts/` | HTML layout templates |
| `assets/css/style.css` | Site stylesheet (light + dark themes) |
| `_config.yml` | Jekyll configuration |
| `blog/index.md` | Blog listing page |
