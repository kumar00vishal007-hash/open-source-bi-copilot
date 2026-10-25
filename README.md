#  Open-Source AI BI Analytics Copilot & Executive Dashboard

An AI-assisted Business Intelligence tool powered by **Open-Source LLM (Qwen2.5-Coder-1.5B)** running locally on GPU via Hugging Face Transformers. It translates plain English queries into executable SQLite commands, calculates executive KPIs, and automatically renders a multi-chart visual dashboard (Bar, Pie, Top 5 Leaderboard, Map/Heatmap) along with AI insights without relying on paid cloud API keys.

---

##  Key Features
- **100% Free & Open-Source:** Runs locally using Hugging Face Transformers on GPU with zero API key cost and complete data privacy.
- **Natural Language to SQL Engine:** Translates plain English business questions into raw, optimized SQLite queries using `Qwen/Qwen2.5-Coder-1.5B-Instruct`.
- **Executive KPI Cards:** Instantly computes Total Aggregated Metric Value, Total Record Counts, and Average Value per Transaction.
- **Multi-Chart Auto-Visualization:** Dynamic visual engine automatically generates:
  - 📊 **Bar / Column Chart** (Categorical breakdowns)
  - 🍩 **Pie Chart** (Share & revenue distribution)
  - 🏆 **Top 5 Leaderboard** (Horizontal performance ranking)
  - 🌐 **Geospatial / Density Map** (Regional distribution analysis)
- **AI Executive Takeaways:** Generates automated text insights highlighting top drivers and key performance summary.
- **Interactive Browser UI:** Powered by Gradio for clean and seamless web deployment.

---

##  Tech Stack
- **Language:** Python 3.10+
- **LLM Model:** `Qwen/Qwen2.5-Coder-1.5B-Instruct` (Hugging Face)
- **Frameworks:** PyTorch, Accelerate, Transformers
- **Database:** SQLite3
- **Data & Visualization:** Pandas, Plotly Express
- **UI Web Framework:** Gradio

---

## ⚡ How to Run in Google Colab
1. Open Google Colab and set Runtime to **T4 GPU** (`Runtime > Change runtime type > T4 GPU`).
2. Upload `AI_BI_Analytics_Copilot.ipynb`.
3. Execute all cells sequentially.
4. Access the live Gradio dashboard via the generated public link.

---

## 📊 Sample Database Schema
- **`products`**: `product_id`, `product_name`, `category`, `price`
- **`sales`**: `sale_id`, `product_id`, `region`, `quantity`, `total_amount`, `sale_date`
