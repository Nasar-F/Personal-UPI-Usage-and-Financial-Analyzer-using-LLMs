# 💰 Personal Financial Analyzer

A Streamlit-based AI-powered application that analyzes **personal financial statements** (UPI/Bank PDFs) using **Google Gemini AI**.  
It extracts transaction data, identifies spending patterns, and provides insights and recommendations for financial improvement.

---

## 🚀 Features

- 📄 **Upload PDF Statements** — Upload UPI or bank transaction PDFs (text-based).  
- 🧠 **AI-Powered Analysis** — Uses Google Gemini (`gemini-2.5-flash`) to interpret transaction data.  
- 📊 **Insightful Summary** — Automatically generates markdown-based insights including:
  - Monthly income & expense summary  
  - Category-wise breakdown  
  - Trend analysis  
  - Savings recommendations  
- 🖥️ **Modern Streamlit UI** — Clean, responsive interface with background styling.  
- 💾 **Download Report** — Export the AI-generated financial report as a markdown (`.txt`) file.

---

## 🧩 Tech Stack

- **Python 3.10+**
- **Streamlit** — Frontend web framework  
- **Google Generative AI (Gemini)** — For text-based analysis  
- **PyPDF2** — PDF text extraction  
- **Tempfile** — Secure temporary storage

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/personal-financial-analyzer.git
cd personal-financial-analyzer
```

### 2️⃣ Create and Activate Virtual Environment
```bash
python -m venv venv
venv\Scripts\activate   # (Windows)
source venv/bin/activate  # (macOS/Linux)
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Set up Google Gemini API Key
Create a `.env` file or set the environment variable manually:

#### Option 1: Using Command Line
```bash
set GEMINI_API_KEY=your_api_key_here        # Windows
export GEMINI_API_KEY=your_api_key_here     # macOS/Linux
```

#### Option 2: Using .env File
```
GEMINI_API_KEY=your_api_key_here
```

---

## 🧠 How It Works

1. Upload your **bank or UPI PDF statement**.  
2. The app extracts text using **PyPDF2**.  
3. The extracted data is sent to **Google Gemini (gemini-2.5-flash)** with a structured prompt.  
4. Gemini analyzes the data and generates financial summaries and insights.  
5. You can view and **download** the markdown report instantly.

---

## 📦 Example Output

```markdown
# Financial Insights Summary

## Monthly Overview
| Month | Income (₹) | Expenses (₹) | Savings (%) |
|--------|-------------|--------------|--------------|
| Jan | 45,000 | 32,000 | 28% |

## Trends
- Spending increased in weekends.
- Food and transport costs are major contributors.

## Recommendations
- Reduce food delivery expenses.
- Consider using a savings auto-transfer.

## Category Breakdown
| Category | Amount (₹) |
|-----------|------------|
| Food | 12,000 |
| Transport | 6,000 |
| Utilities | 4,500 |
```

---

## 🧾 File Structure

```
├── sa.py                # Main Streamlit application
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

---

## 🧰 Requirements.txt (Sample)
```
streamlit
PyPDF2
google-generativeai
python-dotenv
```

---

## 🧑‍💻 Author

**Developed by:** Nasar  
📧 *Contact:* [your_email@example.com]  
🌐 *GitHub:* [https://github.com/yourusername]

---

## 📄 License

This project is open-source under the **MIT License**.
