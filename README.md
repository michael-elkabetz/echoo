<div align="center">
  <img src="assets/logo.png" alt="Echoo Icon" width="128" height="128" />
  <h1>Echoo</h1>
  <p><strong>Your AI Shortcut.</strong></p>
  <p>AI that works where you work. Select any text, press a shortcut - rewrite, translate, dictate, or run custom prompts without leaving your app.<br/>Local or external models, inline or popup, screen-aware context.</p>

  <p>
    <a href="https://www.echoo.ai/">
      <img src="https://img.shields.io/badge/macOS-14+-000000?style=for-the-badge&logo=apple&logoColor=white" alt="macOS 14+" />
    </a>
    <a href="https://github.com/michael-elkabetz/echoo/releases">
      <img src="https://img.shields.io/badge/Version-0.11.1--beta-blue?style=for-the-badge" alt="Version" />
    </a>
    <a href="https://www.echoo.ai/">
      <img src="https://img.shields.io/badge/Price-Free-success?style=for-the-badge" alt="Free" />
    </a>
    <a href="LICENSE">
      <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="MIT License" />
    </a>
  </p>

  <p>
    <a href="https://www.echoo.ai/"><strong>Download for macOS</strong></a> &middot;
    <a href="https://www.echoo.ai/marketplace">Marketplace</a> &middot;
    <a href="../../issues/new?labels=bug">Report Bug</a> &middot;
    <a href="../../issues/new?labels=enhancement">Request Feature</a>
  </p>

  <p>
    <a href="#features">Features</a> &middot;
    <a href="#supported-models">Models</a> &middot;
    <a href="#quick-start">Quick Start</a> &middot;
    <a href="#whats-new">What's New</a>
  </p>

  <br/>

  <img src="assets/examples/echoo.gif" alt="Echoo in action" width="600" />
</div>

---

## Table of Contents

