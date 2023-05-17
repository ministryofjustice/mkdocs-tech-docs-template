# ADR Template

Architectural Decision Records (ADRs) provide a way for project teams to record each decision they make for their product. Well written ADRs provide an incremental view of a product’s development and improvements to user experience along the way.

[The GDS Way provides some guidelines][gds_way] for writing ADRs. This section shows how to record and summarise Architecture Decision Records using the [tags][tags_plugin] plugin, which is included with the MKDocs Tech Docs Template.

In the front matter of your page, add a `tag` keyword and specify a status. For example:

```
---
tags:
    - Proposed
---
```
The tags plugin will automatically include all markdown files in the `docs` repository with a `tags` keyword. This is great because it means you don't have to list the ADRs in the `nav` section of the mkdocs.yml file.

However, it also means you cannot use non ADR-status tags, unless you use mkdocs-insiders with [scoped tags indexes][scoped_tags].

You can also associate [icons][icons] with the ADR status tags in `mkdocs.yml`:

```
extra:
  tags:
    Draft: draft
    Accepted: accepted
    Proposed: proposed
    Superseded: superseded
    Deprecated: deprecated
    Rejected: rejected
```

Now, each page with one of these tags in its front matter will display with the associated icon.

[gds_way]: https://gds-way.cloudapps.digital/standards/architecture-decisions.html#documenting-architecture-decisions
[tags_plugin]: https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags
[scoped_tags]: https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags#+tags.tags_extra_files
[icons]: https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/?h=tags#tag-icons-and-identifiers
