# OpenClaw Launch

Managed hosting for open-source AI agents. Pick OpenClaw, Hermes Agent or a coding harness, click deploy, and it is live in about 30 seconds.

[openclawlaunch.com](https://openclawlaunch.com) · [Pricing](https://openclawlaunch.com/pricing) · [Changelog](https://openclawlaunch.com/changelog) · [中文](https://openclawlaunch.com/zh)

---

## What it is

Self-hosting an agent means a VPS or a spare Mac, Docker, ports and firewall rules, config files, TLS certificates and health checks, usually 2 to 6 hours before the first message. OpenClaw Launch does all of that for you. Each agent gets its own sandboxed cloud machine, and you run everything from the browser. A 30-minute free trial needs no card.

## Pick a runtime

| Runtime | What it is |
|---|---|
| [OpenClaw](https://github.com/openclaw/openclaw) | The original open-source agent framework (MIT) and the largest community. The safe default. |
| [Hermes Agent](https://github.com/NousResearch/hermes-agent) | By Nous Research, built around memory that lasts across sessions. Several bots can share one instance. |
| Coding harness | Not a chat bot: a cloud dev box with Claude Code, Codex, OpenCode, Aider, pi and more installed, driven from a browser terminal or from its own Telegram bot. Code and logins survive a reset. |

All three run on the same plans and infrastructure. You choose at deploy time.

## Where you talk to it

| Channel | OpenClaw | Hermes |
|---|---|---|
| Web chat in the dashboard (works on phones) | ✓ | ✓ |
| Telegram | ✓ | ✓ |
| Discord | ✓ | ✓ |
| WhatsApp | ✓ | ✓ |
| WeChat | ✓ | ✓ |
| Feishu / Lark | ✓ | ✓ |
| Slack | — | ✓ |
| OpenClaw app for iPhone and Android | ✓ | — |
| Hermes Desktop | — | ✓ |

You can ask the bot itself to connect a chat app or show its pairing QR code. You also choose who may talk to it: on WhatsApp only you, an allowlist or anyone, and in Telegram groups it can stay quiet until someone @mentions it.

## Features

### Its own computer

- Full terminal with root inside the bot's own container, plus SSH and Tailscale access.
- File manager: browse, upload, download and edit every file, including folders.
- Live Browser: watch the agent browse in real time and take over for a login or a 2FA tap, then hand control back.
- Live Desktop: a full Linux desktop with browser, terminal and files in a browser tab.
- Connect your own computer so the agent can work on it, with your approval.
- Host static and dynamic websites with automatic HTTPS and custom domains, and show yours off in the public websites gallery if you like.
- Build Android APKs, iOS previews and Expo apps.
- Edit the bot's config and instructions in the browser, with one-click rollback and one-click version updates.
- Large files come back as secure, time-limited download links.

### Apps, tools and skills

- 1,000+ app integrations (Gmail, GitHub, Google Drive, Calendar and Sheets, Slack, Notion, Outlook, Canva and more), connected by OAuth or just by asking the bot.
- Thousands of community skills, security-vetted, installable on one bot or synced to all of them.
- A catalog of 100+ open-source tools and connectors installable in a click: n8n, Ollama, ComfyUI, Playwright, Crawl4AI, SearXNG, yt-dlp, Mem0 and more.
- Long-term memory tools, voice transcription and real-time web search, with your own search key (Tavily, and more on Hermes) if you prefer.
- A catalog of Chinese apps (高德, 12306, 飞书, 企查查 and more) for Chinese-language users.
- Trigger a bot from a webhook, and point desktop AI apps at your bot through an opt-in endpoint.

### Bot teams

- Give each bot one job. Bots hand tasks to each other and bring you one answer.
- Dozens of ready-made crew bots to add in a click, or ask a bot to create a teammate.
- A Telegram Team wizard puts several bots in one group, where they @mention each other.
- OpenClaw personas, each with its own model, memory and skills.

### Dashboard

- Quick Chat: every bot in one chat window, one click to switch. Name each bot, and get starter prompts right after deploy.
- Web chat with slash commands, file, image, PDF and spreadsheet uploads, live tool progress, and inline images and video.
- Interactive views in Hermes chat: charts, drawings and small games, not just text.
- Scheduled tasks in your own timezone.
- Ask OpenClaw, the built-in setup and repair assistant, from the bot card or with `/openclaw` in Telegram. Hermes bots open their native Hermes dashboard from the card with no second password.
- Real-time logs and health monitoring; sleeping bots wake up automatically.
- Automatic daily backups, plus one-click export and import of the whole bot.
- Templates to start from, and a searchable guides library.

### Images, video and voice

- Image generation and editing with several providers, including your ChatGPT plan.
- Video: narrated explainer videos in English or Chinese, plus AI video generation.
- Music generation and text-to-speech.

## Models

GPT, Claude, Gemini, Grok, DeepSeek, Kimi, GLM, MiniMax, Qwen and more, switchable at any time without redeploying, including mid-chat with `/model`. The picker also browses the full OpenRouter catalog. Three ways to pay for them:

- Included AI credits on every paid plan, top-ups when you need more, and free models.
- Bring your own key: OpenAI, Anthropic, Google, xAI, OpenRouter, DeepSeek, Moonshot, Groq, Ollama Cloud (Hermes) and others, or any OpenAI-compatible endpoint.
- Use an existing ChatGPT subscription instead of per-token API billing.

The current list and per-token prices are on [openclawlaunch.com/models](https://openclawlaunch.com/models).

## Pricing

| Plan | Price | Machine | AI credits |
|---|---|---|---|
| Free trial | $0 for 30 minutes, no card | Web chat and chat apps, free models | Free tokens |
| Lite | $3 first month, then $6/mo ($60/yr) | 1 vCPU, 2 GB RAM, 10 GB, 1 instance | $1/mo |
| Pro | $20/mo ($200/yr) | 2 vCPU, 4 GB RAM, 40 GB, up to 3 instances | $10/mo |

OpenClaw and Hermes cost the same. Need more? Add extra bots, storage, CPU and RAM from the dashboard. Monthly plans cancel anytime; annual plans have a 30-day refund. Refer a friend and earn $1 in AI credits when they subscribe. Full details: [pricing](https://openclawlaunch.com/pricing).

## Developer API and CLI

Every account gets a REST API (`/api/v1`), the `openclawlaunch` CLI and scoped API keys. Manage bots, channels, files, export and import, SSH and signed webhooks from code; create coding workspaces (optionally on an isolated gVisor kernel) and run an agent from a single prompt with its output streamed back.

## Build & Resell

Sell agents under your own brand. [Build & Resell](https://openclawlaunch.com/resell) is prepaid by the hour and includes:

- a ready-made storefront at `yourname.openclawlaunch.app`, with customer sign-in and password reset;
- the same API, CLI and keys, scoped to your customers' bots;
- customers who can bring their own model keys and connect their own chat apps;
- moving a customer between Lite and Pro without rebuilding their bot, and a starter credit with your first key.

## Security

- One isolated container per bot, with its own network and resource and disk limits.
- API keys encrypted at rest (AES-256-GCM), TLS everywhere, and two-factor sign-in.
- Your data is never used for training. Logins are handed off in the Live Browser, never typed into chat.

More on the [security page](https://openclawlaunch.com/security).

## Quick start

1. Go to [openclawlaunch.com](https://openclawlaunch.com).
2. Pick a runtime, a model and a chat platform.
3. Click Deploy. Your agent is live in about 30 seconds.

## Guides

- [Install OpenClaw](https://openclawlaunch.com/guides/install-openclaw): managed vs. DIY
- [OpenClaw AI agent guide](https://openclawlaunch.com/guides/openclaw-agent)
- [Hermes hosting](https://openclawlaunch.com/hermes-hosting) · [Hermes vs. OpenClaw](https://openclawlaunch.com/compare/hermes-agent)
- [Manual](https://openclawlaunch.com/guides/manual) · [All guides](https://openclawlaunch.com/guides)
- [Models & pricing](https://openclawlaunch.com/models) · [API providers](https://openclawlaunch.com/api-providers) · [Tools](https://openclawlaunch.com/tools) · [Integrations](https://openclawlaunch.com/integrations)
- [Changelog](https://openclawlaunch.com/changelog) · [News](https://openclawlaunch.com/news)

## Related

- [awesome-china-mcp](https://github.com/zackchewa/awesome-china-mcp): a curated index of MCP servers for Chinese apps such as 高德, 12306, 飞书 and 企查查.

## Support

Email [support@openclawlaunch.com](mailto:support@openclawlaunch.com) or use the live chat on the site.
