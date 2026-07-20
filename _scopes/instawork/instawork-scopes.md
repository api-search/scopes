---
authorization_urls:
- https://finch.instawork.com/mcp/partner/authorize
description: ''
docs: https://github.com/instawork/skills/blob/main/skills/find-workers/setup.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Instawork Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Instawork publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Instawork API on a user''s behalf.


  Tokens are issued from https://finch.instawork.com/mcp/partner/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Instawork
provider_slug: instawork
schemes:
- flows:
  - authorizationUrl: https://finch.instawork.com/mcp/partner/authorize
    flow: authorizationCode
    tokenUrl: https://finch.instawork.com/mcp/partner/token
  name: OAuth2
  source: well-known/instawork-oauth-authorization-server.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to partner staffing data — company locations, positions, position templates, pricing, break rules, payment options, onsite contacts, booking templates, shift groups, and rostered pros.
  flows:
  - authorizationCode
  scope: read
- description: Create draft and confirmed shift bookings on behalf of the partner.
  flows:
  - authorizationCode
  scope: write
slug: instawork-scopes
source_filename: instawork-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://finch.instawork.com/.well-known/oauth-authorization-server/mcp/partner\ndocs: https://github.com/instawork/skills/blob/main/skills/find-workers/setup.md\nschemes:\n  - name: OAuth2\n    source: well-known/instawork-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://finch.instawork.com/mcp/partner/authorize\n        tokenUrl: https://finch.instawork.com/mcp/partner/token\nscopes:\n  - scope: read\n    description: Read access to partner staffing data — company locations, positions, position templates, pricing, break rules, payment options, onsite contacts, booking templates, shift groups, and rostered pros.\n    flows: [authorizationCode]\n    sources: [well-known/instawork-oauth-authorization-server.json]\n  - scope: write\n    description: Create draft and confirmed shift bookings on behalf of the partner.\n    flows: [authorizationCode]\n    sources: [well-known/instawork-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instawork/refs/heads/main/scopes/instawork-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Marketplace
- Staffing
- Gig Economy
- Hospitality
- Workforce
- Labor
- MCP
- Agent
token_urls:
- https://finch.instawork.com/mcp/partner/token
---