- [About](#about)
- [Quick Start](#quick-start)
- [Features](#features)
  - [Text](#-text)
  - [Voice](#-voice)
  - [Screen Context](#-screen-context)
  - [Custom Commands & Marketplace](#-custom-commands--marketplace)
  - [Files](#-files)
  - [Local LLMs](#-local-llms)
  - [Settings](#-settings)
- [Supported Models](#supported-models)
- [Default Shortcuts](#default-shortcuts)
- [What's New](#whats-new)
- [Why Echoo](#why-echoo)
- [Privacy First](#privacy-first)
- [Support the Project](#support-the-project)
- [Community & Contributing](#community--contributing)
- [Links](#links)

---

## About

Echoo is a free, open-source macOS app that transforms text using AI keyboard shortcuts. Fix typos, grammar, change tone, summarize, and rewrite - all with shortcuts. Never break your flow.

It works system-wide across every app, supports on-device voice input, screen-aware context, custom commands, file analysis, a community marketplace, and can run fully offline with local LLMs.

**BYOK** - Bring your own API key. Your text goes directly to your chosen AI provider. Echoo never sees your data.

Built with Swift and SwiftUI. No Electron. No web views. Pure native performance.

---

## Quick Start

1. **Download** - Grab the latest version from [echoo.ai](https://www.echoo.ai/).
2. **Install** - Open the DMG and drag Echoo to your Applications folder.
3. **Set Up** - Launch Echoo and follow the onboarding to grant Accessibility permission and set your API key.
4. **Use It** - Select text anywhere, press your shortcut, and watch the magic happen.

**Optional:**
- **Connect a Local LLM** - Go to Settings and point Echoo at your Ollama, LocalAI, or LiteLLM endpoint for zero-cost, fully private AI.
- **Install Voice Model** - Go to Settings > Commands > Dictate and download the Parakeet v3 model (~650 MB) for on-device speech recognition.
- **Browse the Marketplace** - Discover and install community-created commands at [echoo.ai/marketplace](https://www.echoo.ai/marketplace).

### Permissions

| Permission | Required | Purpose |
|-----------|----------|---------|
| **Accessibility** | Yes | Capture selected text and simulate keyboard shortcuts |
| **Microphone** | Optional | Voice dictation and voice instruction commands |
| **Screen Recording** | Optional | Screen context screenshots for AI processing |

> *Requires macOS 14 (Sonoma) or later.*

---

## Features

### ⚡ Text

Fix typos, grammar, change tone, summarize, and rewrite - all with shortcuts. Never break your flow.

- **Rewrite** (`⌥R`) - Proofread, fix grammar, and polish. Replaces your selection inline.
- **Summarize** (`⌥S`) - TL;DR, main topics, and action items in a popup.
- **Translate** (`⌥T`) - Translate to any language instantly without switching apps.
- **Ask** (`⌥A`) - Ask questions about selected text. Get answers in a popup.
- **Prompt Craft** (`⌥P`) - Optimize any prompt using a multi-layer architecture.

Each command can be configured with your preferred AI provider, model, and temperature.

<div align="center">
  <img src="assets/examples/text-rewrite.gif" alt="Text Rewrite Demo" width="600" />
  <br/><br/>
  <img src="assets/examples/text-summary.gif" alt="Text Summary Demo" width="600" />
</div>

### 🎙️ Voice

4x faster than typing. Echoo's local voice engine, powered by **NVIDIA Parakeet V3**. Blazing fast, 25 languages, post-processing, running locally. Maximum security, zero cost.

- **Dictate** (`⌥V`) - Speak and text appears at your cursor. Push-to-talk or toggle modes.
- **Voice Instruction** (`⌥I`) - Select text, speak an instruction ("make this shorter and professional"), and AI applies it.
- **Voice Custom Commands** - Trigger any custom command by voice.
- **Post-processing** - Chain dictation output into any command (e.g., dictate then auto-translate to French).
- **Read Aloud** (`⌥L`) - Select any text and have it read back using macOS text-to-speech. Auto-detects language for the right voice. Optionally run any AI command (Rewrite, Summarize, Translate, etc.) on the text before speaking. Adjustable speed (0.5x-2x). Press the shortcut again to stop.
- **Voice Launcher** (`⌃` hold) - Hold the Control key, say a command name ("rewrite", "summarize", "translate"), and it executes. Works with all built-in, custom, and marketplace commands. No shortcut memorization needed.

<div align="center">
  <img src="assets/examples/voice-dictate.gif" alt="Voice Dictate Demo" width="600" />
  <br/><br/>
  <img src="assets/examples/voice-instruct.gif" alt="Voice Instruct Demo" width="600" />
</div>

### 📸 Screen Context

Toggle on to attach a screenshot with any command. AI gets your text + what's on screen as context. Uses macOS ScreenCaptureKit. Works with any command - built-in, custom, or voice instruction. When using voice instruction without selected text, Echoo switches to a screen-only analysis mode.

### 🎯 Custom Commands & Marketplace

Build custom AI commands or grab ready-made ones from the [marketplace](https://www.echoo.ai/marketplace). All composable, all yours.

- **Custom system prompts** - Write any prompt, assign a shortcut.
- **Text or voice input** - Create text-based or voice-triggered commands.
- **Inline or popup** - Choose whether the response replaces your text or appears in a popup.
- **Per-command model** - Assign a different AI provider and model to each command.
- **Screenshot context** - Optionally include screen context.
- **Import & export** - Share commands as `.echoo` files or download from the marketplace.

<div align="center">
  <img src="assets/examples/custom.gif" alt="Custom Command Demo" width="600" />
  <br/><br/>
  <img src="assets/examples/marketplace.gif" alt="Marketplace Demo" width="600" />
</div>

### 📄 Files

Select files, use shortcuts to summarize, extract, translate, or ask questions - without opening them. Supports PDF, DOC, and TXT.

<div align="center">
  <img src="assets/examples/file-ask.gif" alt="File Ask Demo" width="600" />
</div>

### 🔒 Local LLMs

Connect **Ollama**, **LocalAI**, or **LiteLLM**. Your data never leaves your device - no API costs, no usage limits, full control. Works offline.

<div align="center">
  <img src="assets/examples/ollama.gif" alt="Local LLM Demo" width="600" />
</div>

### ⚙️ Settings

Customize providers, models, shortcuts, appearance, and more.

- **Dark mode** toggle
- **Completion sound** toggle
- **Show in Dock** toggle
- **Launch at login**
- **Per-command model & provider**

<div align="center">
  <img src="assets/examples/ui.gif" alt="Settings UI Demo" width="600" />
</div>

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Supported Models

Choose your AI engine - top cloud providers or local models for full privacy. Switch anytime, your workflow stays the same.

### Cloud Providers

| Provider | Models | Default |
|----------|--------|---------|
| **OpenAI** | GPT-4.1 Nano, GPT-5 Mini, GPT-5.2 | GPT-4.1 Nano |
| **Anthropic** | Claude Haiku 4.5, Claude Sonnet 4.5, Claude Opus 4.6 | Claude Haiku 4.5 |
| **Google** | Gemini 2.5 Flash Lite, Gemini 2.5 Pro, Gemini 3 Pro, Gemini 3 Flash | Gemini 2.5 Flash Lite |
| **Groq** | Ultra-fast cloud inference | — |
| **OpenRouter** | Multi-provider gateway (100+ models) | — |
| **DeepSeek** | Cost-effective reasoning models | — |
| **Mistral** | European AI provider | — |

### Local Providers

| Provider | Description |
|----------|-------------|
| **Ollama** | Run open-source models locally (Llama, Mistral, etc.) |
| **LocalAI** | OpenAI-compatible local inference server |
| **LiteLLM** | Proxy for 100+ model providers behind a unified API |

Each command can use a different provider and model. Switch freely per workflow.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Default Shortcuts

All shortcuts use the **Option (⌥)** key and are fully customizable in Settings.

| Shortcut | Command |
|----------|---------|
| `⌥R` | **Rewrite** - Fix grammar & polish (inline replace) |
| `⌥S` | **Summarize** - TL;DR & key points (popup) |
| `⌥T` | **Translate** - Translate to chosen language (popup) |
| `⌥A` | **Ask** - Q&A about selected text (popup) |
| `⌥P` | **Prompt Craft** - Optimize a prompt (popup) |
| `⌥V` | **Dictate** - Voice to text (on-device) |
| `⌥I` | **Voice Instruction** - Speak to edit text |
| `⌥L` | **Read Aloud** - Text-to-speech with AI pre-processing |
| `⌃` (hold) | **Voice Launcher** - Say a command name to execute it |

Custom commands get their own shortcuts from a dedicated pool.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## What's New

### v0.11.1-beta - Auto Select All & Voice Launcher Control Key

- **Auto select all** - No more `⌘A` before running inline commands. Echoo automatically selects all text when nothing is selected, so you can just press your shortcut and go.
- **Voice Launcher default key changed** - Voice Launcher now defaults to the Control key (⌃) instead of Fn. Hold Control, speak a command name, and it executes. Fully customizable in Settings.

### v0.11.0-beta - Heading to Official Release

Echoo is heading toward its first official release. This is the most complete version yet.

- **Screen Context** - Attach a screenshot to any command so the AI can see what's on your screen. Uses macOS ScreenCaptureKit. Toggle per-command in Settings. Works with built-in, custom, and voice instruction commands. When using voice instruction without selected text, Echoo switches to screen-only analysis mode.
- **Voice Launcher** - Hold a key (default: Control ⌃), speak a command name, and it executes instantly. Works with all built-in commands, custom commands, and marketplace commands. Recognizes variations ("re-write", "summarise", "read out loud"). A voice-activated command palette - no shortcut memorization needed.
- **Read Aloud with AI Pre-Processing** - Select any text and hear it spoken aloud using macOS text-to-speech. Auto-detects language across 25+ languages. Adjustable speed (0.5x-2x). Chain any AI command as a pre-processing step - e.g., summarize an article, translate the summary to French, then hear it read aloud.
- **Undo support** - Every inline text replacement can be undone with `⌘Z`. Echoo restores your original text instantly.
- **Cleaner command management** - Disabled commands are now removed from the active command list, keeping your workspace clean.
- **UX refinements** - Quality-of-life fixes across text processing, clipboard handling, and voice flows.

### v0.10.6 - Model Updates, Voice Engine & Polish

- **Latest models** - Updated to GPT-5.2, Claude Opus 4.6, Gemini 3 Pro/Flash, and more.
- **Voice custom commands** - Create custom commands triggered by voice input.
- **UI refinements** - Improved settings layout, command cards, and overall polish.
- **Dark mode** - Full dark mode support across the entire app.
- **Notch-aligned toasts** - Processing and error notifications align elegantly with the macOS notch.
- **Onboarding** - Guided first-run experience for permissions, API key, and command overview.
- **Completion sound** - Optional audio feedback when processing finishes.
- **Dramatically improved voice engine** - Parakeet v3 for faster, more accurate on-device speech recognition.
- **Bug fixes and stability improvements** across text processing, clipboard handling, and voice flows.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Why Echoo

Since the AI revolution began, my workflow changed completely - but not entirely for the better.

I found myself constantly writing content in various apps (Slack, Gmail, Notes, VS Code) and then interrupting my flow to:
1. Copy the text.
2. Switch to a browser tab with ChatGPT or Claude.
3. Paste the text and write a prompt ("Make this more professional," "Fix the grammar," "Translate to English").
4. Wait for the result.
5. Copy the result.
6. Switch back to my original app.
7. Paste it back.

The constant context switching was killing my focus. I wanted the AI to come to *me*, right where I was working, without the friction.

**That's why I built Echoo** - AI text transformation directly at your fingertips. Select text anywhere on your Mac, hit a shortcut, and watch it transform instantly. No tab switching. No copy-pasting. Just flow.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Privacy First

Your data belongs to you.

- **BYOK** - Bring your own API key. Your text goes directly to your chosen AI provider. Echoo never sees your data.
- **On-device voice** - Dictation runs entirely on your Mac using Parakeet v3. Your voice never leaves your machine.
- **Local data** - All settings and history stay on your machine in a local database.
- **No training** - Your text is never used to train any models.
- **Local LLM option** - With Ollama, LocalAI, or LiteLLM, your data never leaves your device. Zero external API calls. Works offline.
- **Hardened runtime** - Signed and notarized macOS app with hardened runtime enabled.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Support the Project

Echoo saves you hours. Support the project so we can build tools to save you even more.

<p align="center">
  <a href="https://ko-fi.com/echooai"><strong>Buy me a coffee on Ko-fi</strong></a>
</p>

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Community & Contributing

Have a bug to report or a feature idea? We'd love to hear from you:

- **Bug Reports** - [Open an Issue](../../issues/new?labels=bug) to report problems or unexpected behavior.
- **Feature Requests** - [Open an Issue](../../issues/new?labels=enhancement) to suggest new features or improvements.
- **Discussions** - Use [GitHub Discussions](../../discussions) for general questions, ideas, or community conversations.
- **Marketplace** - Share your custom commands with the community and discover what others have built.

> *"It is exactly what an AI assistant should be, with the minimum interface necessary and very transparent."*
> - Bernard, Writer at [VVMac Magazine](https://vvmac.fr/wordpress_b/?p=10025)

> *"I've tried many tools claiming to do something similar, but none are even remotely as intuitive and user-friendly. Love it!"*
> - Dvir, CEO

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Links

- **Website**: [www.echoo.ai](https://www.echoo.ai/)
- **Download**: [echoo.ai/get/Echoo.dmg](https://www.echoo.ai/get/Echoo.dmg)
- **Releases**: [GitHub Releases](https://github.com/michael-elkabetz/echoo/releases)
- **Marketplace**: [echoo.ai/marketplace](https://www.echoo.ai/marketplace)
- **Blog**: [echoo.ai/blog](https://echoo.ai/blog)
- **Ko-fi**: [ko-fi.com/echooai](https://ko-fi.com/echooai)
- **Twitter**: [@echoo_app](https://twitter.com/echoo_app)
- **About Me**: [mike.org.il](https://mike.org.il)
- **LinkedIn**: [Michael Elkabetz](https://www.linkedin.com/in/michael-elkabetz/)

---

<div align="center">
  <sub>Built for speed ⚡ with ❤️ by <a href="https://www.mike.org.il">Mike</a></sub>
</div>
