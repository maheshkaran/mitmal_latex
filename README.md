# MITMAL reusable LaTeX style

This folder contains a portable style package extracted from your current paper formatting.

## Files

- `mitmalstyle.sty`: main reusable style package
- `mitmalpackages.sty`: reusable package stack (from `packages.sty` + preamble)
- `mitmalfigures.sty`: reusable image/plot definitions (from `include/customization/*`)
- `mitcolor.sty`: MIT color palette and PGFPlots cycles used by the style

## Use in any article type

Copy these `.sty` files into the target project, then in your main `.tex` file:

```tex
\usepackage{mitmalstyle}
```

This works with classes like `article`, `report`, and `llncs`.

`splncs04.bst` is bibliography-format specific (Springer LNCS), so it is not included in the generic style package.
