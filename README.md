# DecodeLabs — AI Engineering Internship 
### Batch 2026 | Industrial Training Kit

A complete portfolio of AI projects built during the DecodeLabs Industrial Training Program. This repository documents a structured progression from foundational rule-based logic through supervised machine learning to recommendation systems — each project a working, deployable milestone.

---

## Progression Map

```
Project 1              Project 2                  Project 3
Rule-Based         →   Data Classification    →   Recommendation Logic
Chatbot                                          (Content-Based Filtering)

Control Flow       →   Pattern Recognition    →   Active Prediction
if-else + dicts        Train / Test / Predict     TF-IDF + Cosine Similarity
White-box AI           Statistical AI             Personalization AI
```

> Each project unlocks the next. Completion is verified for quality by DecodeLabs.

---

## Projects

### Project 1 — Rule-Based AI Chatbot 
**Track:** Control Flow & Logic
**Folder:** `project1-chatbot`

| | |
|---|---|
| **Goal** | Build a deterministic chatbot using if-else logic and keyword matching |
| **Algorithm** | Rule-based intent matching against a structured knowledge base |
| **Key skills** | Control flow, input sanitization, infinite loop, fallback handling |

**What it does:**
- Runs in a continuous `while True` loop, exits cleanly on bye/quit/exit
- Sanitizes input with `.lower().strip()` to normalize case and whitespace
- Matches 12 intent categories with randomized responses for natural variation
- Handles live dynamic queries — current time and today's date
- Displays `[BOT | #TAG]` labels for full white-box traceability

**Intents:** `#Greeting` `#Identity` `#Status` `#Joke` `#Weather` `#Age` `#Thanks` `#Help` `#Time` `#Date` `#Exit` `#Defualt`


---

### Project 2 — Data Classification Using AI 
**Track:** Supervised Machine Learning
**Folder:** `project2-Data classification`

| | |
|---|---|
| **Goal** | Classify Iris flower species from measurements using a trained ML model |
| **Algorithm** | K-Nearest Neighbors (KNN) |
| **Dataset** | Iris Benchmark — 150 samples, 4 features, 3 balanced classes |
| **Key skills** | Feature scaling, train/test split, model evaluation, hyperparameter tuning |

**Pipeline:**
```
Iris Dataset → StandardScaler → 80/20 Split → KNN (k=5) → Confusion Matrix + F1 Score
```


---

### Project 3 — AI Recommendation Logic 
**Track:** Content-Based Filtering & Personalization
**Folder:** `project3-AI Recommendation Logic`

| | |
|---|---|
| **Goal** | Recommend tech career paths by matching user skills to job role profiles |
| **Algorithm** | TF-IDF Vectorization + Cosine Similarity |
| **Dataset** | Hand-crafted knowledge base — 12 job roles × 10 skills each |
| **Key skills** | Vector space models, similarity math, ranking pipelines, cold start handling |

**Pipeline:**
```
User Skills → TF-IDF Vectors → Cosine Similarity → Sort → Top-3 Recommendations
```

**Example output:**
```
Input: python, machine learning, docker

  #1  Machine Learning Engineer    84.2%  ████████████████████████░░░░░░
  #2  Data Scientist               76.3%  ██████████████████████░░░░░░░░
  #3  DevOps Engineer              31.0%  █████████░░░░░░░░░░░░░░░░░░░░░
```



---

## Repository Structure

```
decodelabs-ai-internship/
│
├── README.md                              ← you are here
│
├── project1-chatbot/
│   └──chatbot.ipynb                      ← main script
│   
│
├── project2-iris-knn/
│   └── project2.ipynb               ← full pipeline script               
│   
│
└── project3-recommender/
    └── project3_recommender.ipynb            ← main script 
     
```

---

## Key Concepts Covered

**Foundational AI — Project 1**
- Deterministic vs probabilistic AI systems
- White-box traceability — every decision is fully auditable
- IPO model: Input sanitization → Intent matching → Response generation
- Why rule-based guardrails matter in production LLM systems

**Supervised Machine Learning — Project 2**
- Supervised learning pipeline — train, test, validate
- Feature scaling — why StandardScaler is required before KNN
- Train/test split — preventing data leakage and order bias
- Confusion matrix — TP, FP, FN, TN breakdown per class
- F1-score — robust metric for imbalanced data
- Elbow method — systematic hyperparameter tuning
- The "accuracy mirage" — why raw accuracy alone misleads

**Recommendation Systems — Project 3**
- Content-based filtering vs collaborative filtering
- TF-IDF — penalizing generic skills, rewarding specific ones
- Vector space modeling — converting qualitative tags to numerical arrays
- Cosine Similarity — magnitude-invariant angle measurement (range: 0–1)
- The Cold Start Problem — user and item cold start handling strategies
- 4-step ranking pipeline — Ingestion → Scoring → Sorting → Filtering
- Top-N filtering — preventing choice overload

---

## About

Built as part of the **DecodeLabs Industrial Training Program — Batch 2026**.
DecodeLabs is an AI engineering internship platform based in Greater Lucknow, India.

📞 +91 89330 06408 &nbsp;|&nbsp; ✉ decodelabs.tech@gmail.com &nbsp;|&nbsp; 🌐 www.decodelabs.tech
