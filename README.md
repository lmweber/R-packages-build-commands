# Pipeline of commands for building R packages

## devtools

```r
devtools::document()  # update .Rd documentation files and NAMESPACE
devtools::install()   # install package from current working directory
devtools::build()     # build package as .tar.gz bundle (saved one directory up)
devtools::test()      # run all unit tests
devtools::check()     # run checks
```

See Hadley Wickham's [R packages textbook](http://r-pkgs.had.co.nz/) for more information. The `devtools` package can be installed with `install.packages("devtools")`.


## RStudio

```r
Command-Shift-k  # build vignette
```


## command-line

```r
R CMD BiocCheck .  # run checks for Bioconductor submission
R CMD build .      # build package as .tar.gz bundle (saved in current directory)
R CMD check --as-cran <filename.tar.gz>  # run checks for CRAN submission
```


