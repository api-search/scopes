---
authorization_urls:
- https://www.fibe.in/api/mcp/oauth/authorize
description: ''
docs: https://www.fibe.in/mcp/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Fibe Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fibe publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fibe API on a user''s behalf.


  Tokens are issued from https://www.fibe.in/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fibe
provider_slug: fibe
schemes:
- flows:
  - authorizationUrl: https://www.fibe.in/api/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.fibe.in/api/mcp/oauth/token
  name: OAuth2
  source: https://www.fibe.in/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- loan.read
- loan.apply
scopes:
- description: Read access to a customer's loan and eligibility information.
  flows:
  - authorizationCode
  scope: loan.read
- description: Submit or initiate a loan application on the customer's behalf.
  flows:
  - authorizationCode
  scope: loan.apply
slug: fibe-scopes
source_filename: fibe-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.fibe.in/.well-known/oauth-authorization-server\ndocs: https://www.fibe.in/mcp/\nschemes:\n- name: OAuth2\n  source: https://www.fibe.in/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fibe.in/api/mcp/oauth/authorize\n    tokenUrl: https://www.fibe.in/api/mcp/oauth/token\nscopes:\n- scope: loan.read\n  description: Read access to a customer's loan and eligibility information.\n  flows: [authorizationCode]\n  sources: [https://www.fibe.in/.well-known/oauth-authorization-server]\n- scope: loan.apply\n  description: Submit or initiate a loan application on the customer's behalf.\n  flows: [authorizationCode]\n  sources: [https://www.fibe.in/.well-known/oauth-authorization-server]\nnotes: >-\n  Scopes are advertised verbatim in Fibe's RFC 8414 authorization-server metadata and\n  RFC 9728 protected-resource metadata for the MCP server. Descriptions are\
  \ curated\n  from the scope names; Fibe's /mcp/ documentation page was not reachable at probe time.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fibe/refs/heads/main/scopes/fibe-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Fintech
- Lending
- Personal Loans
- Consumer Finance
- India
- Credit
- MCP
- Agent
token_urls:
- https://www.fibe.in/api/mcp/oauth/token
---
