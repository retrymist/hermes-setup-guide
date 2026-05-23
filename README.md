# Hermes Agent Setup Guide

A simple guide to install and run [Hermes Agent](https://github.com/NousResearch/hermes-agent) — an open-source AI agent that runs in your terminal.

## What is Hermes Agent?

Hermes is an AI agent framework by Nous Research. It works with any LLM provider (OpenRouter, Anthropic, OpenAI, local models, etc.) and gives you a coding assistant that can:

- Run terminal commands
- Read and edit files
- Search the web
- Remember things across sessions
- Connect to Telegram, Discord, and other platforms

## Quick Install

```bash
curl -fsSL https://raw.githubusercontent.com/NousResearch/hermes-agent/main/scripts/install.sh | bash
```

## First Run

```bash
# Interactive setup wizard
hermes setup

# Start chatting
hermes
```

The setup wizard will ask you to pick a model provider and enter your API key.

## Recommended Providers (Free Options)

| Provider | How to get access |
|----------|-------------------|
| OpenRouter | Sign up at [openrouter.ai](https://openrouter.ai), free models available |
| Nous Portal | `hermes login` for OAuth access |
| Google Gemini | Free API key at [aistudio.google.com](https://aistudio.google.com) |

## Basic Usage

```bash
# Ask a single question
hermes chat -q "What files are in this directory?"

# Start interactive session
hermes

# Change model
hermes model

# Check health
hermes doctor
```

## Useful Commands (Inside a Session)

| Command | What it does |
|---------|-------------|
| `/new` | Start fresh session |
| `/model` | Switch model |
| `/help` | Show all commands |
| `/quit` | Exit |

## Connect to Telegram (Optional)

```bash
hermes gateway setup
```

Follow the prompts to connect your Telegram bot. After that, you can chat with Hermes from your phone.

## Links

- [Official Docs](https://hermes-agent.nousresearch.com/docs/)
- [GitHub Repo](https://github.com/NousResearch/hermes-agent)
- [Discord Community](https://discord.gg/nousresearch)

---

*This guide is kept simple on purpose. For advanced features (cron jobs, skills, multi-agent, MCP servers), check the official docs.*
