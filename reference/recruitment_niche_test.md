# Recruitment niche: community-level effects on species recruitment

tests whether the presence of vegetation (i.e any canopy species)
compared to the "Open", enhances, depresses or has a neutral effect on
the recruitment of a given recruit species. **Input**:The canopy-recruit
interactions dataset and the canopy cover dataset (details as explained
in
[`int_significance()`](https://ecologyr.github.io/RecruitNetP/reference/int_significance.md)
documentation).

## Usage

``` r
recruitment_niche_test(int_data, cover_data)
```

## Arguments

- int_data:

  data frame containing interaction data.

- cover_data:

  data frame with the abundance of each canopy species in each plot.

## Value

The same variables provided by the function
[`int_significance()`](https://ecologyr.github.io/RecruitNetP/reference/int_significance.md)
but without distinguishing between canopy species.

## Examples

``` r
recruitment_niche_test (Amoladeras_int, Amoladeras_cover)
#> P-values are unadjusted for multiple tests
#> Warning: Different tests were used for different canopy-recruit pairs. Check column Test_type
#>                   Recruit  Fr       Av  Fro       Ao   testability Significance
#> 1    Artemisia_barrelieri  36 3073.008   54 6926.992  7.598575e-47 5.663873e-02
#> 2    Artemisia_campestris   5 3073.008    1 6926.992  8.421358e-04 1.223189e-02
#> 3         Asparagus_albus  18 3073.008    7 6926.992  1.545583e-13 7.731378e-06
#> 4      Asparagus_horridus  35 3073.008   18 6926.992  6.932272e-28 2.529184e-08
#> 5         Ballota_hirsuta  71 3073.008   11 6926.992  9.554823e-43 5.775852e-28
#> 6    Helichrysum_stoechas 259 3073.008  796 6926.992  0.000000e+00 1.355570e-05
#> 7       Hyparrhenia_hirta  19 3073.008   34 6926.992  6.932272e-28 4.192453e-01
#> 8     Launaea_arborescens  80 3073.008   89 6926.992  2.501864e-87 2.877858e-06
#> 9        Launaea_lanifera   2 3073.008    6 6926.992  7.952607e-05 1.000000e+00
#> 10     Lycium_intrincatum  44 3073.008   20 6926.992  1.599839e-33 4.326202e-11
#> 11         Lygeum_spartum  23 3073.008   80 6926.992  1.655999e-53 6.463875e-02
#> 12  Maytenus_senegalensis   4 3073.008    0 6926.992  8.917739e-03 8.917739e-03
#> 13          Ononis_natrix 273 3073.008 1839 6926.992  0.000000e+00 2.287583e-70
#> 14 Periploca_angustifolia   0 3073.008    1 6926.992  3.073008e-01 1.000000e+00
#> 15     Phagnalon_saxatile 685 3073.008  528 6926.992  0.000000e+00 4.167429e-84
#> 16  Piptatherum_miliaceum   8 3073.008   19 6926.992  1.459552e-14 9.013658e-01
#> 17  Salsola_oppositifolia 112 3073.008   60 6926.992  7.260304e-89 1.448819e-22
#> 18      Stipa_tenacissima   0 3073.008    1 6926.992  3.073008e-01 1.000000e+00
#> 19     Teucrium_charidemi   8 3073.008   14 6926.992  5.326000e-12 5.668366e-01
#> 20   Teucrium_lusitanicum  27 3073.008   16 6926.992  9.230787e-23 5.195970e-06
#> 21        Teucrium_polium 241 3073.008  308 6926.992 4.703989e-282 2.273677e-11
#> 22      Thymelaea_hirsuta 175 3073.008  170 6926.992 1.619845e-177 8.315492e-16
#> 23        Thymus_hyemalis 114 3073.008 1030 6926.992  0.000000e+00 2.499952e-52
#> 24    Whitania_frutescens  45 3073.008    5 6926.992  2.388826e-26 1.048974e-19
#> 25         Ziziphus_lotus   0 3073.008    4 6926.992  8.917739e-03 3.195640e-01
#>     Test_type   Veg_effect
#> 1  Chi-square      Neutral
#> 2    Binomial  Facilitated
#> 3  Chi-square  Facilitated
#> 4  Chi-square  Facilitated
#> 5  Chi-square  Facilitated
#> 6  Chi-square    Depressed
#> 7  Chi-square      Neutral
#> 8  Chi-square  Facilitated
#> 9    Binomial      Neutral
#> 10 Chi-square  Facilitated
#> 11 Chi-square      Neutral
#> 12   Binomial  Facilitated
#> 13 Chi-square    Depressed
#> 14   Binomial Not testable
#> 15 Chi-square  Facilitated
#> 16 Chi-square      Neutral
#> 17 Chi-square  Facilitated
#> 18   Binomial Not testable
#> 19 Chi-square      Neutral
#> 20 Chi-square  Facilitated
#> 21 Chi-square  Facilitated
#> 22 Chi-square  Facilitated
#> 23 Chi-square    Depressed
#> 24 Chi-square  Facilitated
#> 25   Binomial      Neutral
```
