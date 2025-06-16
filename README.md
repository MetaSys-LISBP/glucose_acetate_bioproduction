# Interplay between glucose and acetate metabolisms in *Escherichia coli*

## Overview

This R code perform all analyses detailed in the following publication:

> Acetate as a metabolic booster for glucose-based bioproduction in *Escherichia coli*.
>
> T. Gosselin-Monplaisir, D. Jallet, E. Hascoet, S. Uttenweiler-Joseph, S. Heux, P. Millard. bioRxiv preprint, 2025, doi: [10.1101/XXXXXX](https://doi.org/10.1101/XXXXXX)

The models are available in COPASI format in the `./model/` directory, and in SBML format from the Biomodels database (http://www.ebi.ac.uk/biomodels/) under identifiers MODELXXXXXX and MODELXXXXXX. Details on the model can be found in Millard et al. 2021 (eLife, doi: [10.7554/eLife.63661](https://doi.org/10.7554/eLife.63661)) and at https://github.com/MetaSys-LISBP/acetate_regulation. Figures are saved in the `./results/` directory.

Details on the calculations can be found in the [original publication](https://doi.org/10.1101/XXXXXX) and in the Rmd notebook.

We distribute an HTML file showing the [notebook’s output after execution](https://htmlpreview.github.io/?https://github.com/MetaSys-LISBP/glucose_acetate_bioproduction/blob/main/html/notebook.html)

The code is open-source and available under [GPLv3 license](https://www.gnu.org/licenses/gpl-3.0.txt).

## Dependencies

If not yet done, download and install [Rstudio](https://posit.co/downloads/).

Some R packages are also required.

`RColorBrewer`, `gplots`, `pso`, `colorspace` and `optimx` can be installed
by running the following command in the Rstudio console:

```bash
install.packages(c("RColorBrewer", "gplots", "pso", "optimx", "colorspace"))
```

`CoRC` can be installed
using the following commands:

```bash
install.packages("remotes")
library(remotes)
remotes::install_github("jpahle/CoRC")
library(CoRC)
CoRC::getCopasi()
```

Additional information on CoRC installation and usage are available from the CoRC repository (https://github.com/jpahle/CoRC) and the associated publication (Föster et al., Bioinformatics, 2021, doi: [10.1093/bioinformatics/btab033](https://doi.org/10.1093/bioinformatics/btab033)).

## Usage

To run all analyses detailed in the publication and reproduce Figures 2 and 4:

- download the [GitHub repository tarball](https://github.com/pierremillard/glucose_acetate_bioproduction/archive/refs/heads/main.zip) and unpack it somewhere on your disk

- start Rstudio

- open the file `./notebook.Rmd`

The notebook will open in Rstudio, in each cell you can read/modify/execute the code as well as read accompanying comments.

## Questions
If you have any question, please open a new *issue*
to [our GitHub issue tracker](https://github.com/MetaSys-LISBP/glucose_acetate_bioproduction/issues) so we could discuss together. 

## How to cite
Gosselin-Monplaisir T., Jallet D., Hascoet E., Uttenweiler-Joseph S., Heux S.,  Millard P. Acetate as a metabolic booster for glucose-based bioproduction in *Escherichia coli*. bioRxiv preprint, 2025, doi: [10.1101/XXXXXX](https://doi.org/10.1101/XXXXXX)

## Authors
Pierre Millard

## Contact
:email: Pierre Millard, pierre.millard@insa-toulouse.fr
