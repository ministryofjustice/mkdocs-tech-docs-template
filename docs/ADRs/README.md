---
hide:
  - navigation
---

# Architecture Decision Records

This section demos how to record and summarise Architecture Decision Records [(ADRs)](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions) using the MkDocs Material [tags](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags) in-built plugin.

You'll need to add a `tag` keyword to the front-matter and specify the status for example:

```
---
tags: 
    - Proposed
---
```

You can associate [icons](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags#tag-icons-and-identifiers) with the ADR status tags on the `mkdocs.yml` file.

The tags plugin will automatically include all markdown files in the `docs` repository with a `tags` keyword. This is great because it means you don't have to list the ADRs in the `nav` section of the mkdocs.yml file. However it also means you cannot use non ADR-status tags, unless you use mkdocs-insiders with [scoped tags indexes](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags#+tags.tags_extra_files).
