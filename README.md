<div align="center">
  <img src="assets/logo.png" alt="Echoo Icon" width="128" height="128" />
  <h1>Echoo</h1>
  <p><strong>Your AI assistant, everywhere on macOS.</strong></p>
  <p>Select text anywhere, hit a shortcut, and let AI transform it instantly.<br/>No browser tabs. No copy-pasting. Just flow.</p>

  <p>
    <a href="https://www.echoo.ai/">
      <img src="https://img.shields.io/badge/macOS-14+-000000?style=for-the-badge&logo=apple&logoColor=white" alt="macOS 14+" />
    </a>
    <a href="https://github.com/michael-elkabetz/echoo/releases">
      <img src="https://img.shields.io/badge/Version-0.9.20--beta-blue?style=for-the-badge" alt="Version" />
    </a>
    <a href="https://www.echoo.ai/">
      <img src="https://img.shields.io/badge/Price-Free-success?style=for-the-badge" alt="Free" />
    </a>
  </p>

  <p>
    <a href="https://www.echoo.ai/"><strong>Download for macOS</strong></a> &middot;
    <a href="../../issues/new?labels=bug">Report Bug</a> &middot;
    <a href="../../issues/new?labels=enhancement">Request Feature</a>
  </p>

  <p>
    <a href="#whats-new">What's New</a> &middot;
    <a href="#features">Features</a> &middot;
    <a href="#quick-start">Quick Start</a> &middot;
    <a href="#commands-marketplace">Marketplace</a>
  </p>

  <br/>

  <img src="assets/examples/echoo.gif" alt="Echoo in action" width="600" />
</div>

---

## Table of Contents

