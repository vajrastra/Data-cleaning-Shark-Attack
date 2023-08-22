# Data-cleaning-Shark-Attack

## Shark Attack Data Cleaning Project

Welcome to the Shark Attack Data Cleaning Project repository! This project focuses on cleaning and preparing shark attack data for analysis purposes.

## Project Overview

This project aims to conduct a comprehensive study on shark attacks, with a primary focus on cleaning and imputing the data to ensure its suitability for analysis. The original dataset was sourced from [Kaggle](https://www.kaggle.com/mysarahmadbhat/shark-attacks) and has been cleaned and organized to facilitate meaningful insights.

## Dataset

- **Raw Data**: The raw dataset is available as `shark_attacks_raw.csv`.

- **Processed Data**: The cleaned dataset has been transformed and is available as `shark_attacks_cleaned.xlsx`.

## Data Cleaning Steps

1. **Data Reduction**: The original dataset was streamlined to include only essential columns for the analysis. The following columns were retained:
    - Case Number
    - Year
    - Type
    - Country
    - Area
    - Location
    - Activity
    - Sex
    - Age
    - Injury
    - Fatal

2. **Handling Duplicates**: Duplicate entries were identified using the "Case Number" column as a unique identifier. Duplicates were renamed with the suffix '.1', '.2', and so on.

3. **Filling Missing Values**:
    - "Year" column: Blank values were populated with the first four digits of the corresponding "Case Number".
    - "Type" column: Blank values were filled with "unknown".
    - "Country" column: Rows with blank "Country" values were deleted.
    - Columns between "Area" and "Injury": Blank cells were replaced with "unknown".
    - "Age" column: Non-numeric values were replaced with "unknown".
    - "Fatal" column: Non-"Y" or "N" values were replaced with "unknown".

4. **Data Validation**: Checked for any remaining blank cells to ensure data completeness.

5. **Data Corrections**:
    - Adjusted the "Year" and "Sex" columns to correct anomalies identified using data visualization.

## Getting Started

To use the cleaned dataset for your analysis:

1. Clone this repository: `git clone https://github.com/vajrastra/Data-cleaning-Shark-Attack.git`
2. Access the cleaned dataset in the `shark_attacks_cleaned.xlsx` file.

## Contributing

If you'd like to contribute to this project, feel free to submit pull requests or raise issues in the repository. We welcome your insights and suggestions!

## License

This project is licensed under the [MIT License](LICENSE).

---

For detailed information about the data cleaning steps and project progress, refer to the excel workbook.

For more information about the original dataset and its source, visit [Kaggle](https://www.kaggle.com/mysarahmadbhat/shark-attacks).
