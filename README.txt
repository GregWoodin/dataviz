# README

Operating system used: macOS Big Sur Version 11.4

Please note that some files are too large to render (> 200 KiB). These files must be downloaded to view.

The main folder contains a `.txt` of this README file:
-   `README.txt`

## Preregistration
-   Experiment 1: 
    -   `pre-registration/E1_prereg.docx` 
-   Experiment 2:
    -   `pre-registration/E2_prereg.docx` 
-   Experiment 2 (updated): 
    -   `pre-registration/E2_prereg2_updated.docx` 

See **Registrations** tab for original, time-stamped pre-registrations.

## Stimuli
The graphs shown to participants in both experiments are stored in this folder. 

In the file names, the number after `G` corresponds to the experimental group:

- **1:** Normal graph with quantity on y-axis and time on x-axis
- **2:** Normal graph with quantity on x-axis and time on y-axis
- **3:** Y-axis inverted with quantity on y-axis and time on x-axis
- **4:** Y-axis inverted with quantity on x-axis and time on y-axis
- **5:** X-axis inverted with quantity on y-axis and time on x-axis
- **6:** X-axis inverted with quantity on x-axis and time on y-axis

The number after `V` corresponds to the trial:

- **1:** Positive valence, rising trend
- **2:** Positive valence, falling trend
- **3:** Negative valence, rising trend
- **4:** Negative valence, falling trend

The files are as follows:

-   `G1_V1.png`
-   `G1_V2.png`
-   `G1_V3.png`
-   `G1_V4.png`
-   `G2_V1.png`
-   `G2_V2.png`
-   `G2_V3.png`
-   `G2_V4.png`
-   `G3_V1.png`
-   `G3_V2.png`
-   `G3_V3.png`
-   `G3_V4.png`
-   `G4_V1.png`
-   `G4_V2.png`
-   `G4_V3.png`
-   `G4_V4.png`
-   `G5_V1.png`
-   `G5_V2.png`
-   `G5_V3.png`
-   `G5_V4.png`
-   `G6_V1.png`
-   `G6_V2.png`
-   `G6_V3.png`
-   `G6_V4.png`

## Qualtrics

This folder contains a `.pdf` printout of an example of an experiment that participants completed:

-   `example.pdf`

It also contains the raw code in `.txt` form needed to run the survey for oneself:

-   `example.txt`

## Analysis
The analysis was conducted using the programming language R inside RStudio. The following libraries are required for this analysis:

- plyr         
- tidyverse  
- brms     
- ggmcmc
- tidybayes
- ggpubr

If the reader wants to try the analyses out for themselves, they will need to download the data files outlined in the **Data** section below, as well as the analysis scripts (`.Rmd`) outlined in the **Analysis scripts** section.

### Data
The data for each experiment are presented in six `.csv` spreadsheets, each corresponding to the experimental groups mentioned in the **Stimuli** section (above). The numbers at the end of the following filenames represent the different experimental groups: 

-   Experiment 1
    -   `analysis/E1/data/data_viz_1.csv`
    -   `analysis/E1/data/data_viz_2.csv`
    -   `analysis/E1/data/data_viz_3.csv`
    -   `analysis/E1/data/data_viz_4.csv`
    -   `analysis/E1/data/data_viz_5.csv`
    -   `analysis/E1/data/data_viz_6.csv`
-   Experiment 2
    -   `analysis/E2/data/data_viz_1.csv`
    -   `analysis/E2/data/data_viz_2.csv`
    -   `analysis/E2/data/data_viz_3.csv`
    -   `analysis/E2/data/data_viz_4.csv`
    -   `analysis/E2/data/data_viz_5.csv`
    -   `analysis/E2/data/data_viz_6.csv`

IP addresses and MTurk IDs have been removed from these spreadsheets for anonymity. There were no duplicates, suggesting that no participants completed either experiment more than once, nor did any participant complete both experiments.

The following codebook contains information about the columns in the above spreadsheets and how to interpret the values in these columns:
-   `analysis/codebook.html`

We have also included the valence norms collected by Warriner et al. (2013) that we used to choose the valenced words for use in our experimental materials in the following `.csv` spreadsheet:
-   `analysis/E1/data/valence_list.csv`

For more information about these valence norms, visit https://link.springer.com/article/10.3758/s13428-012-0314-x

### Analysis scripts
The following analysis scripts show the analysis we conducted and the results we obtained. The `.pdf` files are the most readable and should be used for viewing the results. The `.Rmd` files should be opened in R if the reader wants to run the analyses for themselves.

-   Experiment 1:
    - `analysis/E1/code/E1.Rmd`
    - `analysis/E1/code/E1.pdf`
-   Experiment 2:
    -   `analysis/E2/code/E2.Rmd`
    -   `analysis/E1/code/E2.pdf`
-   Valence norms:
    - `analysis/E1/code/valence_norms.Rmd`
    - `analysis/E1/code/valence_norms.pdf`

### Figures
These are the figures presented in the manuscript in `.pdf` format. Figures 3 and 4 were created by running the above analysis scripts (`.Rmd` files). 

-   `analysis/figures/fig1.pdf`
-   `analysis/figures/fig2.pdf`
-   `analysis/figures/fig3.pdf`
-   `analysis/figures/fig4.pdf`

### Table creation
When run, the above **Analysis scripts** (`.Rmd`) create the following files, which were used to create figures 3 and 4. The `.csv` spreadsheet files contain the results from our statistical models. The `.pdf` files contain visualizations of these results.

-   Experiment 1, Figure 3:
    -   `analysis/table_creation/E1_model1.csv`
    -   `analysis/table_creation/E1_model1.pdf`
    -   `analysis/table_creation/E1_model2.csv`
    -   `analysis/table_creation/E1_model2.pdf`
-   Experiment 2, Figure 4:
    -   `analysis/table_creation/E2_model1.csv`
    -   `analysis/table_creation/E2_model1.pdf`
    -   `analysis/table_creation/E2_model2.csv`
    -   `analysis/table_creation/E2_model2.pdf`
    -   `analysis/table_creation/E2_model3.csv`
    -   `analysis/table_creation/E2_model3.pdf`
