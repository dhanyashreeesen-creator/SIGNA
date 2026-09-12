# SIGNA — AI-Powered Document Intelligence & Verification Platform

> **"Upload. Analyze. Verify."**  
> Product Requirements Document (PRD) Implementation for Early-Stage DeepTech SaaS Startup.

---

## 📖 Overview

**SIGNA** combines OCR, computer vision, and machine learning to make document verification faster, more accurate, and accessible to non-technical users. Instead of manually inspecting thousands of high-stakes documents, organizations utilize Signa as an intelligent first layer of verification before human sign-off.

---

## ✨ Features Implemented (Matching 11-Page PRD)

### 1. Marketing Website
- **Hero Section (PRD 11.1, 16)**: *"Trust what you verify."* AI-powered document intelligence, call-to-action buttons ("Launch Live MVP", "Explore Signa"), and real-time scanning simulation card.
- **Problem vs. Solution (PRD 2)**: Visual comparison showing manual verification bottlenecks (time-consuming, repetitive, prone to error, difficult to scale) vs. Signa's intelligent first layer.
- **How It Works (PRD 11.2)**: 3-step workflow — `01 Upload`, `02 Analyze`, `03 Review`.
- **Solutions Grid (PRD 11.3)**:
  - *Document Verification*: Structural and template discrepancy checks.
  - *Information Extraction*: Automatic OCR extraction of key fields.
  - *Anomaly Detection*: Highlighting unusual document characteristics.
  - *Risk Assessment*: Prioritizing documents requiring human review.
- **Technology Architecture (PRD 11.4)**: Credible 2nd-year DeepTech explanation of OCR, Computer Vision (spatial layout & DCT compression artifacts), and Machine Learning classifiers.
- **Target Industries (PRD 3, 11.5)**: Interactive tabs covering Finance, Education, Insurance, Government, Legal, and Enterprise with tailored benchmarks.
- **About Us & Team Structure (PRD 11.6, 15)**: Organizational breakdown across Engineering (5 Devs, 1 AI Engineer, 1 UX Designer), Business, Operations, and Security.
- **"What Signa Is NOT" Responsible AI Guarantee (PRD 4)**: Transparent compliance notice that Signa provides AI-assisted analysis and risk indicators for human review rather than legal absolutes.
- **Future Roadmap (PRD 13)**: Real-time verification, multi-language OCR, custom fine-tuned models, batch processing, and API integration.
- **Lead-Generation Form (PRD 11.7)**: "Talk to Signa" contact form with instant validation and feedback.

### 2. Live Interactive MVP Web Application / Portal
- **Role-Based Experience (PRD 3)**: Live toggle between *Document Verification Officer*, *Compliance / Risk Team*, and *Business Administrator*.
- **Executive Dashboard (PRD 9)**:
  - Live metric counters: **Documents Analyzed (1,248)**, **Low Risk (942)**, **Moderate Risk (231)**, **High Risk (75)**.
  - Recent Activity table matching Document 1024, 1023, 1022 with live filtering and status tags.
- **Document Analyzer Studio (PRD 5.1)**:
  - Drag & Drop zone supporting custom image and PDF uploads.
  - **3 Instant Preloaded Demo Documents**:
    1. 📄 *University Degree Certificate (ABC University)*: High Risk (78/100), font kerning mismatch, digital seal artifact, atypical expiry.
    2. 📄 *Corporate Commercial Invoice*: Low Risk (14/100), verified arithmetic, uniform typography.
    3. 📄 *Government Identity Card*: Moderate Risk (56/100), expired date, edge alpha-blending around portrait.
- **Performance Feedback (PRD 14)**: Multi-stage progress bar showing `"Analyzing document... 67%"` with stage descriptions.
- **Visual Anomaly Highlighter (PRD 6)**: Interactive glowing bounding boxes overlaid on the document viewport. Hovering or clicking on an anomaly highlights its technical indicator in the sidebar.
- **OCR Extraction Table (PRD 5.3)**: Key/value grid (Name, Document ID, Date, Organization, Expiry).
- **Signa Risk Score Gauge (PRD 7)**: 0–100 circular gauge categorized into Low, Moderate, or High Risk.
- **Verification Report & Export (PRD 8)**: Official printable verification report summary with download and PDF export triggers.
- **Human-in-the-Loop Actions (PRD 3, 8)**: "Mark Verified", "Flag for Review", and "Reject Document" buttons that update the live dashboard activity log in real time!

---

## 🚀 How to Run Locally

### Option 1: Native Node.js Server (using Antigravity Node)
```powershell
& "C:\Users\dhanyashree sen\AppData\Roaming\Antigravity\bin\agy-node.cmd" server.js
```
Then open your browser and navigate to:
```
http://localhost:3000
```

### Option 2: Direct File Open
You can open `index.html` directly in Google Chrome, Microsoft Edge, or any modern web browser:
```
file:///C:/Users/dhanyashree%20sen/.gemini/antigravity/scratch/signa-platform/index.html
```

---

## 📁 File Structure

```
signa-platform/
├── assets/                 # Icons and media assets
├── css/
│   └── styles.css          # Design system, glassmorphism, responsive grid, print styles
├── js/
│   ├── app.js              # State management, pipeline animation, interactive bounding boxes
│   └── sample-docs.js      # Rich preset documents (Degree, Invoice, ID) & OCR metadata
├── index.html              # Single-page application (Marketing site & Live MVP app)
├── server.js               # Zero-dependency local HTTP server
└── README.md               # Documentation and execution guide
```
