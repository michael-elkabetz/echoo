<div align="center">
  <img src="assets/logo.png" alt="Echoo Icon" width="128" height="128" />
  <h1>Echoo</h1>
  <p><strong>Use AI in any app without leaving it.</strong></p>
  <p>Write in your language and watch it land in fluent English - same tone, same voice. Echoo rewrites, proofreads, translates, and summarizes inline anywhere on your Mac, powered by Screen Context and a system prompt you fully control. Sign in free, no API key needed, and your text stays private the whole way.</p>

  <p>🌍 Native language → English &middot; 🖥️ Screen Context &middot; 🎛️ Custom system prompts &middot; 🔒 Privacy by design &middot; 🤖 AI writing automation</p>

  <p>
    <a href="https://www.echoo.ai/">
      <img src="https://img.shields.io/badge/macOS-14+-000000?style=for-the-badge&logo=apple&logoColor=white" alt="macOS 14+" />
    </a>
    <a href="https://github.com/michael-elkabetz/echoo/releases">
      <img src="https://img.shields.io/badge/Version-1.2.0-success?style=for-the-badge" alt="Version" />
    </a>
    <a href="https://www.echoo.ai/">
      <img src="https://img.shields.io/badge/Price-Free-success?style=for-the-badge" alt="Free" />
    </a>
  </p>

  <p>
    <a href="https://www.echoo.ai/"><strong>Download for macOS</strong></a> &middot;
    <a href="https://www.echoo.ai/marketplace">Marketplace</a> &middot;
    <a href="../../issues/new?labels=bug">Report Bug</a> &middot;
    <a href="../../issues/new?labels=enhancement">Request Feature</a>
  </p>

  <p>
    <a href="#core-workflows">Workflows</a> &middot;
    <a href="#bring-your-own-model">Models</a> &middot;
    <a href="#quick-start">Quick Start</a> &middot;
    <a href="#whats-new">What's New</a>
  </p>

  <br/>

  <img src="assets/examples/echoo.gif" alt="Echoo in action" width="600" />
</div>

---

## Why Echoo

Echoo is the only Mac text tool that rewrites using what's on your screen, not just what you selected - every other AI writing tool works blind.

Most AI tools live behind a chat window. You copy text, switch tabs, paste it, write a prompt, wait, copy the result, switch back, and paste again. The workflow breaks every time. Echoo skips all of that - select text, trigger a command, get the result inline.

The edits you repeat every day - proofreading, grammar fixes, tone rewrites, translation - become saved commands and multi-step workflows that run from one shortcut in any Mac app.

Free, open source, and built in public.

---

### How it works

1. Echoo detects the current text or file
2. Trigger a command by voice or shortcut
3. Get the result back inline

Echoo also adds a **floating rewrite button** for immediate polishing:

1. Select text in any app
2. Click the floating rewrite button
3. Echoo rewrites it inline without interrupting your flow

**BYOK** - Bring your own API key. Your text goes directly to your chosen provider. Echoo never sees your data. Built with Swift and SwiftUI. No Electron. No web views.

---

## Two Ways to Use Echoo

Pick what fits you - text manipulation (rewrite, proofread, translate, summarize), Screen Context rewrite, and custom system prompts are on both.

- **Managed** - No provider account, no API key to manage. Sign in and start immediately with 10 free credits, then subscribe for unlimited use. It's also the only way to get Memory, where commands learn from your past requests and get better at writing the way you do.
- **BYOK** - Bring your own key from OpenAI, Anthropic, or Google, or run a local model. Free forever, and it's the only way to get voice dictation with your own AI post-processing rules, voice command execution, and local/offline models.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

<details id="table-of-contents">
<summary><strong>Table of Contents</strong></summary>

