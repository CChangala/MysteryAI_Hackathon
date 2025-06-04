# MysteryAI – AI-Powered Murder Mystery Game

MysteryAI is an interactive, AI-driven murder mystery game where each case is dynamically generated using GenAI. Players interrogate suspects in real-time, solve unique mysteries, and experience an immersive narrative powered by cutting-edge machine learning.

## Features

- **AI-Generated Murder Mysteries** using Google Gemini 1.5 Flash API
- **Context-Aware Suspect Interrogation** with Retrieval-Augmented Generation (RAG)
- **Duplicate Case Prevention** via HuggingFace MiniLM embeddings + cosine similarity
- Real-time suspect responses based on embedding a search of prior case facts
- Avatar generation based on suspect name and gender
- Firebase Auth for secure user login
- Seamless frontend experience with React + Tailwind CSS

## How It Works

1. **Case Generation**: A complete murder mystery (crime, suspects, alibis) is generated using Google Gemini.
2. **Embedding & Storage**: A case summary is embedded using HuggingFace’s `MiniLM-L6-v2` model and stored in Firebase Firestore.
3. **Duplicate Detection**: Before storing new cases, cosine similarity is applied to detect and block similar/duplicate cases.
4. **RAG Interrogation**: During questioning, related embeddings are retrieved and fed into Gemini for accurate, context-aware responses.

## Tech Stack

| Area        | Tools/Frameworks                                  |
|-------------|---------------------------------------------------|
| Frontend    | React, Tailwind CSS                               |
| GenAI       | Google Gemini 1.5 Flash API                       |
| Embeddings  | HuggingFace MiniLM-L6-v2                          |
| Database    | Firebase Firestore                                |
| Auth        | Firebase Authentication                           |
| Backend     | Firebase Functions + Client-side RAG              |

## 🔄 Future Enhancements

- 🎙️ Voice-based interrogation
- 🧩 Adaptive difficulty based on player success rate
- 🖼️ Visual clues and map-based exploration
- 🤖 Auto-learning from solved cases for a better future generation
  
# Challenges:

Challenges: Ensuring case variety, handling long conversations, preventing duplicate cases, and creating realistic AI responses.


# Future Enhancements:

Adaptive difficulty based on player behavior.

Auto-learning from solved cases.

Voice-based interactions

Introduce visual clues


# Setup:

To run the Webapp, Clone Git Repo and run the following:

 npm i 
 
 npm run dev 

 # Team:

 Chaitanya Changala

 Sriya Choudary Yalavarthy

 Shubhang Vagvala 
