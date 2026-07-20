# Specification: Stock Agent Pro
## Overview
Autonomous stock screening system with commodity correlation and dividend-safety logic.

## Technical Stack
- Language: Python 3.11+
- Architecture: Spec-Driven Modular Agentic System
- Core Tools: yfinance, google-api-python-client, pandas, playwright

## Dividend Safety Logic
- Scoring Policy:
  - Dividend Yield > 0: Bonus score (yield * 100 * 2)
  - Dividend Yield == 0 or None: -30 points penalty
- Action Signal: 
  - Score > 50: Buy
  - Score 21-50: Hold/Monitor
  - Score <= 20: Avoid

## Workflow
1. SPEC.md update.
2. Agents/Utils code implement.
3. Commit & Push to GitHub (nurefendi/stock-agent).
