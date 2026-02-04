# Ad-Tech AI Safety & Governance Framework

### Bridging Content Integrity and Algorithmic Trust

## 📌 Executive Summary

As AI-driven ad generation scales to thousands of variants per week, traditional manual curation reaches a breaking point. This project presents a **Full-Lifecycle Governance Framework** designed to manage the transition from manual KPO-based policy enforcement to automated, risk-aware AI oversight.

By implementing **NIST AI RMF** functions (Map, Measure, Manage), this framework identified a **14% demographic parity gap** in automated targeting and established the guardrails necessary for compliant, high-scale digital marketing.

---

## 📂 Project Structure

* `01_Risk_Assessment/`: Initial discovery memos and threat models for GenAI ad pipelines.
* `02_Policy_Architecture/`: Formal Responsible AI policies aligned with **ISO 42001** and the **Indian DPDP Act**.
* `03_Audit_Scripts/`: Python notebooks utilizing `Fairlearn` for quantitative bias detection.
* `04_Incident_Response/`: Post-mortem reports and "Kill Switch" playbooks for model failures.

---

## 🛠️ Core Competencies Demonstrated

* **Regulatory Compliance:** Mapping AI outputs to the **EU AI Act** and **ASCI Guidelines**.
* **Algorithmic Fairness:** Quantifying bias using Demographic Parity and Equalized Odds.
* **Risk Mitigation:** Designing **Human-in-the-loop (HITL)** triggers for high-sensitivity ad verticals (Finance/Healthcare).
* **Security & Red Teaming:** Identifying prompt-injection vulnerabilities in creative engines.

---

## 📊 Key Results from Technical Audit

In a simulated audit of 1,000 ad-delivery events, the following disparities were identified using the provided Python scripts:

| Metric | Pre-Mitigation | Post-Mitigation | Status |
| --- | --- | --- | --- |
| **Demographic Parity Diff** | 0.142 | 0.021 | ✅ PASS |
| **Selection Rate (Female)** | 21% | 29% | ✅ IMPROVED |
| **Selection Rate (Male)** | 35% | 31% | ✅ STABILIZED |

---

## 🚀 How to Use This Repository

1. **Read the Risk Memo:** Start in `01_Risk_Assessment/` to understand the business problem.
2. **Review the Policy:** See `02_Policy_Architecture/` for the regulatory solution.
3. **Run the Audit:** Open the Jupyter Notebook in `03_Audit_Scripts/` to see the code in action.
4. **Analyze the Failure:** Read the Post-Mortem in `04_Incident_Response/` to see how to handle a live "Governance Incident."

---

## 📧 Contact & Networking

I am an **AI Governance Analyst** (formerly KPO Analyst at Virtusa) passionate about building trustworthy AI systems.

* **LinkedIn:** https://www.linkedin.com/in/udaya-manisha-iskala-5b58a9241/
* **Email:** manishaiskala008@gmail.com

---
