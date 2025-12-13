# LibRaX

LibRaX is an AI-assisted book discovery and recommendation system designed to help readers
find books using semantic, content-based similarity rather than traditional keyword or
genre-based search.

The system focuses on understanding **context and meaning** in book descriptions to provide
more relevant and personalized recommendations.

This repository hosts the **public Android client (APK)**, which demonstrates the user-facing
experience of the LibRaX platform.

---

## ✨ Features

- **AI-Powered Recommendations**  
  Discover books based on semantic similarity using vector embeddings.

- **Modern Android UI**  
  Built using Jetpack Compose with a reactive and maintainable UI architecture.

- **Material 3 Design**  
  Clean and accessible interface aligned with modern Android design guidelines.

- **Real-Time Search**  
  Instant feedback while browsing and searching the book catalog.

- **Personalized Feeds**  
  Recommendations influenced by user interaction and reading history.

---

## 🧱 System Architecture Overview

LibRaX is designed as a **multi-component system** consisting of a public client and private
backend services.

### Public Component

- **Android Client (APK)**  
  This repository provides the compiled Android application package for local installation
  and feature demonstration.

### Private Components

- **Android Application Source Code**
- **Backend Services and ML Recommendation Engine**

These components are maintained separately and are not publicly available.

---

## 🔐 Why the Android App Source Code Is Private

The Android application source code is maintained in a private repository due to
**security-sensitive configuration** related to backend services.

Specifically:
- The application integrates with **Firebase and Firestore**
- Configuration files (such as Firebase service credentials and JSON-based configuration)
  require strict access control
- Keeping the source private helps prevent accidental exposure or misuse of sensitive
  configuration data

The public APK is provided to demonstrate application functionality without exposing
security-critical integration details.

---

## 🤖 Why the Backend and ML System Are Private

The backend services and recommendation engine are maintained in a private repository for
the following reasons:

- **Custom Data Processing Pipeline**  
  The project includes custom data cleaning, preprocessing, and transformation steps built
  on top of publicly available datasets.

- **Custom Recommendation System Design**  
  The ML system combines embedding generation, similarity search, and ranking logic tailored
  specifically for book discovery.

- **FAISS-Based Vector Search**  
  The recommendation engine uses FAISS for efficient vector similarity search, with custom
  indexing and query strategies.

- **Security and API Integrity**  
  Keeping backend logic private reduces the risk of misuse and protects internal service
  behavior.

The Android client interacts with the backend through a well-defined API, allowing full
functionality without exposing internal ML or infrastructure implementation details.

---

## 🛠️ Tech Stack

### Android Client (Public)

- **Language:** Kotlin
- **UI Framework:** Jetpack Compose
- **Design System:** Material 3
- **Architecture:** MVVM
- **Networking:** Retrofit, OkHttp
- **Backend Integration:** Firebase, Firestore

### Backend & ML (Private)

- **Language:** Python
- **API Framework:** FastAPI
- **Vector Search:** FAISS
- **ML/NLP:** Transformer-based embeddings, custom preprocessing and ranking logic
- **Data Sources:** Publicly available book datasets (e.g., Kaggle)

---

## 🔓 Source Code Access

The Android source code and backend/ML repositories are private.

Access may be granted upon request for:
- Technical evaluation by recruiters
- Academic review
- Research or collaboration purposes

📩 **Contact:** sarathjata@outlook.com

---

## 👤 Author

**Jatavallabhula Sarat Anirudh**  
📧 sarathjata@outlook.com  
🔗 https://www.linkedin.com/in/saratjata/
