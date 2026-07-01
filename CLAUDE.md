# ike-network-site

Source for the **ike.network** organization website — the landing page
and per-project site chrome published by `mvn ike:site-publish`
(`OrgSiteSupport` in ike-maven-plugin regenerates the org-root landing
from a fresh clone; project sub-sites deploy to gh-pages). Authored pages
live in `src/site/asciidoc/`; shared assets in `src/site/resources/`.

Diagram source (GraphViz) for the site diagrams is kept in
`src/site/diagrams/`; the rendered static SVGs live in
`src/site/resources/images/` and are referenced with `image::`.

<!-- BEGIN ike-managed: standards-pointer -->

## IKE Build Standards

This project follows the IKE build standards. Run `mvn validate` to
unpack them into `.claude/standards/` — build artifacts from
`ike-build-standards`, so **do not edit or commit them** — then read and
follow them (start with `MAVEN.md` and `IKE-MAVEN.md`).

Diagrams on web pages (`src/site/asciidoc/`) follow `IKE-DIAGRAMS.md`:
pre-render to committed static SVG under `src/site/resources/images/` and
reference with `image::` — never inline `[plantuml]`/`[graphviz]` blocks
or live Kroki URLs (the Maven site parser does not render them).
<!-- END ike-managed: standards-pointer -->
