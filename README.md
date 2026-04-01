**Recommendation System using Collaborative Filtering**

**Project Overview**

This project implements a **movie recommendation system** using **Collaborative Filtering techniques** on the MovieLens dataset.
It explores how user behavior and item similarity can be leveraged to generate personalized recommendations.

**Objective**

1. To build a recommendation system using **User-Based** and **Item-Based Collaborative Filtering**
2. To understand how similarity between users/items influences recommendations
3. To evaluate model performance using standard metrics like RMSE, MAE, and Precision@K
4. To analyze challenges such as sparsity and cold-start problems

**Dataset**

* **MovieLens 100K Dataset**
* Contains:

  * User ID
  * Movie ID
  * Rating
  * Timestamp

**Methodology**

**User-Based Collaborative Filtering**

* Constructed a **User-Item Matrix**
* Handled missing values
* Computed similarity between users using **Cosine Similarity**
* Identified top similar users
* Predicted ratings for unseen movies
* Generated personalized recommendations

**Item-Based Collaborative Filtering**

* Constructed an **Item-User Matrix**
* Computed similarity between items (Cosine / Pearson)
* Identified similar movies
* Recommended items based on user history

**Evaluation Metrics**

* **RMSE (Root Mean Square Error)** → measures prediction accuracy
* **MAE (Mean Absolute Error)** → measures average error
* **Precision@K** → measures relevance of recommendations

**Analysis & Insights**

* Sparse matrices reduce recommendation accuracy
* Similarity measure plays a key role in performance
* Item-based filtering performs better for scalability
* Recommendations vary depending on user activity

**Visualizations**

* User-Item Matrix Heatmap
* Item Similarity Matrix
* Top Recommended Movies
* Similar Items Graph

**Challenges**

* **Sparsity Problem:** Most users rate very few items
* **Cold-Start Problem:** New users/items lack data
* **Prediction Accuracy:** Naive approaches lead to high RMSE

**Improvements**

* Implement weighted rating prediction (improves RMSE)
* Use Pearson correlation instead of cosine similarity
* Apply matrix factorization techniques (SVD)
* Build hybrid recommendation systems

**Conclusion**

This project demonstrates how collaborative filtering can effectively generate recommendations using user behavior and item similarity.
While simple approaches provide baseline results, improvements in similarity computation and prediction methods significantly enhance performance.
