---
type: service
id: svc-lm-studio
title: "LM Studio"
description: "Desktop app for local model inference with GUI"
tags: [Production, Template]
connections: []
metadata:
  template_category: "Local LLM"
---

## Provider
LM Studio (local)

## Endpoint
http://localhost:1234/v1

## Authentication
None (local only)

## API Compatibility
OpenAI-compatible — use any OpenAI SDK by changing the base URL

## Models
- Download from Hugging Face via built-in browser
- Supports GGUF format models
- Popular: Llama 3, Mistral, Phi, CodeLlama

## Notes
- GUI for model management and chat
- Local API server for programmatic access
- Supports Apple Silicon and NVIDIA GPUs
- Available on macOS, Windows, Linux
