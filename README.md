# LLM_FOR_FINANCIAL_TEXT_UNDERSTANDING
This project focuses on building a financial text understanding system tailored for the Indian stock market. Using a fine-tuned Small Language Model (SLM), the system integrates financial news, corporate statements, and NIFTY 50 stock market data to generate actionable insights such as “Buy,” “Hold,” or “Sell” recommendations. 

# **Financial Text Understanding Using a Small Language Model (SLM)**

### **Overview**
This project focuses on building a financial text understanding system tailored for the Indian stock market. Using a fine-tuned Small Language Model (SLM), the system integrates financial news, corporate statements, and NIFTY 50 stock market data to generate actionable insights such as "Buy," "Hold," or "Sell" recommendations. The project employs sentiment analysis and financial data processing to enhance decision-making for investors and analysts.

---

## **Features**
- **Custom Dataset Creation**:
  - Financial news articles, stock data, and quarterly statements for NIFTY 50 companies.
  - Includes short-term (7-day) and long-term (6-month) stock price impacts.
- **Sentiment Analysis**:
  - News articles classified as Positive, Negative, or Neutral using Roberta Large.
- **Volatility Calculation**:
  - 7-day and 6-month volatility metrics to assess market stability.
- **Fine-Tuned Model**:
  - Utilized Phi-3.5-mini-instruct with LoRA for computational efficiency.
- **Actionable Predictions**:
  - Provides "Buy," "Hold," or "Sell" recommendations with reasoning.

---

## **Dataset**
### **Sources**:
1. **Financial News**:
   - Collected and preprocessed for sentiment classification.
2. **Stock Market Data**:
   - NIFTY 50 historical prices (daily open, close, high, low, and volume).
3. **Financial Statements**:
   - Extracted KPIs like revenue, net income, EPS, and debt ratios.

### **Components**:
- **Short-Term Data**:
  - 7-day stock price movements after financial news.
- **Long-Term Data**:
  - 6-month trends following quarterly statements.

---

## **Methodology**
1. **Data Preprocessing**:
   - Cleaned and aligned data based on publication dates.
   - Mapped sentiment scores to stock price changes.
2. **Model Training**:
   - Fine-tuned the Phi-3.5-mini-instruct model with LoRA for lightweight deployment.
3. **Few-Shot Prompting**:
   - Designed examples to guide the model in structured prediction generation.
4. **Evaluation**:
   - Compared predictions with actual market movements to achieve baseline accuracy.

---

## **Results**
- **Model Accuracy**:
  - Achieved 41.67% accuracy in predicting stock actions ("Buy," "Hold," "Sell").
- **Efficiency**:
  - LoRA fine-tuning reduced computational requirements without sacrificing performance.

---

## **Applications**
- **For Investors**:
  - Helps individuals make informed "Buy/Hold/Sell" decisions based on market sentiment and financial KPIs.
- **For Analysts**:
  - Supports data-driven insights for portfolio management and risk assessment.
- **In Resource-Constrained Environments**:
  - Lightweight deployment using LoRA makes it accessible to broader markets.

---

## **Installation**
### **Prerequisites**
- Python 3.8 or higher
- Libraries: `transformers`, `pandas`, `numpy`, `matplotlib`, `scikit-learn`

# **Financial Text Understanding Using a Small Language Model (SLM)**

### **Setup Instructions**

Follow these steps to set up the project on your local machine and get it running.

---

## **1. Prerequisites**
Ensure you have the following installed:
- **Python 3.8 or higher**
- **Git** (to clone the repository)
- **Pip** (for managing Python packages)
- A virtual environment tool like `venv` (recommended but optional)

---

## **2. Clone the Repository**
Clone the project repository using Git:
```bash
git clone https://github.com/your-username/financial-text-understanding.git
cd financial-text-understanding



