# Final report

LaTeX source of the COMP 4062 final report. Builds to `main.pdf`.

```bash
cd report
latexmk -pdf main.tex
```

CI (`.github/workflows/latex-build.yml`) builds it on every push and uploads the PDF as the `report` artifact.

- Format follows the course rules (they override the CVPR template): letter paper, 12-pt Times, double spaced, 3/4" margins, 20 pages max.
- `main.tex` holds the title page fields; each section lives in `sec/`.
- `\TODO{...}` marks prose still to write. Uncomment the `\renewcommand{\TODO}` line in `preamble.tex` before submitting to hide any left over.
