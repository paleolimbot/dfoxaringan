
<!-- README.md is generated from README.Rmd. Please edit that file -->

# dfoxaringan

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
<!-- badges: end -->

The goal of dfoxaringan is to provide a DFO
[rmarkdown](https://rmarkdown.rstudio.com) template for
[xaringan](https://bookdown.org/yihui/rmarkdown/xaringan.html)
presentations based on the [Canada.ca design
system](https://www.canada.ca/en/government/about/design-system.html).

## Installation

You can install the development version of dfoxaringan from
[GitHub](https://github.com) with:

``` r
# install.packages("remotes")
remotes::install_github("paleolimbot/dfoxaringan")
```

## Create a new presentation

Option 1: In RStudio, go to *File -\> New -\> Rmarkdown…*. Choose *From
Template* and scroll to find *DFO Xaringan Presentation*.

Option 2: From an R console, run `rmarkdown::draft("my_presentation",
"dfoxaringan", package = "dfoxaringan")`

When you have the template up and running hit *Knit* in RStudio or run
`rmarkdown::render("path/to/presentation.Rmd")` in a fresh R session.
The result of this operation is an HTML document that you can open in
Chrome. Make it full-screen by hitting the ‘f’ key and flip through
slides with your arrow keys\!

## Add content

Write your presentation using all the RMarkdown syntax you’re used to\!
You can follow the [xaringan tutorial from the RMarkdown
book](https://bookdown.org/yihui/rmarkdown/xaringan.html) for details of
what is and is not possible. The short answer is that anything is
possible if you’re willing to write custom HTML and CSS; however, I
recommend keeping your slide structure simple. This will save you time
and make your presentation better.

## Print to PDF

If you’re presenting from your computer using a screen share the HTML
version is probably fine. However, if you’re presenting at a conference
you’ll want a PDF backup in case the venue computers don’t have a modern
browser installed. You can make a PDF version using
`pagedown::chrome_print("path/to/presentaion.html")` (you might have to
restart R between attempts).
