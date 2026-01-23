# Lucas Sobral - Personal Blog

Welcome to the repository of my personal blog! This project is a high-performance, minimalist static site built to share my knowledge in Data Engineering, Software Development, and Systems Engineering.

## 🚀 Technologies

This project is built with:

- **[Astro](https://astro.build/)**: The static site generator of choice for its incredible performance and "Island Architecture".
- **Vanilla CSS**: Custom styling for full control and a unique aesthetic.
- **TypeScript**: For type safety and better developer experience.
- **MDX**: For writing content with the power of components.

## 🛠️ Usage

To run this project locally, you'll need [Node.js](https://nodejs.org/) installed.

### 1. Install Dependencies

```bash
npm install
```

### 2. Run Development Server

Start the local server to see your changes in real-time.

```bash
npm run dev
```

The site will be available at imports `http://localhost:4321`.

### 3. Build for Production

To generate the static files for deployment (e.g., to GitHub Pages):

```bash
npm run build
```

The output will be in the `dist/` folder.

## 📝 Creating Content

The blog posts are stored in `src/content/blog/`. To keep things organized, we use a folder structure based on the date:

`src/content/blog/YYYY-MM-DD/YYYY-MM-DD-slug.md`

### Frontmatter

Every post must start with a YAML frontmatter block containing metadata. Here is an example of all available fields:

```yaml
---
title: "Title of Your Post"
description: "A brief summary of what this post is about."
date: 2024-11-03 14:10:00 +0000
categories: [Data Engineering, Python]
tags: [Tutorial, GCP]
image: 
  path: "/assets/img/2024-11-03/cover.png" # Path to the cover image
---
```

### Markdown Features

You can use standard Markdown and some extended features.

#### Code Blocks

Syntax highlighting is supported out of the box.

\`\`\`python
def hello_world():
    print("Hello, World!")
\`\`\`

#### Images

Place your images inside the post folder or in `public/assets/img/`.

```markdown
![Image Description](/assets/img/YYYY-MM-DD/image.png)
_Caption (optional)_
```

#### Alerts & Callouts

You can use special syntax to create colored alert boxes:

```markdown
> This is a tip for the reader.
{: .prompt-tip }

> This is a warning!
{: .prompt-warning }

> This is a danger alert.
{: .prompt-danger }
```

## 📂 Project Structure

```text
├── public/           # Static assets (images, favicon, etc.)
├── src/
│   ├── components/   # Reusable UI components (Header, Footer, etc.)
│   ├── content/      # Blog posts and content collections
│   ├── layouts/      # Page wrappers (Layout.astro, BlogPost.astro)
│   ├── pages/        # Route definitions (index.astro, about.astro, etc.)
│   └── styles/       # Global CSS
├── astro.config.mjs  # Astro configuration
└── package.json      # Project dependencies and scripts
```
