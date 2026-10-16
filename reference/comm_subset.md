# Subset data from one study site

this function is to be used with datasets containing multiple study
sites

## Usage

``` r
comm_subset(data = NULL, site = NULL)
```

## Arguments

- data:

  a dataframe. Must contain a column named Study_site

- site:

  A character string indicating the name of the study site

## Value

a dataframe

## Examples

``` r
if (FALSE) { # interactive()

data<-load_interactions()
comm_subset(data, site="Amoladeras")
}
```
