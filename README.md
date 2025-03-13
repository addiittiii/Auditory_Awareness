# Auditory Awareness Thesis Project

# Cardiac Influence on Bistable Auditory Perception

This repository contains the R code and data analysis for a study investigating the influence of cardiac timing (systole vs. diastole) on the neural processing of a bistable auditory stimulus (BAS). The project explores the relationship between interoceptive signals (specifically, cardiac activity) and exteroceptive auditory perception.

## Overview

The study uses a within-subject experimental design where participants listen to a bistable auditory stimulus (BAS) synchronized with their cardiac cycle (systole and diastole).  Neural responses are measured using EEG, and frequency-following responses (FFRs) are analyzed to assess differences in auditory processing between the two cardiac phases.  The project also explores the relationship between these neural responses and different perceptual interpretations of the BAS (one stream vs. two streams). The analysis includes descriptive statistics, t-tests, ANOVA, Tukey's HSD post-hoc tests, and various visualizations (violin plots, boxplots, bar plots).

## Repository Structure

*   **`finaldata1.xlsx`:** The raw data file (simulated data for this example).  **REPLACE THIS WITH YOUR ACTUAL DATA FILE.**
*   **`analysis.Rmd`:**  The main R Markdown file containing the data analysis, including:
    *   Data loading and preprocessing.
    *   Descriptive statistics.
    *   Paired-samples t-test comparing FFR amplitudes between systole and diastole.
    *   ANOVA comparing FFR amplitudes across different categories based on percentile.
    *   Tukey's HSD post-hoc tests.
    *   Data visualization (violin plots, boxplots, bar plots).
    *   Creation of APA-style tables for t-test and ANOVA results.
*   **`references.bib`:** A BibTeX file containing the bibliographic references.
*   **`apa.csl`:**  A Citation Style Language (CSL) file for APA style citations. You can download this from the Zotero Style Repository ([https://www.zotero.org/styles](https://www.zotero.org/styles)).
*   **`README.md`:** This file, providing an overview of the project.
*   **`overall_summary.csv`**: CSV file containing overall summary statistics.
* **`systole_summary.csv`**: CSV file for summary stats.
* **`diastole_summary.csv`**: CSV file for summary stats.

## Dependencies

The following R packages are required to run the analysis:

*   `readxl`: For reading data from Excel files.
*   `dplyr`: For data manipulation.
*   `tidyr`: For data reshaping (e.g., `pivot_longer`).
*   `ggplot2`: For data visualization.
*   `knitr`: For creating dynamic reports and tables.
*   `kableExtra`: For enhancing `knitr` tables.
*   `forcats`: For working with categorical variables (factors).
*   `rstatix`: For performing statistical tests (ANOVA, Tukey's HSD).
*   `apaTables`:  For generating APA-style ANOVA tables (optional, but recommended).
*   `stringr`: For string manipulation.
*   `gridExtra`: For arranging multiple plots.
*  `citr`: For adding citations.

You can install these packages using the following R command:

```R
install.packages(c("readxl", "dplyr", "tidyr", "ggplot2", "knitr", "kableExtra", "forcats", "rstatix", "apaTables", "stringr", "gridExtra", "citr"))
