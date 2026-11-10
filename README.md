# Interact Gateway PoC projects

API Studio projects for DataPower Interact Gateway 12.1.1.3 (cluster itz-ref4y2).

| Project | Description |
|---|---|
| plant-ops | REST API (plant-ops-api) converted to an MCP server. Subscription auth, SQL injection filter, PII redaction. |
| plant-knowledge | External MCP server (plant-knowledge-mcp) registered behind the gateway. Upstream API key injected by a Set policy. |

`plant-knowledge/set-upstream-key-ei3mr.yaml` contains a placeholder (`REPLACE_WITH_PLANT_MCP_API_KEY`). Replace it before publishing; do not commit the real key.
| llm-openrouter | LLM proxy over OpenRouter (provider connection `llm-openrouter:openrouter:1.0.0`, secret `openrouter-key` created in Settings). Model allow-list, output-token quota, exact cache. |
