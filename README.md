# Expose for ChatGPT

Plugin package for the [ChatGPT and Codex plugin directory](https://platform.openai.com/plugins). It connects to the hosted Expose MCP server at `https://expose.team/mcp`. Sign-in is OAuth. ChatGPT registers its own client. The scope is `expose`.

Each search uses one credit on the connected Expose account.

## Upload

Upload `chatgpt-plugin.zip` at [platform.openai.com/plugins](https://platform.openai.com/plugins). The zip root is `plugin.json`, `mcp.json`, and `assets/`.

Rebuild it from this directory after a listing change:

```bash
zip -r chatgpt-plugin.zip plugin.json mcp.json assets -x '*.DS_Store'
```
