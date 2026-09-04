# ProctorAI: Intelligent Online Proctoring Using Multimodal Behavioral Analytics

<p align="center">
  <img src="assets/proctorai-logo.png" alt="ProctorAI Logo" width="220"/>
</p>

<p align="center">
  <b>AI-Powered Multimodal Online Examination Proctoring Framework</b>
</p>

<p align="center">
  Secure. Intelligent. Risk-Aware.
</p>

---

## 📌 Overview

**ProctorAI** is an intelligent online examination proctoring framework designed to improve academic integrity and examination security in remote and online assessments.

Traditional online proctoring systems often depend on a limited number of behavioral indicators and frequently produce a simple binary outcome such as **"Normal"** or **"Suspicious"**. ProctorAI addresses this limitation by combining **QR-based candidate authentication, multimodal behavioral monitoring, and machine learning-based risk assessment**.

The framework analyzes multiple behavioral signals during an examination and assigns each examination session a **behavioral risk level**, allowing instructors or administrators to prioritize sessions that require further investigation.

ProctorAI is designed as a **modular framework** that can be integrated with existing online examination platforms without requiring major changes to their underlying infrastructure.

---

## 🎯 Objectives

The primary objectives of ProctorAI are:

- To strengthen the security of online examinations.
- To provide secure candidate authentication using QR codes.
- To monitor multiple behavioral indicators during examinations.
- To detect potentially suspicious examination behavior using Machine Learning.
- To move beyond simple binary cheating detection.
- To classify examination sessions into multiple behavioral risk levels.
- To reduce unnecessary manual review.
- To help instructors prioritize high-risk examination sessions.
- To provide a scalable and modular proctoring architecture.
- To enable integration with existing examination platforms.

---

## 🚨 Problem Statement

The increasing adoption of online examinations has created significant challenges related to academic integrity.

Conventional online proctoring approaches may rely heavily on individual behavioral indicators or require extensive manual monitoring. Moreover, many systems simply classify an examination session as either:

> Normal / Suspicious

Such binary classification does not adequately represent the different levels of behavioral risk that may occur during an examination.

For example, occasional head movement and repeated tab switching may not necessarily indicate the same level of risk as persistent face absence combined with unusual gaze behavior and excessive keyboard or mouse activity.

Therefore, there is a need for an intelligent system capable of combining multiple behavioral indicators and producing a more informative risk assessment.

---

# 💡 Proposed Solution

ProctorAI combines multiple security and Artificial Intelligence components into a unified framework.

The system consists of:

1. **QR-Based Candidate Authentication**
2. **Multimodal Behavioral Monitoring**
3. **Feature Extraction and Engineering**
4. **Machine Learning-Based Classification**
5. **Five-Level Behavioral Risk Assessment**
6. **Instructor-Oriented Risk Prioritization**

Instead of generating only a binary cheating decision, ProctorAI estimates the behavioral risk associated with an examination session.

---

# 🔐 Key Features

## 1. QR-Based Candidate Authentication

ProctorAI incorporates QR-code-based authentication to help verify the identity of candidates before entering the examination environment.

The authentication mechanism provides an additional security layer before the examination begins.

---

## 2. Multimodal Behavioral Monitoring

The framework analyzes multiple behavioral signals during an examination session.

The seven primary behavioral features considered are:

| No. | Behavioral Feature | Purpose |
|----:|--------------------|---------|
| 1 | Face Visibility | Determines whether the candidate's face remains visible |
| 2 | Head Movement | Monitors unusual or excessive head movements |
| 3 | Gaze Direction | Analyzes the candidate's viewing direction |
| 4 | Browser Tab Switching | Detects repeated switching between browser tabs |
| 5 | Keyboard Activity | Monitors unusual keyboard interaction |
| 6 | Mouse Activity | Analyzes mouse interaction patterns |
| 7 | Examination Duration | Considers examination time as a behavioral factor |

These signals are combined to provide a more comprehensive representation of examination behavior.

---

# 🤖 Machine Learning-Based Risk Assessment

ProctorAI formulates examination monitoring as a **five-class classification problem**.

The behavioral risk categories include:

### 🟢 Honest
Normal examination behavior with no significant suspicious indicators.

### 🟡 Low Risk
Minor behavioral irregularities that may not necessarily indicate malpractice.

### 🟠 Medium Risk
Multiple behavioral indicators suggesting that the session may require attention.

### 🔴 High Risk
Strong behavioral indications that warrant detailed examination.

### ⚠️ Cheating
Behavioral patterns strongly associated with potential examination malpractice.

The purpose of this classification is not to automatically accuse a candidate of cheating, but to provide a **risk-based prioritization mechanism** for human review.

---

# 📊 Dataset

For large-scale evaluation, the research framework uses an integrated behavioral dataset containing approximately:

**200,000 behavioral samples**

The dataset was constructed by integrating multiple publicly available datasets, followed by data preprocessing and feature engineering.

The resulting dataset was used to train and evaluate supervised machine learning models for five-class behavioral risk classification.

> **Note:** The dataset sources, preprocessing procedures, feature engineering methodology, and experimental configuration are documented in the associated research work.

---

# ⚙️ System Workflow

The overall ProctorAI workflow can be summarized as:

```text
Candidate
    │
    ▼
QR-Based Authentication
    │
    ▼
Online Examination
    │
    ▼
Multimodal Behavioral Monitoring
    │
    ├── Face Visibility
    ├── Head Movement
    ├── Gaze Direction
    ├── Tab Switching
    ├── Keyboard Activity
    ├── Mouse Activity
    └── Examination Duration
    │
    ▼
Feature Extraction & Engineering
    │
    ▼
Machine Learning Model
    │
    ▼
Five-Class Risk Classification
    │
    ├── Honest
    ├── Low Risk
    ├── Medium Risk
    ├── High Risk
    └── Cheating
    │
    ▼
Risk Prioritization
    │
    ▼
Instructor / Administrator Review
