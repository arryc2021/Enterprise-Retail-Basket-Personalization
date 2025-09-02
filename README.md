# 🏬 Enterprise Retail Basket Personalization

This project implements an **AI-powered retail basket personalization system** using **LangChain + Ollama + Gemma 3**.  
It generates **customer-specific promotional emails** and calculates **revenue & profit uplift KPIs** based on basket data, product catalog, and recommendation rules.

---

## 🚀 Features
- **Excel Upload**: Upload basket, catalog, and rules in Excel format.
- **KPI Dashboard**:
  - Revenue uplift per customer
  - Profit uplift per customer
  - Total organization-level uplift
- **AI-Generated Customer Emails**:
  - Personalized promotional content per customer
  - Fast batch generation via **Gemma 3**
- **Outgoing Mailbox Simulation**:
  - View all generated emails in a structured **Sent Items table**
- **Data Visualization**:
  - Revenue & Profit uplift bar charts
  - Comparison plots

---

## 📂 Input Data Format

### Basket Sheet
| customer_id | product_id | product_name | qty | price | margin |
|-------------|------------|--------------|-----|-------|--------|

### Catalog Sheet
| product_id | product_name | price | margin |
|------------|--------------|-------|--------|

### Rules Sheet
| product_id | complimentary_product_id |
|------------|---------------------------|

---

## 🛠️ Tech Stack
- **Python**
- **Streamlit** (interactive UI)
- **Pandas** (data handling)
- **Matplotlib** (visualizations)
- **LangChain + Ollama** (LLM orchestration)
- **Gemma 3** (fast LLM for promo generation)

---

## ▶️ How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Start the Streamlit app:
   ```bash
   streamlit run app.py
   ```

3. Upload an Excel file containing:
   - `basket`
   - `catalog`
   - `rules`  
   or use `KPI Dashboard` + `Recommendations` sheets.

4. View:
   - 📊 KPI Dashboard
   - 📧 AI-Generated Emails
   - 📤 Outgoing Mailbox

---

## 📊 Example Output

- **KPI Dashboard**: Revenue & Profit uplift charts per customer  
- **Customer Emails**: Personalized promo messages  
- **Outgoing Mailbox**: Sent items table with `To`, `Subject`, `Body`  

---

## 🔮 Future Enhancements
- Integration with **SMTP or SendGrid API** for real email delivery
- Export Outgoing Mailbox as **Excel/CSV**
- Add support for **multi-lingual email campaigns**
- A/B testing of generated promos

---

## 📜 License
This project is licensed under the MIT License.
