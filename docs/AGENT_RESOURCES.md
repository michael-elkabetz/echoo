# Echoo public catalog resources

Use the [API and setup guide](https://www.echoo.ai/docs), [CLI reference](https://www.echoo.ai/docs/cli), and [MCP reference](https://www.echoo.ai/docs/mcp).

The live service is published in the [official MCP Registry](https://registry.modelcontextprotocol.io/v0.1/servers/ai.echoo.www%2Fpublic-catalog/versions/1.0.0) under `ai.echoo.www/public-catalog`, verified through HTTP proof on `www.echoo.ai`. [server.json](../server.json) contains the published remote-server metadata. The MCP protocol's ServerInfo name remains `ai.echoo/public-catalog`; registry ownership uses the exact verified www namespace.

The root plugin.json and mcp.json follow Agent Plugins 1.0.0; compatible clients discover the skill in skills/echoo-catalog. The MCP service is remote, public and read-only. No install hook or local executable is bundled. Other clients can install the standalone skill and configure the remote MCP URL separately.
