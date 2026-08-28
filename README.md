# Conditional deviance thresholds for low-count Poisson spectra

Simulation and saddlepoint code for *Conditional Hypothesis Testing on
Low Count Poisson Data* (M. Chockler, supervised by D. van Dyk, 2026).

## Contents
- `power_law_final.Rmd` — the complete analysis. The manifest at the top maps
  each chunk to the report figure or table it produces.
- `power_law_final.html` — the rendered notebook, so all printed numbers can be
  inspected without running anything.

## Reproducing
Requires R (rmarkdown, reticulate) and Python 3 with the packages in
`requirements.txt`. Knit with
`Rscript -e 'rmarkdown::render("power_law.Rmd")'` from a clean session.
All seeds are fixed; chunks must run in order (the single-dataset example
chunk shares the null generator). A full knit takes tens of minutes on a
laptop; the 55 ms/point timing in the report was measured on an Intel
i5-1038NG7 on mains power.

## Notes
The two 3-D surface images in the report are manual exports of the
interactive plotly figure (camera preset in the chunk); they are the only
non-scripted artefacts. Everything else is produced by the notebook.
