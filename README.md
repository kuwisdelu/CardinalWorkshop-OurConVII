# Analysis of MSI Experiments with Cardinal

*Materials for the Cardinal workshop at OurCon VII, Saint-Malo, France, 2019*

Updated: Sunday, October 27, 2019

The workshop focuses on computational and statistical analysis of mass spectrometry-based experiments, using open-source R-based software Cardinal (http://cardinalmsi.org) The workshop is designed for scientists who work with DESI- or MALDI-based experiments, and who are comfortable with basics of R. The program includes an introductory lecture describing Cardinal and statistical analysis of MSI experiments, and a hands-on session discussing workflows for clustering, classification, and class comparison.

# Course material

The teaching material for the workshop is provided here in R markdown (.Rmd) format, which allows interleaving of R code with text markup to generate the provided HTML documents. This allows you to reproduce the analysis by re-running the same R code used in the workshop. If you are using RStudio, you can generate the final document by opening the R markdown file and clicking the "Knit" button (it may take a while to re-run all of the R code).

# Installation instructions

This workshop will use __R >= 3.6.1__ and __Bioconductor >= 3.10__.

Please note that the official release of Bioconductor 3.10 is Wednesday, October 30, 2019. We will be using a preview of Bioconductor 3.10 so that the workshop material will remain up-to-date after the conference.

This may require you to re-install packages you already have, and may lead to small discrepancies on the day of the workshop, but the code used here will be correct for the newest version of Bioconductor going forward.

## Installing R and RStudio

Download and install R >= 3.6.1 for your platform from CRAN: https://cran.r-project.org

We recommend (but do not require) the use of RStudio, which provides a nicer environment for working with R.

You can download and install (the free version of) RStudio here: https://rstudio.com/products/rstudio/download

## Installing BiocManager

After starting R, run the following code in R or RStudio:

```{r}
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
```

This will install *BiocManager*, an R package for installing and managing packages from the Bioconductor repository.

## Installing Cardinal

After installing *BiocManager*, run the following R code:

```{r}
BiocManager::install(c("Cardinal",  "CardinalWorkflows"), version="3.10")
```

This will install *Cardinal* from Bioconductor version 3.10. (After the official release of Bioconductor 3.10, you may omit the `version` argument.)

# Schedule

09:00 - 09:30 Lecture: Introduction to Cardinal and statistical analysis for MSI

09:30 - 10:00 Hands-on: Basics of R and Cardinal

10:00 - 10:30 Hands-on: Visualizing MSI data with Cardinal

10:30 - 10:45 Break / practice

10:45 - 11:45 Hands-on: Classification and segmentation in Cardinal

11:45 - 12:00 Break / practice

12:00 - 12:45 Hands-on: Statistical testing in Cardinal

12:45 - 13:00 Wrap-up


