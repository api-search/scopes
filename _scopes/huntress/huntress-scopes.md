---
api_specs:
- filename: huntress-accounts-api-openapi.yml
  format: yaml
  label: Huntress Accounts API
  slug: huntress-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-accounts-api-openapi.yml
- filename: huntress-actor-api-openapi.yml
  format: yaml
  label: Huntress Actor API
  slug: huntress-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-actor-api-openapi.yml
- filename: huntress-agents-api-openapi.yml
  format: yaml
  label: Huntress Agents API
  slug: huntress-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-agents-api-openapi.yml
- filename: huntress-escalations-api-openapi.yml
  format: yaml
  label: Huntress Escalations API
  slug: huntress-escalations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-escalations-api-openapi.yml
- filename: huntress-external-recon-api-openapi.yml
  format: yaml
  label: Huntress External Recon API
  slug: huntress-external-recon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-external-recon-api-openapi.yml
- filename: huntress-identities-api-openapi.yml
  format: yaml
  label: Huntress Identities API
  slug: huntress-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-identities-api-openapi.yml
- filename: huntress-incident-reports-api-openapi.yml
  format: yaml
  label: Huntress Incident Reports API
  slug: huntress-incident-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-incident-reports-api-openapi.yml
- filename: huntress-invoices-api-openapi.yml
  format: yaml
  label: Huntress Invoices API
  slug: huntress-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-invoices-api-openapi.yml
- filename: huntress-known-vpns-api-openapi.yml
  format: yaml
  label: Huntress Known VPNs API
  slug: huntress-known-vpns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-known-vpns-api-openapi.yml
- filename: huntress-organizations-api-openapi.yml
  format: yaml
  label: Huntress Organizations API
  slug: huntress-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-organizations-api-openapi.yml
- filename: huntress-platform-actions-api-openapi.yml
  format: yaml
  label: Huntress Platform Actions API
  slug: huntress-platform-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-platform-actions-api-openapi.yml
- filename: huntress-reseller-api-openapi.yml
  format: yaml
  label: Huntress Reseller API
  slug: huntress-reseller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-reseller-api-openapi.yml
- filename: huntress-siem-api-openapi.yml
  format: yaml
  label: Huntress SIEM API
  slug: huntress-siem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-siem-api-openapi.yml
- filename: huntress-signals-api-openapi.yml
  format: yaml
  label: Huntress Signals API
  slug: huntress-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-signals-api-openapi.yml
- filename: huntress-summary-reports-api-openapi.yml
  format: yaml
  label: Huntress Summary Reports API
  slug: huntress-summary-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-summary-reports-api-openapi.yml
- filename: huntress-unwanted-access-rules-api-openapi.yml
  format: yaml
  label: Huntress Unwanted Access Rules API
  slug: huntress-unwanted-access-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-unwanted-access-rules-api-openapi.yml
- filename: huntress-users-api-openapi.yml
  format: yaml
  label: Huntress Users API
  slug: huntress-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-users-api-openapi.yml
authorization_urls:
- https://api.huntress.io/v1/mcp/authorize
description: ''
docs: https://api.huntress.io/.well-known/oauth-protected-resource
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Huntress Scopes
name_suffix: OAuth Scopes
note: The Huntress REST API uses HTTP Basic auth (no OAuth scopes). OAuth 2.1 applies only to the remote MCP server, whose authorization-server metadata advertises a single coarse-grained scope.
overview: 'Huntress publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Huntress API on a user''s behalf.


  Tokens are issued from https://api.huntress.io/v1/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Huntress
provider_slug: huntress
schemes:
- flows:
  - authorizationUrl: https://api.huntress.io/v1/mcp/authorize
    flow: authorizationCode
    tokenUrl: https://api.huntress.io/v1/mcp/token
  - flow: clientCredentials
    tokenUrl: https://api.huntress.io/v1/mcp/token
  name: MCP OAuth
  source: https://api.huntress.io/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Grants an OAuth client access to the Huntress remote MCP server.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp
slug: huntress-scopes
source_filename: huntress-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.huntress.io/.well-known/oauth-authorization-server\ndocs: https://api.huntress.io/.well-known/oauth-protected-resource\nnote: >-\n  The Huntress REST API uses HTTP Basic auth (no OAuth scopes). OAuth 2.1 applies\n  only to the remote MCP server, whose authorization-server metadata advertises a\n  single coarse-grained scope.\nschemes:\n  - name: MCP OAuth\n    source: https://api.huntress.io/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.huntress.io/v1/mcp/authorize\n        tokenUrl: https://api.huntress.io/v1/mcp/token\n      - flow: clientCredentials\n        tokenUrl: https://api.huntress.io/v1/mcp/token\nscopes:\n  - scope: mcp\n    description: Grants an OAuth client access to the Huntress remote MCP server.\n    flows: [authorizationCode, clientCredentials]\n    sources: [https://api.huntress.io/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/scopes/huntress-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Endpoint Security
- SOC
- SIEM
- Identity Threat Detection
- MSP
- Webhooks
token_urls:
- https://api.huntress.io/v1/mcp/token
---
