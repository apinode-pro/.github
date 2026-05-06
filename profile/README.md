# API NODE

OpenAI-compatible AI API gateway for developers using Claude, GPT, Gemini, Cursor, Codex CLI, and Claude Code.

Use one endpoint to test models, connect developer tools, and keep AI integrations portable.

```text
Base URL: https://apinode.pro
API:      OpenAI Responses API
Model:    gpt-5.5
```

## Repositories

- [OpenAI-Compatible AI Gateway Examples](https://github.com/apinode-pro/openai-compatible-ai-gateway-examples)
- [AI API Gateway Benchmark](https://github.com/apinode-pro/ai-api-gateway-benchmark)

## Quick Test

```bash
export APINODE_API_KEY="your_api_key"
export APINODE_BASE_URL="https://apinode.pro"
export APINODE_MODEL="gpt-5.5"

curl "$APINODE_BASE_URL/responses" \
  -H "Authorization: Bearer $APINODE_API_KEY" \
  -H "Content-Type: application/json" \
  -d "{\"model\":\"$APINODE_MODEL\",\"input\":\"Say hello from API NODE\"}"
```

[Try API NODE](https://apinode.pro)

