# Peer Review Notes — *Deep Learning Approaches for Automated Abnormal EEG Detection*

Overleaf: https://www.overleaf.com/project/699754dc364940fa38341419

Authors: Hayes Waddell; John Thomas  
Reviewer: Piter Z. Garcia



---
## Background Information
---

🟢 **What works**
- Intro clearly motivates the problem (clinical workload, access, trust/interpretability).
- Background is structured (signal characteristics, then deep learning for time-series data, then interpretability).

🟡 **What could improve**
- Add a 1–2 sentence “scope/roadmap” in **Section 1 (Introduction, p.1)**, right after the last sentence of the intro paragraph (the one ending with “black boxes \[7, 1, 2\]”). Say what “abnormal EEG” means in this survey (seizures/epileptiform events, or broader abnormalities) and what the rest of the survey will cover (models, data, evaluation, interpretability).
- Add 1 sentence on **evaluation metrics** at the end of **Section 2.2 (Deep Learning for Time-Series Data, p.1)**, right after the final sentence ending with “labeled data \[8, 3, 4\]”. Name common metrics (AUC, sensitivity/recall, specificity) and one line on why they matter clinically (missing an abnormal event is costly).

---
## Citations / Formatting
---

🟢 **What works**
- Numeric in-text citations are consistently used.
- Reference list is mostly IEEE-like.

🟡 **What could improve**
- Reference formatting is inconsistent in the **References list (p.3–4)**:
  - **\[3\]** includes “vol. Volume 15 - 2021” (duplicate/awkward volume formatting).
  - **\[1\], \[3\], \[4\], \[6\], \[10\]** include “[Online]. Available:” links, while **\[2\], \[5\], \[7\], \[8\], \[9\]** do not. Pick one consistent style and apply it across the list.
  Tightening the reference fields (journal, volume, number, pages, year, doi/url) would clean this up quickly.
- In **Section 3.2 (CNN-based Approaches, p.2)**, the sentence ending with “outperforming all other models.” should have the citation number at the end of that sentence.
- In **Section 3.4 (Emerging Approaches, p.3)**, the “1:1250 spike to normal” imbalance ratio sentence should include the citation number right after the paper/year mention.

---
## Related Work Descriptions
---

🟢 **What works**
- Organizing related work by model family (traditional ML, then CNN-based approaches, then RNN/LSTM approaches, then emerging approaches) is easy to follow.

🟡 **What could improve**
- In **Section 3 (Related Work)**, especially **p.2 (Sections 3.1–3.3)**, the writing often stays at the “model family” level. To make it easier to skim, pick the **2–4 papers you rely on most** and give each one a quick 1–2 sentence mini-summary: what data they used, what model they used, the key result (with the metric), and one line on why it matters for your project or what the limitation is.

---
## Conclusion (Novelty vs Prior Work)
---

🟢 **What works**
- Conclusion identifies core gaps (generalization, imbalance, interpretability) and ties back to the motivation.

🟡 **What could improve**
- The “my project” statement is still high-level. In **Section 4 (Conclusion)**, add 1–2 contrast sentences **right after the sentence where you describe what your project will do**, so it’s immediately clear what is different from prior work.

---
## Presentation
---

🟢 **What works**
- Clean, professional-looking PDF; sections are clear; no obvious formatting artifacts.

🟡 **What could improve**
- Minor polish: ensure consistent capitalization (EEG, DL), and consistent spacing around citations.

---
## Readability / Flow
---

🟢 **What works**
- Overall structure is clear and easy to skim.

🟡 **What could improve**
- Add a 1-sentence transition **after Section 2.3** (end of Background) and **right before Section 3** (Related Work), and another 1-sentence transition **after Section 3.4** (end of Related Work) and **right before Section 4** (Conclusion). This will make the flow feel more intentional.
