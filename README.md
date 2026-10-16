# DS4I Assignment 2

Quarto report for STA5073Z Assignment 2 on writer identification with CNN
and Siamese neural networks.

## Render the website

Run the package-install command at the top of [index.qmd](index.qmd) from R,
then restart R and run the setup checks there. Run those checks from outside
the project directory (for example, with the working directory set to
Downloads) so reticulate can create its managed `r-keras` environment instead
of selecting the project's unrelated `.venv`. The report explicitly selects
`r-keras`. These one-time setup steps are not run automatically while
rendering:

```sh
quarto render
```

The generated website is written to `docs/`. Commit the generated files in that
folder along with the report source whenever you update the report. Quarto's
frozen execution is enabled to reuse results for an unchanged report; changes
to the report or data can require re-running model training before the output is
ready to publish.

## GitHub Pages

This repository uses branch-based publishing rather than GitHub Actions. In
repository Settings → Pages, choose **Deploy from a branch**, select `main` and
the `/docs` folder, and save. Push the rendered `docs/` files to `main` to
publish an update. Changes on feature branches or `dev` are not public until
they are merged into `main`.

For collaboration, work on feature branches and merge reviewed pull requests
to `dev` for validation. Merge the reviewed `dev` changes into `main` when they
are ready to publish. Render the report after merging, then commit and push the
updated `docs/` output to `main`.
