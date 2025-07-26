---
title: "How I Built This Site with Hugo, GitHub, and Netlify — For Free"
date: 2025-07-26
tags: ["hugo", "netlify", "github", "static sites", "guide"]
categories: ["tech", "how-to"]
draft: false
---

Building this site — **Pingryte** — cost me exactly £0. Here's how.

## 🛠️ The Stack

- **Hugo** – A lightning-fast static site generator.
- **PaperMod** – A clean, minimal Hugo theme with no fluff.
- **GitHub** – Free repo hosting + version control.
- **Netlify** – Free continuous deployment and global CDN.

## 🚀 Why I Chose This Setup

I didn’t want WordPress, Wix, or anything bloated. I wanted:
- Full control over my content
- No recurring fees
- Speed, minimalism, and flexibility

This stack checked every box.

## 🔧 Step-by-Step Setup

### 1. Install Hugo

```bash
brew install hugo
```

> Note: If you're not on macOS, [check Hugo's install guide](https://gohugo.io/getting-started/installing/).

---

### 2. Create the site

```bash
hugo new site pingryte-site
cd pingryte-site
```

---

### 3. Add the PaperMod theme

```bash
git init
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

Then update `config.yml` (or `config.toml`) to set the theme:

```yaml
theme: PaperMod
```

---

### 4. Add content

```bash
hugo new posts/my-first-post.md
```

Edit the generated file in `content/posts/` and set `draft: false`.

---

### 5. Serve it locally

```bash
hugo server
```

Then visit `http://localhost:1313`.

---

### 6. Push to GitHub

```bash
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/your-username/pingryte-site.git
git push -u origin main
```

---

### 7. Deploy to Netlify

- Go to [Netlify](https://netlify.com)
- Connect your GitHub repo
- Set build command to `hugo`
- Set publish directory to `public`

Netlify will auto-deploy on every push.

---

## 🧠 Final Thoughts

- Hosting is free
- Deployment is automatic
- Load times are blazing fast
- No plugins, no maintenance, no nonsense

Got questions or want help setting this up? [Email me](mailto:mail@pingryte.com) — or just steal this site structure and make it yours.

---

Pingryte is about practical tech and automation — no fluff. Subscribe via RSS or check back for more posts like this.