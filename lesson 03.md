# Module 03 — AI & Misinformation
## Lesson Notes & Reading Guide

---

### 🎯 Learning Objectives
- Explain how misinformation spreads and why Africa faces particular vulnerabilities
- Understand TF-IDF and how machines represent text as numbers
- Train and evaluate a basic text classifier in Python

---

### 1. The Misinformation Problem in Africa

Misinformation — false or misleading information spread regardless of intent — is not new. But digital platforms have changed its velocity and reach dramatically.

In African contexts, specific dynamics amplify the problem:
- **WhatsApp-first information ecosystems** — news spreads primarily through private messaging, making it harder to trace and debunk
- **Low-resource language gaps** — AI moderation tools are overwhelmingly trained on English/French, performing poorly on Pidgin, Camfranglais, Hausa, Swahili, and hundreds of other languages
- **Trust deficits** — in contexts where institutional trust is low, rumours fill the void
- **Election periods** — coordinated disinformation campaigns around elections are well-documented across the continent

**Examples:** COVID-19 vaccine misinformation, electoral fraud claims, health remedy hoaxes

---

### 2. How Does a Machine Detect Misinformation?

At its core, automated misinformation detection is a **text classification** problem: given a piece of text, predict whether it is reliable or unreliable.

#### Step 1 — Represent text as numbers
Machines cannot read words directly. We convert text to numerical vectors.

**TF-IDF (Term Frequency — Inverse Document Frequency):**
- **TF:** How often does a word appear in *this* document?
- **IDF:** How rare is that word across *all* documents?
- Words that are common everywhere (like "the") get low weight. Words that appear often in this document but rarely elsewhere get high weight.

#### Step 2 — Train a classifier
Feed thousands of labelled examples (true/false) to a model. The model learns which word patterns associate with each class.

#### Step 3 — Evaluate honestly
- **Accuracy** alone is misleading if classes are imbalanced
- Use **precision, recall, and F1-score**
- Always test on data the model has never seen

---

### 3. Limitations of Automated Detection

This is critical: AI misinformation detection is an **imperfect tool**, not a solution.

| Limitation | Why it matters |
|-----------|----------------|
| Context blindness | A statement can be true in one context, false in another |
| Language coverage | Most models work well in English only |
| Adversarial manipulation | Bad actors adapt to fool classifiers |
| False positives | Wrongly flagged content silences legitimate voices |
| Accountability gap | Who is responsible when the AI is wrong? |

The most effective misinformation responses combine AI tools with **human fact-checkers, community literacy programmes, and platform policy** — not AI alone.

---

### 4. Responsible Deployment Framework

Before deploying any AI misinformation tool, ask:

1. What is the error rate, and who bears the cost of false positives?
2. Is the system transparent and auditable?
3. Is there a human appeal process?
4. Has the system been tested on the languages and dialects of the target community?
5. Who controls the system, and what are their incentives?

---

### 📖 Further Reading
- AfricaCheck: https://africacheck.org
- Dubawa (Nigeria): https://dubawa.org
- Penplusbytes (Ghana): https://penplusbytes.org
- Mozilla Foundation — *Misinformation & AI* report
- Wardle & Derakhshan (2017). *Information Disorder*. Council of Europe
