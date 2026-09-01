# Nirnay 📊
### Multi-Agent Equity Research & Risk Intelligence Platform

Nirnay is an explainable multi-agent equity research platform designed to analyze stocks from multiple independent perspectives and combine the results into a single risk-aware research insight.

Instead of depending on one model or one source of information, Nirnay uses specialized agents to analyze **market momentum, financial sentiment, and company filings** before a synthesis layer combines their results.

---

## 🚀 Key Features

- 📈 **Momentum Analysis**
  - Analyzes daily price movement
  - Compares trading volume with average volume
  - Evaluates multi-session price trends

- 📰 **Sentiment Analysis**
  - Analyzes financial headlines
  - Detects positive and negative signals
  - Measures disagreement between headlines

- 📄 **Financial Filing Analysis**
  - Uses TF-IDF-based lexical retrieval
  - Searches company-specific filing information
  - Prevents information from another company being incorrectly cited

- 🧠 **Multi-Agent Decision System**
  - Each agent works independently
  - Agents provide both a score and confidence level
  - A synthesis layer combines the results

- ⚖️ **Risk-Aware Profiles**
  - Conservative
  - Moderate
  - Aggressive

  Each profile uses different weights, decision thresholds, conviction requirements, and position limits.

- 🛡️ **Failure Handling**
  - Handles unavailable market data
  - Handles missing or irrelevant filings
  - Detects disagreement between agents
  - Reduces conviction when evidence is weak

- 📊 **Portfolio & Session Analytics**
  - Portfolio holdings
  - Concentration analysis
  - Session metrics
  - Research history
  - Universe-wide stock scanning

---

## 🏗️ How It Works

Nirnay follows a simple research pipeline:

```text
                STOCK
                  │
        ┌─────────┼─────────┐
        ↓         ↓         ↓
   Momentum   Sentiment   Filings
     Agent      Agent      Agent
        │         │         │
        └─────────┼─────────┘
                  ↓
          Synthesis Engine
                  ↓
          Risk-Weighted Score
                  ↓
       Research Decision & Insight
