# Lint Markdown post for rOpenSci blog

Lint Markdown post for rOpenSci blog

## Usage

``` r
ro_lint_md(path = NULL)
```

## Arguments

- path:

  Path to the Markdown post (not source Rmd!) – if `NULL`, and in
  RStudio, roblog will default to the md resulting from the active Rmd.

## Examples

``` r
if (FALSE) { # \dontrun{
path <- system.file(
  file.path("examples", "bad-no-alt.md"),
  package = "roblog"
)
} # }
```
