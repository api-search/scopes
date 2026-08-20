---
authorization_urls:
- https://app.agentio.com/connector/consent
description: ''
docs: https://www.agentio.com/connector
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Agentio Scopes
name_suffix: OAuth Scopes
note: 'Agentio publishes no scope reference page. The single scope below is the only scope advertised by either discovery document — both the RFC 9728 protected-resource metadata and the RFC 8414 authorization-server metadata list scopes_supported = ["brand-connector:read"]. The connector documentation corroborates it: "Every connection is read-only and scoped to one brand."'
overview: 'Agentio publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agentio API on a user''s behalf.


  Tokens are issued from https://api.agentio.com/o/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agentio
provider_slug: agentio
schemes:
- flows:
  - authorizationUrl: https://app.agentio.com/connector/consent
    flow: authorizationCode
    tokenUrl: https://api.agentio.com/o/token
  issuer: https://api.agentio.com/o
  name: AgentioBrandConnectorOAuth
  source: well-known/agentio-oauth-authorization-server.json
scope_count: 1
scope_names:
- brand-connector:read
scopes:
- description: Read-only access to a single brand's Agentio data through the hosted MCP connector — campaigns, creator deals and deliverables, YouTube ad performance, and conversion reporting. Cannot write, cannot act on the user's behalf, and cannot reach another brand's data.
  flows:
  - authorizationCode
  scope: brand-connector:read
slug: agentio-scopes
source_filename: agentio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://mcp.agentio.com/.well-known/oauth-protected-resource/mcp\ndocs: https://www.agentio.com/connector\nnote: >-\n  Agentio publishes no scope reference page. The single scope below is the only scope advertised\n  by either discovery document — both the RFC 9728 protected-resource metadata and the RFC 8414\n  authorization-server metadata list scopes_supported = [\"brand-connector:read\"]. The connector\n  documentation corroborates it: \"Every connection is read-only and scoped to one brand.\"\nschemes:\n- name: AgentioBrandConnectorOAuth\n  source: well-known/agentio-oauth-authorization-server.json\n  issuer: https://api.agentio.com/o\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.agentio.com/connector/consent\n    tokenUrl: https://api.agentio.com/o/token\nscopes:\n- scope: brand-connector:read\n  description: >-\n    Read-only access to a single brand's Agentio data through the hosted MCP connector\
  \ —\n    campaigns, creator deals and deliverables, YouTube ad performance, and conversion\n    reporting. Cannot write, cannot act on the user's behalf, and cannot reach another\n    brand's data.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/agentio-oauth-protected-resource.json\n  - well-known/agentio-oauth-authorization-server.json\nscope_count: 1\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - url: https://mcp.agentio.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n  - url: https://api.agentio.com/.well-known/oauth-authorization-server/o\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentio/refs/heads/main/scopes/agentio-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- AdTech
- Advertising
- Creator Economy
- Influencer Marketing
- Marketing
- Artificial Intelligence
- YouTube
- MCP
- Agents
- Analytics
token_urls:
- https://api.agentio.com/o/token
---
