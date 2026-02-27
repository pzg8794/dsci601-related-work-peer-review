# DSCI 601 — Related Work Survey Peer Review Notes (Feb 27, 2026)

This file tracks review notes for two PDFs in `Semester5/DSCI601/related_work_survey-peer_review/`:

- `dsci_601_Waddell_related_work_survey.pdf` (4 pages)
- `Realted_Work_Survey.pdf` (8 pages)

Rubric items to address:
1) Background information clarity/sufficiency  
2) Citations and reference formatting (e.g., BibTeX/IEEE style)  
3) Related work descriptions (methodology, results, and main contributions)  
4) Conclusion (contrast with proposed project and novelty)  
5) Presentation (professional formatting/quality)  
6) Readability/flow  

---

## What to read (fast, rubric-aligned)

If time is limited, for each paper:
- Read **Introduction and Background** (rubric #1).
- Skim **Related Work** headings, then read **2–3 representative subsections** in detail (rubric #3 and #6).
- Read **Conclusion** carefully (rubric #4).
- Scan **References** for consistency, missing fields, and formatting (rubric #2).

For giving feedback back to teammates (Overleaf/PDF), the easiest approach is:
- Reference **page and section heading**, then paste a short suggested rewrite or bullet suggestion.
- Prioritize “must-fix” issues first (formatting/placeholder notes/citation problems), then “nice-to-have” polish.

---

## Paper A — Hayes Waddell: *Deep Learning Approaches for Automated Abnormal EEG Detection*

### Background information
**What works**
- Intro clearly motivates the problem (clinical workload, access, trust/interpretability).
- Background is structured (signal characteristics, then deep learning for time-series data, then interpretability).

**What could improve**
- Add a 1–2 sentence “scope/roadmap” in **Section 1 (Introduction, p.1)**, right after the last sentence of the intro paragraph (the one ending with “black boxes \[7, 1, 2\]”). Say what “abnormal EEG” means in this survey (seizures/epileptiform events, or broader abnormalities) and what the rest of the survey will cover (models, data, evaluation, interpretability).
- Add 1 sentence on **evaluation metrics** at the end of **Section 2.2 (Deep Learning for Time-Series Data, p.1)**, right after the final sentence ending with “labeled data \[8, 3, 4\]”. Name common metrics (AUC, sensitivity/recall, specificity) and one line on why they matter clinically (missing an abnormal event is costly).

### Citations / formatting
**What works**
- Numeric in-text citations are consistently used.
- Reference list is mostly IEEE-like.

**What could improve**
- Reference formatting is inconsistent in the **References list (p.3–4)**:
  - **\[3\]** includes “vol. Volume 15 - 2021” (duplicate/awkward volume formatting).
  - **\[1\], \[3\], \[4\], \[6\], \[10\]** include “[Online]. Available:” links, while **\[2\], \[5\], \[7\], \[8\], \[9\]** do not. Pick one consistent style and apply it across the list.
  Tightening the reference fields (journal, volume, number, pages, year, doi/url) would clean this up quickly.
- In **Section 3.2 (CNN-based Approaches, p.2)**, the sentence ending with “outperforming all other models.” should have the citation number at the end of that sentence.
- In **Section 3.4 (Emerging Approaches, p.3)**, the “1:1250 spike to normal” imbalance ratio sentence should include the citation number right after the paper/year mention.

### Related work descriptions
**What works**
- Organizing related work by model family (traditional ML, then CNN-based approaches, then RNN/LSTM approaches, then emerging approaches) is easy to follow.

**What could improve**
- In **Section 3 (Related Work)**, especially **p.2 (Sections 3.1–3.3)**, the writing often stays at the “model family” level. To make it easier to skim, pick the **2–4 papers you rely on most** and give each one a quick 1–2 sentence mini-summary: what data they used, what model they used, the key result (with the metric), and one line on why it matters for your project or what the limitation is.

### Conclusion (novelty vs prior work)
**What works**
- Conclusion identifies core gaps (generalization, imbalance, interpretability) and ties back to the motivation.

**What could improve**
- The “my project” statement is still high-level. In **Section 4 (Conclusion)**, add 1–2 contrast sentences **right after the sentence where you describe what your project will do**, so it’s immediately clear what is different from prior work.

### Presentation
**What works**
- Clean, professional-looking PDF; sections are clear; no obvious formatting artifacts.

**What could improve**
- Minor polish: ensure consistent capitalization (EEG, DL), and consistent spacing around citations.

### Readability / flow
**What works**
- Overall structure is clear and easy to skim.

**What could improve**
- Add a 1-sentence transition **after Section 2.3** (end of Background) and **right before Section 3** (Related Work), and another 1-sentence transition **after Section 3.4** (end of Related Work) and **right before Section 4** (Conclusion). This will make the flow feel more intentional.

---

## Paper B — Harkin / Doma / Gopu: *Analysis of Sponsorship and Co-Sponsorship… (Graph, Visualization, and Conversational AI)*

### Background information
**What works**
- Problem and motivation are clear: they explain that Congress.gov/Bioguide contain the needed sponsorship and co-sponsorship data, but that the scale/complexity makes it hard for non-experts to interpret; the proposed map UI plus chatbot is framed as a practical way to turn that data into “askable” questions and interpretable views for the general public.
- Background categories are relevant to the project (graph modeling, community detection, visualization, IR/LLMs).

**What could improve**
- Background should define (briefly) what the **core project outputs** are (e.g., “graph construction, metrics, UI, and grounded QA”), so the reader knows what the related work is “in service of”. A natural place is **right after the “2 Background” heading (p.1) and before Section 2.1**, as a 1–2 sentence “roadmap” that names the pipeline outputs, then the subsections (2.1–2.4) read like supporting components for each output.

### Citations / formatting
**What works**
- Numeric citation style is used and there is a references section.

**What could improve**
- A few “bridge”/takeaway sentences make broader claims without an explicit citation on that *specific* sentence. In **p.4, Section 3.2 (Moody paragraph)**, the paragraph ends with “Similar structural cohesion metrics can be used to determine if Congress is becoming more polarized or more integrated.” Since that paragraph is discussing **Moody \[7\]**, adding a trailing citation (e.g., “...integrated \[7\].”) would make the bridge feel grounded instead of interpretive.
- References: a couple entries look inconsistent in style/fields, such as in the **References list (p.7–8)**:
  - **\[4\] vs \[10\] (p.7)**: same title, but formatting differs (journal capitalization and “pp.” vs “p.”). Make them match (or merge if it is the same work).
  - **\[6\] (p.7)**: title uses “us” instead of “U.S.” and includes an “Online: Available” URL block while nearby entries don’t. Make this entry match the rest.
  - **\[14\]–\[15\] (p.8)**: these two entries are formatted differently, and \[14\] looks cut off. Make them consistent and complete.

### Related work descriptions
**What works**
- The sectioning matches the project components well (network modeling, then analysis, then visualization, then chatbot/GraphRAG).
- Some subsections provide concrete interpretation of what the cited method enables for the project. This is good.

**What could improve**
- A few paragraphs combine **concept definition, results, and takeaway** in a single section, such as:
  - **Section 3.1 (p.2), Cho & Fowler paragraph**: it defines “small-world,” states the result (“more structurally connected; they report it passes more important laws”), then jumps straight to the project takeaway. It will read better if you keep it in this order: method, key finding, relevance to your system, limitation or gap.
  - **Section 3.2/3.1 bridge (p.4), “polarized or more integrated” sentence**: this reads like a general conclusion; adding a short “as measured by [X] in [citation]” clause would make it feel grounded instead of interpretive.
  - **Section 3.3 (p.4), signed-edges visualization paragraph**: strong content, but it will skim better if you keep the same order as in Section 3.1: method, key finding, connection to visualization, and limitation that motivate your design choices.
- Not critical, but the sections below would read better if you add at least a sentence tying back to why it matters for the map and chatbot. In Sections **3.1–3.5**, you can end with a one-liner like:
  - **3.1 Graph construction**: “These studies justify representing sponsorship/co-sponsorship as a weighted graph and motivate computing path length/clustering metrics that our system can expose through the interface.”
  - **3.2 Network analysis/community detection**: “These methods provide the clustering/modularity features our map can visualize (by state/party/time) and that the chatbot can reference when answering ‘who collaborates with whom’ questions.”
  - **3.3 Visualization**: “Signed-edge/signed-community ideas motivate UI encodings (color/line style) that make cooperation vs opposition interpretable to non-technical users.”
  - **3.4 Chatbot / factual QA**: “These works support grounding chatbot answers in verified graph-derived statistics rather than generating unsupported claims.”
  - **3.5 GraphRAG**: “Graph-augmented retrieval provides the mechanism for citing structured evidence (nodes/edges/communities) in responses, aligning the chatbot with provenance and factuality.”

### Conclusion (novelty vs prior work)
**What works**
- Conclusion states two clear contributions: accessibility/visualization and grounded conversational querying.

**What could improve**
- Strengthen “contrast” by naming 1–2 explicit gaps in prior work:
  - *“Prior work analyzes networks but does not provide an interactive public-facing interface.”*
  - *“GraphRAG work is general; this project grounds retrieval specifically in verified Congressional graph schema and provenance.”*

### Presentation
**What could improve**
- Typos/spacing (examples in the PDF):
  - **p.2, Section 2.4**: change “webistes” to “websites”.
  - **p.4, Section 3.2**: change citation punctuation from “\[7\]..” to “\[7\].”.
  - **p.4, Section 3.2**: change “Newmark” to “Newman” (the surrounding sentences are referring to Newman’s framework/metrics).
  - **p.5, Section 3.4**: change “Bayesian item-response.The” to “Bayesian item-response. The”.
- Style consistency (examples in the PDF):
  - “graph based” / “Graph Based” appears in headings and body (e.g., **p.1 Introduction**, **p.1–2 Section 2.1/3.1 headings**). Keep this wording consistent throughout.
  - “cosponsorship” vs “co-sponsorship” are both used (e.g., **p.1 Introduction** vs later Related Work sections). Pick one spelling and keep it consistent.
  - “U.S.” vs “US” (e.g., **p.1 “U.S. map”** vs **p.5 “US House”**). Standardize one style.
- Heading capitalization (examples in the PDF):
  - **p.2, Section 2.4**: change “Information Retrieval for chatbot system” to Title Case (e.g., “Information Retrieval for Chatbot System”) to match the other headings.

### Readability / flow
**What works**
- Top-level narrative is easy to follow: it starts from the *data source/problem*, moves into *graph construction*, then *network measures/community structure*, then *UI/visual encodings*, and ends with the *chatbot/grounded QA* component.

**What could improve**
- Break up a few longer paragraphs (especially in **Section 3.1** and **Section 3.2**) into shorter ones where each paragraph does one job: (i) *paper and approach*, (ii) *key finding/result*, (iii) *why it matters for your map/chatbot*.
