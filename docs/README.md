---
title: GOVUK MkDocs Material
hide:
- navigation
- toc
---

<style>
  .md-typeset h1 {
    display: none;
  }
  
  .md-main__inner {
    margin-top: 0px;
  }

  .md-content__button {
    display: none;
  }
</style>

!!! banner "Build flexible documentation"

    ![Services][homepage_illustration]{ align=right width=300px height=300px}

    The **GOVUK MkDocs Material** is a Python-based alternative to the Ruby-based [Tech Docs Template][TDT] with the following benefits:

    - easy to [set up][setup], [customise][customise] and [enhance][contribute]
    - adapts the [MkDocs Materials theme][material] to follow the [GOV.UK style][gov-uk]
    - compatible with the vast ecosystem of [MkDocs plugins][plugins]
    - unified tech stack for Python-based projects

    [Get Started ＞][setup]{ .md-button .md-button--primary}

!!! warning inline end "Prototype"

    This template is under construction. As it has not yet passed an accessibility audit, we currently do not recommend using it.

!!! quote "Restrictions"

    You can use GOVUK MkDocs Material even if your documentation site is not part of GOV.UK, but it must not:

    - identify itself as part of GOV.UK
    - use the crown or GOV.UK logotype in the header
    - use the GDS Transport typeface
    - say or suggest that it is an official UK government website

<br>

[gov.ukStyle]: https://design-system.service.gov.uk/
[homepage_illustration]: homepage-illustration.svg
[TDT]: https://tdt-documentation.london.cloudapps.digital/
[setup]: ./setup/
[customise]: ./setup/customise.md
[contribute]: ./setup/CONTRIBUTE.md
[material]: https://squidfunk.github.io/mkdocs-material/
[plugins]: plugins/
[gov-uk]: https://design-system.service.gov.uk/
