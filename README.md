# CompTox-Reproducibility-Organ-Effects
This code accompanies the manuscript, "Reproducibility of organ-level effects in repeat dose animal studies" by Paul Friedman et al. The code walks through the data cleaning and analysis of the reproducibility of organ-level effects in the US EPA Toxicity Reference Database. Additionally, the code can be more easily browsed as an html report (the knitted Rmarkdown), which is accessible publicly here along with Supplemental Files: https://clowder.edap-cluster.com/datasets/646d247fe4b08a6b394d2853

Disclaimer: The United States Environmental Protection Agency (EPA) GitHub project code is provided on an "as is" basis and the user assumes responsibility for its use. EPA has relinquished control of the information and no longer has responsibility to protect the integrity, confidentiality, or availability of the information. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by EPA. The EPA seal and logo shall not be used in any manner to imply endorsement of any commercial product or activity by EPA or the United States Government. 

## Abstract

This work estimates benchmarks for new approach method (NAM) performance in predicting organ-level effects in repeat dose studies of adult animals based on variability in replicate animal studies. Treatment-related effect values from the Toxicity Reference database (v2.1) for weight, gross, or histopathological changes in the adrenal gland, liver, kidney, spleen, stomach, and thyroid were used. Rates of chemical concordance among organ-level findings in replicate studies, defined by repeated chemical only, chemical and species, or chemical and study type, were calculated. Concordance was 39 - 88%, depending on organ, and was highest within species. Variance in treatment-related effect values, including lowest effect level (LEL) values and benchmark dose (BMD) values when available, was calculated by organ. Multilinear regression modeling, using study descriptors of organ-level effect values as covariates, was used to estimate total variance, mean square error (MSE), and root residual mean square error (RMSE). MSE values, interpreted as estimates of unexplained variance, suggest study descriptors accounted for 52-69% of total variance in organ-level LELs. RMSE ranged from 0.41 – 0.68 log10-mg/kg/day. Differences between organ-level effects from chronic (CHR) and subchronic (SUB) dosing regimens were also quantified. Odds ratios indicated CHR organ effects were unlikely if the SUB study was negative. Mean differences of CHR - SUB organ-level LELs ranged from -0.38 to -0.19 log10 mg/kg/day; the magnitudes of these mean differences were less than RMSE for replicate studies. Finally, in vitro to in vivo extrapolation (IVIVE) was employed to compare bioactive concentrations from in vitro NAMs for kidney and liver to LELs. The observed mean difference between LELs and mean IVIVE dose predictions approached 0.5 log10-mg/kg/day, but differences by chemical ranged widely. Overall, variability in repeat dose organ-level effects suggests expectations for quantitative accuracy of NAM prediction of LELs should be at least ± 1 log10-mg/kg/day, with qualitative accuracy not exceeding 70%. 

## What does this project do?

This project provides the input and code to regenerate the analysis for Paul Friedman et al. "Reproducibility of organ-level effects in repeat dose animal studies." The code cleans the dataset obtained from ToxRefDB v2.1, and then proceeds through several analyses including an analysis of concordance of responses at the tissue level; estimates of variance in replicate organ level observations; estimates of qualitative and quantitative differences in effect level estimates between subchronic and chronic exposures; and estimates of quantitative differences in animal-based effect level estimates and effect level estimates based on in vitro assay data and generic toxicokinetic models.

## Why is this useful?

This project is useful for ensuring reproducibility and technical details for this manuscript are public.

## How can users get started?

Mostly, this code is intended to be browsed. However, users can clone this repo and re-run the code in the .Rmd file.
The folder "source" contains the source files needed to run the code.
The folder "output" contains the organized Supplemental File outputs that accompany the manuscript.
Supplemental File 1 contains the datasets used in MLR for estimation of variance.
Supplemental File 2 contains tabular reporting of input data for concordance analysis and results as percent concordance observed by chemical-endpoint, chemical-endpoint-species, and chemical-endpoint-study type combinations.
Supplemental File 3 contains MLR study descriptors and results for quantitative estimates of variance.
Supplemental File 4 contains odds ratio datasets and results.
Supplemental File 5 contains summarized LEL and HED values, ToxCast assay endpoint information, and calculated AED50 values using library(httk) v2.2.2.



## Where users can get help with this project

Users can contact Katie Paul Friedman (paul-friedman.katie@epa.gov) for questions on this repo. For using ToxRefDB, there is a user guide, referenced in the ToxRefDB Git repo: https://github.com/USEPA/CompTox-ToxRefDB

