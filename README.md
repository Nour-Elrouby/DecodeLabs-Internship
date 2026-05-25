# DecodeLabs — AI Engineering Internship 
### Batch 2026 | Industrial Training Kit

A complete of AI projects built during the DecodeLabs Industrial Training Program. This repository documents a structured progression from foundational rule-based logic through supervised machine learning, recommendation systems, and computer vision — each project a working, deployable milestone.

---

## Progression Map

```
Project 1          Project 2             Project 3               Project 4
Rule-Based     →   Classification    →   Recommendation      →   Image & Text
Chatbot            (KNN)                 (Content Filtering)     Recognition 

Control Flow   →   Pattern           →   Active Prediction    →   Machine Perception
if-else            Recognition           TF-IDF + Cosine         OCR / Object Detection
White-box AI       Statistical AI        Personalization AI      Pre-trained Models
```


---

## Projects

### Project 1 — Rule-Based AI Chatbot 
**Track:** Control Flow & Logic &nbsp;|&nbsp; **Folder:** `project1-chatbot`


**What it does:** Runs in a continuous `while True` loop · Sanitizes input with `.lower().strip()` · Matches 12 intent categories with randomized responses · Handles live time/date queries · Displays `[Bot | #Tag]` labels for full white-box traceability

**Intents:** `#Greeting` `#Identity` `#Status` `#Joke` `#Weather` `#Age` `#Thanks` `#Help` `#Time` `#Date` `#Exit` `#Defualt`


---

### Project 2 — Data Classification Using AI 
**Track:** Supervised Machine Learning &nbsp;|&nbsp; **Folder:** `project2-Data Classification`



**Pipeline:** `Iris Dataset → StandardScaler → 80/20 Split → KNN (k=5) → Confusion Matrix + F1`

**Results:** 100% accuracy on test set · Outputs: `confusion_matrix.png` · `elbow_method.png`


---

### Project 3 — AI Recommendation Logic 
**Track:** Content-Based Filtering &nbsp;|&nbsp; **Folder:** `project3-recommender`


**Pipeline:** `User Skills → TF-IDF Vectors → Cosine Similarity → Sort → Top-3 Recommendations`

**Example output:**
```
Input: python, machine learning, docker

  #1  Machine Learning Engineer    84.2%  ████████████████████████░░░░░░
  #2  Data Scientist               76.3%  ██████████████████████░░░░░░░░
  #3  DevOps Engineer              31.0%  █████████░░░░░░░░░░░░░░░░░░░░░
```


---

### Project 4 — Image & Text Recognition
**Track:** Computer Vision & Pre-trained Models &nbsp;|&nbsp; **Folder:** `project4-recognition`



**OCR Pipeline:** `Load → Grayscale → Gaussian Blur → Otsu Threshold → pytesseract → Text + Confidence`

**Detection Pipeline:** `Load → Blob (300×300) → MobileNet-SSD → 80% Gate → Labelled Bounding Boxes`

---

## Repository Structure

```
decodelabs-ai-internship/
│
├── README.md                                  ← you are here
│
├── project1-chatbot/
│   └── chatbot.ipynb
│
├── project2-iris-knn/
│   └── project2_iris_knn.ipynb
│   
├── project3-recommender/
│   └── project3_recommender.py
│
└── project4-recognition/
    ├── project4_recognition.ipynb
    ├── MobileNetSSD_deploy.prototxt           ← download for Path 2
    └── MobileNetSSD_deploy.caffemodel         ← download for Path 2
```

---

## Key Concepts Covered

**Foundational AI — Project 1**
Deterministic vs probabilistic AI · White-box traceability · IPO model · Rule-based guardrails in production LLM systems

**Supervised Machine Learning — Project 2**
Supervised learning pipeline · Feature scaling (StandardScaler) · Train/test split · Confusion matrix (TP/FP/FN/TN) · F1-score · Elbow method · The accuracy mirage

**Recommendation Systems — Project 3**
Content-based vs collaborative filtering · TF-IDF vectorization · Shared vocabulary space · Cosine similarity (magnitude-invariant) · Cold Start Problem · 4-step ranking pipeline · Top-N filtering

**Computer Vision — Project 4**
Structured vs unstructured data · Transfer learning from ImageNet · Image as 3D array (H×W×C) · Grayscale conversion · Gaussian blur · Adaptive thresholding (Otsu's method) · Blob construction · Softmax & confidence scores · The 80% confidence gate · Bounding box coordinates

---

## About

Built as part of the **DecodeLabs Industrial Training Program — Batch 2026**.

📞 +91 89330 06408 &nbsp;|&nbsp; ✉ decodelabs.tech@gmail.com &nbsp;|&nbsp; 🌐 www.decodelabs.tech
