# Quickstart guide

This page provides a guide on how to configure the MKDocs Tech Docs Template. In a few simple steps, you can begin building your documentation site.

## Before you begin

In order to use the MKDocs Tech Docs Template, you require the following:

- a device with permissions to install new packages
- Python 3 and Pip installed on your device
- GitHub account with [a configured SSH key][gh_ssh]
- GitHub repository to store your documentation (see [GitHub's documentation][gh_newRepo] for instructions)

You should also be comfortable writing content in Markdown, and using the Git workflow to push your changes to a repository.

## Install MKDocs TDT

The MkDocs TDT publishes as a Python package, so you can use pip to install it. In your terminal, navigate to the directory you want to install the template and run the following:

```
pip install mkdocs-tech-docs-template
```

Next, bootstrap your project documentation:

```
mkdocs new .
```

This creates the following structure in the directory:

```
.
├─ docs/
│  └─ index.md
└─ mkdocs.yml
```

## Update mkdocs.yml

So that the template displays properly, in `mkdocs.yml` insert the relevant values for `site_name` and `repo_url`, and set the `theme` so that it uses our MKDocs tech docs template:

```
- site_name: <your-website-name>
- repo_url: <your-website-url>
- theme:
    name: tech_docs_template
```

## Preview your documentation

MkDocs includes a live preview server that automatically rebuilds when you save a file, so you can preview your changes as you write. To start the server, in your terminal run:

```
mkdocs serve
```

To stop the server, in your terminal press Ctrl+C. If the page stops loading, check your terminal: an error may have occurred you need to fix before you can restart the server.

## Build your documentation

You can use [GitHub Actions](https://github.com/features/actions) to automate the deployment of your documentation to [GitHub Pages](https://pages.github.com/) when a commit is pushed to either the master or main branches. See [publishing your site](https://squidfunk.github.io/mkdocs-material/publishing-your-site/) for more details and alternatives.

## Customise your documentation

We have provided some customisation options in [customise](customise.md), but we encourage you to read the [Material for MkDocs guidance][material] for more detailed information on customisation.

[gh_newRepo]: https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository
[gh_ssh]: https://docs.github.com/en/authentication/connecting-to-github-with-ssh
[material]: https://squidfunk.github.io/mkdocs-material/
