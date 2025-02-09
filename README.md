
<!-- README.md is generated from README.Rmd. Please edit that file -->

# sacRebleu

<!-- badges: start -->
<!-- badges: end -->

The goal of sacRebleu is to provide a simple interface to the BLEU
score, a metric for evaluating the quality of generated text. This
package is inspired by the NLTK and sacrebleu implementations of the
BLEU score, and is implemented in C++ for the R programming language.

## Installation

You can install the development version of sacRebleu from
[GitHub](https://github.com/) with:

### Installation

``` r
# install.packages("devtools")
devtools::install_github("LazerLambda/sacRebleu")
```

## Example

``` r
library(sacRebleu)
cand_corpus <- list("This is good", "This is not good")
ref_corpus <- list(list("Perfect outcome!", "Excellent!"), list("Not sufficient.", "Horrible."))
bleu_corpus <- bleu_corpus(ref_corpus, cand_corpus)
```
