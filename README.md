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

**Workflow**

Step 1: Customer submits feedback
- The customer fills out the n8n Form.
- The form collects:
    - Name
    - Email
    - Product/Service
    - Feedback
  
Step 2: AI analyzes the feedback
- n8n sends the feedback to Ollama using an HTTP Request.
- Llama 3.2 (Local LLM) classifies the feedback as:
   - Positive
   - Negative

Step 3: Business rule execution

- Based on the AI response:

Sentiment   	Discount
Positive	      ✅ Yes
Negative	      ❌ No

Step 4: Store the result

- The workflow automatically appends the following information to Google Sheets:

   - Customer Name
   - Email
   - Product/Service
   - Feedback
   - AI Sentiment
   - Discount Status
