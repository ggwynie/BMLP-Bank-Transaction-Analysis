# Bank Transaction Analysis: Fraud Detection Using Machine Learning

## Project Overview

This project analyzes banking transaction data to identify patterns and anomalies that could indicate fraudulent activities. Using a dataset of 2,512 bank transactions with 16 features, I developed two complementary machine learning approaches: unsupervised clustering to discover natural groupings in transaction behavior, and supervised classification to predict transaction categories.

The work demonstrates practical application of machine learning techniques to address real-world financial security challenges, where detecting fraudulent transactions early can prevent significant financial losses and protect customer accounts.

## Business Impact

Financial institutions face substantial losses from fraudulent transactions. This analysis provides:

- Automated pattern recognition to identify suspicious transaction clusters
- Predictive models that can flag high-risk transactions in real-time
- Insight into behavioral characteristics that distinguish normal from anomalous transactions
- Scalable framework applicable to larger transaction datasets

Early detection of fraud patterns can reduce investigation costs and prevent losses before they occur. The clustering analysis reveals distinct customer segments based on transaction behavior, enabling more targeted fraud prevention strategies.

## Technical Approach

### Dataset

The dataset contains 2,512 banking transactions with features including:

- Transaction metadata: amount, date, type (credit/debit), duration
- Account information: ID, balance, previous transaction date
- Channel details: location, device ID, IP address, merchant ID, transaction channel
- Customer profile: age, occupation, login attempts

### Methodology

**Clustering Analysis**

Applied K-Means clustering to identify natural groupings in transaction patterns. Used the Elbow Method to determine optimal cluster count and implemented PCA for dimensionality reduction to visualize high-dimensional transaction data. Evaluated cluster quality using silhouette scores.

**Classification Analysis**

Built and compared multiple supervised learning models to predict transaction categories. Tested Decision Trees, Random Forest, and hyperparameter-tuned variants. Evaluated performance using accuracy metrics and confusion matrices to understand model behavior across different transaction types.

### Technology Stack

- Python 3.x
- Data processing: pandas, numpy
- Machine learning: scikit-learn (KMeans, PCA, Decision Tree, Random Forest, StandardScaler, LabelEncoder)
- Visualization: matplotlib, seaborn, yellowbrick
- Model persistence: joblib

## Repository Structure

```
notebooks/
  [Clustering]_Submission_Akhir_BMLP_Gwyneth_Eunice_Widjaja.ipynb
  [Klasifikasi]_Submission_Akhir_BMLP_Gwyneth_Eunice_Widjaja.ipynb

data/
  bank_transactions_data_edited.csv
  bank_transactions_data_edited_.xlsx
  data_clustering.csv
  data_clustering_inverse.csv

models/
  model_clustering.h5
  PCA_model_clustering.h5
  decision_tree_model.h5
  explore_random_forest_classification.h5
  tuning_classification.h5
```

## Running the Analysis

Install dependencies:
```bash
pip install -r requirements.txt
```

Run notebooks in order:
1. Clustering analysis notebook
2. Classification analysis notebook

Both notebooks load data directly from remote sources for reproducibility.

## Results

**Clustering Analysis**

Successfully segmented transactions into distinct behavioral clusters. The PCA-reduced visualization reveals clear separation between transaction types, with silhouette scores indicating strong cluster cohesion.

**Classification Analysis**

Compared multiple classification approaches. Random Forest with hyperparameter tuning achieved the best performance, demonstrating the value of ensemble methods and optimization for this transaction classification task.

## Future Improvements

- Real-time transaction scoring system
- Feature engineering incorporating temporal patterns
- Deep learning approaches for sequence-based fraud detection
- Integration with streaming data pipelines

## Author

Gwyneth Eunice Widjaja

Completed as part of Dicoding's Machine Learning for Beginners course.
