# Pre-publication checklist

## Confirmed from Emitd's public documentation
- [x] Hosted MCP endpoint: https://mcp.emitd.com/mcp
- [x] Authentication pattern: Authorization: Bearer <Emitd API key>
- [x] Tool availability depends on key permissions and enabled features
- [x] Official guide: https://docs.emitd.com/docs/guides/agents

## Must verify before directory submission
- [x] Create this repository under the correct Emitd-owned GitHub organization/account. (https://github.com/tponnam/emitd-mcp-server)
- [x] Publish the repository with public visibility. (Confirmed public)
- [x] Verify publisher namespace ownership for `com.emitd/emitd` using the official registry's current process (verified via HTTP domain proof on https://emitd.com/.well-known/mcp-registry-auth).
- [x] Validate `.mcp/server.json` against the current official registry schema (description <= 100 characters and icons configured).
- [x] Confirm the endpoint's current transport compatibility with the registry and target directory (streamable-http).
- [x] Test a connection using a valid test API key (live initialization, 72 tools, and 4 resources verified).
- [x] Check the exact live tool inventory with a test client (72 tools discovered and verified).
- [x] Add an official support contact if required (hello@emitd.com).
- [ ] Decide whether to add a license. Do not imply open-source licensing without one.
- [x] Recheck each store's current form, policy, and price (MCP Market, Glama, Smithery, MCP.so).
- [x] Never commit a live API key.

## Validation status

- **Schema:** Strictly validated against `https://static.modelcontextprotocol.io/schemas/2025-12-11/server.schema.json`.
- **Live Endpoint:** `https://mcp.emitd.com/mcp` tested with authentic Emitd Bearer auth.
- **Registry Publication:** Published to the official MCP Registry (`registry.modelcontextprotocol.io`) under namespace `com.emitd/emitd@1.0.1` (`status: active`).
