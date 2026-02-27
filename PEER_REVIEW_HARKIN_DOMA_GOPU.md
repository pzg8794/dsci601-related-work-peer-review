# Peer Review Notes — *Analysis of Sponsorship and Co-Sponsorship of Legislation in the U.S. Congress through Graph Based Visualization and Conversational AI*

Overleaf: https://www.overleaf.com/project/699b5e6e21d0a83c694121dd

Authors: Tony Harkin; Aditi Reddy Doma; Sai Kiran Gopu  
Reviewer: Piter Z. Garcia

🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦🟦


---
## Background Information

🟢 **What works**
- Problem and motivation are clear: they explain that Congress.gov/Bioguide contain the needed sponsorship and co-sponsorship data, but that the scale/complexity makes it hard for non-experts to interpret; the proposed map UI plus chatbot is framed as a practical way to turn that data into “askable” questions and interpretable views for the general public.
- Background categories are relevant to the project (graph modeling, community detection, visualization, IR/LLMs).

🟡 **What could improve**
- Background should define (briefly) what the **core project outputs** are (e.g., “graph construction, metrics, UI, and grounded QA”), so the reader knows what the related work is “in service of”. A natural place is **right after the “2 Background” heading (p.1) and before Section 2.1**, as a 1–2 sentence “roadmap” that names the pipeline outputs, then the subsections (2.1–2.4) read like supporting components for each output.

---
## Citations / Formatting

🟢 **What works**
- Numeric citation style is used and there is a references section.

🟡 **What could improve**
- A few “bridge”/takeaway sentences make broader claims without an explicit citation on that *specific* sentence. In **p.4, Section 3.2 (Moody paragraph)**, the paragraph ends with “Similar structural cohesion metrics can be used to determine if Congress is becoming more polarized or more integrated.” Since that paragraph is discussing **Moody \[7\]**, adding a trailing citation (e.g., “...integrated \[7\].”) would make the bridge feel grounded instead of interpretive.
- References: a couple entries look inconsistent in style/fields, such as in the **References list (p.7–8)**:
  - **\[4\] vs \[10\] (p.7)**: same title, but formatting differs (journal capitalization and “pp.” vs “p.”). Make them match (or merge if it is the same work).
  - **\[6\] (p.7)**: title uses “us” instead of “U.S.” and includes an “Online: Available” URL block while nearby entries don’t. Make this entry match the rest.
  - **\[14\]–\[15\] (p.8)**: these two entries are formatted differently, and \[14\] looks cut off. Make them consistent and complete.

---
## Related Work Descriptions

🟢 **What works**
- The sectioning matches the project components well (network modeling, then analysis, then visualization, then chatbot/GraphRAG).
- Some subsections provide concrete interpretation of what the cited method enables for the project. This is good.

🟡 **What could improve**
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

---
## Conclusion (Novelty vs Prior Work)

🟢 **What works**
- Conclusion states two clear contributions: accessibility/visualization and grounded conversational querying.

🟡 **What could improve**
- Strengthen “contrast” by naming 1–2 explicit gaps in prior work:
  - *“Prior work analyzes networks but does not provide an interactive public-facing interface.”*
  - *“GraphRAG work is general; this project grounds retrieval specifically in verified Congressional graph schema and provenance.”*

---
## Presentation

🟡 **What could improve**
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

---
## Readability / Flow

🟢 **What works**
- Top-level narrative is easy to follow: it starts from the *data source/problem*, moves into *graph construction*, then *network measures/community structure*, then *UI/visual encodings*, and ends with the *chatbot/grounded QA* component.

🟡 **What could improve**
- Break up a few longer paragraphs (especially in **Section 3.1** and **Section 3.2**) into shorter ones where each paragraph does one job: (i) *paper and approach*, (ii) *key finding/result*, (iii) *why it matters for your map/chatbot*.
