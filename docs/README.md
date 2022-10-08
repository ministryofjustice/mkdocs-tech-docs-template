# Introduction

!!! warning "Warning" 

    This Template is under construction and should not be used for public-facing documentation

The MkDocs Tech Docs Template is an [MkDocs Template](https://www.mkdocs.org/) that you can use to build technical documentation with a GOV.UK style.

The MkDocs Tech Docs Template is an alternative to the Middleman [Tech Docs Template](https://github.com/alphagov/tech-docs-template) but with the following advantages:

- Easier to [setup and use](https://www.mkdocs.org/getting-started/)
- Uses the [MkDocs Materials theme](https://squidfunk.github.io/mkdocs-material/) and all it's associated features
- Compatible with a vast and growing ecosystem of [MkDocs Plugins](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Plugins)
- Simpler tech stack for python-based teams

You’re welcome to use the template even if your service isn’t considered part of GOV.UK, but your site or service must not:

- identify itself as being part of GOV.UK
- use the crown or GOV.UK logotype in the header
- use the GDS Transport typeface
- suggest that it’s an official UK government website if it’s not

## Usage

You are encouraged to read the MkDocs [getting started](https://www.mkdocs.org/getting-started/) pages before proceeding.

### For new repositories

This is the simplest method and more suitable for documentation-specific repositories.

Copy the template to create a new [repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)

### For existing repositories

Copy the following into the same location on your existing repository:

- `docs/assets` directory 
- `mkdocs.yml`
- `requirements-doc.txt` 

### Installation

Run the following command from the command line:

```bash
pip install -r requirements-docs.txt
```

For more details, see the MkDocs [Installation Guide](https://github.com/mkdocs/mkdocs/blob/master/docs/user-guide/installation.md).

### Preview

MkDocs includes a live preview server, so you can preview your changes as you write your documentation. The server will automatically rebuild the site upon saving. Start it with:

``` sh
mkdocs serve
```

## Contribute

👉 Find out how to [contribute](CONTRIBUTE.md).

## Licence

Unless stated otherwise, the codebase is released under [the MIT License](LICENSE).
This covers both the codebase and any sample code in the documentation.

The documentation is [© Crown copyright](http://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/) and available under the terms of the [Open Government 3.0](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) licence.