- [Why Echoo](#why-echoo)
- [Two Ways to Use Echoo](#two-ways-to-use-echoo)
- [Quick Start](#quick-start)
- [Core Workflows](#core-workflows)
  - [Transform text inline](#transform-text-inline)
  - [Dictate and post-process](#dictate-and-post-process)
  - [Run commands on files](#run-commands-on-files)
  - [Commands adapt to text, screen, and voice](#commands-adapt-to-text-screen-and-voice)
- [Bring Your Own Model](#bring-your-own-model)
- [Default Shortcuts](#default-shortcuts)
- [What's New](#whats-new)
- [FAQ](#faq)
- [Privacy](#privacy)
- [Keep Echoo Shipping](#keep-echoo-shipping)
- [Community](#community)
- [Links](#links)

</details>

---

## Quick Start

1. **Download** - Grab the latest version from [echoo.ai](https://www.echoo.ai/).
2. **Install** - Open the DMG and drag Echoo to Applications.
3. **Set up** - Launch Echoo, grant Accessibility permission, then either sign in for the managed plan (10 free credits, no key needed) or add your own API key for BYOK (free forever).
4. **Use it** - Select text anywhere, press a shortcut, get the result inline.

**Optional:**
- **Local LLM** - Point Echoo at Ollama, LocalAI, or LiteLLM for fully private, zero-cost AI.
- **Voice model** - Download Parakeet v3 (~650 MB) in Settings for on-device speech recognition.
- **Marketplace** - Browse and install community commands at [echoo.ai/marketplace](https://www.echoo.ai/marketplace).

### Permissions

| Permission | Required | Purpose |
|-----------|----------|---------|
| **Accessibility** | Yes | Capture selected text and simulate keyboard shortcuts |
| **Microphone** | Optional | Voice dictation and voice instruction commands |
| **Screen Recording** | Optional | Screen context screenshots for AI processing |

> *Requires macOS 14 (Sonoma) or later.*

---

## Core Workflows

### Transform text inline

Echoo detects the current text automatically, runs the command you trigger by voice or shortcut, and returns the result inline. Fix grammar, proofread, rewrite in a different tone, translate, summarize, or run a custom prompt without breaking flow.

- **Rewrite** (`⌥R` or floating button) - Proofread, fix grammar, and polish. Replaces your selection inline.
- **Summarize** (`⌥S`) - Key points and action items in a popup.
- **Translate** (`⌥T`) - Translate to any language without switching apps. Write in your native language and translate inline into English (or back) while Echoo keeps your tone and style - casual stays casual, formal stays formal.
- **Ask** (`⌥A`) - Ask questions about selected text. Answers in a popup.
- **Prompt Craft** (`⌥P`) - Optimize any prompt using a multi-layer architecture.

Each command can use a different AI provider, model, and temperature.

<div align="center">
  <img src="assets/examples/text-rewrite.gif" alt="Text Rewrite Demo" width="600" />
  <br/><br/>
  <img src="assets/examples/text-summary.gif" alt="Text Summary Demo" width="600" />
</div>

### Dictate and post-process

Speak the text you want to insert, then optionally run a command before Echoo places the final result in your app. On-device transcription powered by NVIDIA Parakeet v3 - 25 languages, zero cloud dependency.

- **Dictate** (`⌥V`) - Speak and text appears at your cursor. Push-to-talk or toggle mode.
- **Post-processing** - Chain dictation into any command (e.g., dictate then auto-translate to French).
- **Voice Instruct** (`⌥I`) - Instead of dictating content, say what should happen: "Make this shorter" or "Translate this to Spanish."
- **Read Aloud** (`⌥L`) - Select text and hear it spoken aloud. Auto-detects language. Optionally run any AI command before speaking (summarize, translate, simplify). Adjustable speed (0.5x–2x).
- **Voice Launcher** (`⌃` hold) - Hold the Control key, say a command name, and it executes. That now includes **Claude Code Skills**, so repo-aware workflows can start with your voice instead of a terminal command.

<div align="center">
  <img src="assets/examples/voice-dictate.gif" alt="Voice Dictate Demo" width="600" />
  <br/><br/>
  <img src="assets/examples/voice-instruct.gif" alt="Voice Instruct Demo" width="600" />
</div>

### Run commands on files

Select files in Finder and run the same command system on them. Summarize documents, translate content, extract information, or ask questions - without opening each file. Supports PDF, DOC, and TXT.

<div align="center">
  <img src="assets/examples/file-ask.gif" alt="File Ask Demo" width="600" />
</div>

### Commands adapt to text, screen, and voice

In Echoo, commands are reusable system prompts that work across different inputs and outputs. Use them to post-process dictation, add screen context when the answer depends on what you see, or clean up text before Read Aloud plays it back.

- **Custom system prompts** - Write any prompt, assign a shortcut.
- **Text or voice input** - Create text-based or voice-triggered commands.
- **Inline or popup** - Choose whether the response replaces text or appears in a popup.
- **Per-command model** - Assign a different provider and model to each command.
- **Claude Code Skills** - This is the new workflow. Run Claude Code Skills by voice or shortcut, skip the CLI, and get the result back on screen. When needed, Echoo still uses the right folder in the background for repo-aware work.
- **Real skill example** - Ask `/github-trending` for a daily AI-powered summary and Echoo brings back the top repositories, what they do, and why they matter in one compact result.
- **Screen Context** - Toggle on to attach a screenshot with any command. The AI sees your text *and* what's on screen - the only Mac rewrite tool that can do this. Uses macOS ScreenCaptureKit.
- **Memory** - Toggle on and the command remembers your earlier requests and its own earlier results, then learns from them: your terminology and names, your tone, how long your sentences run, how much detail you keep. Each result needs a little less fixing than the last, and your company's name stops getting "corrected" out of your writing. Per command, so translation memory never bleeds into rewrite, and resettable whenever you want a clean slate. Managed plan only.
- **Import & export** - Share commands as `.echoo` files or download from the [marketplace](https://www.echoo.ai/marketplace).

<div align="center">
  <img src="assets/examples/custom.gif" alt="Custom Command Demo" width="600" />
  <br/><br/>
  <img src="assets/examples/marketplace.gif" alt="Marketplace Demo" width="600" />
</div>

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Bring Your Own Model

Echoo does not lock you into one provider. Keep the same shortcut and command workflow while choosing the model that fits your privacy, speed, and cost needs.

### Cloud models

Best for reach, speed, and the latest frontier models.

| Provider | Powerful | Balanced | Fast |
|----------|----------|----------|------|
| **OpenAI** | GPT-5.5 | GPT-5.4 Mini | GPT-5.4 Nano |
| **Anthropic** | Claude Opus 4.8 | Claude Sonnet 5 | Claude Haiku 4.5 |
| **Google Gemini** | Gemini 3.5 Pro | Gemini 3.6 Flash | Gemini 3.5 Flash-Lite |

### Local models

Best for privacy, offline use, and full control. Your data never leaves your device.

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
| `⌥R` | **Rewrite** - Proofread, fix grammar & polish (inline replace) |
| `⌥S` | **Summarize** - Key points (popup) |
| `⌥T` | **Translate** - Translate to chosen language (popup) |
| `⌥A` | **Ask** - Q&A about selected text (popup) |
| `⌥P` | **Prompt Craft** - Optimize a prompt (popup) |
| `⌥V` | **Dictate** - Voice to text (on-device) |
| `⌥I` | **Voice Instruct** - Speak to edit text |
| `⌥L` | **Read Aloud** - Text-to-speech with AI pre-processing |
| `⌃` (hold) | **Voice Launcher** - Say a command name to execute it |

Custom commands get their own shortcuts from a dedicated pool.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## What's New

### v1.2.0 - Memory

- **Memory** - Turn it on for any command and it starts learning from your past requests: your terminology and names, your tone, how long your sentences run, how much detail you keep. Each result needs a little less fixing than the last, and your company's name stops getting "corrected" out of your writing. Each command keeps its own memory, and you can reset it whenever you want a clean slate. Managed plan only.
- **Voice Launcher is off by default** - It now waits until you switch it on in Settings instead of claiming its shortcut on a fresh install.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## FAQ

**What is Echoo?**
Echoo is a macOS AI shortcut layer that rewrites, proofreads, translates, and summarizes text inline in any app - triggered by voice or keyboard shortcut, with no chat window and no copy-paste.

**Is Echoo free?**
Yes. BYOK (bring your own API key) is free forever, including text manipulation, Screen Context rewrite, custom system prompts, voice dictation with your own AI post-processing rules, and voice command execution. The managed plan (no key needed) starts with 10 free credits.

**Do I need an API key to use Echoo?**
No. Sign in to the managed plan and Echoo handles the key for you, starting with 10 free credits. If you'd rather use your own OpenAI, Anthropic, or Google key - or a local model via Ollama, LocalAI, or LiteLLM - BYOK is free forever.

**What makes Echoo different from other AI writing tools?**
Screen Context: Echoo can attach a screenshot to any rewrite, so the AI sees the thread, doc, or design behind your selected text - not just an isolated sentence. No other Mac text tool does this.

**Does Echoo work offline?**
Yes, for voice. Dictation runs entirely on-device using NVIDIA Parakeet v3, with zero cloud dependency. Text commands need a model - either a cloud provider or a local model via Ollama, LocalAI, or LiteLLM for a fully offline setup.

**What languages does Echoo support?**
On-device dictation covers 25+ languages. Translate and rewrite commands support any language your chosen AI model handles, including translating inline into English while keeping your original tone and style.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Privacy

Your data belongs to you.

- **BYOK** - Bring your own API key. Text goes directly to your chosen provider. Echoo never sees your data.
- **On-device voice** - Dictation runs entirely on your Mac using Parakeet v3. Your voice never leaves your machine.
- **Local data** - All settings and history stay on your machine in a local database.
- **No training** - Your text is never used to train models.
- **Local LLM option** - With Ollama, LocalAI, or LiteLLM, everything stays on-device. Zero external API calls. Works offline.
- **Hardened runtime** - Signed and notarized macOS app with hardened runtime enabled.

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Keep Echoo Shipping

Echoo is free, open source, and built in public. If it saves you time, support the project and help fund more workflows, integrations, and polish.

<p align="center">
  <a href="https://ko-fi.com/echooai"><strong>Buy me a coffee on Ko-fi</strong></a>
</p>

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Community

People understand the workflow once they use it.

> *"It is exactly what an AI assistant should be, with the minimum interface necessary and very transparent."*
> - Bernard, Writer at [VVMac Magazine](https://vvmac.fr/wordpress_b/?p=10025)

> *"I've tried many tools claiming to do something similar, but none are even remotely as intuitive and user-friendly. Love it!"*
> - Dvir, CEO

Have a bug or a feature idea?

- **Bug Reports** - [Open an Issue](../../issues/new?labels=bug)
- **Feature Requests** - [Open an Issue](../../issues/new?labels=enhancement)
- **Discussions** - [GitHub Discussions](../../discussions) for questions, ideas, or community conversations
- **Marketplace** - Share your custom commands with the community at [echoo.ai/marketplace](https://www.echoo.ai/marketplace)

<p align="right">(<a href="#table-of-contents">back to top</a>)</p>

---

## Links

- **Website**: [www.echoo.ai](https://www.echoo.ai/)
- **Download**: [echoo.ai/get/Echoo.dmg](https://www.echoo.ai/get/Echoo.dmg)
- **Releases**: [GitHub Releases](https://github.com/michael-elkabetz/echoo/releases)
- **Marketplace**: [echoo.ai/marketplace](https://www.echoo.ai/marketplace)
- **Blog**: [echoo.ai/blog](https://echoo.ai/blog)
- **Guides**: [Best AI rewrite tools for Mac](https://www.echoo.ai/learn/best-ai-rewrite-tools) &middot; [Best AI proofreading tools](https://www.echoo.ai/learn/best-ai-proofreading-tools) &middot; [AI writing automation on Mac](https://www.echoo.ai/use-cases/ai-writing-automation-mac)
- **Ko-fi**: [ko-fi.com/echooai](https://ko-fi.com/echooai)
- **Twitter**: [@echoo_app](https://twitter.com/echoo_app)
- **About Me**: [mike.org.il](https://mike.org.il)
- **LinkedIn**: [Michael Elkabetz](https://www.linkedin.com/in/michael-elkabetz/)

---

<div align="center">
  <sub>Built for speed by <a href="https://www.mike.org.il">Mike</a></sub>
</div>
