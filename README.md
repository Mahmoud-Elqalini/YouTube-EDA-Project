
# YouTube Video Popularity Analysis

This repository contains a data analysis project that explores the 1,000 most popular YouTube videos to uncover trends in viewership, engagement, and content categories from 2005 to 2025. The project is implemented using Python in a Jupyter Notebook, leveraging libraries like Pandas, NumPy, Matplotlib, and Seaborn.

## Project Overview

The goal of this project is to analyze a dataset of popular YouTube videos to understand how viewership has evolved over time and identify key factors driving video popularity. The analysis includes data cleaning, trend visualization, and insights into audience engagement metrics like likes and dislikes.

### Objectives
- Analyze trends in video views over the years (2005–2025).
- Investigate engagement metrics (likes and dislikes).
- Identify dominant content categories (e.g., Music, Gaming).
- Clean and preprocess the dataset for accurate analysis.

## Dataset

The dataset (`Most popular 1000 Youtube videos.csv`) includes 1,000 records with the following columns:
- **rank**: Video ranking based on popularity.
- **Video**: Video title.
- **Video views**: Total views (string with commas).
- **Likes**: Number of likes (string with commas).
- **Dislikes**: Number of dislikes (string with commas, with missing values).
- **Category**: Video category (e.g., Music, Gaming, with some missing values).
- **published**: Year of publication.

The dataset is stored in the `dataset/` directory.

## Methodology

The project is implemented in a Jupyter Notebook (`ytb_analysis.ipynb`) and follows these steps:

1. **Data Loading**: Load the dataset using Pandas and inspect its structure.
2. **Data Cleaning**:
   - Convert Video views, Likes, and Dislikes from strings to numeric values.
   - Handle missing values: Impute Dislikes with the median and Category with the mode.
3. **Analysis**: Group data by publication year to calculate total views.
4. **Visualization**: Create a line plot to show the trend in views over time using Seaborn.

## Tools and Technologies

- **Language**: Python 3.8+
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn
- **Environment**: Jupyter Notebook
- **Data Source**: Most popular 1000 Youtube videos.csv

## Key Findings

- **Viewership Trends**: Significant peaks in views are driven by viral music and gaming videos.
- **Engagement**: Missing Dislikes (47% of records) were imputed with the median due to YouTube's policy changes.
- **Categories**: Music and Gaming are the most popular categories.
- **Recent Surge**: Videos from 2023–2025 show a sharp increase in views, reflecting YouTube's growing reach.

## Installation and Setup

To run the project locally, follow these steps:

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/Mahmoud-Elqalini/YouTube-EDA-Project.git
    cd YouTube-EDA-Project
    ```

2. **Install Dependencies**: Ensure Python 3.8+ is installed, then install the required libraries:

    ```bash
    pip install pandas numpy matplotlib seaborn
    ```

3. **Prepare the Dataset**: Place the dataset file (`Most popular 1000 Youtube videos.csv`) in the `dataset/` directory.

4. **Run the Notebook**: Launch Jupyter Notebook and open `ytb_analysis.ipynb`:

    ```bash
    jupyter notebook
    ```

5. **Execute Cells**: Run all cells in the notebook to reproduce the analysis and visualizations.

## Project Structure

```
youtube-video-analysis/
├── dataset/
│   └── Most popular 1000 Youtube videos.csv
├── ytb_analysis.ipynb
└── README.md
```

## Results

The main visualization is a line plot showing the trend in total video views from 2005 to 2025, highlighting key growth periods and category-driven peaks.

## Challenges and Solutions

- **Missing Data**: Handled 473 missing Dislikes and 18 missing Category values using median and mode imputation.
- **String Formatting**: Converted comma-separated strings to numeric values using Pandas.
- **Long Time Range**: Customized x-axis ticks for clear visualization of the 2005–2025 timeline.


## Contributing

Contributions are welcome! Please open an issue or submit a pull request for suggestions or improvements.

## Contact

For questions or feedback, feel free to reach out via LinkedIn or open an issue in this repository.

Thank you for exploring this projectو Star the repository if you find it useful, and happy analyzing.
