# Project Name: Customer Segmentation Analysis

## Introduction
This project involves analyzing customer data to identify segmentation using clustering techniques. The analysis is conducted using Python with libraries such as Pandas and Scikit-learn. It aims to understand customer behavior and group similar customers based on various metrics like average amount spent, booking channels, travel destinations, and membership statuses.

## Requirements
- Python 3.x
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## Installation
To set up the project environment:
1. Ensure Python 3.x is installed on your system.
2. Install the required Python libraries using pip:
   ```
   pip install pandas scikit-learn matplotlib seaborn
   ```

## Usage
Run the Python scripts to perform clustering and visualization:
1. Load the data using Pandas:
   ```python
   import pandas as pd
   data_df = pd.read_csv("Clustering Data.csv")
   ```
2. Perform data preprocessing and clustering:
   ```python
   from sklearn.cluster import KMeans
   kmeans = KMeans(n_clusters=5, random_state=77)
   dummy_df['cluster'] = kmeans.fit_predict(dummy_df.drop(['uid'], axis=1))
   ```
3. Visualize the results using Matplotlib and Seaborn:
   ```python
   import matplotlib.pyplot as plt
   import seaborn as sns
   sns.countplot(x='cluster', data=dummy_df)
   plt.show()
   ```

## Contributing
Contributions to this project are welcome! To contribute, please fork the repository, make your changes, and submit a pull request.

## Contact
For any queries, you can reach out at patil.anurag.auto@gmail.com.

---

