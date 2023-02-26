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

The tags plugin will automatically include all markdown files in the `docs` repository with a `tags` keyword. This is great because it means you don't have to list the ADRs in the `nav` section of the mkdocs.yml file. However it means you cannot use non ADR-status tag values. With mkdocs-insiders it is possible to limit to markdown pages with [specified tags](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags#:~:text=tags%20index%20page.-,tags_extra_files,-insiders%2D4.20.0%20%C2%B7) only.
