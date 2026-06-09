---
date_published: 2026-05-10
date_modified: 2026-05-10
canonical_url: https://ike.network/brand.html
---

# Powered by IKE

The **Powered by IKE** badge marks the projects, products, and pages built on the Integrated Knowledge Exchange — and links them back to the community building it.

## [#what-it-means-to-be-powered-by-ike](#what-it-means-to-be-powered-by-ike)What it means to be Powered by IKE

IKE is a foundation of versioned knowledge graphs with pluggable formalisms. Every vertex carries STAMP coordinates — Status, Time, Author, Module, Path — so a project can say not just *what* is true, but *when* it was true, *who* asserted it, and *how* one version relates to the next. Change-sets are first-class, so work-in-progress curation and published, finalized artifacts run on the same machinery rather than bolted-on process.

It doesn’t replace the standards you already use. SNOMED, LOINC, and RxNorm carry the world’s clinical meaning but stop just short of the part a computer needs. IKE adds the layer beneath — the number, the unit, the provenance — so a code you already record becomes something a quality measure, a registry, or a model can compute, and can show its work.

Displaying the badge says your project stands on that foundation: the knowledge underneath is versioned, traceable, and shared. It is also a way for everyone building in the open to find each other.

## [#whos-building-on-ike](#whos-building-on-ike)Who’s building on IKE

A directory of projects and collaborators built on IKE. Building something on the foundation? [Tell us](mailto:info@ike.network)[1] and we’ll add you.

### [#community-and-collaborators](#community-and-collaborators)Community and collaborators

| Project | What it is |
| --- | --- |
| [komet-claude-plugin](https://github.com/knowledge-graphlet/komet-claude-plugin)[2] | In-Komet Claude assistant — read-only LLM tools that execute in-process over the live knowledge graph. Inherits `ike-parent`. |

### [#reference-projects-from-the-ike-network](#reference-projects-from-the-ike-network)Reference projects from the IKE Network

The templates new projects start from, each built on the IKE foundation:

| Project | What it is |
| --- | --- |
| [project-example](https://github.com/IKE-Network/project-example)[3] | Java + docs reference template. Inherits `ike-parent`; produces a jar plus rendered HTML and PDF. |
| [doc-example](https://github.com/IKE-Network/doc-example)[4] | Docs-only template using `ike-doc` packaging; multi-renderer PDF and HTML. |
| [workspace-reactor-example](https://github.com/IKE-Network/workspace-reactor-example)[5] | Multi-repo workspace aggregator driven by the `ws:*` orchestration goals. |

## [#the-badge](#the-badge)The badge

The badge pairs the "POWERED BY" lockup with the IKE wordmark in its signature pill. It ships in two treatments — **color** (gradient pill) and **mono** (single ink) — each in an on-light and on-dark variant.

## [#which-variant-to-use](#which-variant-to-use)Which variant to use

| Variant | Background | When to use |
| --- | --- | --- |
| `color-on-light` | Light | **Primary.** Default badge on white or light surfaces. |
| `color-on-dark` | Dark | **Primary.** The same badge for dark surfaces. |
| `mono-on-light` | Light | Single-color contexts — print, faxes, low-color UIs. |
| `mono-on-dark` | Dark | Single-color on dark surfaces. |

Prefer the **color** variants wherever the gradient will reproduce well. Fall back to **mono** only when color is unavailable.

## [#files](#files)Files

Each variant is available as `SVG` (use this on the web — sharp at any size, ~3 KB, self-contained), `PNG` (raster fallback, 5457×832), and `PDF` (vector, for print).

| Variant | SVG | PNG | PDF |
| --- | --- | --- | --- |
| color-on-light | [svg](https://ike.network/brand/powered-by/powered-by-ike-color-on-light.svg)[6] | [png](https://ike.network/brand/powered-by/powered-by-ike-color-on-light.png)[7] | [pdf](https://ike.network/brand/powered-by/powered-by-ike-color-on-light.pdf)[8] |
| color-on-dark | [svg](https://ike.network/brand/powered-by/powered-by-ike-color-on-dark.svg)[9] | [png](https://ike.network/brand/powered-by/powered-by-ike-color-on-dark.png)[10] | [pdf](https://ike.network/brand/powered-by/powered-by-ike-color-on-dark.pdf)[11] |
| mono-on-light | [svg](https://ike.network/brand/powered-by/powered-by-ike-mono-on-light.svg)[12] | [png](https://ike.network/brand/powered-by/powered-by-ike-mono-on-light.png)[13] | [pdf](https://ike.network/brand/powered-by/powered-by-ike-mono-on-light.pdf)[14] |
| mono-on-dark | [svg](https://ike.network/brand/powered-by/powered-by-ike-mono-on-dark.svg)[15] | [png](https://ike.network/brand/powered-by/powered-by-ike-mono-on-dark.png)[16] | [pdf](https://ike.network/brand/powered-by/powered-by-ike-mono-on-dark.pdf)[17] |

Or download everything as a pack: [powered-by-ike-original-pack.zip](https://ike.network/brand/powered-by/powered-by-ike-original-pack.zip)[18].

## [#use-it-in-a-readme](#use-it-in-a-readme)Use it in a README

Markdown, color-on-light (most READMEs render on white):

```
[![Powered by IKE](https://ike.network/brand/powered-by/powered-by-ike-color-on-light.svg)](https://ike.network)
```

To follow the reader’s light/dark theme automatically, use HTML with `<picture>` (GitHub honors `prefers-color-scheme` in READMEs):

```
<a href="https://ike.network">
  <picture>
    <source media="(prefers-color-scheme: dark)"
            srcset="https://ike.network/brand/powered-by/powered-by-ike-color-on-dark.svg">
    <img alt="Powered by IKE" height="28"
         src="https://ike.network/brand/powered-by/powered-by-ike-color-on-light.svg">
  </picture>
</a>
```

## [#use-it-on-a-website](#use-it-on-a-website)Use it on a website

```
<a href="https://ike.network" rel="noopener">
  <img src="https://ike.network/brand/powered-by/powered-by-ike-color-on-light.svg"
       alt="Powered by IKE" height="32">
</a>
```

Hot-linking these URLs is fine — they are served from a CDN. You may also self-host a copy.

## [#usage-rules](#usage-rules)Usage rules

The badge is provided for projects, products, and pages that build on or integrate with IKE Network software. Display it to indicate that relationship, and link it back to [https://ike.network](https://ike.network)[19].

Keep it legible and unmodified:

- Do **not** recolor, restyle, or change the gradient
- Do **not** rotate, skew, distort, or change the proportions
- Do **not** add effects (shadows, glows, outlines) or change transparency
- Do **not** alter or substitute the wordmark or typeface
- Do **not** crop the pill or remove the "POWERED BY" lockup

Give the badge room to breathe: leave clear space around it equal to at least half its height. Minimum size is **20 px** tall on screen (24–32 px is typical); **6 mm** in print.

Need a different lockup, format, or color treatment? Email [info@ike.network](mailto:info@ike.network)[1].

## [#color-reference](#color-reference)Color reference

The pill gradient runs horizontally, Blush → Drift:

| Stop | Hex | Position |
| --- | --- | --- |
| Blush (start) | `#F4BFB9` | left |
| Drift (end) | `#C98CEC` | right |
