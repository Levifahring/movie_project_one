# Does Money Really Matter? 

This project analyzes movie data from the TMDB dataset, specifically focusing on films released between January 1, 2019, and December 31, 2023. The analysis aims to understand the relationship between various factors such as budget, revenue, profit percentage, vote averages, and genres. The code is implemented in Python using libraries like `pandas`, `matplotlib`, `numpy` and `scipy`.

## Dataset

The dataset used for this analysis is the **TMDB Movie Dataset v11**, which contains information about movies, including their budget, revenue, genres, and ratings. Dataset can be found at https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies


## Data Preparation

1. **Filtering by Date**: The dataset is filtered to include only movies released between January 1, 2019, and December 31, 2023.
2. **Calculating Total Budget and % Profit**: The total budget is calculated as 1.5 times the reported budget. The percentage profit is calculated as `(revenue - total budget / total budget) * 100`.
3. **Cleaning**: Movies with a total budget and revenue of less than $10 million are excluded to focus on significant releases.

## Analysis

### Total Budget vs % Profit

This analysis explores the relationship between the total budget and the percentage profit of movies. A scatter plot is generated, and a linear regression line is added to visualize the trend.

### Total Budget vs Revenue

Here, we analyze how the total budget correlates with the revenue generated. The revenue is converted into millions for better readability.

### Total Budget vs Vote Average

This analysis examines the relationship between the total budget and the average votes a movie receives. The vote averages are clipped to a range of 0 to 10.

### Vote Average vs % Profit

In this section, we investigate whether higher vote averages correlate with higher profits.

## Genre Analysis

### Mean Budgets by Genre

We categorize movies into genres such as SciFi, Horror, Action, RomCom, Comedy, and Other. The mean budgets for each genre are calculated.

### Mean Revenues by Genre

Similarly, the mean revenues for each genre are calculated to understand the financial success of different genres.

## Visualizations

The following visualizations are generated in this analysis:

- **Total Budget vs % Profit**
  ![budge_profit](https://github.com/user-attachments/assets/ea448d73-6990-4b61-bcd7-abb23c7a90a7)

- **Total Budget vs Revenue**
  ![budget_revenue](https://github.com/user-attachments/assets/f22505b5-f21f-4bfc-9314-84e6d53bb8cc)

- **Total Budget vs Vote Average**
  ![budget_vote_average](https://github.com/user-attachments/assets/a60f7aa9-bd24-43ae-ac52-0c5b03ea5020)

- **Vote Average vs % Profit**
  
![profit_vote](https://github.com/user-attachments/assets/0f885258-3116-4d80-b847-2238069d6b63)

- **Gener vs Total Budget and Revenue**
![mean_budget_and_revenue_by_genre](https://github.com/user-attachments/assets/e47d7ed2-cf43-4107-b2b2-afce2ef3abe2)

- **Gener vs % % Profit**
![perct_profit_by_genre](https://github.com/user-attachments/assets/021002fe-d0b2-4361-86d6-6c474faa1def)

All visualizations are saved as PNG files in the `graphics` directory.

