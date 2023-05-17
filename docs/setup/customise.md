# Customise your template

This page explains the customisation used in the demo. You are encouraged to read the Material for MkDocs [guidance][material] for more detailed information on customisation.

When customising, be mindful of your users. Make sure you do not overcomplicate things for them or anyone else who might contribute to your documentation.

## Page Layout

The `nav` configuration setting in your `mkdocs.yml` file defines which pages are included in the global site navigation menu as well as the structure of that menu.

If not provided, the navigation will be automatically created by discovering all the Markdown files in the documentation directory. See [Configure Pages and Navigation][pageNav] for more details.

### Nesting pages

Parent items can either contain a single page or a nested list of child pages, but not both:

```
- Home: index.md
- Parent:
    - 'Nested Page': 'somepage.md'
    - 'Nested Parent':
        - 'Nested nested page': `someotherpage.md`
```

### Top bar navigation

Top bar navigation tabs are disabled by default. To enable them, update `mkdocs.yml` with the following:
```
theme:
    features:
        - navigation.tabs
        - navigation.tabs.sticky
        - navigation.indexes
```

### Right-hand navigation

By default, this template displays page sections on the right-hand table of contents. To merge the sections into the left-hand table of comments, in `mkdocs.yml`, uncomment `toc.integrate`.

For more information on how you can customise navigation, see [setting up navigation][navSetup].

## Logos and Images

To use your department's images you can use one of the provided [logos][logos] and [favicons][favicons] and specify the path in the `mkdocs.yml` for example:

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

## Admonitions

Admonitions, also known as call-outs, are an excellent choice for including side content without significantly interrupting the document flow. They can also be used to provide structure and coloured headings as in used on the [home page][home]. Please refer to [admonitions][admonitions] for more details. Do consider adding the images to the template for sharing with colleagues!

## Footer

### Social links

Social links are rendered above the copyright notice as part of the
footer of your project documentation. Add a list of social links in `mkdocs.yml`
with:

``` yaml
extra:
  social:
    - icon: fontawesome/brands/mastodon
      link: https://fosstodon.org/@squidfunk
```

Please refer to [social links][social] for more details.

## Dark Mode

Use the sun icon in the top bar to switch between light and dark mode.

See [Changing the colors](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/) for more details.

[material]: https://squidfunk.github.io/mkdocs-material/
[pageNav]: https://www.mkdocs.org/user-guide/writing-your-docs/#configure-pages-and-navigation
[no_tabs]: no_tabs.png
[navSetup]: https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/
[logos]: ../tech_docs_template/logos/
[favicons]: ../tech_docs_template/favicons/
[social]: https://squidfunk.github.io/mkdocs-material/setup/setting-up-the-footer/?h=social#navigation
[home]: README.md
[admonitions]: https://squidfunk.github.io/mkdocs-material/reference/admonitions/#admonition-icons
