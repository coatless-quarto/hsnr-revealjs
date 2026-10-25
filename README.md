# HSNR-themed Revealjs Extension For Quarto

A [quarto extension](https://quarto.org/docs/extensions/) featuring an HSNR-inspired theme for the [reveal.js format](https://quarto.org/docs/presentations/revealjs/).

See the included [template.qmd](template.qmd) file for an example of the theme and integration into Quarto or explore the rendered version [here](http://quarto.thecoatlessprofessor.com/hsnr-revealjs/).

For details on how to convert from a single-themed document into a Quarto Extension for RevealJS see [PR #1](https://github.com/coatless-quarto/hsnr-revealjs/pull/1)

## Installing

To start a new presentation from the template, use:

```bash
quarto use template coatless-quarto/hsnr-revealjs
```

This will install the extension and create an example qmd file that
you can use as a starting place for your presentation slides.

To add the extension to an existing project without the example slides, use:

```bash
quarto add coatless-quarto/hsnr-revealjs
```

## Using

Once the extension is installed, you can use the extension by setting the `format` inside of the document header to `hsnr-revealjs`.

```markdown
---
title: A title
subtitle: A subtitle
format:
  hsnr-revealjs: default
author:
  - name: Your Name
    orcid: 0000-0000-0000-0000
    email: alias@email.com
    affiliations: Your Institution
date: last-modified
---
```

### Changing the footer and language

The format sets a placeholder footer ("Prof. Dr. Theo Rethisch | Fachbereich 10 | Hochschule Niederrhein") and German as the document language (`lang: de`). You can override both in your document header:

```markdown
---
title: A title
lang: en
format:
  hsnr-revealjs:
    footer: "Your Name | Your Department | Your Institution"
---
```

`lang` sets the language of the page and of Quarto's built-in labels, such as callout titles ("Note" in place of "Hinweis"). To leave the footer empty, use `footer: ""`.

## Acknowledgements

This theme was developed as a result of answering a question asked by [Joe Slam](https://github.com/produnis) on the [Quarto issue tracker (#7470)](https://github.com/quarto-dev/quarto-cli/issues/7470#issuecomment-1875929330).

