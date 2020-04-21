# Sample Collobrative Publishing with Github and Markdown

This is a simple repo that illustrates how to use Github as a collobrative publishing tool. 

The basic premise is that it's easy to convert Markdown files to a Github Page site, `github.io` site, through Github's Jekyll integration. 

## Pages 
Github will autoamtically serve an `index.md` or `README.md` at `github.io/{repo name}`. Any other Markdown file will be automatically converted to HTML. 

The site's url structure will mirror the page URL structure so [folders](folder/example.html) and [pages](page.html) are supported.

## PRs
Since all of the pages on the site are just Markdown, any changes to the published pages can be made via Github's standard PR process. This can be helpful to manage changes to site in an open transparent way.

## Setup  

1. Create a Github repo
2. Add a `_config.yaml` file.
    A basice config file is
    ```yaml
    plugins:
    - jekyll-relative-links
    relative_links:
    enabled: true
    collections: true
    ```
3. Activate the [Github Page integration](https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site)

## Acknowldegments 

This is guide is based off [this guide](https://nicolas-van.github.io/easy-markdown-to-github-pages/)