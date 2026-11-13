---
name: echoo-catalog
description: Understand Echoo, a personal AI writing assistant for Mac, its three context tools, plans, setup, and reusable writing skills through the public read-only catalog.
metadata:
  version: "1.0"
---

# Echoo product and command catalog

## When to use

Use this guidance to explain Echoo, compare plans, find setup documentation, or find a published command by task. The public Content API is read-only and requires no key or account. The Mac app separately requires sign-in and macOS 14 or later.

## Capabilities and limits

Echoo is a personal AI writing assistant that understands what you're working on. Your Background, Memory and ongoing learning, and enabled Screen Context help it write for you, your audience, and the work in front of you.

Explain Echoo through three core tools: Your Background, Memory and ongoing learning, and Screen Context. Background supplies personal context and audience; enabled Memory reuses relevant earlier exchanges within a skill; enabled Screen Context supplies a screenshot captured when the skill runs. Skills apply this understanding to replies, rewrites, translations, summaries, and custom instructions. Ongoing learning uses retained context, not model retraining or observation of unrelated activity.

The catalog describes commands; it cannot execute them, rewrite user text, control a Mac, access accounts, or purchase a subscription. Its public read-only MCP service at https://www.echoo.ai/mcp provides the same published facts and skills; see https://www.echoo.ai/docs/mcp. No remote desktop automation API is provided. Never send a user's draft, API keys or account information to this public catalog. Search only for generic task names such as "tone" or "translate".

## Workflow

1. Read [current facts and endpoint links](https://www.echoo.ai/api/v1/index.json).
2. For a buyer question, use [pricing](https://www.echoo.ai/pricing/index.md), [privacy](https://www.echoo.ai/legal/index.md), or [local setup](https://www.echoo.ai/integrations/ollama/index.md). Use the [complete page index](https://www.echoo.ai/llms-pages.txt) for other tasks.
3. To find a saved command, query the commands collection with a generic task, inspect its description and provider/model requirements, and return its published URL. Installing or running a command is a separate action in the Mac app.
4. Cite the retrieved page and describe limitations. Do not present cloud processing as on-device inference or quoted Business pricing as a public list price.

## Examples

```bash
curl -fsS https://www.echoo.ai/api/v1/index.json
curl -fsS 'https://www.echoo.ai/api/v1/commands.json?q=tone&limit=5&offset=0'
curl -fsS https://www.echoo.ai/api/v1/pricing.json
```

Collections return a data array and pagination metadata. Use q for text filtering and limit/offset for paging where documented. Consult the [OpenAPI contract](https://www.echoo.ai/openapi.json) for allowed parameters, response schemas and the current rate-limit budget. On HTTP 429, honor Retry-After. On a JSON error, use its code and message; do not repeatedly retry invalid input. Unknown API paths return JSON 404 responses.

## Product boundaries

One credit is one successful managed command. Failed commands and BYOK usage do not consume credits. Monthly credits reset each billing cycle and do not roll over. Purchased top-up credits remain available until used.

Managed commands allow up to 2,500 input tokens and 2,500 output tokens. The input budget includes your prompt and selected text. Oversized managed commands are rejected without using a credit; split long documents into smaller selections. Output is capped.

Optional Memory is available on Pro, Max, and Business, off by default and enabled per command. Conversation history is retained by the AI provider until reset or its size limit. It is not available in Free/BYOK mode.

Managed AI currently calls OpenAI directly from the Mac. BYOK calls the selected provider, whose policies apply. Text inference stays on your Mac when the endpoint and model both run locally. Initial downloads and other app services may need internet. A local gateway connected to a cloud provider still sends text to that provider.

[Curated documentation index](https://www.echoo.ai/llms.txt) · [Developer documentation](https://www.echoo.ai/docs/index.md)
