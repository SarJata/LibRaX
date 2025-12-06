# LibRaX — Where Books Find You

## Overview

**LibRaX** is an AI-assisted book discovery and recommendation system designed to help readers find their next favorite book through intelligent, content-based matching. Unlike traditional keyword searches, LibRaX understands the *context* and *nuance* of book content.

This repository hosts the **public Android client**, built with modern mobile technologies like **Jetpack Compose** and **Material 3**. It serves as the polished, user-facing interface for our powerful recommendation engine.

## Features

*   **AI-Powered Recommendations**: Discover books based on semantic similarity rather than just genre tags.
*   **Modern Android UI**: Built entirely with Jetpack Compose for a fluid, reactive user experience.
*   **Material 3 Design**: Adheres to the latest Google design guidelines for a clean, accessible, and beautiful interface.
*   **Real-time Search**: Instant feedback as you explore the library.
*   **Personalized Feeds**: Curated lists based on your reading history and preferences.

## Architecture & Design Philosophy

The LibRaX ecosystem is architected into two distinct components: a **Public Frontend** and a **Private Backend**.

### Public vs. Private Components

*   **Public Repository (This Repo)**: Contains the Android client code. We believe in transparency regarding our user interface and client-side logic. This allows developers to inspect the app's behavior, security, and UI implementation.
*   **Private Repository (Backend & ML)**: Contains the core machine learning pipeline, including the **FAISS** index, embedding generation models, and proprietary clustering algorithms.

### Why is the Backend Private?

The decision to keep the backend closed-source is a strategic measure to protect:
1.  **Intellectual Property**: The specific tuning of our embedding models and clustering logic represents significant R&D effort.
2.  **Proprietary Data**: The training datasets used to refine our recommendations are curated internally.
3.  **Security**: Limiting exposure of the raw model internals reduces the attack surface against our API and data integrity.

We expose our capabilities through a secure, documented API, ensuring that the client can leverage the full power of the ML engine without exposing its internal mechanics.

## Tech Stack

### Frontend (Public)
*   **Language**: Kotlin
*   **UI Framework**: Jetpack Compose
*   **Design System**: Material 3
*   **Architecture**: MVVM (Model-View-ViewModel)
*   **Networking**: Retrofit / OkHttp

### Backend (Private)
*   **Language**: Python
*   **Vector Search**: FAISS (Facebook AI Similarity Search)
*   **ML/NLP**: Transformers (Embeddings), Scikit-learn (Clustering)
*   **API**: FastAPI / Flask

## How It Works: The Recommendation Engine

At the heart of LibRaX is a high-performance similarity search engine. Here is the conceptual workflow:

1.  **Vectorization**: Every book in our database is converted into a high-dimensional vector (embedding) that represents its semantic meaning—plot, tone, writing style, etc.
2.  **Indexing**: We use **FAISS** to index these vectors efficiently. FAISS allows us to search through millions of vectors in milliseconds.
3.  **Querying**: When a user likes a book or searches for a query, we convert that input into a vector.
4.  **Similarity Search**: The engine finds the "nearest neighbors" in the high-dimensional space. Books that are mathematically close to each other are semantically similar, resulting in highly relevant recommendations.

### 🔐 APK Source Code Access
The core backend + machine learning engine for LibRaX is private and not publicly available.
However, access to the **APK source code** (Android client only) may be granted upon request
for technical review, recruitment, or collaboration purposes.

Access may be granted for:
• Recruiters reviewing Android development capability
• Research or collaboration review
• Academic evaluation

👉 Request APK Source Access: sarathjata@outlook.com

## Setup (Android Client)

To build and run the Android application locally:

1.  **Prerequisites**:
    *   Android Studio Hedgehog or later.
    *   JDK 17.
2.  **Clone**:
    ```bash
    git clone https://github.com/your-username/librax-android.git
    ```
3.  **Open**: Open the project in Android Studio.
4.  **Sync**: Allow Gradle to sync dependencies.
5.  **Run**: Select an emulator or physical device and click **Run**.

## Contact

*   **Developer**: Jatavallabhula Sarat Anirudh
*   **Email**: sarathjata@outlook.com
*   **LinkedIn**: https://www.linkedin.com/in/saratjata/
