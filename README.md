# DecodeLabs — AI Engineering Internship Portfolio
### Batch 2026 | Industrial Training Kit

A complete portfolio of AI projects built during the DecodeLabs Industrial Training Program. This repository documents a structured progression from foundational rule-based logic through supervised machine learning — each project a working, deployable milestone.

---

## Progression Map

```
Project 1                        Project 2
Rule-Based Chatbot       →       Data Classification 
(Deterministic Logic)            (Supervised Learning)

Control Flow             →       Pattern Recognition
if-else + dictionaries   →       Train / Test / Predict
White-box AI             →       Statistical AI
```

> Each project unlocks the next. Completion is verified for quality by DecodeLabs.

---

## Projects

### Project 1 — Rule-Based AI Chatbot 🤖
**Track:** Control Flow & Logic  
**Folder:** `project1-chatbot/`

| | |
|---|---|
| **Goal** | Build a deterministic chatbot that responds to predefined user inputs using if-else logic |
| **Algorithm** | Keyword-matching against a structured rules dictionary |
| **Dataset** | Hand-crafted knowledge base — 12 intent categories |
| **Key skills** | Control flow, input sanitization, infinite loop architecture, fallback handling |

**What it does:**
- Runs in a continuous `while True` loop — exits cleanly on bye/quit/exit
- Sanitizes input with `.lower().strip()` to normalize case and whitespace
- Matches user intent against a knowledge base of 12 rule categories
- Returns randomized responses per rule for natural variation
- Handles live dynamic queries — current time and today's date
- Displays `[BOT | #TAG]` labels for full white-box traceability

**Intents supported:** `#GREETING` `#IDENTITY` `#STATUS` `#JOKE` `#WEATHER` `#AGE` `#THANKS` `#HELP` `#TIME` `#DATE` `#EXIT` `#DEFAULT`

---

### Project 2 — Data Classification Using AI 🌸
**Track:** Supervised Machine Learning  
**Folder:** `project2-iris-knn/`

| | |
|---|---|
| **Goal** | Build a classification model that predicts Iris flower species from measurements |
| **Algorithm** | K-Nearest Neighbors (KNN) |
| **Dataset** | Iris Benchmark — 150 samples, 4 features, 3 balanced classes |
| **Key skills** | Feature scaling, train/test split, model evaluation, hyperparameter tuning |

**Pipeline:**
```
Iris Dataset → StandardScaler → 80/20 Split → KNN (k=5) → Confusion Matrix + F1 Score
```

**Results:**

| Class | Precision | Recall | F1-Score |
|-------|-----------|--------|----------|
| Setosa | 1.00 | 1.00 | 1.00 |
| Versicolor | 1.00 | 1.00 | 1.00 |
| Virginica | 1.00 | 1.00 | 1.00 |

> Overall accuracy: **100%** on the test set with k=5 and StandardScaler applied.

**Outputs generated on run:**
- `confusion_matrix.png` — heatmap of predicted vs actual labels
- `elbow_method.png` — error rate curve across k=1–30



---

## Repository Structure

```
decodelabs-ai-internship/
│
├── README.md                          ← you are here
│
├── project1-chatbot/
│   ├── chatbot.ipynb                  ← Jupyter notebook implementation
│   ├── chatbot.py                     ← standalone Python script
│   └── README.md                      ← project-level documentation
│
└── project2-iris-knn/
    ├── project2_iris_knn.py           ← full pipeline script
    ├── confusion_matrix.png           ← generated on run
    ├── elbow_method.png               ← generated on run
    └── README.md                      ← project-level documentation
```

---

## Tech Stack

| Tool | Used In | Purpose |
|------|---------|---------|
| Python 3.10+ | All projects | Core language |
| `random` | Project 1 | Randomized chatbot responses |
| `datetime` | Project 1 | Live time and date handling |
| `scikit-learn` | Project 2 | KNN model, StandardScaler, metrics |
| `pandas` | Project 2 | Data loading and exploration |
| `matplotlib` | Project 2 | Plotting confusion matrix and elbow curve |
| `seaborn` | Project 2 | Heatmap visualization |

---

## Key Concepts Covered

**Foundational AI (Project 1)**
- Deterministic vs probabilistic AI systems
- White-box traceability — every decision is fully auditable
- IPO model: Input sanitization → Intent matching → Response generation
- Why rule-based guardrails matter in production LLM systems

**Supervised Machine Learning (Project 2)**
- Supervised learning pipeline — train, test, validate
- Feature scaling — why StandardScaler is required before KNN
- Train/test split — preventing data leakage and order bias
- Confusion matrix — breaking down TP, FP, FN, TN per class
- F1-score — robust evaluation metric for imbalanced data
- Elbow method — systematic hyperparameter tuning for optimal K
- The "accuracy mirage" — why raw accuracy alone can be misleading

---

## About

Built as part of the **DecodeLabs Industrial Training Program — Batch 2026**.  
DecodeLabs is an AI engineering internship platform based in Greater Lucknow, India.

📞 +91 89330 06408 &nbsp;|&nbsp; ✉ decodelabs.tech@gmail.com &nbsp;|&nbsp; 🌐 www.decodelabs.tech
