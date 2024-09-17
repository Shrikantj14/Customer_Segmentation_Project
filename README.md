# Customer_Segmentation_Project
This project demonstrates customer segmentation using the K-means clustering algorithm applied to a real-world e-commerce sales dataset. The goal is to group customers based on their purchasing behavior to enable targeted marketing and improved customer relationship management.

Dataset
The dataset contains sales data from November 2018 to April 2019 with approximately 25,000 unique customers. For each customer, the following features were extracted:

Number of products ordered
Average return rate
Total spending
Project Steps
1. Business Case
The objective was to determine if customers can be grouped into distinct segments based on their purchasing behavior, enabling the company to develop customized relationships with each group.

2. Data Preparation
The dataset was cleaned and well-formatted, with no missing values.
The three key features (products ordered, return rate, and total spending) were extracted for each customer.
Since the data had varying scales, logarithmic transformation was applied to normalize the features, making them suitable for K-means clustering.
3. K-means Clustering
The K-means algorithm was used to segment customers. This algorithm forms clusters by minimizing the within-cluster sum of squared distances (inertia).
The model was initialized using the K-means++ method to improve centroid placement, with a maximum of 500 iterations per run.
4. Choosing Optimal Number of Clusters (k)
The elbow method was used to select the optimal number of clusters. By plotting inertia against different k-values, the optimal number of clusters was determined to be 4.
5. Segmentation Results
The customers were segmented into the following four clusters:

Cluster 1 (Blue): New customers with low spending and high return rates (42% of customers).
Cluster 2 (Red): Moderate spenders with few products ordered and a low return rate.
Cluster 3 (Purple): Customers similar to Cluster 2 but with slightly higher spending.
Cluster 4 (Green): High spenders with no product returns, making them the most valuable customers (8% of customers).
6. Strategy Recommendations
Blue group: Focus on reducing return rates and engaging newcomers with promotions or incentives to improve spending behavior.
Red & Purple groups: Keep these customers engaged through specialized communications, discounts, and personalized offers.
Green group: Maintain loyalty with special deals, early product launches, and VIP-like treatment to encourage continuous purchases.
Conclusion
This project demonstrates how K-means clustering can be used to segment customers based on their behavior, helping businesses develop tailored strategies for each customer group. By clustering customers into distinct segments, companies can increase revenue, improve customer retention, and provide personalized experiences.

Technologies Used
Python
scikit-learn
pandas
numpy
matplotlib
Plotly (for visualization)
How to Run the Project
Clone this repository.
Install the required dependencies:
bash
Copy code
pip install -r requirements.txt
Run the Jupyter Notebook to follow along with the steps or use the provided scripts to apply the model to your own datasets.
References
This project was inspired by a customer segmentation case study and interview task, and demonstrates the practical application of machine learning in e-commerce.
