---
hide:
  - navigation
---

# Architecture Decision Records

This section demos how to record and summarise Architecture Decision Records [(ADRs)](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions) using the MkDocs Material [tags](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags) in-built plugin.

You'll need to add a `tag` keyword to the front-matter and specify the ADR status for example:

```
---
tags: 
    - Proposed
---
```

I have associated [icons](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags#tag-icons-and-identifiers) with the ADR status tags on the `mkdocs.yml` file.

I have modified the background colors for the ADR status tags by [adding a separate style sheet](https://squidfunk.github.io/mkdocs-material/customization/#additional-css).

The tags plugin will automatically include all markdown files in the `docs` repository with a `tags` keyword. This is great because it means you don't have to list the individual ADRs in the `nav` section of the mkdocs.yml file. However it also means you cannot use non ADR-status tags, unless you use [mkdocs material Insiders](https://squidfunk.github.io/mkdocs-material/insiders/) with [scoped tags indexes](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags#+tags.tags_extra_files).
