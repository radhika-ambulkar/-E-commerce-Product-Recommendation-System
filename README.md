This is my second internship project at Next24tech Technology and Services. This project deals with the house price prediction using data analytics and ML algorithm.
The dataset contains 1465 entries and 16 columns, primarily focused on product information, user reviews, and pricing data. Here's a breakdown of the columns:

1. **product_id**: Unique identifier for the product.
2. **product_name**: The name of the product.
3. **category**: Product categories.
4. **discounted_price**: The discounted price of the product.
5. **actual_price**: The original price of the product.
6. **discount_percentage**: The discount percentage.
7. **rating**: The product rating.
8. **rating_count**: The number of ratings the product has received.
9. **about_product**: Product description or key features.
10. **user_id**: The user who reviewed the product.
11. **user_name**: Name of users who reviewed the product.
12. **review_id**: Review ID associated with each user review.
13. **review_title**: Title of the user review.
14. **review_content**: Content of the user review.
15. **img_link**: Link to the product image.
16. **product_link**: Link to the product page.

### Step-by-Step Process to Develop the E-Commerce Recommendation System

#### 1. **Data Preprocessing**
   - **Convert price columns** (`discounted_price`, `actual_price`) into numerical values by removing currency symbols.
   - **Handle missing values**: Clean columns like `rating_count`, which may have missing data.
   - **Convert ratings** to float.
   - **Create interaction matrix** for users and products using `user_id` and `product_id`.

#### 2. **Exploratory Data Analysis (EDA)**
   - Analyze product popularity, ratings, and sales trends.
   - Understand user interaction with products based on reviews and ratings.

#### 3. **Recommendation System Approaches**
   - **Collaborative Filtering**:
     - Based on user-product interactions (using `user_id`, `product_id`, and ratings).
   - **Content-Based Filtering**:
     - Recommend products based on product attributes (like `category`, `about_product`).

#### 4. **Model Training**
   - Train the model using algorithms like **Matrix Factorization (SVD)** or **KNN** for collaborative filtering.
   - For content-based, use similarity measures like **TF-IDF** or **Cosine Similarity** on the product descriptions.

#### 5. **Evaluation**
   - Use metrics like **Precision@K** or **Recall@K** to evaluate the system’s recommendations.
   - A/B test the recommendations in a real environment to assess performance.

#### 6. **Deployment**
   - Deploy the model in production, integrating it with the platform’s user interface for real-time recommendations.

I’ll start with preprocessing the dataset. Shall I proceed?
