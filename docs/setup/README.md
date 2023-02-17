# Minimal Setup

This page contains the minimal steps to use the MKDocs Tech Docs Template. Some additional customisation is provided in [customise](customise.md). You are encouraged to read the Material for MkDocs [guidance](https://squidfunk.github.io/mkdocs-material/) for more detailed information on setting up and customisation.

## Installation

MkDocs Tech Docs template is published as a Python package and can be installed with pip, ideally by using a virtual environment. Open up a terminal and install with:

```
pip install mkdocs-tech-docs-template
```

Bootstrap your project documentation:

```
mkdocs new .
```

This creates the following structure:

```
.
├─ docs/
│  └─ index.md
└─ mkdocs.yml
```

## Configuration

Update/add the following variables to `mkdocs.yml`:

```
- site_name: <website-name>
- repo_url: <url>
- theme:
    name: tech_docs_template
```

## Preview

MkDocs includes a live preview server, so you can preview your changes as you write your documentation. The server will automatically rebuild the site upon saving. Start it with:

``` sh
mkdocs serve
```

## Publish

You can use [GitHub Actions](https://github.com/features/actions) to automate the deployment of your documentation to [GitHub Pages](https://pages.github.com/) when a commit is pushed to either the master or main branches. 

See [publishing your site](https://squidfunk.github.io/mkdocs-material/publishing-your-site/) for more details and alternatives.
