# 🖼️ Imaginify — AI-Powered Image SaaS Platform

An AI-driven image editing SaaS platform where users can restore old photos, remove backgrounds, recolor objects, fill in missing areas with generative AI, and manage everything through a credit-based billing system.

> 🎓 **Credit:** This project was built by following the excellent full-stack tutorial by [**JavaScript Mastery**](https://www.youtube.com/@javascriptmastery) on YouTube. I built it hands-on to learn the stack and the patterns involved — all credit for the original design, architecture, and teaching goes to their team. You can find the original tutorial [here](https://youtu.be/Ahwoks_dawU).

---

## ✨ Features

- **Authentication & Authorization** — secure sign-up, login, and protected routes via Clerk
- **Image Restoration** — revive old or damaged photos
- **Background Removal** — cleanly extract subjects from their background
- **Object Recoloring** — recolor specific objects in an image
- **Generative Fill** — expand or fill in missing areas of an image using AI
- **Object Removal** — remove unwanted objects with precision
- **Community Showcase** — browse transformations made by other users, with pagination
- **Image Search** — find images by content or objects present in them
- **Credit System** — earn free credits or purchase more via Stripe
- **Profile Dashboard** — track your transformations and remaining credits
- **Responsive UI** — built with Tailwind CSS and Shadcn UI components for a clean experience on any device

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Framework | Next.js (App Router), TypeScript |
| Styling | Tailwind CSS, Shadcn UI |
| Database | MongoDB (Mongoose) |
| Authentication | Clerk |
| Image Processing | Cloudinary AI |
| Payments | Stripe (with webhooks) |

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- A MongoDB database (e.g. via [MongoDB Atlas](https://www.mongodb.com/))
- Accounts for [Clerk](https://clerk.com/), [Cloudinary](https://cloudinary.com/), and [Stripe](https://stripe.com/)

### Installation

```bash
git clone https://github.com/Divyanshi-Sharma2007/ai-image-saas.git
cd ai-image-saas
npm install
```

### Environment Variables

Create a `.env.local` file in the project root with the following:

```
# NEXT
NEXT_PUBLIC_SERVER_URL=

# MONGODB
MONGODB_URL=

# CLERK
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
WEBHOOK_SECRET=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# CLOUDINARY
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=

# STRIPE
STRIPE_SECRET_KEY=
STRIPE_WEBHOOK_SECRET=
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=
```

### Run Locally

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📂 Project Structure

```
ai-image-saas/
├── app/            # Next.js app router pages & API routes
├── components/     # Reusable UI components
├── constants/      # Static config (plans, nav links, transformation types)
├── lib/            # Server actions, database models, utility functions
├── public/         # Static assets
└── types/          # Shared TypeScript types
```

---
