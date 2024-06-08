# Recommendation--system

 Recommendation System for E-commerce using Deep Learning

# Description

This project builds a recommendation system for e-commerce, specifically predicting the next products a user might buy based on their purchase history. The project uses deep learning techniques, specifically LSTM networks, to model sequential data of product purchases.

# Dataset

Amazon Beauty Products dataset  from Kaggle: (https://www.kaggle.com/skillsmuggler/amazon-ratings)

# Workflow

1. Data Loading and Preprocessing: Load the dataset, clean it, and aggregate product IDs for each user.
2. Tokenization and Sequence Preparation: Tokenize product IDs and prepare padded sequences for model training.
3. Model Building and Training: Define and train an LSTM model to predict the next product.
4. Prediction: Use the trained model to predict the next `n` products for a given user sequence.

 # Code Structure

•	google.colab.drive: Mounts Google Drive to access datasets.
•	pandas, numpy, sklearn, tensorflow: Libraries used for data processing and model building.
•	Tokenization and Padding: Convert product IDs to sequences and pad them for equal length.
•	LSTM Model: Sequential model with Embedding, LSTM, and Dense layers.
•	Prediction Functions: Functions to predict the next product or the next `n` products a user might buy.

# How to Run

1. Load the dataset from Google Drive.
2. Preprocess the data by removing unnecessary columns and aggregating product IDs.
3. Tokenize product IDs and prepare sequences.
4. Build and train the LSTM model.
5. Use the trained model to predict the next products.

# Example Usage

# python
# Predict the next 5 products
sample_sequence = ['B001E4KFG0', 'B000VJRN2I', 'B0016B2C1K']  # Example product sequence

next_products = predict_next_n_products(model, tokenizer, sample_sequence, max_sequence_len, 5)

print(f'Next 5 product predictions: {next_products}')




