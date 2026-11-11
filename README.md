Evaluating and comparing the effectiveness of XGBoost, Decision Tree, and Random Forest algorithms in predicting customer churn rates of telecom company dataset

1. Dataset: https://www.kaggle.com/datasets/blastchar/telco-customer-churn

2. Kiến trúc tổng quát:
   Hệ thống được xây dựng theo kiến trúc huấn luyện và đánh giá mô hình học máy cho bài toán dự đoán.

#### Pipeline xử lý và xây dựng mô hình:

```text
Input Data
    │
    ▼
EDA (Exploratory Data Analysis)
    │
    ▼
Xác định X và Y
    │
    ▼
Preprocessing
    │
    ▼
Chia Train / Test
    │
    ├──► Train XGBoost
    ├──► Train Decision Tree
    └──► Train Random Forest
          │
          ▼
Soft Voting Ensemble (Baseline)
    │
    ▼
So sánh và Đánh giá các Model
    │
    ├──► Biểu đồ so sánh
    ├──► Confusion Matrix
    └──► Error Analysis
    │
    ▼
Xử lý Imbalance Data
    │
    ▼
Model Tuning
    │
    ▼
Threshold Tuning
    │
    ▼
New Soft Voting (Improved Model)
    │
    ▼
So sánh Baseline và Improved Model
