# API NODE

OpenAI-compatible AI API Gateway for Cursor, Claude Code, Codex, SDKs, and self-built AI apps.

Use one `base_url` to access multiple model APIs, keep app integrations portable, and centralize API keys, quota, usage logs, and provider/model switching behind one gateway layer.

```text
Base URL: https://apinode.pro
API:      OpenAI-compatible Chat Completions / Responses API
Use in:   Cursor, Claude Code, Codex CLI, Python, Node.js, agent workflows
```

## Start here

- Examples for developer tools and SDKs: https://github.com/apinode-pro/openai-compatible-ai-gateway-examples
- Fork-ready starter templates: https://github.com/apinode-pro/apinode-starter-templates
- Reproducible gateway benchmark: https://github.com/apinode-pro/ai-api-gateway-benchmark
- Website and dashboard: https://apinode.pro

## Quick test

```bash
export APINODE_API_KEY="your_api_key"
export APINODE_BASE_URL="https://apinode.pro/v1"
export APINODE_MODEL="gpt-5.5"

curl "$APINODE_BASE_URL/chat/completions" \
  -H "Authorization: Bearer $APINODE_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-5.5",
    "messages": [{"role": "user", "content": "Say hello from API NODE"}]
  }'
```

## Common use cases

- Configure Cursor, Claude Code, Codex CLI, Aider, OpenHands, Flowise, LangChain, or LlamaIndex with one OpenAI-compatible endpoint.
- Keep production apps independent from a single upstream provider.
- Add model/provider switching without changing every client integration.
- Centralize API key management, quota, and usage logs for team workflows.
- Reproduce latency and success-rate checks in GitHub Actions.

## Need trial credits?

Open a "Request trial credits" issue in the examples repo and include what you want to test first:

- Cursor / Claude Code / Codex / self-built app / agent workflow
- Current problem: 429, timeout, provider switching, quota, logs, cost, or setup
- Expected monthly usage range

We prefer concrete developer feedback over generic coupon drops.
