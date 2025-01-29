# caltech-data-science-ecommerce-marketing-campaign
This project is a Caltech applied data science project using Python. The main objective was to conduct exploratory data analysis, hypothesis testing, and data visualization to enhance comprehension of the diverse factors influencing a store’s customer acquisition and average spend across product categories and sales channels. We were not given the name or type of store, but based on the products and data visualization at the end, I concluded it was most likely a wine/liquor store that also offered a few other grocery items.

Key Tools Used:
- Python
- Pandas
- NumPy
- MatplotLib
- Seaborn
- Scikit-Learn
- Regression Analysis
- Pearson Correlation Coefficient

Writeup (charts and a more detailed analysis can be found in the "Marketing Campaign Project PDF"):

After importing the relevant libraries (Pandas, NumPy, Seaborn, MatplotLib, DateTime), I conducted missing value imputation and data cleaning, along with converting data types to their proper format. I found the unique values in key categories like Education, Marital Status, and Income to remove outliers and typos, as well as group categories with similar existing cateogires to standardize for simplicity.

I then created new variables to represent a customers' total number of children, customers' age, and a customers' total amount of money spent across the different products.

Continuing with data cleaning, I analyzed and removed outliers that were drastically skewing the data so I could better analyze the distributions and make more accurate predicitons with the data.

I also applied ordinal encoding on Education and One-Hot encoding on Marital Status and Country.

Now that all my data was clean and in proper formatting I was able to visualize the data and test different hypotheses on the dataset correlations. I did this in multiple ways, broken down below:
- Correlation Matrix Heatmaps
- Scatter plots (with Pearson's Correlation)
- Regression analysis
- Bar charts
- Box plots
- Violin plots

Conclusions based on the data visualizations:
- Older customers prefer shopping in the store as opposed to a catelog or online, BUT, they are beginning to use the web more and adjust with the changing technologies.
- Shopping across all channels decreases as the number of children a customer has increases. Parents with more children are busier and have less time for shopping, so they may have someone else do their shopping for them so they can focus on their children. Or, they don't buy as much alcohol as they have more children.
- Physical store shopping is NOT at risk of cannibalization by other sales channels. If anything, they are complementary.
- This is a global store, and purchases from the U.S. are dwarfed by sales from the rest of the world.
- The best selling product at this store is Wine, followed by Meat Products. Fruit is the worst selling product.
- There is no correlation between a customers' age and their willingess to spend money due to a campaign ad. More people accept the campaign than decline it, regardless of age.
- Spain has the highest number of customers who spent money due to an ad campaign.
- The fewer children a customer has, the more they will spend in the store.
- Customers with a graduate-level education file the most complaints.


