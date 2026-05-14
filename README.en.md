> 🌐 **中文版**: [README.md](./README.md)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made with Claude Code](https://img.shields.io/badge/Made_with-Claude_Code-d97706)](https://docs.claude.com/en/docs/claude-code/overview)
[![Skills](https://img.shields.io/badge/Skills-11_and_growing-10a37f)](https://www.skills.sh/)
[![Status](https://img.shields.io/badge/Status-evolving-5dd4f5)](https://github.com/huasanai/huasan-skills)

<p align="center">
  <img src="./assets/logo.svg" alt="huasan-skills — a growing toolkit of Claude Code skills" width="900">
</p>

# huasan-skills

> **A growing toolkit of Claude Code skills by huasan. Each skill lives in its own repo with a full README, logo, hero, and release notes. This is the front door.**

An evolving toolkit covering AI Coding & learning, content creation, productivity tooling, infrastructure setup, and personal-OS templates.

---

## 5 Categories · 11 Skills

### 🎯 AI Coding · Learning

Help non-programmers understand code, read tools, and turn what they learn into reusable knowledge.

| Skill | ⭐ | One-liner |
|---|---|---|
| [**handcode-tutor**](https://github.com/huasanai/handcode-tutor) | ![Stars](https://img.shields.io/github/stars/huasanai/handcode-tutor?style=flat&label=) | AI coach for hand-typed coding practice. Autocomplete off — type, break, own it. The AI just explains why |
| [**coding-mentor**](https://github.com/huasanai/coding-mentor) | ![Stars](https://img.shields.io/github/stars/huasanai/coding-mentor?style=flat&label=) | AI coding mentor for non-programmers: understand code, break down GitHub projects, grow an Obsidian knowledge base |
| [**ai-coding-wiki**](https://github.com/huasanai/ai-coding-wiki) | ![Stars](https://img.shields.io/github/stars/huasanai/ai-coding-wiki?style=flat&label=) | AI Coding learning skill for Chinese non-programming users (Claude Code / Codex CLI) |

### 🛠 Claude Code · Tooling

Workflow tools for Claude Code daily-use enhancement.

| Skill | ⭐ | One-liner |
|---|---|---|
| [**cc-provider-add**](https://github.com/huasanai/cc-provider-add) | ![Stars](https://img.shields.io/github/stars/huasanai/cc-provider-add?style=flat&label=) | Wire any Anthropic-compatible API endpoint (MiMo / GLM / Kimi etc.) with per-provider `CLAUDE_CONFIG_DIR` isolation. Zero binary deps |
| [**conversation-logger**](https://github.com/huasanai/conversation-logger) | ![Stars](https://img.shields.io/github/stars/huasanai/conversation-logger?style=flat&label=) | Auto-save every Claude Code session as Markdown — zero token cost, real-time, Obsidian-compatible. Captures build-in-public material |

### 🌐 Infra · Environment Setup

| Skill / Doc | ⭐ | One-liner |
|---|---|---|
| [**vps-vpn-setup**](https://github.com/huasanai/vps-vpn-setup) | ![Stars](https://img.shields.io/github/stars/huasanai/vps-vpn-setup?style=flat&label=) | One-click skill to deploy VPS + VPN + Clash proxy via Claude Code / Codex — no manual SSH or commands |
| [**vps-vpn-clash-setup**](https://github.com/huasanai/vps-vpn-clash-setup) 📖 | ![Stars](https://img.shields.io/github/stars/huasanai/vps-vpn-clash-setup?style=flat&label=) | ↑ Paired hand-holding tutorial: get a clean overseas IP via VPS + v2ray-agent + Clash, reducing Claude/ChatGPT ban risk |

### ✍️ Content Creation

| Skill | ⭐ | One-liner |
|---|---|---|
| [**podcast-to-md**](https://github.com/huasanai/podcast-to-md) | ![Stars](https://img.shields.io/github/stars/huasanai/podcast-to-md?style=flat&label=) | One podcast / YouTube URL → structured Chinese markdown: speaker-attributed transcript + summary + quotes + oral script. Free ASR via Groq Whisper |
| [**artifact-html**](https://github.com/huasanai/artifact-html) | ![Stars](https://img.shields.io/github/stars/huasanai/artifact-html?style=flat&label=) | Turn any content (notes, knowledge, flows, comparisons, plans) into a claude.ai-style standalone HTML page with one-click PNG export |
| [**github-epub-productizer**](https://github.com/huasanai/github-epub-productizer) | ![Stars](https://img.shields.io/github/stars/huasanai/github-epub-productizer?style=flat&label=) | Turn book-style GitHub Markdown repos into sellable digital products — EPUB generation, AI-generated covers (Gemini), and product poster rendering |

### 📦 Template

| Skill | ⭐ | One-liner |
|---|---|---|
| [**lifeos-template**](https://github.com/huasanai/lifeos-template) | ![Stars](https://img.shields.io/github/stars/huasanai/lifeos-template?style=flat&label=) | A self-evolving personal OS template with your custom AI assistant — runs on Claude Code & Codex CLI |

---

## How to install

**Each skill is independent.** Click into a repo for its full README with installation. Most are this one line:

```bash
npx skills add huasanai/<skill-name> -g -y
```

For example:

```bash
npx skills add huasanai/handcode-tutor -g -y
npx skills add huasanai/coding-mentor -g -y
```

Compatible with Claude Code / Codex CLI / Cursor / Gemini CLI and other agents in the [skills.sh](https://www.skills.sh/) ecosystem.

---

## Coming soon · Local-only for now

These skills are in long-term local use and will progressively open-source under `huasanai/*`:

- **push-github** — Standardized polish flow for first-time GitHub publishing, with Step 0 auto-sanitization + animated-logo style library + narrative animation patterns
- **learn-by-doing** — Hand-by-hand new-tool teaching + collaborative `howto` distillation (iron rule: verify before answering)
- **Content creation suite** — `cta` (long-form articles) / `oral` (speeches) / `short` (short visuals) / `ill` (illustrations) / `decode` (commentary) / `refine` (fine-tuning)
- **More** — Business toolkits, foreign-trade team workflow suites, etc.

To get notified → ⭐ Star + Watch this repo.

---

## Why independent + aggregate dual-track

Each skill has its own full story, visuals, and release rhythm — **not merged into one repo** — preserving each skill's product-grade ritual. This repo is just the **front door**:
- Want the full set → start here, browse by category
- Want a specific skill's demo, deep docs, or issues → click into its repo

Inspired by [baoyu-skills](https://github.com/JimLiu/baoyu-skills) (Baoyu) and [qiaomu-skills](https://github.com/joeseesun/qiaomu-skills) (Qiaomu), but choosing **"independent repo + aggregated index"** dual-track over packing everything into one repo.

---

## Support & Connect

### Reach me

| Platform | Handle |
|---|---|
| 💬 WeChat | `huasanai` |
| 🐦 X | [@yfusionai](https://x.com/yfusionai) |
| 🎬 Douyin | [@画伞](https://v.douyin.com/zHu4VUhztes/) |

---

## License

MIT © 画伞 (huasan)
