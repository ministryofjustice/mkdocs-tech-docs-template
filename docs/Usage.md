# Usage

This page contains the minimal steps to use the MKDocs Tech Docs Template. You are encouraged to read the Material for MkDocs [guidance](https://squidfunk.github.io/mkdocs-material/) for more detailed information on setting up and customisation.

## Setup

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

## Logos and Images

To use your department's images you can use one of the provided [logos](../tech_docs_template/logos/) and [favicons](../tech_docs_template/favicons/) and specify the path in the `mkdocs.yml` for example:

```
theme:
    logo: logos/moj.png
    favicon: favicons/moj.ico             
```

Alternatively you can add the images to the `docs/assets` directory in your own repository and specify the path for example:

```
theme:
    logo: assets/ho_logo.png
    favicon: assets/ho_icon.ico             
```

Do consider adding the images to the template for sharing with colleagues!

## Site Navigation

To use the same navigation structure as displayed in the demo update the `mkdocs.yml` as follows:
```
theme:
    features:
        - navigation.tabs
        - navigation.tabs.sticky
        - navigation.indexes
```

Please refer to [setting up navigation](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/) for alternate navigation structures.

## Preview

MkDocs includes a live preview server, so you can preview your changes as you write your documentation. The server will automatically rebuild the site upon saving. Start it with:

``` sh
mkdocs serve
```

## Publish

You can use [GitHub Actions](https://github.com/features/actions) to automate the deployment of your documentation to [GitHub Pages](https://pages.github.com/) when a commit is pushed to either the master or main branches. 

See [publishing your site](https://squidfunk.github.io/mkdocs-material/publishing-your-site/) for more details and alternatives.
