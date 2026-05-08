# VeriVolunte

AI-Powered Trusted Volunteer Coordination Platform

VeriVolunte is an intelligent volunteer coordination platform designed to help NGOs respond faster during emergencies and disaster situations by combining Artificial Intelligence, smart volunteer matching, trust verification, and map-based decision systems.

The platform converts scattered and unstructured information such as WhatsApp messages, handwritten notes, and text inputs into structured actionable tasks, then intelligently matches verified volunteers based on skills, availability, trust score, and proximity.

---

## Problem Statement

During emergencies, NGOs face two major challenges:

- Information is scattered across WhatsApp messages, social media posts, surveys, and images.
- Volunteers may claim skills without proper verification, making trust difficult.

This leads to:
- Delayed response times
- Manual workload
- Poor coordination
- Risk of fake or unqualified volunteers

---

# Our Solution

VeriVolunte solves these challenges using AI + verification systems + intelligent matching.

The system:
- Extracts structured needs from messy inputs
- Verifies volunteer credentials
- Matches the best volunteers automatically
- Visualizes urgent needs on maps
- Creates a reusable trust ecosystem across NGOs

---

# Key Features

## 1. AI-Based Need Extraction
- Accepts:
  - Text input
  - WhatsApp messages
  - Handwritten/image uploads
- Extracts:
  - Location
  - Urgency level
  - Required skills
  - Number of people required
- Uses:
  - Google Gemini API
  - Google Vision API

### Additional Enhancements
- AI Confidence Score
- Source Trust Score
  - NGO Verified → High Trust
  - Volunteer → Medium Trust
  - Social Media → Low Trust

---

## 2. Smart Volunteer Matching System
Automatically ranks volunteers using:
- Skill relevance
- Distance
- Availability
- Verification status

### Multi-Factor Scoring System
Final score is calculated using:
- Skill Match
- Distance Score
- Availability Score
- Trust Score

This helps NGOs instantly find the most suitable volunteers.

---

## 3. Map-Based Need Visualization
Displays all active needs on an interactive map.

### Urgency Color Coding
- 🔴 Red → High urgency
- 🟡 Yellow → Medium urgency
- 🟢 Green → Low urgency

### Benefits
- Real-time decision making
- Resource prioritization
- Critical zone identification

---

## 4. AI-Powered Certificate Verification
Volunteers can upload:
- CPR certificates
- First Aid certifications
- Medical credentials

AI extracts:
- Name
- Certificate type
- Expiry date
- Issuing organization

### Verification Workflow
- High confidence → Auto-suggest approval
- Low confidence → Human review

---

## 5. Verified Badge System
Approved volunteers receive:
- ✅ Verified Badge

This helps NGOs instantly identify trusted volunteers.

---

## 6. Cross-NGO Trust Sharing
Once verified by one NGO:
- Other NGOs can trust the same volunteer
- No repeated verification needed

Stored data includes:
- Verifying NGO
- Timestamp
- Credential hash

---

## 7. Privacy-Safe Blockchain Layer (Hybrid Concept)
Instead of storing personal data:
- Only secure hashes are stored

Benefits:
- Privacy protection
- Tamper-proof verification
- Lightweight trust architecture

---

## 8. WhatsApp-Compatible Workflow
NGOs can simply:
- Copy-paste WhatsApp messages into the platform

No workflow changes required.

> “We don’t replace existing tools — we enhance them.”

---

# Tech Stack

## Frontend
- HTML
- CSS
- JavaScript

## Backend
- Node.js
- Google Cloud Run

## Database
- Firebase Firestore

## AI & APIs
- Google Gemini API
- Google Vision API
- Google Maps JavaScript API
- Google Maps Geocoding API

## Storage
- Google Cloud Storage

---

# System Architecture

```text
User Input (Text/Image/WhatsApp)
        ↓
Cloud Run Backend
        ↓
Vision API (OCR if image)
        ↓
Gemini API (AI Extraction)
        ↓
Firestore Database
        ↓
Volunteer Matching Engine
        ↓
Map Visualization + NGO Dashboard


MVP Features Implemented
  AI Need Extraction
  Volunteer Matching
  Verification + Badge System
  Map Visualization
  WhatsApp-style Input

Future Scope
  Full blockchain-based credential network
  Multi-NGO trust ecosystem
  Advanced analytics dashboard
  Real-time notifications
  Heatmaps & clustering
  AI-assisted deployment suggestions

Impact

VeriVolunte helps:

  NGOs respond faster
  Volunteers contribute effectively
  Communities receive timely assistance

By combining AI, trust systems, and intelligent coordination, VeriVolunte transforms scattered information into coordinated action.
