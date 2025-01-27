# Online-Retail-Data-Analysis-and-Visualization

# Overview

The main objectives of this assignment are:

- To combine and clean data from multiple sources.
- To perform quantitative and qualitative analyses on the data.
- To create interactive visualizations for better insights.

The content is presented in a Quarto Markdown file (`Assignment 3.qmd`), which can be rendered into an HTML document for easy sharing and presentation.

---

# Prerequisites

To run the scripts provided in this repository, ensure you have R and RStudio installed on your machine. Additionally, the following R packages are required:

## Data Manipulation and Wrangling

- **`tidyr`**: For data tidying.
- **`readxl`** and **`readr`**: For reading Excel and CSV files.
- **`plyr`** and **`dplyr`**: For data manipulation.

## Modeling

- **`mgcv`**: For Generalized Linear Models (GLMs).

## Text Mining and Visualization

- **`tm`**: For text mining tasks.
- **`wordcloud`**: For generating word clouds.
- **`stringr`**: For string manipulation functions.

## Interactive Visualization

- **`plotly`**: For creating interactive bar charts.
- **`leaflet`**: For creating geographical visualizations.

---

# Installation

To install the required packages, run the following commands in your R console:

```r
install.packages("tidyr")   # Data tidying.
install.packages("readxl")  # Reading Excel files.
install.packages("readr")   # Reading CSV files.
install.packages("plyr")    # Data manipulation.
install.packages("dplyr")   # Data manipulation.
install.packages("mgcv")    # Generalized Linear Models.
install.packages("tm")      # Text mining.
install.packages("wordcloud") # Word clouds.
install.packages("stringr") # String manipulation.
install.packages("plotly")  # Interactive charts.
install.packages("leaflet") # Geographical mapping.
```
---

# Workflow

## Step 1: Load Libraries and Read Data

After installing the necessary packages, load them into your R session. Next, read the datasets from Excel and CSV files into R. The datasets are combined using `rbind`, cleaned by omitting rows with missing values (`na.omit`), and removing duplicate rows.

## Step 2: Data Preprocessing

Cleaned data is processed further by:

- Formatting dates.
- Extracting relevant subsets for focused analysis.
- Managing computational load and narrowing down analysis to specific areas of interest.

## Step 3: Quantitative Analysis

We employ a **Generalized Linear Model (GLM)** to explore relationships within the data. For example, we analyze how factors like unit price and month of sale influence transaction quantities.

## Step 4: Qualitative Analysis

We preprocess product descriptions by:

- Converting text to lowercase.
- Removing punctuation, numbers, and stopwords.

A **term-document matrix** is created, and prevalent themes and words are identified. Results are visualized through word clouds and bar charts of word frequencies.

## Step 5: Visualization

- **Interactive Bar Chart (Plotly)**: Transactions per country are visualized, offering an engaging exploration of the data.
- **Word Cloud**: Highlights significant terms in product descriptions.
- **Geographical Mapping (Leaflet)**: Transactions are mapped geographically with dynamic color scales to show distribution and intensity.


# How to Use

1. Clone the repository to your local machine:
   ```bash
   git clone <repository-url>
   ```
2. Open the Assignment 3.qmd file in RStudio.
3. Install the required packages if not already installed.
4. Render the Quarto file to generate the HTML output
5. Explore the output for insights and visualizations.


# File Structure

- Assignment 3.qmd: The main Quarto Markdown file containing all instructions and scripts.
- README.md: This file, providing an overview of the repository.

# Contributing

If you would like to contribute to this project, please fork the repository, make your changes, and submit a pull request. Contributions are welcome!

# License

This project is licensed under the MIT License. See the LICENSE file for more details.

# Acknowledgments

Thanks to the authors of the R packages used in this assignment for their invaluable tools and contributions to the R ecosystem.
