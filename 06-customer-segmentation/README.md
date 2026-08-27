## Project Summary

The goal of this project was to segment customers based on their **age, annual income, and spending behavior** using the K-Means clustering algorithm.

During EDA, the dataset was analyzed to understand the distributions, relationships, and potential outliers. `CustomerID` was excluded from the clustering process. The selected numerical features were standardized using `StandardScaler` before applying K-Means.

The **Elbow Method** and **Silhouette Score** were used to determine the optimal number of clusters. Both methods indicated that **6 clusters** provided a suitable segmentation.

The final model identified six distinct customer segments, including **high-income/high-spending customers**, **high-income/low-spending customers**, and **low-income/high-spending customers**. The results show that customers can have significantly different spending behaviors despite having similar income levels.

Overall, the project demonstrates how **unsupervised learning can be used to identify meaningful customer groups** and provide insights that could support targeted marketing and customer strategies.