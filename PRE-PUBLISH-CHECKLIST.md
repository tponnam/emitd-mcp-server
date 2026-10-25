# Pre-publication checklist

## Confirmed from Emitd's public documentation
- [x] Hosted MCP endpoint: https://mcp.emitd.com/mcp
- [x] Authentication pattern: Authorization: Bearer <Emitd API key>
- [x] Tool availability depends on key permissions and enabled features
- [x] Official guide: https://docs.emitd.com/docs/guides/agents

## Must verify before directory submission
- [ ] Create this repository under the correct Emitd-owned GitHub organization/account.
- [ ] Publish the repository with public visibility.
- [ ] Verify publisher namespace ownership for `com.emitd/emitd` using the official registry's current process.
- [ ] Validate `.mcp/server.json` against the current official registry schema and publisher checks.
- [ ] Confirm the endpoint's current transport compatibility with the registry and target directory.
- [ ] Test a connection using a restricted test API key.
- [ ] Check the exact live tool inventory with a test client.
- [ ] Add an official support contact if required.
- [ ] Decide whether to add a license. Do not imply open-source licensing without one.
- [ ] Recheck each store's current form, policy, and price.
- [ ] Never commit a live API key.

## Validation status

The JSON file is syntactically valid and the required endpoint/authentication fields are present. This is a structural check only, not live validation against the official registry and not proof that the service has been published.
