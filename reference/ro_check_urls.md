# Check URLs in Markdown post

Check URLs in Markdown post

## Usage

``` r
ro_check_urls(path = NULL)
```

## Arguments

- path:

  Path to the Markdown post (not source Rmd!) – if `NULL`, and in
  RStudio, roblog will default to the md resulting from the active Rmd.

## Examples

``` r
if (FALSE) { # \dontrun{
path <- system.file(file.path("examples", "bad-no-alt.md"),
  package = "roblog"
)
ro_check_urls(path)
} # }
```
