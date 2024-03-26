# Sentiment Analysis using Twitter Data

## Problem and Dataset 
The primary objective of this project is to conduct sentiment analysis on Twitter data to discern the emotional tone of tweets. The dataset comprises 74,996 tweets initially, each with attributes including tweet ID, entity, sentiment, and tweet content. Sentiment categories analyzed are positive or negative, with "Neutral" and "Irrelevant" categories dropped. The dataset was pre-split into training and testing sets, with subsequent data cleaning steps including handling null values and encoding sentiment labels. After preprocessing, the dataset contains 43,506 entries, ready for model processing.

## Deep Learning Models
Two deep learning models were employed for sentiment analysis: Long Short-Term Memory (LSTM) and Transformer. LSTM, designed for sequential data, utilizes layers for sequence modeling and captures long-term dependencies. Transformers leverage attention mechanisms to process input data efficiently, capturing both global and local patterns effectively. Both models were chosen to compare their performance on sentiment analysis tasks.

## Implementation
The LSTM model is designed for binary sentiment classification, comprising embedding layers, LSTM layers with dropout for regularization, and a dense layer for binary classification. The Transformer model utilizes self-attention mechanisms, Token and Position Embedding layers, and Transformer blocks for multiclass sentiment classification. Both models are trained with the Adam optimizer, undergo five epochs with a batch size of 32, and employ different loss functions to accommodate their respective classification tasks.

## Evaluation
Evaluation metrics include accuracy and loss. The LSTM model demonstrates a steady improvement in accuracy over epochs, with decreasing loss values indicating improving sentiment prediction precision. The Transformer model exhibits consistently high accuracy with some variability in loss, potentially attributed to the nature of sentiment expressions in Twitter data. Overall, both models show similar high performance in sentiment analysis.

## Conclusion
Both LSTM and Transformer models perform exceptionally well in sentiment analysis, achieving approximately 98% accuracy. The LSTM model slightly outperforms in loss function optimization. These models provide valuable insights into consumer sentiments, aiding in decision-making, understanding customer needs, and brand monitoring. Lessons learned in model optimization and performance tuning are highlighted, along with potential avenues for future research, such as incorporating neutral sentiment and exploring additional deep learning architectures like Convolutional Neural Networks (CNN). Comprehensive evaluation using confusion matrices and classification reports can further enrich model assessment in sentiment analysis tasks.

## Notes
* For replication and further exploration, various model configurations were tested, including different numbers of layers, epochs, and batch sizes.
* Future iterations of the study may include additional models and incorporate neutral sentiment for enhanced sentiment analysis accuracy.
* Detailed model performance evaluation using confusion matrices and classification reports can provide deeper insights into model strengths and weaknesses.
