
# ACI Motors Data Analysis Project

This project is a comprehensive data analytics pipeline built for **ACI Motors** to uncover actionable business insights from various datasets, including credit risk, fraud detection, market segmentation, financial monitoring, and customer sentiment.

## 🧠 Sections Covered

### 🔹 SECTION A — Tractor Credit Risk Analysis
- Calculates EMI Paid Ratio and Risk Scores
- Segments customers into `Low`, `Medium`, and `High` risk categories
- Aggregates average payment delays by risk level

### 🔹 SECTION B — Dealership Fraud Pattern Detection
- Identifies dealerships with high instances of NID/Phone duplication
- Computes suspicious activity rate and visualizes top 10 risky dealers

### 🔹 SECTION C — Location-Based Market Segmentation
- Segments Yamaha customers using K-Means clustering
- Labels customers as:
  - **Premium Enthusiasts**
  - **Frequent Browsers**
  - **Budget Commuters**
- Recommends high-potential upazilas for targeted campaigns

### 🔹 SECTION D — Financial Monitoring & ROI Analysis
- Analyzes regional Return on Investment (ROI)
- Evaluates profit vs. marketing spend correlation
- Visualizes KPIs with Plotly dashboards

### 🔹 SECTION E — Customer Feedback Sentiment & Topic Modeling
- Cleans and pre-processes feedback data
- Performs sentiment analysis using **VADER**
- Generates positive & negative word clouds
- Applies topic modeling (TF-IDF + K-Means) to find complaint themes

---

## 🗂️ Data Files Required

Please ensure the following CSV files are available in your working directory or update the script paths accordingly:

- `tractor_credit_data.csv`
- `dealer_transaction_data.csv`
- `yamaha_customer_data_with_geo.csv`
- `financial_tracking_data.csv`
- `yamaha_mock_customer_feedback.csv`

---

## 🛠️ Setup & Dependencies

Run the following to install required Python libraries:

```bash
pip install pandas numpy pandasql nltk matplotlib seaborn plotly wordcloud scikit-learn vaderSentiment
```

Also download required NLTK resources:

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```

---

## 🚀 Running the Script

To execute the entire analysis:

```bash
python aci_task.py
```

The script will:
- Load datasets
- Clean and transform data
- Perform various analytics tasks
- Save output images such as:
  - `top_10_dealers_suspicious_activity_rate.png`
  - `wordcloud_positive.png`
  - `wordcloud_negative.png`
  - `sentiment_by_product_category.png`
- Export results like:
  - `top_upazilas.csv`

---

## 📊 Output Highlights

- **Dashboards:** Interactive visualizations (via Plotly)
- **Customer Clustering:** Market segmentation insights
- **Fraud Detection:** Dealer-level anomaly detection
- **Sentiment Analysis:** Text mining & visualization

---

## 👨‍💼 Business Impact

This project equips ACI Motors with:

- Better credit risk profiling
- Fraudulent dealer monitoring
- Geolocation-based marketing strategy
- Financial performance analysis
- Voice-of-customer insights to guide product and service improvement

---

## 📬 Contact

*Author:* Pranta Khandaker  
*Role:* AI / Data Engineer  
*Email:* [Insert your email or LinkedIn]

---
