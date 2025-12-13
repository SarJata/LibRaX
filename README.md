# LibRaX

LibRaX is an AI-assisted book discovery and recommendation system designed to help readers
find books through semantic, content-based matching rather than simple keyword or genre filters.

This repository hosts the **public Android client (APK)**, which serves as the user-facing
interface for the LibRaX recommendation system.

---

## Features
- **AI-Powered Recommendations**: Book discovery based on semantic similarity.
- **Modern Android UI**: Built using Jetpack Compose with a reactive UI architecture.
- **Material 3 Design**: Clean, accessible interface following modern Android guidelines.
- **Real-Time Search**: Instant feedback while browsing and searching.
- **Personalized Feeds**: Recommendations influenced by reading history and preferences.

---

## Architecture Overview

LibRaX is designed as a two-part system:

### Public Component
- **Android Client (APK)**  
  This repository provides the compiled Android application for local execution and feature demonstration.

### Private Components
- **Android Source Code (Private)**  
  The full Android source code corresponding to the APK.
- **Backend & ML Pipeline (Private)**  
  Includes the recommendation service, vector search index, and embedding generation logic.

---

## Why the Backend Is Private

The backend and ML components are maintained in a private repository due to:
- Use of internally curated datasets
- Custom tuning of embedding and similarity search logic
- Security considerations around exposed APIs

The Android client interacts with the backend through a well-defined API, allowing full
functionality without exposing internal implementation details.

---

## Tech Stack

### Android Client (Public)
- **Language:** Kotlin
- **UI:** Jetpack Compose, Material 3
- **Architecture:** MVVM
- **Networking:** Retrofit, OkHttp

### Backend & ML (Private)
- **Language:** Python
- **API:** FastAPI
- **Vector Search:** FAISS
- **ML/NLP:** Transformer-based embeddings, scikit-learn utilities

---

## APK Source Code Access

The Android source code and backend repositories are private.
Access may be granted upon request for:
- Recruiter technical review
- Academic evaluation
- Research or collaboration

📩 **Contact:** sarathjata@outlook.com

---

## Author
**Jatavallabhula Sarat Anirudh**  
📧 sarathjata@outlook.com  
🔗 https://www.linkedin.com/in/saratjata/
