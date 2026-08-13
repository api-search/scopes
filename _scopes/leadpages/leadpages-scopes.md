---
authorization_urls:
- https://leadpages.com/api/mcp/oauth/authorize
description: ''
docs: https://leadpages.com/developers/docs
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Leadpages Scopes
name_suffix: OAuth Scopes
note: Scopes are read from the provider's own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata, both served anonymously from leadpages.com. This is a machine-readable first-party source, not a derivation from an OpenAPI — Leadpages publishes no OpenAPI of its own (see conventions/leadpages-conventions.yml). Descriptions for the three agent scopes are quoted verbatim from the A2A agent card; the remaining eight scopes are published as bare identifiers with no provider-supplied description, and none has been invented here.
overview: 'Leadpages publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Leadpages API on a user''s behalf.


  Tokens are issued from https://leadpages.com/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Leadpages
provider_slug: leadpages
schemes:
- flows:
  - authorizationUrl: https://leadpages.com/api/mcp/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://leadpages.com/api/mcp/oauth/register
    tokenUrl: https://leadpages.com/api/mcp/oauth/token
    token_endpoint_auth_methods:
    - client_secret_post
  issuer: https://leadpages.com
  name: oauth2
  source: https://leadpages.com/.well-known/oauth-authorization-server
scope_count: 11
scope_names:
- pages:read
- pages:write
- sites:read
- sites:write
- blogs:read
- blogs:write
- funnels:read
- agents:chat
- agents:approve
- ads:read
- ads:write
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: pages:read
- description: ''
  flows:
  - authorizationCode
  scope: pages:write
- description: ''
  flows:
  - authorizationCode
  scope: sites:read
- description: ''
  flows:
  - authorizationCode
  scope: sites:write
- description: ''
  flows:
  - authorizationCode
  scope: blogs:read
- description: ''
  flows:
  - authorizationCode
  scope: blogs:write
- description: Read funnels, metrics, and agent proposals
  flows:
  - authorizationCode
  scope: funnels:read
- description: Converse with the agent team (spends org AI credits)
  flows:
  - authorizationCode
  scope: agents:chat
- description: Approve/dismiss agent proposals (mutates live ad accounts)
  flows:
  - authorizationCode
  scope: agents:approve
- description: ''
  flows:
  - authorizationCode
  scope: ads:read
- description: ''
  flows:
  - authorizationCode
  scope: ads:write
slug: leadpages-scopes
source_filename: leadpages-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://leadpages.com/.well-known/oauth-authorization-server\ndocs: https://leadpages.com/developers/docs\nnote: >-\n  Scopes are read from the provider's own RFC 8414 authorization-server metadata\n  and RFC 9728 protected-resource metadata, both served anonymously from\n  leadpages.com. This is a machine-readable first-party source, not a derivation\n  from an OpenAPI — Leadpages publishes no OpenAPI of its own (see\n  conventions/leadpages-conventions.yml). Descriptions for the three agent scopes\n  are quoted verbatim from the A2A agent card; the remaining eight scopes are\n  published as bare identifiers with no provider-supplied description, and none\n  has been invented here.\nschemes:\n- name: oauth2\n  source: https://leadpages.com/.well-known/oauth-authorization-server\n  issuer: https://leadpages.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://leadpages.com/api/mcp/oauth/authorize\n    tokenUrl:\
  \ https://leadpages.com/api/mcp/oauth/token\n    registrationUrl: https://leadpages.com/api/mcp/oauth/register\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post]\nprotected_resource:\n  resource: https://leadpages.com/mcp\n  authorization_servers: [https://leadpages.com]\n  bearer_methods_supported: [header]\nscopes:\n- scope: pages:read\n  description: null\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource]\n- scope: pages:write\n  description: null\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource]\n- scope: sites:read\n  description: null\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource]\n- scope: sites:write\n  description: null\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource]\n- scope: blogs:read\n  description:\
  \ null\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource]\n- scope: blogs:write\n  description: null\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource]\n- scope: funnels:read\n  description: Read funnels, metrics, and agent proposals\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource, agent-card]\n- scope: agents:chat\n  description: Converse with the agent team (spends org AI credits)\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource, agent-card]\n- scope: agents:approve\n  description: Approve/dismiss agent proposals (mutates live ad accounts)\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource, agent-card]\n- scope: ads:read\n  description: null\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource]\n- scope: ads:write\n\
  \  description: null\n  flows: [authorizationCode]\n  sources: [oauth-authorization-server, oauth-protected-resource]\nsummary:\n  scope_count: 11\n  pattern: \"<resource>:<read|write> plus three agent-specific scopes\"\n  resources: [pages, sites, blogs, funnels, ads, agents]\n  consent_note: >-\n    agents:approve is the only scope the provider explicitly flags as mutating\n    external state — the agent card says it \"mutates live ad accounts\" and requires\n    an explicit confirmation round-trip.\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - {url: 'https://leadpages.com/.well-known/oauth-authorization-server', status: 200}\n  - {url: 'https://leadpages.com/.well-known/oauth-protected-resource', status: 200}\n  - {url: 'https://leadpages.com/.well-known/agent-card.json', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadpages/refs/heads/main/scopes/leadpages-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Company
- Landing Pages
- Marketing
- Conversion Optimization
- A/B Testing
- Website Builder
- Lead Generation
- Content Management
- Agents
- Analytics
token_urls:
- https://leadpages.com/api/mcp/oauth/token
---
