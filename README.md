# QuartoTemplate

This template is designed to create [`quarto`](https://quarto.org) projects that are deployed using **GitHub Pages**(https://docs.github.com/en/pages).

## Requirements and Setup

Before using this template, ensure the following:

* ✅ **Quarto installed**: Version **1.4 or higher** is required.
* ✅ **GitHub Pages is configured**:
  You can do this either:

  * Using R: `usethis::use_github_pages()` [^github_pat]
 
  * Manually: Create the `gh-pages` branch, and go to your repository’s Pages settings (https://github.com/organisation/repository/settings/pages) to configure deployment from `gh-pages` branch.
  
* ✅ **GitHub Actions has write permissions**:
  Go to Actions settings (https://github.com/organisation/repository/settings/actions) and ensure that under *Workflow permissions* **Read and write permissions** is selected.

[^github_pat]: Make sure Git is configured and `GITHUB_PAT` is set up beforehand.
