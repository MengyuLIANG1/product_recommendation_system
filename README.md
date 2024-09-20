# product_recommendation_system

## Project Overview:
The Product Recommendation System is designed to provide personalized product recommendations to users based on product attributes such as images and metadata (e.g., category, gender, etc.). The system leverages machine learning techniques to analyze product embeddings, identifying items that are visually or contextually similar to the one the user is currently viewing or has previously interacted with.

## Key Features:
### Image-Based Recommendations:

Extract visual features from product images using convolutional neural networks (pretrained Resnet50).
Generate image embeddings that capture the visual characteristics of each product.
Recommend visually similar products by calculating similarity metrics between image embeddings.

### Metadata-Based Recommendations:

Leverage product metadata (e.g., masterCategory, gender, season) to enhance the recommendations.
Generate metadata embeddings using one-hot encoding .
Combine image and metadata embeddings to improve recommendation relevance.

### recommandation

Provide the recommendation products based on cosine similarity.
