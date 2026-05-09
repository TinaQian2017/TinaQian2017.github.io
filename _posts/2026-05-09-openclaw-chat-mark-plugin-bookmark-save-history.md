---
layout: post
title: "OpenClaw Chat Mark Plugin – Bookmark and Reinject Past Chats in OpenClaw Dashboard"
date: 2026-05-09
category: OpenClaw
tags: [OpenClaw, plugin, chatbot, productivity, open-source]
description: "OpenClaw Chat Mark Plugin lets you bookmark, star, and mark specific past chat messages in OpenClaw web UI, then automatically reinject them as context into future conversations."
permalink: /openclaw-chat-mark-plugin/
---

Have you ever been deep in a long conversation with an AI agent in [OpenClaw](https://github.com/openclaw/openclaw) and wished you could reference a specific earlier message without copy-pasting manually? That's exactly the problem **OpenClaw Chat Mark Plugin** solves.

<!-- more -->

## What Is the OpenClaw Chat Mark Plugin?

The [OpenClaw Chat Mark Plugin](https://github.com/TinaQian2017/openclaw-dashboard-chat-mark-plugin) (also known as **openclaw-dashboard-chat-mark-plugin**) is a lightweight, browser-side plugin for the [OpenClaw Control UI / Dashboard](https://docs.openclaw.ai/dashboard). It adds a **@ button** to every chat message — click it to **mark** that message and add it to a personal context pool.

When you send your next message, all marked context is automatically prepended to your input, formatted like this:

```
=== Marked Context (selected by user) ===
<<USER>>
the user's original message
<<AGENT>>
the agent's original response
```

This gives the agent instant "memory" of specific moments in your conversation, without any manual copy-pasting.

## Key Features

- **One-click mark** — hover over any chat message and click the **@** button to toggle it in/out of your context pool
- **Right panel** — all currently marked messages are listed in a **Marked Context** panel for easy review
- **Auto-inject** — on your next send, all marked context is automatically appended to your message via WebSocket interception
- **Privacy-first** — runs entirely in your browser; no data is sent to any external server
- **Easy install** — one command on Linux, macOS, or Windows (Git Bash); no build step required

## Why Bookmarking Chat History Matters in OpenClaw

OpenClaw is a powerful multi-channel AI gateway with a web-based Control UI. When you're working on complex, multi-turn tasks, you often need to reference specific earlier exchanges — a specific clarification, a key decision, an important code snippet. Copying and pasting manually is tedious and breaks your flow.

The OpenClaw Chat Mark Plugin bridges this gap by letting you **bookmark specific chat messages** and **reinject them as context** in one click. It's a small quality-of-life improvement that makes a big difference in long-running AI conversations.

## Supported Platforms

The plugin works with the **OpenClaw Control UI / Dashboard** on all major desktop platforms:

| Platform | Installation |
|----------|-------------|
| **Linux** | One command (see below) |
| **macOS** | One command (see below) |
| **Windows** | Git Bash required (not CMD or PowerShell) — [install Git](https://git-scm.com/download/win) |

Requirements: Node.js (any recent version) and curl. Both are standard on Linux/macOS; Git Bash on Windows includes curl by default.

## Quick Install

```bash
curl -sL "https://raw.githubusercontent.com/TinaQian2017/openclaw-dashboard-chat-mark-plugin/main/install.sh" | bash
```

Restart the OpenClaw gateway after installation. For specific versions or manual install steps, see the [full README on GitHub](https://github.com/TinaQian2017/openclaw-dashboard-chat-mark-plugin#quick-install).

## Uninstall

Simply run the reverse steps or delete the plugin file and restart the gateway. Full removal instructions are in the [GitHub README](https://github.com/TinaQian2017/openclaw-dashboard-chat-mark-plugin#plugin-removal).

## About This Plugin

This is an open-source community plugin for OpenClaw. It is not affiliated with the OpenClaw core team. If you find it useful, feel free to leave feedback or open an issue on [GitHub](https://github.com/TinaQian2017/openclaw-dashboard-chat-mark-plugin).

---

*Plugin developed by [Tina Qian](https://www.linkedin.com/in/yue-qian-0b7110102/).*
