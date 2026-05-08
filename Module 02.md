# Module 02 — Data & Society
## Lesson Notes & Reading Guide

---

### 🎯 Learning Objectives
- Explain what training data is and why its composition matters
- Perform basic data cleaning and exploratory analysis in Python
- Apply a data ethics checklist to a real dataset

---

### 1. Data is Not Neutral

A common misconception is that data is objective — just facts. In reality, every dataset is the product of choices:

- **What to measure** (and what to ignore)
- **Who gets measured** (and who is excluded)
- **Who owns and controls the data**
- **How the data is labelled** (and by whom)

These choices shape what AI systems learn, and who they serve or harm.

**Example:** A hiring algorithm trained on historical recruitment data will learn to replicate past hiring patterns — including any historical discrimination. The data was "accurate" in recording what happened, but what happened was biased.

---

### 2. Data Sovereignty & Africa

Data sovereignty refers to a community's or nation's right to control data about itself. For African countries, this raises important questions:

- Much African health, agricultural, and demographic data is collected by international organisations and stored on servers outside Africa
- Consent frameworks do not always reflect local norms and languages
- Extracted data generates commercial value that rarely returns to source communities

**The AU Data Policy Framework (2022)** is an important step toward continental data governance standards.

---

### 3. The Data Ethics Checklist

Before using any dataset, ask:

- [ ] **Consent** — Did the people in this dataset agree to its collection and use?
- [ ] **Representation** — Who is in the dataset? Who is missing?
- [ ] **Purpose** — Was data collected for this purpose, or repurposed?
- [ ] **Harm** — Could analysis of this data harm individuals or communities?
- [ ] **Transparency** — Is the collection methodology documented and auditable?
- [ ] **Benefit** — Who benefits from this analysis, and is that equitable?

---

### 4. Bias in Practice

Three types of bias to watch for:

| Type | Description | Example |
|------|-------------|---------|
| **Sampling bias** | Data does not represent the full population | Survey only reaching urban, educated respondents |
| **Labelling bias** | Human annotators bring their own assumptions | Moderators flagging minority-language content as spam |
| **Historical bias** | Data reflects past inequities | Credit scoring models trained on exclusionary lending history |

---

### 📖 Further Reading
- African Union Data Policy Framework: https://au.int/en/documents
- D'Ignazio & Klein (2020). *Data Feminism*. MIT Press (Ch. 1–2)
- Abebe et al. (2021). *Narratives and Counternarratives on Data Sharing in Africa*. ACM FAccT
- Open Data Institute — Data Ethics Canvas: https://theodi.org/insights/tools/the-odi-data-ethics-canvas
