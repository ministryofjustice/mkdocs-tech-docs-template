# Customise

This page explains the customisation used in the demo. You are encouraged to read the Material for MkDocs [guidance](https://squidfunk.github.io/mkdocs-material/) for more detailed information on customisation.

## Documentation Layout

The `nav` configuration setting in your `mkdocs.yml` file defines which pages are included in the global site navigation menu as well as the structure of that menu.

If not provided, the navigation will be automatically created by discovering all the Markdown files in the documentation directory. See [Configure Pages and Navigation](https://www.mkdocs.org/user-guide/writing-your-docs/#configure-pages-and-navigation) for more details.

## Navigation Formatting

Tabs are disabled by default:

![No tabs](no_tabs.png)

To enable tabs and use the same navigation structure as displayed in the demo update the `mkdocs.yml` as follows:
```
theme:
    features:
        - navigation.tabs
        - navigation.tabs.sticky
        - navigation.indexes
```

You can hide the navigation and contents page on individual pages using the front matter:

```
---
hide:
  - navigation
  - toc
---

# MkDocs Tech Docs Template

```

Please refer to [setting up navigation](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/) for more details.

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

## Social links

Social links are rendered above the copyright notice as part of the 
footer of your project documentation. Add a list of social links in `mkdocs.yml` 
with:

``` yaml
extra:
  social:
    - icon: fontawesome/brands/mastodon
      link: https://fosstodon.org/@squidfunk
```

Please refer to [social links](https://squidfunk.github.io/mkdocs-material/setup/setting-up-the-footer/?h=social#navigation) for more details.

## Admonitions

Admonitions, also known as call-outs, are an excellent choice for including side content without significantly interrupting the document flow. They can also be used to provide structure and coloured headings as in used on the [home](README.md) page. Please refer to [admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#admonition-icons) for more details.

## Dark Mode

Under construction!

See [Changing the colors](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/) for more details.
