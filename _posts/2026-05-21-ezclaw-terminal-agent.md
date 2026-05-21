---
layout: post
title: "EzClaw: The Zero-Fuss Terminal Agent for Ollama"
---

Sometimes you just want an AI agent that lives in your terminal, knows your files, and doesn't require a PhD in configuration to set up. Most agents today are either too heavy, too "cloudy," or just plain messy.

That’s why I built **EzClaw**.

EzClaw is a minimalist, tool-equipped terminal assistant powered by Ollama. It’s designed to be the "Swiss Army Knife" for local LLM workflows—focused on speed, persistence, and utility.

### Why "Ez"?
The goal was "Zero-Fuss." You clone it, you install the requirements, and you're talking to your local models with full filesystem access in seconds. No complex YAML manifests, no heavy Docker containers—just Python and SQLite.

### The Power of Native Memory
One of the biggest frustrations with local agents is their "amnesia." Every time you restart the process, they forget who you are. EzClaw solves this with a native SQLite-backed memory system. 
- **Persistent History**: Every conversation is saved.
- **Fact Recall**: You can explicitly tell EzClaw to `remember` something (like your project goals or code preferences) and it will `recall` it in a future session.

### Beyond Just Chat
EzClaw isn't just a wrapper for Ollama. It’s a functional agent with a suite of built-in tools:
- **Filesystem Mastery**: It can read, write, and list files autonomously.
- **Shell Execution**: It can run commands and analyze the output.
- **Heartbeat Monitor**: It includes a background task scheduler that monitors `heartbeat.md` for pending tasks and notifies you when they're due.
- **Diagnostics**: Built-in `/diagnose` commands to check your NVIDIA GPU health and Ollama model status.

### The UI
Using the `Rich` and `prompt_toolkit` libraries, I’ve given EzClaw a clean, modern terminal interface. It supports real-time "thinking" blocks, syntax-highlighted markdown, and a command-palette style prompt.

### Open Source
If you’re looking for a local agent that "just works" and respects your privacy, give EzClaw a try.

[**GitHub: xaymup/ezclaw**](https://github.com/xaymup/ezclaw)

Local AI is getting faster, and with tools like EzClaw, it's getting a lot more useful.
