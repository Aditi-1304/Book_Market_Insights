# Book Market Insights Dashboard

## Project Overview

This project analyzes a dataset of book sales and ratings to provide actionable insights for businesses in the publishing industry, such as bookstores, online booksellers, or publishing houses. By leveraging data cleaning, exploratory data analysis (EDA), and interactive dashboard creation, this project aims to identify top-performing books, authors, and genres, understand customer preferences, and uncover market trends to inform strategic decisions.

## Problem Statement

In the competitive book market, understanding consumer behavior, identifying best-selling titles, and recognizing reader preferences are crucial for business success. This project addresses the need for data-driven insights to optimize purchasing, marketing, and inventory management, ultimately aiming to increase sales and profitability.

## Data Source

The dataset used for this analysis is "Books Sales and Ratings" from Kaggle.

- **Kaggle Link:** [https://www.kaggle.com/datasets/thedevastator/books-sales-and-ratings/data](https://www.kaggle.com/datasets/thedevastator/books-sales-and-ratings/data)

## Tools & Technologies

- **Programming Language:** Python
- **Libraries:** `pandas` (for data manipulation), `numpy` (for numerical operations), `matplotlib` (for basic plotting), `seaborn` (for advanced visualizations).
- **Interactive Dashboard:** Microsoft Power BI Desktop
- **Development Environment:** VS Code (with Jupyter Notebooks extension)
- **Version Control:** Git & GitHub

## Project Structure

The repository is organized as follows:
Okay, this is the final crucial step for showcasing your project! A well-crafted README.md on GitHub is your project's resume. It tells the story of your analysis, highlights your skills, and provides a quick overview for recruiters and hiring managers.

Here's a comprehensive README.md content template tailored for your "Book Market Insights" project, including sections for your .ipynb, data, and .pbix files.

Markdown

# Book Market Insights Dashboard

## Project Overview

This project analyzes a dataset of book sales and ratings to provide actionable insights for businesses in the publishing industry, such as bookstores, online booksellers, or publishing houses. By leveraging data cleaning, exploratory data analysis (EDA), and interactive dashboard creation, this project aims to identify top-performing books, authors, and genres, understand customer preferences, and uncover market trends to inform strategic decisions.

## Problem Statement

In the competitive book market, understanding consumer behavior, identifying best-selling titles, and recognizing reader preferences are crucial for business success. This project addresses the need for data-driven insights to optimize purchasing, marketing, and inventory management, ultimately aiming to increase sales and profitability.

## Data Source

The dataset used for this analysis is "Books Sales and Ratings" from Kaggle.

- **Kaggle Link:** [https://www.kaggle.com/datasets/thedevastator/books-sales-and-ratings/data](https://www.kaggle.com/datasets/thedevastator/books-sales-and-ratings/data)

## Tools & Technologies

- **Programming Language:** Python
- **Libraries:** `pandas` (for data manipulation), `numpy` (for numerical operations), `matplotlib` (for basic plotting), `seaborn` (for advanced visualizations).
- **Interactive Dashboard:** Microsoft Power BI Desktop
- **Development Environment:** VS Code (with Jupyter Notebooks extension)
- **Version Control:** Git & GitHub

## Methodology

The project followed a structured approach:

1.  **Data Acquisition:** Downloaded the "Books Sales and Ratings" dataset from Kaggle.
2.  **Data Cleaning & Preprocessing (Python - `book_data_cleaning_and_feature_engineering.ipynb`):**
    - Handled missing values (e.g., `Publishing Year`, `Book Name`, `language_code`).
    - Cleaned and standardized column names (e.g., stripping whitespace from 'Publisher ').
    - Converted data types (e.g., `Publishing Year` to integer).
    - Engineered new features such as `Primary Author`, `Rating Category`, `Total Revenue`, `Publisher Profit`, and `Books Sold`.
    - Saved the cleaned data to `cleaned_books_data_for_powerbi.csv`.
3.  **Exploratory Data Analysis (EDA) (Python - `book_eda.ipynb`):**
    - Performed univariate analysis to understand distributions of key metrics (ratings, sales, units).
    - Conducted bivariate analysis to identify relationships (e.g., `Book_average_rating` vs. `units sold`).
    - Identified top authors and genres by various metrics.
    - Explored trends over `Publishing Year`.
    - Generated hypotheses and discovered potential "hidden gems" (highly-rated books with lower sales).
4.  **Power BI Dashboard Development (`Book_Market_Insights_Dashboard.pbix`):**
    - Imported the `cleaned_books_data_for_powerbi.csv` into Power BI Desktop.
    - Created necessary DAX measures for KPIs and aggregated metrics.
    - Designed three interactive dashboard pages:
      - **Page 1: Overview & Key Performance:** High-level market snapshot with key KPIs, overall trends, and top genres/authors.
      - **Page 2: Author & Genre Deep Dive:** Detailed analysis of author and genre performance, including average ratings and units sold.
      - **Page 3: Key Trends & Actionable Recommendations:** Visualized relationships (e.g., rating vs. units sold), highlighted "hidden gems," and provided explicit actionable insights.

## Key Findings & Insights

Based on the analysis, here are some key insights into the book market:

- **Average Rating Distribution:** The majority of books in the dataset exhibit an average rating between X and Y, indicating a generally positive reader reception.
- **Sales vs. Reviews:** There is a strong positive correlation between the number of ratings a book receives and its total units sold, suggesting that reader engagement significantly impacts commercial success.
- **Top Genres:** The 'Fiction' genre (including 'genre fiction') consistently leads in terms of both the number of books published and total units sold, followed by 'Nonfiction'.
- **Author Impact:** Authors classified as 'Famous' or 'Excellent' consistently demonstrate higher average units sold compared to 'Novice' or 'Intermediate' authors, underlining the importance of author reputation.
- **Publishing Trends:** The number of books published has shown a [increase/decrease/stable trend] since [Year], with a peak around [Year/Period], indicating evolving market dynamics.
- **Hidden Gems:** Identified several highly-rated books with relatively low units sold. These titles represent potential untapped marketing opportunities, as they are well-received but might lack visibility. (Refer to Page 3 of the dashboard for specific examples).

## Actionable Recommendations

Leveraging these insights, the following recommendations can be made to a book-related business:

1.  **Strategic Marketing for "Hidden Gems":** Invest in targeted promotional campaigns for highly-rated books that currently have lower sales/review counts. These books have proven quality and could see significant sales growth with increased exposure.
2.  **Focus on Engagement for New Releases:** Implement strategies to encourage reader reviews and engagement for new book releases. Given the strong correlation between `Book_ratings_count` and `units sold`, early engagement can be crucial for long-term sales.
3.  **Genre-Specific Procurement/Marketing:** Continue to prioritize procurement and marketing efforts in top-performing genres like 'Fiction'. Simultaneously, explore opportunities within highly-rated niche genres (identified on Page 2) to cater to specific reader preferences.
4.  **Leverage Author Reputation:** Partner with 'Famous' and 'Excellent' authors for new titles or promotions, as their established readership tends to drive higher unit sales. Consider mentorship programs or collaborative marketing with 'Intermediate' authors who show promising average ratings.

## Dashboard Preview

Here's a sneak peek at the interactive Power BI dashboard:

![Power BI Dashboard Page 1 Screenshot](powerbi_reports/dashboard_page_1.png)
_(Replace `powerbi_reports/dashboard_page_1.png` with the actual path to your screenshot. It's best to have 1-3 screenshots, one for each page, or a combined one if possible)._

## How to View/Run the Project

To explore this project:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/your-username/Book_Market_Insights.git](https://github.com/your-username/Book_Market_Insights.git)
    cd Book_Market_Insights
    ```
2.  **Download Raw Data:**
    - Download the `books.csv` (or whatever your original file is named) from the Kaggle link provided in the "Data Source" section.
    - Place this file into the `data/` directory of your cloned repository.
3.  **Run Python Notebooks (for data processing):**
    - Ensure you have Python (3.x recommended) and the required libraries (`pandas`, `numpy`, ``matplotlib`, `seaborn`) installed (`pip install pandas numpy matplotlib seaborn`).
    - Open the `Book_Market_Insights` folder in VS Code.
    - Navigate to the `notebooks/` folder and open `book_data_cleaning_and_feature_engineering.ipynb`. Run all cells to process the raw data and generate `cleaned_books_data_for_powerbi.csv`.
    - Next, open `book_eda.ipynb` in the `notebooks/` folder and run all cells to see the detailed exploratory data analysis and insights.
4.  **View Power BI Dashboard:**
    - Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
    - Open the `powerbi_reports/Book_Market_Insights_Dashboard.pbix` file using Power BI Desktop to interact with the dashboard.

## Challenges & Learnings

- **Data Consistency:** Handling inconsistencies like the trailing space in the 'Publisher ' column required careful inspection and robust cleaning techniques.
- **Feature Engineering:** Deriving meaningful features like `Primary Author`, `Rating Category`, and ensuring accurate `Books Sold` from available data was crucial for deeper analysis.
- **Storytelling with Data:** The project emphasized not just analysis but also the importance of presenting complex insights in a clear, actionable, and visually appealing manner through Power BI.

---

### **About Me**

- <b>Me</b> : Aditi Agrawal <br>
- [LinkedIn](https://www.linkedin.com/in/aditi-agr)<br>
- [Portfolio Website](https://aditi-1304.github.io/index.html)

---
