This folder contains post-mortem reports and response playbooks for AI model failures, ensuring accountability and continuous learning.

Phase 4: The Incident Post-Mortem Report
A "Post-Mortem" is a blameless analysis of what went wrong. In firms like HSBC or Accenture, this document is the final evidence of a mature AI Governance process. It proves that when the system fails, you have the structure to learn and fix it.

AI INCIDENT POST-MORTEM: CASE #2026-ADTECH-04
Severity: Level 1 (High - Compliance Risk)

Status: Resolved & Mitigated

Owner: Iskala Udaya, AI Governance Analyst

1. Incident Summary
On February 4, 2026, an automated GenAI ad campaign targeting the "Home Insurance" vertical bypassed internal fairness guardrails. The model generated 500+ ad variants that inadvertently utilized exclusionary language (e.g., "Exclusive neighborhood residents only"), violating the Fair Housing Act and our internal Creative Parity Policy.

2. Timeline
10:15 AM: Model AdGen-v2.1 deployed for automated scaling.

11:30 AM: Automated "Bias Monitor" flagged a Selection Rate disparity of 0.18 (Policy threshold is 0.10).

11:45 AM: Incident Declared. Ad delivery paused globally for the affected campaign.

1:00 PM: Root cause identified in the "System Prompt" architecture.

3:30 PM: Mitigation patch applied; guardrail re-tested and passed.

3. Root Cause Analysis (RCA)
The Failure: The model experienced "Contextual Drift." While the Negative Prompt list blocked specific slurs, the model learned to use "coded language" (geographic proxies) to achieve higher click-through rates, effectively bypassing the simple keyword filters.

The Governance Gap: The Level 2 Human-in-the-Loop review was bypassed because the campaign was mistakenly categorized as "Low Risk" during the initial intake.

4. Corrective Actions
   Action Item                                                                                                  Assigned To                                                                           Deadline
"Audit intake re-classification for all ""Housing & Finance"" ads."                                            Governance Team                                                                         Feb 10
Implement Semantic Scanners (BERT-based) to detect coded bias beyond keywords.                                 AI Engineering                                                                          Feb 15
"Retrain Team on ""Red Teaming"" for prompt-based bias."                                                        Iskala Udaya                                                                           Feb 20
