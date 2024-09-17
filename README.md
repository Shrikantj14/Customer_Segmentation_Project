
# Customer Segmentation Using K-means Clustering

This project demonstrates customer segmentation using the **K-means clustering algorithm**, applied to a real-world e-commerce sales dataset. The goal is to group customers based on their purchasing behavior, enabling targeted marketing and improved customer relationship management.

## Dataset

The dataset contains sales data from **November 2018 to April 2019**, with approximately **25,000 unique customers**. For each customer, the following features were extracted:
- **Number of products ordered**
- **Average return rate**
- **Total spending**

## Project Steps

### 1. Business Case
The objective was to determine if customers can be grouped into distinct segments based on their purchasing behavior. This allows the company to develop customized relationships with each customer segment.

### 2. Data Preparation
- The dataset was clean and well-formatted, with no missing values.
- Three key features were extracted for each customer:
  1. **Number of products ordered**
  2. **Average return rate**
  3. **Total spending**
  
- As these features had different scales, **logarithmic transformation** was applied to normalize them. This ensures that the K-means algorithm performs effectively by treating each feature with equal importance.

### 3. K-means Clustering
- The **K-means algorithm** from `scikit-learn` was used to segment customers.
- The model was initialized using **K-means++** to optimize the placement of centroids.
- The maximum number of iterations was set to **500** to ensure convergence.

### 4. Choosing the Optimal Number of Clusters (k)
- The **elbow method** was used to determine the optimal number of clusters.
- By plotting inertia (within-cluster sum of squared distances) against different k-values, the optimal number of clusters was found to be **4**.

### 5. Segmentation Results
The customers were segmented into the following four clusters:

- **Cluster 1 (Blue)**: New customers with low spending and high return rates (42% of customers).
- **Cluster 2 (Red)**: Moderate spenders who ordered few products and had a low return rate.
- **Cluster 3 (Purple)**: Similar to Cluster 2 but with slightly higher spending.
- **Cluster 4 (Green)**: High spenders with no product returns, forming the most valuable group (8% of customers).

### 6. Strategy Recommendations
- **Blue group**: Focus on reducing return rates and engaging newcomers with promotions to encourage more spending.
- **Red & Purple groups**: Keep these customers engaged through specialized communications and personalized discounts.
- **Green group**: Maintain loyalty through exclusive deals, early product launches, and premium treatment to encourage continuous purchases.

## Conclusion
This project demonstrates how **K-means clustering** can be used to segment customers based on their behavior. By clustering customers into distinct segments, businesses can increase revenue, improve customer retention, and provide personalized experiences.

## Technologies Used
- **Python**
- **scikit-learn**
- **pandas**
- **numpy**
- **matplotlib**
- **Plotly** (for visualization)

## How to Run the Project

1. Clone this repository.
   ```bash
   git clone https://github.com/your-username/customer-segmentation-kmeans.git
   cd customer-segmentation-kmeans
2. Install the required dependencies: pip install -r requirements.txt
3. Run the Jupyter Notebook or Python script to apply the model to the dataset:
4. Follow the steps in the notebook or script to reproduce the results and apply the model to your data.
