---
authorization_urls:
- https://app.allstacks.com/oauth/authorize/
description: ''
docs: https://app.allstacks.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Allstacks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allstacks publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allstacks API on a user''s behalf.


  Tokens are issued from https://app.allstacks.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allstacks
provider_slug: allstacks
schemes:
- flows:
  - authorizationUrl: https://app.allstacks.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://app.allstacks.com/oauth/token/
  name: OAuth2
  source: well-known/allstacks-oauth-authorization-server.json
scope_count: 1
scope_names:
- connector
scopes:
- description: 'Access granted to a registered connector/agent integration against the Allstacks platform. This is the only scope advertised in the authorization server and protected-resource metadata (scopes_supported: ["connector"]).'
  flows:
  - authorizationCode
  scope: connector
slug: allstacks-scopes
source_filename: allstacks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://app.allstacks.com/.well-known/oauth-authorization-server\ndocs: https://app.allstacks.com/.well-known/oauth-protected-resource\nschemes:\n- name: OAuth2\n  source: well-known/allstacks-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.allstacks.com/oauth/authorize/\n    tokenUrl: https://app.allstacks.com/oauth/token/\nscopes:\n- scope: connector\n  description: >-\n    Access granted to a registered connector/agent integration against the\n    Allstacks platform. This is the only scope advertised in the authorization\n    server and protected-resource metadata (scopes_supported: [\"connector\"]).\n  flows: [authorizationCode]\n  sources: [well-known/allstacks-oauth-authorization-server.json]\nnotes: >-\n  Scopes captured verbatim from Allstacks' live OAuth discovery metadata. The\n  platform publishes exactly one OAuth scope (\"connector\"); no broader scope /\n\
  \  permission reference is published publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allstacks/refs/heads/main/scopes/allstacks-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Software Engineering Intelligence
- Value Stream Management
- Developer Productivity
- DevOps
- Analytics
- AI Agents
token_urls:
- https://app.allstacks.com/oauth/token/
---
