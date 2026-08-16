# AI Website Builder 🚀

An intelligent, full-stack website builder that allows users to generate and iteratively refine complete, responsive web pages using natural language. Built with a modern React frontend, an Express/PostgreSQL backend, and powered by OpenRouter LLMs.

## ✨ Features

* **Prompt-to-Website Generation**: Type your idea, and the AI will expand it into a detailed prompt and generate a complete, production-ready, single-page HTML document with Tailwind CSS.
* **Iterative Refinements**: Don't like a color or want to add a new section? Just tell the AI, and it will modify the existing code to match your vision.
* **Version History & Rollbacks**: Every change is tracked. Easily roll back to previous versions of your website if you don't like the latest AI edits.
* **Conversational Interface**: Chat with the AI builder in real-time as you construct your site, maintaining the full context of your design choices.
* **Credit System & Monetization**: Built-in Stripe integration for users to purchase credits and fund their AI generations.
* **Live Previews**: See your generated website immediately alongside the chat interface.

## 🛠️ Tech Stack

### Frontend (Client)
* **Framework**: React 19 with Vite
* **Styling**: Tailwind CSS v4, class-variance-authority, clsx
* **Routing**: React Router DOM v7
* **Icons & UI**: Lucide React, Sonner (Toasts), Better Auth UI
* **Network**: Axios

### Backend (Server)
* **Framework**: Node.js / Express (TypeScript)
* **Database**: PostgreSQL
* **ORM**: Prisma (with `@prisma/adapter-pg`)
* **Authentication**: Better Auth
* **AI Integration**: OpenAI SDK (Routing to OpenRouter / `kwaipilot/kat-coder-pro:free`)
* **Payments**: Stripe

## 🧠 How the AI Works

The AI integration uses a dual-step pipeline for both creation and modification:
1. **Prompt Enhancement**: User input is sent to the LLM to be fleshed out into a highly detailed, professional web design specification (adding layout logic, color schemes, typography, and responsive rules).
2. **Code Generation**: The enhanced specification is sent back to the LLM with strict system instructions to act as an expert developer. It outputs pure HTML containing Tailwind CSS classes, inline JavaScript, and placeholder assets.

## 🚀 Getting Started

### Prerequisites
* Node.js
* PostgreSQL database
* OpenRouter API Key
* Stripe Secret Key (for payments)

### Setup Instructions
*(Add your specific installation and run instructions here based on the `How to Run Project.pdf` provided in the repository)*
