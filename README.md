ggmuller
========

Create Muller Plots of Evolutionary Dynamics

### Installation

To install the [CRAN version](https://cran.r-project.org/web/packages/ggmuller/index.html):
``` r
library(ggmuller)
```

To install the github version using devtools:

``` r
install.packages("devtools")
library(devtools)
  
install_github("robjohnnoble/ggmuller")
library(ggmuller)
```

### Basic usage

The main functions in `ggmuller` are `get_Muller_df` and `Muller_plot`, which we can run on some data included in the package:

``` r
# reformat data ready for plotting:
Muller_df <- get_Muller_df(example_edges, example_pop_df, threshold = 0.005)

# generate the plot:
Muller_plot(Muller_df)
```

### How-to guides

The best place to start is the [CRAN vignette](https://cran.r-project.org/web/packages/ggmuller/vignettes/ggmuller.html), which includes an overview of features and some worked examples.

An older, slightly different set of instructions can be found in a blog post on [Visualizing evolutionary dynamics with ggmuller](https://thesefewlines.wordpress.com/2016/08/20/how-to-ggmuller/).

### Version history

0.1.0: First release.

0.1.1: Essential update for compatibility with ggplot2 version 2.2.0.

0.1.2: Better plotting of the points at which genotypes emerge.

0.1.3: Compatibility with dplyr version 0.7.2; add option for smoother plotting of genotype emergence points.

0.2.0: New function Muller_pop_plot shows variation in population size as well as frequency (also known as a fish plot).

0.2.1: Correct mistake in calculating population sizes for Muller_pop_plot.

### Citation

To cite ggmuller in publications please use

    Robert Noble (2017). ggmuller: Create Muller Plots of Evolutionary Dynamics. R package version 0.2.1. https://CRAN.R-project.org/package=ggmuller

A BibTeX entry for LaTeX users is

    @Manual{,
    title = {ggmuller: Create Muller Plots of Evolutionary Dynamics},
    author = {Robert Noble},
    year = {2017},
    note = {R package version 0.2.1},
    url = {https://CRAN.R-project.org/package=ggmuller},
    }

Please amend the version number as appropriate.
