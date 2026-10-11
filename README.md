# DS4I Assignment 2

Quarto report for STA5073Z Assignment 2 on writer identification with CNN
and Siamese neural networks.

## Render the website

Install the R packages and TensorFlow backend as described at the top of
[index.qmd](index.qmd), then restart R and render the Quarto website from the
repository root:

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
