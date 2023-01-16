# data-analyst-exercise
This exercise will involve merging the data from two data files and producing some simple
visualizations.
## Data Files
The purchase history from two point of sale systems are contained in the following files `detroit_purchases.csv` and
`new_york_purchases.csv`. It is important to note that the timestamps contained in `detroit_purchases.csv` should be
assumed to be in the eastern time zone.
Both files have a `type` field that represents product categorization. However, each file has a different level of
granularity with respect to this field. There are two levels of granularity: a product line such as "bakery" which
contains multiple lower levels of categories such as "cakes" and "pizza". How to map one type to the other is
represented by the `mapping.yml` file.
### Assignment
Use either Python or R to complete the following:
1. Merge the two CSV files into a single dataset. Use the mapping YAML file to normalize the type field to a product
line.
2. Filter the data such that it only contains transactions for 1/2/2023.
3. Using the merged and filtered data, create two histograms:
   1. Total revenue in each product line for 1/2.
   2. Total number of items purchased for each hour of the day on 1/2.
4. Create a GitHub repository with your scripts/notebooks.