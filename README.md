# DS4I Assignment 2

Quarto report for STA5073Z Assignment 2 on writer identification with CNN
and Siamese neural networks.

## Render locally

Install the R packages and TensorFlow backend as described at the top of
[index.qmd](index.qmd), then restart R and render the Quarto website from the
repository root:

```sh
quarto render
```

The site is written to `_site/`. Quarto's frozen execution is enabled to reuse
results for an unchanged report. Changes to the report or data can require
re-running the model training, including on the first GitHub Actions build.

## GitHub Pages

The `Render and publish Quarto website` workflow builds the report on pushes to
`main` and `dev`. Builds on `dev` validate the report but do not publish it;
only a run on `main` deploys the site to GitHub Pages. Manual runs are available
in the GitHub Actions tab, and deploy only when run against `main`. Builds on
different branches do not cancel each other. In repository Settings → Pages,
select **GitHub Actions** as the build and deployment source.

For collaboration, work on feature branches and merge reviewed pull requests
to `dev` for validation. Merge the reviewed `dev` changes into `main` when they
are ready to publish. The deployment workflow does not commit generated files
back to the repository.
