# Auditory Awareness Thesis Project

# Cardiac Influence on Bistable Auditory Perception

This repository contains the R code and data analysis for a study investigating the influence of cardiac timing (systole vs. diastole) on the neural processing of a bistable auditory stimulus (BAS). The project explores the relationship between interoceptive signals (specifically, cardiac activity) and exteroceptive auditory perception.

## Overview

The study uses a within-subject experimental design where participants listen to a bistable auditory stimulus (BAS) synchronized with their cardiac cycle (systole and diastole).  Neural responses are measured using EEG, and frequency-following responses (FFRs) are analyzed to assess differences in auditory processing between the two cardiac phases.  The project also explores the relationship between these neural responses and different perceptual interpretations of the BAS (one stream vs. two streams). The analysis includes descriptive statistics, t-tests, ANOVA, Tukey's HSD post-hoc tests, and various visualizations (violin plots, boxplots, bar plots).

## Repository Structure

*   **`finaldata1.xlsx`:** The data file with subjects, systole and diastole FFR amplitudes and frequencies.
*   **`analysis.Rmd`:**  The main R Markdown file containing the data analysis, including:
    *   Data loading and preprocessing.
    *   Descriptive statistics.
    *   One-sample t-test comparing difference in FFR amplitudes between systole and diastole.
    *   ANOVA comparing FFR amplitudes across different categories based on percentile.
    *   Data visualization (violin plots, boxplots, bar plots).
    *   Creation of APA-style tables for t-test and ANOVA results.
*   **`bibliography.bib`:** A BibTeX file containing the bibliographic references.
*   **`README.md`:** This file, providing an overview of the project.
*   **`overall_summary.csv`**: CSV file containing overall summary statistics.
* **`systole_summary.csv`**: CSV file for summary stats.
* **`diastole_summary.csv`**: CSV file for summary stats.
* **`Plotting_Function.R`**: An R script with a plotting function for easier plots

## Dependencies

The following R packages are required to run the analysis:

*   `readxl`: For reading data from Excel files.
*   `dplyr`: For data manipulation.
*   `tidyr`: For data reshaping (e.g., `pivot_longer`).
*   `ggplot2`: For data visualization.
*   `knitr`: For creating dynamic reports and tables.
*   `kableExtra`: For enhancing `knitr` tables.
*   `forcats`: For working with categorical variables (factors).
*   `stringr`: For string manipulation.
*   `gridExtra`: For arranging multiple plots.
*   `broom`: Converts statistical analysis objects into tidy data frames.
*   `flextable`: Creates customizable and aesthetically pleasing tables for reporting.
*   `readr`: For reading and writing csv files
*   `kableExtra`: Extends knitr::kable with advanced table styling and formatting features.

You can install these packages using the following R command:

```R
install.packages(c("readxl", "dplyr", "tidyr", "ggplot2", "knitr", "kableExtra", "forcats","stringr", "gridExtra", "broom", "flextable", "readr", "kableExtra"))
```
*   **Quarto Extensions:**
    *   `wjschne/apaquarto`: An extension to format Quarto documents according to APA style guidelines.

## Setup and Installation

1.  **Install R:** Download and install R from [https://www.r-project.org/](https://www.r-project.org/).
2.  **Install RStudio (Recommended):** Download and install RStudio Desktop from [https://www.rstudio.com/products/rstudio/download/](https://www.rstudio.com/products/rstudio/download/).
3.  **Install Quarto:** Download and install Quarto from [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/).
4.  **Install R Packages:** Open R or RStudio and run the following code to install the required R packages:
5.  **Install `apaquarto` Quarto Extension:**
    ```bash
    quarto extensions install wjschne/apaquarto
    ```

## Usage

1.  **Clone the Repository:** Clone this repository to your local machine.
2.  **Open the Project:** Open the `_auditory_awareness.qmd` file in RStudio or a text editor.
3.  **Render the Document:** Use the Quarto CLI to render the document to the desired output format (PDF, HTML).

    *   **Render to PDF (APA Style):**
        ```bash
        quarto render _auditory_awareness.qmd --to pdf
        ```

    The output file (`_auditory_awareness.pdf`) will be created in the same directory as the `.qmd` file.

## Analysis

The analysis is performed using R code embedded within the `_auditory_awareness.qmd` file. Key analyses include:

*   **Descriptive Statistics:** Calculating means, standard deviations, etc.
*   **One Samples t-tests:** Comparing the FFR amplitudes
*   **ANOVA:**  ategories of FFR amplitude in Sytolic vs. Diastolic conditions
*   **Data Visualizations:**  Creating bar plots, scatter plots, and boxplots to visualize the data and results.

## Troubleshooting

*   **Missing Packages:** If you encounter errors related to missing R packages, make sure you have installed all the required packages using `install.packages()`.
*   **Pandoc Issues:** If you encounter errors related to PDF rendering, make sure you have a recent version of Pandoc installed and that it's in your system's PATH. Quarto usually handles this.
*   **`apaquarto` Errors:** If you encounter errors related to the `apaquarto` extension, try updating the extension or simplifying your figure and table captions. Check the apaquarto documentation for more information on APA style and the settings needed for quarto.  Be sure that figure cross-references are working.
*   **Character encoding issues:** Excel and R may sometimes cause problems.  Be sure that column headers do not contain special characters.

  ## Contact

Aditi Joshi - [aditij@uchicago.edu]

