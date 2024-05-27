# ALGORITHMS & DATA STRUCTURES IN PYTHON
## Project Overview
In this project, we apply our knowledge of algorithms and data structures to analyze a dataset containing the purchase history of a hypothetical Students' Union. The analysis is implemented using a Jupyter Notebook provided by the professor, and the code is enhanced with clear and concise comments for readability and understanding.

## Dataset Description
The dataset is a list of dictionaries, with each dictionary representing a single purchase. Each purchase contains the following information:
  1. Name: The name of the student (string). Each name is assumed to be unique, although multiple purchases can be associated with the same name.
  2. Date: The date of the purchase (tuple of three integers: DD, MM, YYYY). The dataset includes purchases made between January 1st, 2023, and May 1st, 2023.
  3. Item: The name of the purchased item (string).
  4. Unit Price: The price per unit of the item (floating-point number in Euros).
  5. Quantity: The number of items purchased (integer).

## Project Tasks
### Information Extraction
  1. Recency: Calculate the number of days since each student's latest purchase, using May 1st, 2023, as the current date.
  2. Frequency: Calculate the total number of purchases made by each student within the given date interval.
  3. Monetary Value: Calculate the total amount spent by each student on purchases within the given date interval.

### Data Visualization
Plot histograms for recency, frequency, and monetary value using Matplotlib.

### Sorting and Scoring
1. First RFM Score (RFM):
  - Recency: Sort students by recency and divide into three equal parts. Assign scores: 3 for the most recent, 2 for the middle, and 1 for the least recent.
  - Frequency: Sort students by frequency and divide into three equal parts. Assign scores: 3 for the most frequent, 2 for the middle, and 1 for the least frequent.
  - Monetary Value: Sort students by monetary value and divide into three equal parts. Assign scores: 3 for the highest spenders, 2 for the middle, and 1 for the lowest spenders.
  - Combine the scores to get the RFM score and sort students in descending order of their RFM scores.
2. Second RFM Score (RFM'):
  - Recency: Rank students by recency and divide into three buckets.
  - Frequency: Within each recency bucket, rank students by frequency and create three frequency buckets.
  - Monetary Value: Within each frequency bucket, rank students by monetary value and create three monetary buckets.
  - Recalculate the RFM scores and use scipy.stats.spearmanr to correlate RFM and RFM'.

### Searching
1. Linear Search: Find the RFM scores of your group members using linear search.
2. Binary Search: Sort students in alphabetical order.
3. Search for your group members using binary search and find their RFM scores.
4. Compare the time taken for linear search and binary search using the timeit module.

### Libraries and Restrictions
1. You are allowed to use NumPy and Matplotlib for this project.
2. The use of pandas is not permitted.

### Feel free to explore the code in the provided Jupyter Notebook and refer to the comments for detailed explanations of each step.
