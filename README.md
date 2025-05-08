# 🏛️ Analyzing Federal Reserve Meeting Minutes with Classical and Modern NLP (2015–2025)

## 📌 Overview

This project presents a **comprehensive NLP pipeline** to analyze over **100+ Federal Reserve meeting minutes** from **2015 to 2025**. The goal is to examine how the tone, topics, and key messages of the Federal Open Market Committee (FOMC) evolved across a decade—using both **classical NLP** methods (like VADER and LDA) and **modern transformer-based approaches** (like FinBERT and BERTopic).

We explore the intersection of **financial communication**, **monetary policy signals**, and **language evolution**—uncovering how sentiment and key topics shift in relation to major economic changes.

---

## 📂 Project Structure

### ✅ Step 1: Data Collection (Notebook 1)
- Scraped transcripts of **FOMC meeting minutes** from the [Federal Reserve website](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm)
- Extracted key metadata:
  - 📅 Meeting Date
  - 🕒 Time (if available)
  - 📜 Full Transcript Text
  - 🧾 Additional document metadata
- Collected over **100 high-quality transcripts**
- Implemented **robust error handling** to ensure completeness

---

### 📊 Step 2: Classical NLP - Sentiment Analysis (Notebook 2)
- Applied **VADER (Valence Aware Dictionary and sEntiment Reasoner)**:
  - Extracted **positive**, **negative**, **neutral**, and **compound** scores
  - Visualized sentiment trends over time
  - Plotted sentiment vs. economic indicators (optional integration)
- Generated yearly **word clouds**:
  - 9x9 subplots of top 20 sentiment-related words for each year (2015–2025)
  - Tracked shifts in sentiment vocabulary
- Documented patterns in tone during economic highs, lows, and transitions

---

### 🧠 Step 3: Classical NLP - Topic Modeling (Notebook 2)
- Used **Gensim's LDA (Latent Dirichlet Allocation)** for topic modeling
  - Extracted dominant themes from FOMC transcripts
  - Tracked topic evolution across 10+ years
  - Visualized topic distributions and linked them with sentiment results
- Merged topic and sentiment insights to reveal **narrative arcs** across policy cycles

---

### 🔍 Step 4: Transformer-Based Sentiment Analysis (Notebook 3)
- Used **FinBERT** (financially tuned BERT) via Hugging Face Transformers:
  - Zero-shot sentiment classification on full transcripts
  - Created visualizations of sentiment change over time
  - Compared sentiment results with classical VADER analysis
- Added **text noise detection and cleaning visualizations**
- Enhanced narrative interpretation with deep-context sentiment intelligence

---

### ✂️ Step 5: Transformer-Based Extractive Summarization (Notebook 4)
- Applied **FinBERT-based summarization**:
  - Generated concise summaries of each FOMC transcript
  - Evaluated **summary quality**, retention, and relevance
  - Compared summaries across time to detect shifts in focus
  - Helped reduce data volume for downstream modeling

---

### 🧠 Step 6: Transformer-Based Topic Modeling with BERTopic (Notebook 5)
- Used **BERTopic** for contextual topic extraction:
  - Leveraged transformer embeddings + UMAP + HDBSCAN
  - Identified rich, evolving themes in financial discourse
  - Compared topic clusters with LDA results
  - Visualized temporal topic distributions
- Revealed policy shifts, market focus areas, and emerging concerns

---

## 📌 Key Outcomes

- ✅ **Hybrid NLP methodology** combining rule-based, probabilistic, and transformer models
- 📈 Detected **sentiment shifts** aligning with rate hikes, inflation news, and COVID-era policy
- 🧠 Extracted **core themes** like "labor market," "inflation outlook," "policy normalization"
- ✂️ Generated **high-quality summaries** of long FOMC documents
- 🔁 Enabled **comparative analysis** between classical and modern NLP approaches

---

## 🛠️ Tech Stack
- Python (BeautifulSoup, Requests, Pandas, Matplotlib)
- NLP Libraries:
  - Classical: VADER, Gensim (LDA)
  - Modern: HuggingFace Transformers (FinBERT), BERTopic, UMAP, HDBSCAN
- Visualization: Seaborn, WordCloud, Plotly

