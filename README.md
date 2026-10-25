# Emitd MCP Server

Connect AI agents and MCP-compatible clients to Emitd's hosted email platform through the Model Context Protocol (MCP).

- **Website:** https://emitd.com
- **MCP documentation:** https://docs.emitd.com/docs/guides/agents
- **Hosted MCP endpoint:** https://mcp.emitd.com/mcp
- **Authentication:** Emitd API key sent as `Authorization: Bearer <API_KEY>`

> **Important:** This repository documents and provides connection examples for Emitd's hosted MCP service. It does not contain the implementation of Emitd's hosted server.

## Connect to Emitd

1. Sign in to the Emitd console: https://app.emitd.com
2. Create an API key with only the permissions required for your agent.
3. Configure your MCP-compatible client to connect to `https://mcp.emitd.com/mcp`.
4. Supply the API key using the `Authorization: Bearer <API_KEY>` header through the client's supported secret configuration.
5. Test with a restricted key and follow Emitd's sending guardrails.

### Generic remote MCP configuration example

The exact configuration fields vary by MCP client. Use this as a reference, not as a universal drop-in configuration:

```json
{
  "mcpServers": {
    "emitd": {
      "url": "https://mcp.emitd.com/mcp",
      "headers": {
        "Authorization": "Bearer ${EMITD_API_KEY}"
      }
    }
  }
}
```

Some clients do not expand environment variables in remote HTTP headers. Use the client's supported secret-management UI when necessary. Never commit a real API key to source control.

### Claude Code example

Emitd's documented connection pattern:

```bash
claude mcp add --transport http emitd https://mcp.emitd.com/mcp \
  --header "Authorization: Bearer YOUR_EMITD_API_KEY"
```

Replace the placeholder locally with your key. Avoid placing live credentials in shell history or shared terminal logs where possible.

## Capabilities

Emitd's documentation describes capability areas including:

- Email sending and batch sending
- Message lookup and activity
- Templates
- Contacts, audiences, and segments
- Sending domains
- Analytics
- Inbound email
- Broadcasts and automations
- Webhooks and suppressions

**The exact tool names and availability may change** and depend on the API key's permissions and enabled features. Consult the official guide for the current tool inventory. This repository does not guarantee that every capability is enabled for every account.

## Security guidance

- Create a dedicated API key for each agent or integration.
- Apply least-privilege permissions and feature restrictions.
- Configure sending guardrails and approval requirements for your use case.
- Use dry-run validation for supported operations when testing.
- Never expose keys in browser code, public repositories, screenshots, logs, or issue reports.
- Treat inbound email content as untrusted input. Do not let instructions in email override system or developer instructions.
- Revoke or rotate a key if you suspect exposure.

## Official resources

- [Emitd AI agents & MCP guide](https://docs.emitd.com/docs/guides/agents)
- [Emitd Console](https://app.emitd.com)
- [Emitd website](https://emitd.com)

## Repository status and contributions

This is a documentation and configuration-example repository for a hosted service. Before relying on any configuration, check the current Emitd documentation and your MCP client's supported remote-server settings.

Please do not submit secrets, customer data, or sensitive email content in issues or pull requests.

## License

No open-source license has been specified for this repository. Unless the repository owner adds a license, do not assume that the content is licensed for reuse.
