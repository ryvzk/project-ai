**# Project AI

An enterprise-grade, secure, local, and unrestricted AI interface featuring an admin-managed user authentication system, encrypted Supabase backend storage, live web search capabilities, and local execution via Ollama or OpenAI-compatible endpoints.

---

## Features

* **Secure Authentication & Role Management:** Powered by Supabase Auth with bcrypt password hashing, unified username/email login resolution, and an administrative console for user role adjustments.
* **Unrestricted Local Execution:** Directly connects to local LLM runners (such as Ollama or LM Studio) to support unaligned or abliterated models without corporate safety filters or refusals.
* **Live Web Research & Archive:** Integrated Tavily and Brave Search providers with automatic weekly news syncing, historical date-range backfilling, and a shared intelligence archive.
* **Local Memory & Persistence:** Per-account chat history storage, export/import JSON utilities, and custom trainer memory injections.
* **Sleek, Responsive UI:** Single-file HTML application featuring a centered model status bar, dynamic ambient background lighting, custom SVG branding, and markdown/code block formatting with one-click copy.

---

## Tech Stack

* **Frontend:** Single-file HTML5/CSS3/JavaScript, Tailwind-inspired custom CSS variables, and Marked.js for markdown rendering.
* **Backend & Database:** Supabase (PostgreSQL, Auth, custom SQL RPC functions, and Row Level Security).
* **AI Engine:** Ollama / LM Studio local runtime (`qwen3:8b`, abliterated variants, or custom `Modelfiles`).

---

## Quick Start & Deployment

1. **Host the Interface:** Drop `Project AI.html` (or `index.html`) into a static hosting provider like **Cloudflare Pages**, **Netlify Drop**, or **GitHub Pages**.
2. **Configure Supabase:** Run the required SQL migration schema in your Supabase SQL Editor to set up the `profiles` table, handle-new-user triggers, and login identifier resolution.
3. **Connect to Your Local LLM:** 
   * Ensure your local model runner (Ollama) is active and accessible over your network or Tailscale tunnel.
   * Open the app interface, navigate to **Settings → Connection**, input your server URL (e.g., `http://100.x.x.x:11434`), specify your model name, and click **Connect**.**
