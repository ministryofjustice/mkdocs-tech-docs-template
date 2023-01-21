# Introduction

!!! danger ""

    This template is under construction and should only be used for prototyping

The MkDocs Tech Docs Template is an [MkDocs theme](https://www.mkdocs.org/) that you can use to build technical documentation with a GOV.UK style. For a demo visit [mkdocs-tech-docs-template](https://ministryofjustice.github.io/mkdocs-tech-docs-template/).

The MkDocs Tech Docs Template is a python-based alternative to the ruby-based Middleman [Tech Docs Template](https://github.com/alphagov/tech-docs-template) with the following benefits:

- simple to setup, use and customise
- exploits the [MkDocs Materials theme](https://squidfunk.github.io/mkdocs-material/) and all it's associated features
- compatible with the vast and growing ecosystem of [MkDocs Plugins](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Plugins)
- unified tech stack for python-based teams and projects
- easy to upgrade as new versions of the theme are released

You’re welcome to use the MkDocs Tech Docs Template even if your service isn’t considered part of GOV.UK, but your site or service must not:

- identify itself as being part of GOV.UK
- use the crown or GOV.UK logotype in the header
- use the GDS Transport typeface
- suggest that it’s an official UK government website if it’s not

## Usage

You are encouraged to read the Material for MkDocs [getting started](https://squidfunk.github.io/mkdocs-material/getting-started/) pages before proceeding.

### Quick Start

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

### Customisation

Update/add the following variables in `mkdocs.yml`:

```
- site_name: <website-name>
- repo_url: <url>
- theme:
  - name: tech_docs_template
```

To use your department's images:

- add the images to the `docs/assets` directory in your repository
- replace the logo and favicon file name in the `mkdocs.yml` file
- consider adding the images to the template for sharing with colleagues

For additional customisation, please refer to MkDocs Material [instructions](https://squidfunk.github.io/mkdocs-material/customization/).

### Preview

MkDocs includes a live preview server, so you can preview your changes as you write your documentation. The server will automatically rebuild the site upon saving. Start it with:

``` sh
mkdocs serve
```

### Publish

You can use [GitHub Actions](https://github.com/features/actions) to automate the deployment of your documentation to [GitHub Pages](https://pages.github.com/) when a commit is pushed to either the master or main branches. 

See [publishing your site](https://squidfunk.github.io/mkdocs-material/publishing-your-site/) for more details and alternatives.

## Questions

Please raise on [Discussions](https://github.com/ministryofjustice/mkdocs-tech-docs-template/discussions).

## Contribute

👉 Find out how to [contribute](CONTRIBUTE.md).

## Licence

Unless stated otherwise, the codebase is released under [the MIT License](LICENSE).
This covers both the codebase and any sample code in the documentation.

The documentation is [© Crown copyright](http://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/) and available under the terms of the [Open Government 3.0](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) licence.
