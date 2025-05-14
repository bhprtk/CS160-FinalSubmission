# 📋 EcoMarket – Description & Requirements Documentation

This document outlines the core features of EcoMarket and their intended purposes. It acts as a functional guide to ensure all team members and future developers understand the user-facing goals of the platform.

---

## 🛍️ Product Listings

**Description:**  
Allow sellers to post products with detailed sustainability information.

**Requirements:**
- Seller must be authenticated.
- Product form should include:
  - Title, description, image, price
  - Materials used
  - Certifications (e.g., USDA Organic, Fair Trade)
  - Packaging type (e.g., recyclable, zero waste)
  - Ethical/social attributes (e.g., minority-owned, local artisan)
  - End-of-life and care instructions
- On submission, product is saved to Firestore and visible to all users.

**Purpose:**  
Empower small eco-conscious businesses to showcase their products with transparency.

---

## 👥 User Authentication

**Description:**  
Secure login system to manage buyers and sellers.

**Requirements:**
- Sign in with Google via Firebase Auth.
- Save basic user info (name, photo, email) to Firestore on first login.
- Only authenticated users can list products or start chats.

**Purpose:**  
Create personalized experiences and enforce secure, authenticated access to features.

---

## 💬 Product-Specific Chat

**Description:**  
Allow buyers to initiate a conversation with the seller about a specific product.

**Requirements:**
- Each product chat is 1:1 between buyer and seller.
- Chats are stored under `/chats/{chatId}`.
- Real-time messaging via Firestore `onSnapshot`.
- Messages include:
  - senderId, senderName, photoURL
  - text and timestamp
- Chat list only includes chats with at least one message.

**Purpose:**  
Enable direct, contextual communication to ask questions and build trust before purchase.

---

## 👤 User Profile Page

**Description:**  
Showcase a user’s profile and their posted listings.

**Requirements:**
- Visible only when logged in.
- Displays:
  - Profile image, name, email
  - List of user’s product listings
- Includes logout button.

**Purpose:**  
Allow users to manage their presence and track their contributions to the platform.

---

## 📦 Product Page

**Description:**  
Detailed view for each product.

**Requirements:**
- Accessible via `/products/[id]`.
- Shows:
  - Image, price, title, description
  - Sustainability features
  - Seller info
  - Button to start chat with seller

**Purpose:**  
Provide a transparent and informative shopping experience that highlights sustainability credentials.

---

## 💬 Chat List Page

**Description:**  
View all conversations where the user is a participant.

**Requirements:**
- Route: `/chat`
- Displays list of chats with:
  - Other user’s name and profile photo
  - Product image and title
  - Last message and timestamp
- Clicking a chat takes user to `/chat/[chatId]`

**Purpose:**  
Offer a unified, easy-to-navigate inbox for buyers and sellers.

---

## 🔒 Firestore Security Rules

**Description:**  
Restrict access to only appropriate users and actions.

**Requirements:**
- Only buyers/sellers of a chat can read/write messages.
- Chats must be created by either participant.
- Profile info is readable by anyone; editable only by owner.
- Products are public but only editable by owner.

**Purpose:**  
Maintain data privacy, integrity, and enforce fair access control.

---
