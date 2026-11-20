# Manuscript

This folder contains one Quarto template for an academic manuscript or analysis
report. The content is structured as a general manuscript, but you can replace
it with whatever structure your project needs.

`manuscript.qmd` supports self-contained HTML (the default) and Word output.
From the project root, render the format you need:

```sh
quarto render products/manuscript/manuscript.qmd
quarto render products/manuscript/manuscript.qmd --to docx
```

These commands create `manuscript.html` and `manuscript.docx`, respectively.
Use `--to all` to create both. Rerender after changing the source or the results
it displays. See `usage.md` at the project root for the analysis workflow.

There are no active manual page breaks in the template. A commented, escaped
page-break example in `manuscript.qmd` explains how to add them for Word output.

Most manuscripts have supplementary material. Place those files in the
`supplement/` folder, or next to the manuscript folder if that works better for
your project.

Figures, tables, and computed values should be pulled from their project
locations by code, as shown in the example.

Many journals prefer the main manuscript as a Word file and the supplement as a
PDF. You may need to adjust this based on the target journal or project.

The example manuscript includes an optional software/session information section using base R `sessionInfo()`. Keep, remove, or adapt that section depending on the journal, project, or user needs.
