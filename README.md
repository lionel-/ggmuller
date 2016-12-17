ggmuller
========

Create Muller Plots of Evolutionary Dynamics

### Installation

To install & load in R with devtools:

``` r
install.packages("devtools")
library(devtools)
  
install_github("robjohnnoble/ggmuller")
library(ggmuller)
```

### Basic usage

The main functions in `ggmuller` are `get_Muller_df` and `Muller_plot`, which we can run on some data included in the package:

``` r
# get data
Muller_df <- get_Muller_df(example_edges, example_pop_df, threshold = 0.005)

# generate pretty plot
Muller_plot(Muller_df)
```

![](readme_files/figure-markdown_github/example-1.png)<!-- -->

### How-to guide with examples

For an introduction to how the package works, an overview of its features, and some worked examples, see the blog post on [Visualizing evolutionary dynamics with ggmuller](https://thesefewlines.wordpress.com/2016/08/20/how-to-ggmuller/).
