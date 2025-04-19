# 👕 PakClothIntel: AI-Powered Fashion Intelligence from Pakistan's Clothing Brands

**PakClothIntel** is a full-stack AI-powered data pipeline that scrapes, processes, and analyzes fashion data from Pakistani clothing brands — turning raw web data into actionable business insights.

---

## 🚀 Features

- 🧽 **Web Scraping**: Extract product and store data from brand websites (e.g., Khaadi, GulAhmed).
- ☁️ **AWS Cloud Integration**: Run scraping on AWS Lambda & Step Functions, store data in S3.
- 🧼 **ETL & Warehousing**: Clean and transform data using Glue, load into Snowflake warehouse.
- 🤖 **AI Insights**: Use LangChain & LLMs to query, summarize, and generate business reports.
- 🔁 **LangGraph Workflows**: Automate multi-step AI pipelines for data + insight generation.
- 🔍 **Semantic Search** *(Bonus)*: Vector-based product similarity and search.
- 🌐 **UI**: Interactive dashboard using Streamlit to explore trends, discounts, and insights.

---

## 🧱 Tech Stack

| Category        | Tools/Frameworks                          |
|----------------|-------------------------------------------|
| Scraping       | Python, Playwright/Scrapy                 |
| ETL & Storage  | AWS Lambda, Step Functions, S3, Glue      |
| Data Warehouse | Snowflake                                 |
| AI Layer       | LangChain, OpenAI, LangGraph              |
| Semantic Search| FAISS, OpenAI Embeddings                  |
| Frontend       | Streamlit                                 |
| Deployment     | AWS EC2 / Lambda + API Gateway            |

---

## 📁 Project Structure
PakClothIntel/ ├── scrapers/ # Brand-specific scrapers ├── pipeline/ # ETL scripts ├── aws/ # Infra: Lambda, Glue, Step Functions ├── ai/ # LangChain + LLM agents ├── vector_search/ # Bonus: Product similarity ├── app/ # Streamlit frontend ├── notebooks/ # EDA and experiments ├── data/ # Data storage └── utils/ # Helpers (e.g., logger, S3)

## 💡 Sample Business Queries

- Which brands offer the highest discounts in women's wear this month?
- What price range dominates across all brands?
- Which cities have the most physical stores?
- How does product pricing differ between casual and formal wear?
- Are there brands launching similar products in the same timeframe?

---

## 🔨 Setup Instructions

```bash
# 1. Clone this repo
git clone https://github.com/your-username/PakClothIntel.git && cd PakClothIntel

# 2. Install Python dependencies
pip install -r requirements.txt

# 3. Run a sample scraper
python scrapers/khaadi.py

# 4. Launch Streamlit dashboard
streamlit run app/main.py
