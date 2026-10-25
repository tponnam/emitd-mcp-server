# Claude Code connection

1. Create a restricted Emitd API key in the Emitd console.
2. Add the hosted MCP server:

```bash
claude mcp add --transport http emitd https://mcp.emitd.com/mcp \
  --header "Authorization: Bearer YOUR_EMITD_API_KEY"
```

3. Replace the placeholder locally.
4. Test the tools that are enabled for your API key.

Do not commit a real key or include it in screenshots, logs, or public issues.
