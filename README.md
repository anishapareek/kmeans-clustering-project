# KMeans Clustering Project

This project demonstrates the use of KMeans Clustering to cluster universities into two groups: Private and Public.

## Overview

KMeans Clustering is an unsupervised learning algorithm used for clustering data into distinct groups. In this project, the algorithm is used to cluster universities based on various features, without using the labels (Private or Public) during the clustering process. The labels are only used at the end to evaluate the performance of the clustering.

### Note

While the dataset includes labels indicating whether a university is private or public, these labels are not used for the KMeans clustering algorithm itself, as it is an unsupervised learning method. However, the labels are used post-clustering to evaluate the algorithm's performance using a classification report and a confusion matrix.

## The Data

The dataset consists of 777 observations on the following 18 variables:

- **Private**: A factor with levels 'No' and 'Yes' indicating whether a university is private or public.
- **Apps**: Number of applications received.
- **Accept**: Number of applications accepted.
- **Enroll**: Number of new students enrolled.
- **Top10perc**: Percentage of new students from the top 10% of their high school class.
- **Top25perc**: Percentage of new students from the top 25% of their high school class.
- **F.Undergrad**: Number of full-time undergraduates.
- **P.Undergrad**: Number of part-time undergraduates.
- **Outstate**: Out-of-state tuition.
- **Room.Board**: Room and board costs.
- **Books**: Estimated book costs.
- **Personal**: Estimated personal spending.
- **PhD**: Percentage of faculty with Ph.D.’s.
- **Terminal**: Percentage of faculty with a terminal degree.
- **S.F.Ratio**: Student/faculty ratio.
- **perc.alumni**: Percentage of alumni who donate.
- **Expend**: Instructional expenditure per student.
- **Grad.Rate**: Graduation rate.

## Project Workflow

1. **Exploratory Data Analysis (EDA):**
   - A scatterplot of `Grad.Rate` vs. `Room.Board` with points colored by the `Private` column.
   - A scatterplot of `F.Undergrad` vs. `Outstate` with points colored by the `Private` column.
   - A stacked histogram showing out-of-state tuition based on the `Private` column.
   - Identification and correction of a data anomaly where a private school had a graduation rate greater than 100%.

2. **Model Training:**
   - Instantiation of a KMeans model with 2 clusters.
   - Training the KMeans model and obtaining the cluster center vectors.

3. **Model Evaluation:**
   - Although clustering is an unsupervised learning task and does not inherently provide a way to evaluate performance, the available labels are used to evaluate the clusters.
   - A confusion matrix and a classification report are printed to assess the clustering performance.

## Files in the Repository

- `K Means Clustering Project.ipynb`: The Jupyter Notebook containing the complete code and analysis.

## How to Run

1. Clone the repository.
2. Ensure you have the necessary dependencies installed (e.g., `scikit-learn`, `seaborn`, `matplotlib`, `pandas`).
3. Open the Jupyter Notebook `K Means Clustering Project.ipynb`.
4. Run the cells in the notebook to see the analysis and results.

## Conclusion

This project showcases the application of KMeans Clustering to categorize universities into private and public groups based on various features. While the labels were not used during the clustering process, they were utilized to evaluate the performance of the clustering, providing insight into the effectiveness of the KMeans algorithm for this dataset.
