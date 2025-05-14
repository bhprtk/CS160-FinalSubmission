# 🌿 Eco Marketplace Project Documentation

Welcome to the documentation hub for the **Eco Marketplace Web Application** — a sustainability-focused platform where users can buy, sell, and chat about eco-friendly products.

This folder includes all project deliverables, documentation, source code, and final presentation materials.

---

## 📁 Folder Structure

```

.
├── 📄 README.md                  # This file
├── 📁 Documentation              # All documentation
│   ├── 📝 Requirements.md        # Feature descriptions & expected functionality
│   ├── 🧱 Architecture           # Diagrams
│   │   ├── BlockArchitecture.png
│   │   ├── LayerDiagram.png
│   │   ├── ClassDiagram1.txt
│   │   ├── SequenceDiagrams.txt
│   └── 📘 UserGuide.md           # How to run, login, and use the app
├── 📁 SourceCode                 # Source code (Next.js + Firebase)
└── 📊 FinalPresentation.pdf      # 8–10 minute slide deck

```

---

## 📄 Documentation Overview

- **Requirements.md**  
  Describes the purpose and goals of each key feature (e.g., product listing, user profile, chat system).

- **Architecture/**
  - **BlockArchitecture.png**: High-level system components and data flow.
  - **LayerDiagram.png**: Logical separation into presentation, application, and data layers.
  - **ClassDiagram1.png**: Data model and relationships (User, Product, Chat).
	- **ClassDiagram2.png**: Data model and relationships (User, Message).
  - **SequenceDiagrams.txt**: Step-by-step user interactions (e.g., creating a product, initiating a chat).

- **UserGuide.md**  
  Brief instructions on:
  - Starting the app
  - How to log in
  - Posting a product
  - Viewing chats and profiles

---

## 🚀 Getting Started

To run the web application:

1. Clone the repo and navigate to the `src` folder.
2. Run `npm install` to install dependencies.
3. Set up Firebase config in `.env.local`.
4. Run `npm run dev` to start the development server.

Refer to `docs/UserGuide.md` for full details.

---

## 🧑‍🏫 Final Presentation

Check out `FinalPresentation.pdf` for an 8–10 minute summary of the project’s vision, architecture, features, and challenges.

---

## ✅ Project Summary

- Built with **Next.js 15**, **Firebase Firestore/Auth/Storage**
- Features include:
  - Sustainable product listings
  - Real-time chat per product
  - User authentication and profiles
- Designed with separation of concerns and scalable structure

---

## 🤝 Contributors

* Pratik Bhandari – Full-stack development, database integration, chat system
* Gabriel Danekari – Firebase integration, Firestore rules, authentication, image uploads
* Swan Pyae Sone Tun – UI/UX, handled design consistency, responsive layout, and testing.

---