---
type: workflow
id: templates-services
title: "Service Templates"
description: "LLM providers, MCP servers, external services, and vector database templates"
tags: [Production, Templates]
connections:
  - target: svc-anthropic
    type: uses
  - target: svc-openai
    type: uses
  - target: svc-google-gemini
    type: uses
  - target: svc-mistral
    type: uses
  - target: svc-cohere
    type: uses
  - target: svc-ollama
    type: uses
  - target: svc-lm-studio
    type: uses
  - target: svc-llamacpp
    type: uses
  - target: svc-claude-desktop
    type: uses
  - target: svc-chatgpt-desktop
    type: uses
  - target: svc-mcp-github
    type: uses
  - target: svc-mcp-filesystem
    type: uses
  - target: svc-mcp-postgres
    type: uses
  - target: svc-mcp-sqlite
    type: uses
  - target: svc-mcp-brave-search
    type: uses
  - target: svc-mcp-puppeteer
    type: uses
  - target: svc-mcp-memory
    type: uses
  - target: svc-mcp-custom
    type: uses
  - target: svc-slack
    type: uses
  - target: svc-jira
    type: uses
  - target: svc-linear
    type: uses
  - target: svc-notion
    type: uses
  - target: svc-github-api
    type: uses
  - target: svc-email
    type: uses
  - target: svc-pinecone
    type: uses
  - target: svc-chroma
    type: uses
  - target: svc-qdrant
    type: uses
  - target: llm-service
    type: runs_on
metadata:
  estimated_duration: "1 minute"
  trigger: manual
  template: true
output_step: "svc-anthropic"
composite_steps:
  - "svc-anthropic"
  - "svc-openai"
  - "svc-google-gemini"
  - "svc-mistral"
  - "svc-cohere"
  - "svc-ollama"
  - "svc-lm-studio"
  - "svc-llamacpp"
  - "svc-claude-desktop"
  - "svc-chatgpt-desktop"
  - "svc-mcp-github"
  - "svc-mcp-filesystem"
  - "svc-mcp-postgres"
  - "svc-mcp-sqlite"
  - "svc-mcp-brave-search"
  - "svc-mcp-puppeteer"
  - "svc-mcp-memory"
  - "svc-mcp-custom"
  - "svc-slack"
  - "svc-jira"
  - "svc-linear"
  - "svc-notion"
  - "svc-github-api"
  - "svc-email"
  - "svc-pinecone"
  - "svc-chroma"
  - "svc-qdrant"
execution:
  - skill: "svc-anthropic"
    step_type: "generation"
---

## Overview

This skrpt contains 27 service templates for use when creating new service nodes. Import this skrpt to add these templates to your template picker.

## Templates

### LLM Provider

- **Anthropic Claude** — Claude models via the Anthropic API
- **OpenAI** — GPT-4, o1, o3 models via OpenAI API
- **Google Gemini** — Gemini models via Google AI Studio or Vertex AI
- **Mistral AI** — Mistral models via Mistral API
- **Cohere** — Command models via Cohere API

### Local LLM

- **Ollama** — Local LLM runner for private/offline use
- **LM Studio** — Desktop app for running local models with OpenAI-compatible API
- **llama.cpp** — Lightweight C++ inference engine for GGUF models

### Desktop App

- **Claude Desktop** — Anthropic's desktop app with native MCP support
- **ChatGPT Desktop** — OpenAI's desktop app

### MCP Server

- **GitHub MCP** — Repository access, PRs, issues via MCP
- **Filesystem MCP** — Local file system read/write access via MCP
- **PostgreSQL MCP** — PostgreSQL database access via MCP
- **SQLite MCP** — SQLite database access via MCP
- **Brave Search MCP** — Web search via Brave Search API and MCP
- **Puppeteer MCP** — Browser automation and web scraping via MCP
- **Memory MCP** — Persistent knowledge graph memory via MCP
- **Custom MCP Server** — Blank template for a custom MCP server

### External Service

- **Slack** — Slack messaging and notifications
- **Jira** — Jira issue tracking integration
- **Linear** — Linear issue tracking integration
- **Notion** — Notion workspace and database integration
- **GitHub API** — GitHub REST/GraphQL API for webhooks and automation
- **Email / SMTP** — Email sending via SMTP or API

### Vector Database

- **Pinecone** — Managed vector database for RAG and similarity search
- **Chroma** — Open-source embedding database
- **Qdrant** — High-performance vector database

