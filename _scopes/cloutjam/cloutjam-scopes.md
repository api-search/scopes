---
authorization_urls: []
description: ''
docs: https://www.cloutdesk.com/agent-platform
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cloutjam Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CloutJam publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CloutJam API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CloutJam
provider_slug: cloutjam
schemes:
- flows:
  - flow: authorizationCode
  name: oauth2
  source: https://www.cloutdesk.com/agent-platform
scope_count: 3
scope_names:
- campaigns
- collaborations
- agreements:write
scopes:
- description: Access to campaigns
  flows:
  - authorizationCode
  scope: campaigns
- description: Access to collaborations
  flows:
  - authorizationCode
  scope: collaborations
- description: Write access to agreements
  flows:
  - authorizationCode
  scope: agreements:write
slug: cloutjam-scopes
source_filename: cloutjam-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.cloutdesk.com/agent-platform\nstatus: beta\nnotes: >-\n  OAuth scopes documented on CloutDesk's Agent Platform page (Beta). No scope\n  reference / permissions page is published yet; this is the scope set shown in\n  the page's MCP OAuth-login example (`npx @cloutdesk/mcp oauth login`).\n  Enumerated scopes below are those the vendor explicitly names; the full scope\n  catalog is not yet published.\ndocs: https://www.cloutdesk.com/agent-platform\nschemes:\n  - name: oauth2\n    source: https://www.cloutdesk.com/agent-platform\n    flows:\n      - flow: authorizationCode\nscopes:\n  - scope: campaigns\n    description: Access to campaigns\n    flows: [authorizationCode]\n    sources: [https://www.cloutdesk.com/agent-platform]\n  - scope: collaborations\n    description: Access to collaborations\n    flows: [authorizationCode]\n    sources: [https://www.cloutdesk.com/agent-platform]\n  - scope: 'agreements:write'\n\
  \    description: Write access to agreements\n    flows: [authorizationCode]\n    sources: [https://www.cloutdesk.com/agent-platform]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloutjam/refs/heads/main/scopes/cloutjam-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Influencer Marketing
- Creator Management
- Creator Economy
- Marketing
- Agentic AI
- Agents
token_urls: []
---
