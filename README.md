# product_recommendation_system

## Project Overview:
The Product Recommendation System is designed to provide personalized product recommendations to users based on product attributes such as images and metadata (e.g., category, gender, etc.). The system leverages machine learning techniques to analyze product embeddings, identifying items that are visually or contextually similar to the one the user is currently viewing or has previously interacted with.

## Dataset:
The dataset is obtained from Kaggle: [Fashion Product Images Dataset](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset). It contains:

Images: Around 44,000 high-resolution images of fashion products with a size of 2400x1600 pixels.

Metadata: Each image is accompanied by metadata including the product category, subcategory, article type, and base color.

**Note:** Given the computational constraints and the size of the dataset, we have decided to adopt a sampling strategy for our analysis. Specifically, we will use 10% of the data from each subCategory. This approach ensures that the distribution of the data across different categories is maintained while significantly reducing the volume of data to be processed. By doing so, we aim to balance between computational efficiency and maintaining enough data for meaningful insights.

## Key Features:
### Image-Based Recommendations:

* Extract visual features from product images using convolutional neural networks (pretrained Resnet50 or VGG16).
* Generate image embeddings that capture the visual characteristics of each product.
* Recommend visually similar products by calculating similarity metrics between image embeddings.

### Metadata-Based Recommendations:

* Leverage product metadata (e.g., masterCategory, gender, season) to enhance the recommendations.
* Generate metadata embeddings using one-hot encoding .
* Combine image and metadata embeddings to improve recommendation relevance.

### Recommandation

Provide the recommendation products based on cosine similarity.
