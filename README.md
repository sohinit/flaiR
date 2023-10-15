
## <u>`flairR`</u>: An R Wrapper for Accessing Flair NLP Tagging Features <img src="man/figures/logo.png" align="right" width="180"/>

[![R](https://github.com/davidycliao/flaiR/actions/workflows/r_macos.yml/badge.svg)](https://github.com/davidycliao/flaiR/actions/workflows/r_macos.yml)
[![R-CMD-check](https://github.com/davidycliao/flaiR/actions/workflows/r.yml/badge.svg)](https://github.com/davidycliao/flaiR/actions/workflows/r.yml)
[![coverage](https://github.com/davidycliao/flaiR/actions/workflows/test-coverage.yaml/badge.svg)](https://github.com/davidycliao/flaiR/actions/workflows/test-coverage.yaml)
[![codecov](https://codecov.io/gh/davidycliao/flaiR/graph/badge.svg?token=CPIBIB6L78)](https://codecov.io/gh/davidycliao/flaiR)
[![CodeFactor](https://www.codefactor.io/repository/github/davidycliao/flair/badge)](https://www.codefactor.io/repository/github/davidycliao/flair)

<!-- README.md is generated from README.Rmd. Please edit that file -->

<div style="text-align: justify">

`{flaiR}` is a R wrapper of the {`flairNLP/flair`} for R users,
particularly for social science researchers. It offers streamlined
access to the core features of {`flairNLP`}. `{flairNLP}` is an advanced
NLP framework in Python that incorporates the advanced techniques
developed by [Zalando
Research](https://engineering.zalando.com/posts/2018/11/zalando-research-releases-flair.html)
based in Berlin. For a deeper understanding of {flairNLP/flair}’s
architecture, refer to the research article ‘[Contextual String
Embeddings for Sequence
Labeling](https://aclanthology.org/C18-1139.pdf)’ and the official
[mannual](https://flairnlp.github.io) in Python. Here is an R wrapper
providing R users with a seamless way to use Flair without dealing with
Python.

For R users, {`flairR`} primarily consists of two main components. The
first is a wrapper function built on top of {`reticulate`}, which
enables you to interact directly with Python modules in R and provides
seamless support for documents and [tutorial (in
progress)](https://davidycliao.github.io/flaiR/articles/tutorial.html)
in the R community. Secondly, to facilitate more efficient use for
social science research, {`flairR`} extend {`flairNLP/flair`}’s core
functionality for working with three major functions to extract features
in a tidy and fast format–
[data.table](https://cran.r-project.org/web/packages/data.table/index.html)
in R.

The core features include:

- [**part-of-speech
  tagging**](https://davidycliao.github.io/flaiR/articles/get_pos.html)

- [**transformer-based sentiment
  analysis**](https://davidycliao.github.io/flaiR/articles/get_entities.html)

- [**named entity
  recognition**](https://davidycliao.github.io/flaiR/articles/get_sentiments.html)

</div>

<br>

### Installation via <u>**`GitHub`**</u>

<div style="text-align: justify">

The installation consists of two parts: First, install [Python
3.7](https://www.python.org/downloads/) or higher, and [R
3.6.3](https://www.r-project.org) or higher. Although we have tested it
on Github Action with R 3.6.2, we strongly recommend installing [R 4.0.0
or above](https://github.com/davidycliao/flaiR/actions/runs/6416611291)
to ensure compatibility between the R environment and {`reticulate`}. If
there are any issues with the installation, feel free to ask in the
<u>[Discussion](https://github.com/davidycliao/flaiR/discussions) </u>.

</div>

``` r
install.packages("remotes")
remotes::install_github("davidycliao/flaiR", force = TRUE)
```

``` r
library(flaiR)
#> flaiR: An R Wrapper for Accessing Flair NLP Tagging Features      
#> Python: 3.11                                           
#> Flair: 0.12.2  
```

<br>

## Contribution and Open Source Support

<div style="text-align: justify">

R developers who want to contribute to {`flaiR`} are welcome – {`flaiR`}
is an open source project. I warmly invite R users who share similar
interests to join in contributing to this package. Please feel free to
shoot me an email to collaborate on the task. Contributions – whether
they be comments, code suggestions, tutorial examples, or forking the
repository – are greatly appreciated. Please note that the `flaiR` is
released with the [Contributor Code of
Conduct](https://github.com/davidycliao/flaiR/blob/master/CONDUCT.md).
By contributing to this project, you agree to abide by its terms.

The main communication channel is in the
[Discussion](https://github.com/davidycliao/flaiR/discussions). Feel
free to ask help, report problems and share insights with the
[Discussion](https://github.com/davidycliao/flaiR/discussions).

</div>

<br>

## Citing the Contributions of `Flair NLP`

<div style="text-align: justify">

If you use this tool in academic research, we recommend citing the
research article, [Contextual String Embeddings for Sequence
Labeling](https://aclanthology.org/C18-1139.pdf) from
[Flair](https://flairnlp.github.io) and [Zalando
Research](https://engineering.zalando.com/posts/2018/11/zalando-research-releases-flair.html).

</div>

    @inproceedings{akbik2018coling,
      title={Contextual String Embeddings for Sequence Labeling},
      author={Akbik, Alan and Blythe, Duncan and Vollgraf, Roland},
      booktitle = {{COLING} 2018, 27th International Conference on Computational Linguistics},
      pages     = {1638--1649},
      year      = {2018}
    }
