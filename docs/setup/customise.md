# Customise your template

This page explains the different components we use to configure page layout for the demo site you are currently viewing. You can apply these to your template to make your site look similar. 

When customising, keep your users in mind. The template is flexible, but try not to complicate things for readers, or anyone contributing to your documentation.

For more information on customisation, see the [Material for MkDocs guidance][material].

## Page Layout

The `nav` setting in your `mkdocs.yml` file defines which pages to include in your table of contents and their structure.

If you do not define `nav`, the template automatically search for Markdown files in the docs directory and creates a table of contents. For more information on how this works, see the [MkDocs documentation on configuring pages and navigation][pageNav].

### Nesting pages

Parent items can contain a single page or a nested list of child pages, but not both:

```
nav:
- Home: index.md
- Parent:
    - 'Nested Page': 'somepage.md'
    - 'Nested Parent':
        - 'Nested nested page': `someotherpage.md`
```

### Top bar navigation

Top bar navigation tabs do not display by default. To display them, update `mkdocs.yml` with the following:
```
theme:
    features:
        - navigation.tabs
        - navigation.tabs.sticky
        - navigation.indexes
```

### Right-hand navigation

By default, this template displays page sections on the right-hand table of contents. To merge the sections into the left-hand table of comments, add `toc.integrate` in `mkdocs.yml`:

```
theme:
    features:
        - toc.integrate
```

For more information on how you can customise navigation, see the [Material for MkDocs documentation on setting up navigation][navSetup].

## Logos and Images

To use government images on your site you can use one of the provided [logos][logos] and [favicons][favicons] and specify the path in `mkdocs.yml`, for example:

```
theme:
    logo: logos/moj.png
    favicon: favicons/moj.ico             
```

Alternatively, you can add images to the `docs/assets` directory in your own repository and specify the path, for example:

```
theme:
    logo: assets/ho_logo.png
    favicon: assets/ho_icon.ico             
```

## Admonitions

[Admonitions][admonitions] (also known as call-outs) are a way of including content without interrupting the flow of your content. They can also help to provide structure and coloured headings, such as those on the [homepage][home].

## Social links

Social links are rendered above the copyright notice as part of the footer of your project documentation. Add a list of social links in `mkdocs.yml` using the following:
with:

``` yaml
extra:
  social:
    - icon: fontawesome/brands/mastodon
      link: https://fosstodon.org/@squidfunk
```

Please refer to [social links][social] for more details.

## Dark Mode (experimental)

To enable Dark Mode, add the following in `mkdocs.yml`

```
palette: 
    # Palette toggle for light mode
    - scheme: default
      toggle:
        icon: material/brightness-7 
        name: Switch to dark mode
    # Palette toggle for dark mode
    - scheme: slate
      toggle:
        icon: material/brightness-4
        name: Switch to light mode
```

Use the sun icon in the top bar to switch between light and dark mode.

[material]: https://squidfunk.github.io/mkdocs-material/
[pageNav]: https://www.mkdocs.org/user-guide/writing-your-docs/#configure-pages-and-navigation
[no_tabs]: no_tabs.png
[navSetup]: https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/
[logos]: ../govuk_mkdocs_material/logos/
[favicons]: ../govuk_mkdocs_material/favicons/
[social]: https://squidfunk.github.io/mkdocs-material/setup/setting-up-the-footer/?h=social#navigation
[home]: README.md
[admonitions]: https://squidfunk.github.io/mkdocs-material/reference/admonitions/#admonition-icons
