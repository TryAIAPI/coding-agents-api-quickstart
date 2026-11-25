# Coding Agents & Multi-Model API Quickstart (Claude Code / Codex CLI / SDKs)

Minimal configuration snippets and connectivity verification script for pointing **Claude Code**, **Codex CLI**, **OpenAI SDK**, and **Anthropic SDK** at a unified OpenAI/Anthropic-compatible gateway (defaults to [Try AI API](https://tryaiapi.com/en/docs/coding-agents/)).

## 1. One-line AI Agent setup

Paste this into Claude Code, Codex CLI, or Antigravity:

```text
Follow https://tryaiapi.com/SKILL.md to set up Try AI API
```

## 2. Claude Code (Anthropic native protocol — no `/v1` suffix)

```bash
export ANTHROPIC_BASE_URL="https://tryaiapi.com"
export ANTHROPIC_API_KEY="your-api-key"
```

## 3. Codex CLI & OpenAI SDK (include `/v1` suffix)

```bash
export OPENAI_BASE_URL="https://tryaiapi.com/v1"
export OPENAI_API_KEY="your-api-key"
```

## 4. Verify live models & auth (free, zero token cost)

```bash
curl -sS https://tryaiapi.com/v1/models \
  -H "Authorization: Bearer $OPENAI_API_KEY" | head -c 500
```

## References
- Coding Agents Setup Guide: https://tryaiapi.com/en/docs/coding-agents/
- Image Generation Guide (GPT Image & Gemini Image): https://tryaiapi.com/en/docs/image-model/
- Live Model Catalog & Pricing: https://tryaiapi.com/en/models/

## License

MIT