- [About](#about)
- [Features](#features)
  - [Text Transformation](#-text-transformation)
  - [Custom Commands](#-custom-commands)
  - [Voice](#-voice)
  - [Files](#-files)
  - [Local LLM Support](#-local-llm-support)
  - [Commands Marketplace](#-commands-marketplace)
  - [Settings](#-settings)
- [Quick Start](#quick-start)
- [What's New](#whats-new)
- [Why Echoo](#why-echoo)
- [Privacy First](#privacy-first)
- [Community & Contributing](#community--contributing)
- [Links](#links)

---

## About

Echoo is a native macOS app that brings AI text transformation anywhere you work. Select text in any app, hit a shortcut, and transform it instantly — rewrite, summarize, translate, or run custom prompts — without leaving your flow.

It works system-wide across every app, supports voice input, custom commands, file analysis, a community marketplace, and can run fully offline with local LLMs.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Features

### ⚡ Text Transformation

Select any text, hit a shortcut, and transform it instantly. Rewrite, summarize, translate, or run any prompt.

<div align="center">
  <img src="assets/examples/text-rewrite.gif" alt="Text Rewrite Demo" width="600" />
  <br/><br/>
  <img src="assets/examples/text-summary.gif" alt="Text Summary Demo" width="600" />
</div>

### 🎯 Custom Commands

Create your own prompts, assign a shortcut, and execute anywhere. Your workflow, your rules.

<div align="center">
  <img src="assets/examples/custom.gif" alt="Custom Command Demo" width="600" />
</div>

### 🎙️ Voice

Dictate text and translate simultaneously. Give voice instructions to edit selected text naturally. Create **voice custom commands** — trigger any of your custom prompts by speaking their name. Powered by **Parakeet v3** and **FluidAudio** for fast, accurate recognition.

<div align="center">
  <img src="assets/examples/voice-dictate.gif" alt="Voice Dictate Demo" width="600" />
  <br/><br/>
  <img src="assets/examples/voice-instruct.gif" alt="Voice Instruct Demo" width="600" />
</div>

### 📄 Files

Select a PDF, DOC, or TXT file in Finder and summarize, translate, or ask questions about it — without opening it.

<div align="center">
  <img src="assets/examples/file-ask.gif" alt="File Ask Demo" width="600" />
</div>

### 🔒 Local LLM Support

Run AI completely on your machine with **Ollama**, **LocalAI**, or connect through **LiteLLM** proxy. Maximum data security. Zero costs.

<div align="center">
  <img src="assets/examples/ollama.gif" alt="Local LLM Demo" width="600" />
</div>

### 🛒 Commands Marketplace

Download commands created by other users and share your own. The community decides what's useful.

<div align="center">
  <img src="assets/examples/marketplace.gif" alt="Marketplace Demo" width="600" />
</div>

### ⚙️ Settings

Customize your experience — providers, models, shortcuts, and more.

<div align="center">
  <img src="assets/examples/ui.gif" alt="Settings UI Demo" width="600" />
</div>

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Quick Start

1. **Download** — Grab the latest version from [echoo.ai](https://www.echoo.ai/).
2. **Install** — Unzip and move Echoo to your Applications folder.
3. **Grant Permissions** — Open Echoo and allow Accessibility access when prompted (required for system-wide text selection).
4. **Use It** — Select text anywhere, press your shortcut, and watch the magic happen.

**Optional:**
- **Connect a Local LLM** — Go to Settings and point Echoo at your Ollama, LocalAI, or LiteLLM endpoint for zero-cost, fully private AI.
- **Browse the Marketplace** — Discover and install community-created commands to supercharge your workflow.

> *Requires macOS 14 (Sonoma) or later.*

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## What's New

### UI Improvements, Dark Mode & Bug Fixes

Refined UI with improved polish throughout. Full **Dark Mode** support for comfortable use in low-light environments. Plus stability improvements and bug fixes across the board.

### Voice Custom Commands

Create custom commands that you can trigger by voice. Define your own voice-activated prompts and execute them hands-free — dictate a command name, and Echoo runs it instantly.

### Dramatically Improved Voice Engine

Voice input has been completely overhauled. Echoo now uses **Parakeet v3** for faster, more accurate speech recognition and **FluidAudio** for seamless audio processing — resulting in a dramatically smoother and more reliable voice experience.

### Notch-Aligned Toast Notifications

Toast notifications have been redesigned to appear elegantly alongside the macOS notch, giving you unobtrusive, polished feedback exactly where you'd expect it.

### Onboarding Dialog & Completion Sound

First-time users now get a friendly onboarding dialog to get started quickly. Plus, hear a satisfying completion sound when AI finishes transforming your text.

### Local / In-House LLM Support

Connect Echoo to models running locally with **Ollama**, **LocalAI**, or through a proxy with **LiteLLM**. Your data never leaves your machine and there are zero API costs.

<div align="center">
  <img src="assets/examples/ollama.gif" alt="Local LLM with Ollama" width="600" />
</div>

### Commands Marketplace

Browse, download, and share AI commands created by the community. Find the perfect command for your workflow or publish your own.

<div align="center">
  <img src="assets/examples/marketplace.gif" alt="Commands Marketplace" width="600" />
</div>

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Why Echoo

Since the AI revolution began, my workflow changed completely — but not entirely for the better.

I found myself constantly writing content in various apps (Slack, Gmail, Notes, VS Code) and then interrupting my flow to:
1. Copy the text.
2. Switch to a browser tab with ChatGPT or Claude.
3. Paste the text and write a prompt ("Make this more professional," "Fix the grammar," "Translate to English").
4. Wait for the result.
5. Copy the result.
6. Switch back to my original app.
7. Paste it back.

The constant context switching was killing my focus. I wanted the AI to come to *me*, right where I was working, without the friction.

**That's why I built Echoo** — AI text transformation directly at your fingertips. Select text anywhere on your Mac, hit a shortcut, and watch it transform instantly. No tab switching. No copy-pasting. Just flow.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Privacy First

Your data belongs to you.

- **Local Data** — All your settings and history stay on your machine.
- **No Training** — Your text is never used to train any models.
- **Secure Keys** — API keys are stored securely in the macOS Keychain.
- **Local LLM Option** — With Ollama or LocalAI, your data never leaves your machine. Zero external API calls.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Community & Contributing

Echoo is growing fast — approaching **1,000 users** through word of mouth alone.

Have a bug to report or a feature idea? We'd love to hear from you:

- **Bug Reports** — [Open an Issue](../../issues/new?labels=bug) to report problems or unexpected behavior.
- **Feature Requests** — [Open an Issue](../../issues/new?labels=enhancement) to suggest new features or improvements.
- **Discussions** — Use [GitHub Discussions](../../discussions) for general questions, ideas, or community conversations.
- **Marketplace** — Share your custom commands with the community and discover what others have built.

Your input helps make Echoo better!

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Links

- **Website**: [www.echoo.ai](https://www.echoo.ai/)
- **Releases**: [GitHub Releases](https://github.com/michael-elkabetz/echoo/releases)
- **Commands Marketplace**: [echoo.ai/marketplace](https://www.echoo.ai/marketplace)
- **Blog**: [echoo.ai/blog](https://echoo.ai/blog)
- **About Me**: [mike.org.il](https://mike.org.il)
- **LinkedIn**: [Michael Elkabetz](https://www.linkedin.com/in/michael-elkabetz/)

---

<div align="center">
  <sub>Built with ❤️ by Michael Elkabetz</sub>
</div>
