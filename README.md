# mitmal_latex

Reusable MIT-MAL LaTeX starter files.

## Included files
- `main.tex` — initial blank document
- `llncs.cls`
- `mitmalstyle.sty`
- `mitmalpackages.sty`
- `mitmalfigures.sty`
- `mitcolor.sty`

## Editorial macros (`mitmalstyle.sty`)
- `\todo{...}` / `\todoIL{...}` — inline / margin yellow notes
- `\rfc{...}` / `\rfcIL{...}` — inline / margin blue request-for-comment notes
- `\comment{color}{name}{text}` — inline note tinted `color!30`, prefixed `@name:`
- `\commentKaran{...}`, `\commentAll{...}` — shortcuts for the above

## Page layout
`llncs.cls` is patched (lines marked "Local edit") to roughly one-inch margins on US letter:
`\textwidth` 6.5in, `\textheight` 8.75in, zero side margins, `\topmargin` -0.25in.
The stock LNCS block is 12.2cm x 19.3cm with 1in + 63pt side margins.

## Build
```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

If you add a bibliography, run BibTeX as usual.
