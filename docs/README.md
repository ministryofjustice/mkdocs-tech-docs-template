# Introduction

!!! danger ""

    This template is under construction and should only be used for prototyping

The MkDocs Tech Docs Template is an [MkDocs Template](https://www.mkdocs.org/) that you can use to build technical documentation with a GOV.UK style. For a demo visit [mkdocs-tech-docs-template](https://ministryofjustice.github.io/mkdocs-tech-docs-template/).

The MkDocs Tech Docs Template is a python-based alternative to the ruby-based Middleman [Tech Docs Template](https://github.com/alphagov/tech-docs-template) with the following benefits:

- simple to setup, use and customise
- uses the [MkDocs Materials theme](https://squidfunk.github.io/mkdocs-material/) and all it's associated features
- compatible with the vast and growing ecosystem of [MkDocs Plugins](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Plugins)
- unified tech stack for python-based teams

You’re welcome to use the template even if your service isn’t considered part of GOV.UK, but your site or service must not:

- identify itself as being part of GOV.UK
- use the crown or GOV.UK logotype in the header
- use the GDS Transport typeface
- suggest that it’s an official UK government website if it’s not

## Usage

You are encouraged to read the MkDocs [getting started](https://www.mkdocs.org/getting-started/) pages before proceeding.

### For new repositories

This is the simplest method and more suitable for documentation-specific repositories.

Copy the template to create a new [repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

### For existing repositories

Copy the following into the same location on your existing repository:

- `docs/assets` 
- `mkdocs.yml`
- `requirements-doc.txt`
- `.github/workflows/gh-deploy.yml`

### Customisation

Update the following variables in `mkdocs.yml`:

- site_name
- repo_url

The template is configured to use the MOJ logo and favicon. To use your department's images:

- add the images to the `docs/assets` directory in your repository
- replace the logo and favicon file name in the `mkdocs.yml` file
- consider adding the images to the template for sharing with colleagues

For additional customisation, please refer to MkDocs Material [instructions](https://squidfunk.github.io/mkdocs-material/customization/).

### Installation

Run the following command from the command line:

``` sh
pip install -r requirements-docs.txt
```

For more details, see the MkDocs [Installation Guide](https://github.com/mkdocs/mkdocs/blob/master/docs/user-guide/installation.md).

### Preview

MkDocs includes a live preview server, so you can preview your changes as you write your documentation. The server will automatically rebuild the site upon saving. Start it with:

``` sh
mkdocs serve
```

### Publish

The template uses [GitHub Actions](https://github.com/features/actions) to automate the deployment of your documentation to [GitHub Pages](https://pages.github.com/) when a commit is pushed to either the master or main branches. 

See [publishing your site](https://squidfunk.github.io/mkdocs-material/publishing-your-site/) for more details and alternatives.

## Questions

Please raise on [Discussions](https://github.com/ministryofjustice/mkdocs-tech-docs-template/discussions).

## Contribute

👉 Find out how to [contribute](CONTRIBUTE.md).

## Licence

Unless stated otherwise, the codebase is released under [the MIT License](LICENSE).
This covers both the codebase and any sample code in the documentation.

The documentation is [© Crown copyright](http://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/) and available under the terms of the [Open Government 3.0](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) licence.
