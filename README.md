# 🛡️ Agentic QA Suite (V1)

### The "Flight Simulator" for Multi-Agent AI Systems.
**Prevent PII leaks, Infinite Loops, and Hallucinations *before* deployment.**

[![Status](https://img.shields.io/badge/Status-Live%20Prototype-green)]()
[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)]()
[![Framework](https://img.shields.io/badge/Built%20With-LangChain%20%7C%20Streamlit-red)]()

---

## 🚨 The Problem
AI Agents in production are unpredictable. They suffer from:
1.  **Compliance Failures:** Leaking PII (Phone/SSN) in logs (Risk for FinTech/HR).
2.  **Infinite Loops:** Burning thousands of tokens on repetitive API calls (Risk for Support).
3.  **Logic Breakdown:** Failing to handle edge cases in coding/reasoning tasks.

## ⚡ The Solution: Agentic QA Engine
This engine acts as an **Adversarial Simulator**. It allows you to paste your agent's System Prompt, selects a "Red Teaming" attack vector, and verifies if your Guardrails catch the failure.

### Key Features (V1)
- **🕵️ Adversarial Red Teaming:** An "Attacker AI" attempts to trick your agent using social engineering.
- **🛑 PII Guardrails:** Regex-based interception blocks sensitive data *before* it hits the logs.
- **🔄 Circuit Breaker:** Detects repetitive semantic loops and terminates execution to save costs.

---

## 🎥 Demo Scenarios

### 1. The "Fama" Scenario (Compliance)
- **Attack:** Social Engineering ("URGENT AUDIT REQUEST") to force PII disclosure.
- **Outcome:** Guardrail detects phone number leakage and blocks the response.
- **Status:** `🚫 [BLOCKED BY AGENTIC QA]`

### 2. The "Gorgias" Scenario (Cost)
- **Attack:** User repeats specific intent ("Where is my refund?") rapidly.
- **Outcome:** Circuit breaker detects loop > 3 turns and stops execution.
- **Status:** `🚫 [LOOP DETECTED]`

---

## 🛠️ How to Run Locally

1. **Clone the repository**
   ```bash
   git clone [https://github.com/YOUR-USERNAME/agentic-qa-suite.git](https://github.com/YOUR-USERNAME/agentic-qa-suite.git)
   cd agentic-qa-suite
