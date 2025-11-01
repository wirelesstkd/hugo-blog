# Hugo Blog Starter with PaperMod and Decap CMS

This repository contains a ready-to-run Hugo blog configured with the PaperMod theme, Decap CMS for editing posts, and a `netlify.toml` file for easy deployment on Netlify.

## Structure Overview

- `config.yaml` – site configuration specifying the PaperMod theme, menu items, social icons and parameters.
- `content/posts/` – write your blog posts here as Markdown files. A sample `first-post.md` is included.
- `content/about/` – a sample About page.
- `static/admin/` – files required for Decap CMS:
  - `index.html` – loads the Decap CMS application and Netlify Identity widget.
  - `config.yml` – defines the Git backend and how posts are managed from the CMS.
- `netlify.toml` – build settings for Netlify: runs `hugo` and publishes the `public` directory with a pinned Hugo version.

## Usage

1. Replace `YOURUSER/YOURREPO` in `static/admin/config.yml` with your GitHub username and repository name.
2. Commit this project to GitHub and connect it to Netlify. Netlify will detect the Hugo site and build it automatically using the settings in `netlify.toml`.
3. Enable Netlify Identity and Git Gateway in your Netlify dashboard (see the Decap CMS documentation for details).
4. Access the CMS at `/admin` on your live site to create and edit posts without touching the repository.

For a detailed walkthrough of integrating Decap CMS with Hugo and Netlify, refer to the official documentation.
