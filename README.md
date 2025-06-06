# QuartoTemplate

This template is designed to create [quarto](https://quarto.org) projects that are deployed using [GitHub Pages](https://docs.github.com/en/pages).

## Requirements and Setup

Before using this template, ensure the following:

* ✅ **Quarto installed**: Version **1.4 or higher** is required.


## 🌐 Create Your Own Website

Follow these steps to set up and publish your Quarto-based website using GitHub Pages:

### 1. Create a New Repository

Use the template to get started: 🔗 [Create from QuartoTemplate](https://github.com/new?template_name=QuartoTemplate&template_owner=oxford-pharmacoepi)

### 📘 Post-Setup Instructions

After creating a repo from this template:

1. Go to **Settings > Pages**
2. Under "Build and deployment":
   - Choose "Deploy from a branch"
   - Select `gh-pages` as the source branch (leave `/` as the folder)
3. Save — your site will be published at: `https://organisation.github.io/repository/`

### 2. Open Locally in RStudio

Clone the repository and open the project in **RStudio**.

### 3. Set Up the Environment

Restore and update the project dependencies using `renv`:

```
renv::restore()   # Restores required packages
renv::update()    # Updates packages to avoid deployment issues
```

> 💡 Don’t forget to commit and push the updated `renv.lock` file after running `renv::update()`.

### 4. Customize Your Website

Edit the homepage using `index.qmd`.
To add new pages:

* Create additional `.qmd` files.
* Add them to the navigation in the `_quarto.yml` file.

### 5. Publishing Workflow

* ✅ **On push to `main`**: your site will be **rendered and published** to GitHub Pages.
* 🔄 **On pull requests**: your site will be **rendered for preview**, but **not published** until the PR is merged.

### 🔗 Website URL

Your published site will be available at: `https://organisation.github.io/repository/`
