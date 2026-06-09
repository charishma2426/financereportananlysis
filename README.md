# Autonomous Financial Research Assistant (Agentic AI)

An autonomous, multi-step AI Agent built in Python using the **Phidata** framework and powered by Google's **Gemini 1.5 Flash** large language model. This agent acts as an automated market analyst, bridging the real-time gap of classic LLMs by natively accessing, parsing, and summarizing live stock indicators.

## 🧠 Core Architecture



Unlike basic generative chatbots that work on single prompt-and-response dynamics, this framework implements **Agentic workflows**:
1. **Goal Reception:** Takes broad, multi-step prompts (e.g., asset comparison and financial evaluation).
2. **Autonomous Tool Selection:** Recognizes missing information gaps and programmatically triggers background API instances (`YFinanceTools`).
3. **Data Integration:** Dynamically pulls and executes targeted structural payloads (`stock_price`, `analyst_recommendations`).
4. **Context Synthesis:** Validates raw data returns and structures comprehensive Markdown reports for users.

## 🚀 Key Features
* **Live Market Access:** Bypasses LLM temporal cutoff walls by integrating real-time market data directly from Yahoo Finance.
* **Reasoning Traceability:** Displays actual background tool execution flows via terminal parameters (`show_tool_calls=True`).
* **Gemini Pipeline Integration:** Configured explicitly to leverage Google AI Studio's infrastructure natively for rapid text streaming.

## 🛠️ Installation & Setup

### Prerequisites
* Python 3.8 or higher installed
* A valid Google AI Studio API key

### 1. Installation
Install the upgraded framework core along with the necessary Google integration and financial packages:
```bash
pip install -U google-generativeai phidata yfinance
