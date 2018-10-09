# The Stan Book

This is the repository for *Bayesian Statistics Using Stan", which serves as both the Stan users' guide and an introduction to Bayesian statistics.

## Style Guide 

* y ~ normal(mu, sigma)  # Not:  N(), not sigma^2, regular font for "normal", Latex math for $y$, $\mu$, $\sigma$

* norma(y | mu, sigma) # Vertical bar, not semicolon

* Poisson, Weibull, LKJ # Use capital letters for distributions that are named after people

* E(y)  # Regular font, parentheses not brackets

* ()  # Always parentheses, never brackets

* No special fonts for distributions, just latex roman and math fonts

* p(y) # Probability density and probability mass function

* Pr(A)  # probability of an event

* Follow the Stan style guide for code
    - int<lower = 0> N;  # Put in the lower bound
    - for (n in 1:N); # Not:  for (i in 1:n);
    - foo_bar # Underscores rather than dots or CamelCase

* No R/Python code in the finished book except in appendix

* All Stan code should be best practice except when explaining something, in which case we should explicitly show the best-practice alternative

## Licensing

The code is licensed under BSD-3 and the text under CC-BY ND 4.0.  

## Building

* In RStudio: to build the project, open `index.Rmd` in RStudio and click `knit`
    - change output on first line of `index.Rmd` for `gitbook` and `pdf_book` (not differeing `_`)
    
* Use `bookdown::render('index.Rmd')` from within R in the top-level directory

* Use the shell scripts `> ./_build.sh` to build both PDF and HTML versions
* From the command line
