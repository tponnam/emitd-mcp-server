# Emitd MCP Store & Directory Submission Pack

This document contains canonical listing copy, direct submission links, and exact form inputs for submitting the Emitd MCP Server to all major Model Context Protocol registries and directories.

---

## Canonical Metadata

- **Server Identifier / Namespace:** `com.emitd/emitd`
- **Display Name / Title:** `Emitd MCP Server`
- **Short Description (under 100 chars):**  
  `Connect AI agents to Emitd email sending, message tracking, templates, and automations.`
- **Canonical Long Description:**  
  `Emitd hosts a Model Context Protocol server for integrating supported email operations into AI-agent workflows. Connect a compatible client to the hosted endpoint (https://mcp.emitd.com/mcp) and authenticate with an Emitd API key. Available tools depend on the key's permissions and enabled features. Emitd's capability areas include sending email, message activity, templates, contacts, audiences, segments, domains, analytics, inbound email, broadcasts, automations, webhooks, and suppressions. Use restricted keys, sending guardrails, and approval settings appropriate to each workflow.`
- **Remote Endpoint URL:** `https://mcp.emitd.com/mcp`
- **Transport Type:** `Streamable HTTP`
- **Authentication:** `HTTP Authorization header with Bearer token` (`Authorization: Bearer <API_KEY>`)
- **Public GitHub Repository:** `https://github.com/tponnam/emitd-mcp-server`
- **Official Website:** `https://emitd.com`
- **Official Documentation:** `https://docs.emitd.com/docs/guides/agents`
- **Support Contact:** `hello@emitd.com`
- **License:** `MIT`

---

## 1. Official MCP Registry (registry.modelcontextprotocol.io)

- **Status:** **PUBLISHED & ACTIVE**
- **Registered Name:** `com.emitd/emitd`
- **Version:** `1.0.1`
- **Discovery Endpoint:** `https://registry.modelcontextprotocol.io/v0.1/servers?search=com.emitd/emitd`

---

## 2. Smithery.ai

- **Submission URL:** [smithery.ai/new](https://smithery.ai/new)
- **Repository URL:** `https://github.com/tponnam/emitd-mcp-server`
- **Remote Server URL:** `https://mcp.emitd.com/mcp`
- **Configuration:** The repository already contains a valid `smithery.yaml` configuring `startCommand: { type: "http" }` with the `apiKey` schema.
- **Action:** Sign in to Smithery via GitHub, enter the repository URL, and confirm submission.

---

## 3. Glama.ai

- **Submission URL:** [glama.ai/mcp/connectors](https://glama.ai/mcp/connectors) / [glama.ai/mcp/servers](https://glama.ai/mcp/servers)
- **Connector Type:** Remote MCP Server
- **Server Name:** `Emitd MCP Server`
- **Namespace:** `com.emitd`
- **Endpoint:** `https://mcp.emitd.com/mcp`
- **GitHub Repository:** `https://github.com/tponnam/emitd-mcp-server`
- **Auth Scheme:** Bearer Token (API Key)
- **Action:** Authenticate with GitHub, submit repository URL or remote connector endpoint. Glama automatically runs sandbox and license checks.

---

## 4. MCP Market (mcpmarket.com)

- **Submission URL:** [mcpmarket.com/submit](https://mcpmarket.com/submit)
- **Submission Source:** `GitHub repo`
- **GitHub URL:** `https://github.com/tponnam/emitd-mcp-server`
- **Listing Choice:** Free Queue ($0) or Get Listed Now ($29 for 24h + Official badge)
- **Try Now URL:** `https://emitd.com/?utm_source=mcpmarket&utm_medium=directory&utm_campaign=mcp_launch`
- **Email:** Your admin account email

---

## 5. MCP.so

- **Submission URL:** [mcp.so/submit](https://mcp.so/submit)
- **Repository URL:** `https://github.com/tponnam/emitd-mcp-server`
- **Name:** `Emitd MCP Server`
- **Category:** `Communication` / `Email`
- **Website URL:** `https://emitd.com`
- **Documentation URL:** `https://docs.emitd.com/docs/guides/agents`
- **Action:** Paste GitHub URL. Details are auto-scraped from `README.md` and `server.json`.

---

## 6. PulseMCP (pulsemcp.com)

- **Website:** [pulsemcp.com](https://www.pulsemcp.com)
- **Action:** PulseMCP automatically indexes public repositories with `.mcp/server.json` and official registry packages (`com.emitd/emitd`). Verify listing search once re-crawl completes.

---

## 7. Curated GitHub Lists (Awesome MCP Servers)

### A. Awesome Remote MCP Servers (`punkpeye/awesome-remote-mcp-servers`)
Add under `### 💬 Communication`:
```markdown
- [Emitd](https://emitd.com) `https://mcp.emitd.com/mcp`
  [![Emitd MCP connector](https://glama.ai/mcp/connectors/com.emitd/emitd/badges/score.svg)](https://glama.ai/mcp/connectors/com.emitd/emitd)
  🔑 - Transactional email, message activity, templates, contacts, automations, and inbound mail for AI agents.
```
*(Requires listing on Glama first to generate the connector badge).*

### B. Awesome MCP Servers (`punkpeye/awesome-mcp-servers`)
Add under `### 💬 Communication`:
```markdown
- [tponnam/emitd-mcp-server](https://github.com/tponnam/emitd-mcp-server) 🎖️ ☁️ - Transactional and broadcast email for AI agents: sending, message activity, templates, contacts, automations, and inbound mail with security guardrails.
```
