---
date_published: 2026-05-10
date_modified: 2026-05-10
canonical_url: https://ike.network/brand.html
---

# Powered by IKE — Brand Badge

Building on or integrating with IKE Network software? Show it with the **Powered by IKE** badge. This page has the files, the usage rules, and copy-paste snippets for your README or website.

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
| color-on-light | [svg](https://ike.network/brand/powered-by/powered-by-ike-color-on-light.svg)[1] | [png](https://ike.network/brand/powered-by/powered-by-ike-color-on-light.png)[2] | [pdf](https://ike.network/brand/powered-by/powered-by-ike-color-on-light.pdf)[3] |
| color-on-dark | [svg](https://ike.network/brand/powered-by/powered-by-ike-color-on-dark.svg)[4] | [png](https://ike.network/brand/powered-by/powered-by-ike-color-on-dark.png)[5] | [pdf](https://ike.network/brand/powered-by/powered-by-ike-color-on-dark.pdf)[6] |
| mono-on-light | [svg](https://ike.network/brand/powered-by/powered-by-ike-mono-on-light.svg)[7] | [png](https://ike.network/brand/powered-by/powered-by-ike-mono-on-light.png)[8] | [pdf](https://ike.network/brand/powered-by/powered-by-ike-mono-on-light.pdf)[9] |
| mono-on-dark | [svg](https://ike.network/brand/powered-by/powered-by-ike-mono-on-dark.svg)[10] | [png](https://ike.network/brand/powered-by/powered-by-ike-mono-on-dark.png)[11] | [pdf](https://ike.network/brand/powered-by/powered-by-ike-mono-on-dark.pdf)[12] |

Or download everything as a pack: [powered-by-ike-original-pack.zip](https://ike.network/brand/powered-by/powered-by-ike-original-pack.zip)[13].

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

The badge is provided for projects, products, and pages that build on or integrate with IKE Network software. Display it to indicate that relationship, and link it back to [https://ike.network](https://ike.network)[14].

Keep it legible and unmodified:

- Do **not** recolor, restyle, or change the gradient
- Do **not** rotate, skew, distort, or change the proportions
- Do **not** add effects (shadows, glows, outlines) or change transparency
- Do **not** alter or substitute the wordmark or typeface
- Do **not** crop the pill or remove the "POWERED BY" lockup

Give the badge room to breathe: leave clear space around it equal to at least half its height. Minimum size is **20 px** tall on screen (24–32 px is typical); **6 mm** in print.

Need a different lockup, format, or color treatment? Email [info@ike.network](mailto:info@ike.network)[15].

## [#color-reference](#color-reference)Color reference

The pill gradient runs horizontally, Blush → Drift:

| Stop | Hex | Position |
| --- | --- | --- |
| Blush (start) | `#F4BFB9` | left |
| Drift (end) | `#C98CEC` | right |
