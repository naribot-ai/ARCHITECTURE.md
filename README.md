# NariBot System Architecture

## Overview
Technical blueprint for NariBot’s DPI ecosystem. It maps how USSD, SMS, and IVR interface with AI to provide real-time livelihood navigation for women entrepreneurs. Built for population-scale growth, vernacular accessibility, and strict data privacy to empower the next billion users.

## 1. High-Level Logic Flow

The following diagram illustrates how a user's request travels from their feature phone to the NariBot engine for processing and back again.



## 2. Technical Stack

| Layer | Technology | Responsibility |
| :--- | :--- | :--- |
| **User Interface** | USSD / IVR (Voice) / SMS | Low-bandwidth feature phone interaction. |
| **Carrier Adapter** | Telecom Gateway | Generic API bridge connecting GSM networks to the web. |
| **Backend** | Node.js (GCP Cloud Run) | Session orchestration and core business logic. |
| **Intelligence** | Gemini 1.5 Flash | Vernacular-first livelihood advice and scheme matching. |
| **Data Store** | Cloud Firestore | User profiles, session state, and localized scheme data. |

## 3. Deployment Context

NariBot is designed as **Digital Public Infrastructure (DPI)**. This architecture ensures high-concurrency state management, strict PII data privacy, and can be scaled to support millions of rural entrepreneurs across Indian states.

---
**Developed by BossMa Studio Works Pvt Ltd**
*Livelihood Navigator Architecture v1.12*
