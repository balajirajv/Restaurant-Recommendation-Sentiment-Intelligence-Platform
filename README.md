# DineSmart — Restaurant Recommendation & Sentiment Analysis

## 📌 Overview
DineSmart is an end-to-end Unstructured Data Analytics project that analyzes Yelp review data to extract customer sentiment, discover hidden topics, and build an intelligent restaurant recommendation system.  

The project combines Natural Language Processing (NLP), Machine Learning, and similarity modeling to generate data-driven insights for customers, restaurant owners, and entrepreneurs.

This system helps:
- Customers discover similar restaurants
- Business owners understand customer sentiment
- Entrepreneurs identify promising restaurant categories in a target location

---

## 🎯 Project Objectives
- Analyze large-scale unstructured Yelp review text
- Perform sentiment analysis on customer reviews
- Discover key themes using topic modeling (LDA)
- Build a content-based restaurant recommendation system
- Suggest business categories for new restaurant owners
- Generate business-level insights using data visualization

---

## 🛠 Tools & Technologies

- **Python**
- Jupyter Notebook
- Pandas
- NumPy
- scikit-learn
- Gensim
- spaCy
- Sentence-Transformers (BERT embeddings)
- Matplotlib
- Seaborn
- pyLDAvis
- WordCloud

---

## ⚙️ Methodology

### 1️⃣ Data Preparation
- Merged multiple Yelp datasets using `business_id`
- Built a data dictionary to understand all attributes
- Cleaned missing values and handled multi-category columns
- Preprocessed text using:
  - Tokenization
  - Stop-word removal
  - Lemmatization

---

### 2️⃣ Sentiment Analysis
- Applied NLP techniques (TextBlob/VADER)
- Calculated:
  - Polarity score
  - Compound score
  - Custom **super_score** combining sentiment + star ratings
- Ranked restaurants based on overall sentiment impact

---

### 3️⃣ Topic Modeling
- Implemented **Latent Dirichlet Allocation (LDA)** using Gensim
- Identified major discussion themes:
  - Food quality
  - Service
  - Pricing
  - Ambience
  - Specific dishes
- Visualized inter-topic distance using pyLDAvis

---

### 4️⃣ Recommendation System
Built a **content-based recommendation engine** using:

- TF-IDF Vectorization
- Sentence-BERT embeddings
- Cosine Similarity
- PCA for dimensionality reduction

The system:
- Recommends top 5 similar restaurants
- Allows recommendation by restaurant name
- Suggests similar categories for entrepreneurs
- Provides location-specific insights

---

### 5️⃣ Data Visualization
Generated insights using:
- Review distribution by state and city
- Sentiment heatmaps
- Category-wise boxplots
- Positive & negative word clouds
- Correlation matrices

---

## 📊 Results & Business Insights

- Identified highly preferred restaurant categories in target cities
- Discovered customer sentiment patterns affecting ratings
- Revealed common pain points (service delay, pricing, quality)
- Built a recommendation engine that improves discovery
- Provided actionable insights for entrepreneurs planning new restaurants

---

## 🚀 How to Run the Project

```bash
# Clone the repository
git clone <your-repo-link>

# Navigate into the project folder
cd DineSmart

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter lab

```
## 📈 Future Improvements

- Hybrid recommendation system (Content + Collaborative Filtering)
- Deep Learning sentiment models (Fine-tuned BERT)
- Real-time dashboard deployment (Streamlit)
- Cloud-based scalable architecture
- API-based recommendation service


## 📚 References

- Yelp Open Dataset
- Scikit-learn Documentation
- Gensim Documentation
- spaCy Documentation
- Research papers on NLP & Recommendation Systems
