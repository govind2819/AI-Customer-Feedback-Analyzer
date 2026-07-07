# AI-Customer-Feedback-Analyzer
AI-powered customer feedback analyzer built with n8n, Ollama (Llama 3.2), and Google Sheets for automated sentiment analysis and discount decisioning using a local LLM.

**Built With**
1. n8n
2. Ollama
3. Llama 3.2 1B
4. Google Sheets

**Features**
1. Collect customer feedback
2. Perform local AI sentiment analysis
3. Automatically decide discount eligibility
4. Store results in Google Sheets

**Architecture diagram**
Customer
   │
   ▼
n8n Form
   │
   ▼
Ollama (Llama3.2)
   │
Sentiment Analysis
   │
   ▼
Decision Logic
   │
   ▼
Google Sheets
