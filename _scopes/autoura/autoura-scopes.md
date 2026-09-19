---
authorization_urls:
- https://api.autoura.com/api/auth/oauth2/authorize
description: ''
docs: https://api.autoura.com/api/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Autoura Scopes
name_suffix: OAuth Scopes
note: 'Derived from the provider''s live discovery documents, not from an OpenAPI -- Autoura publishes none. The three documents disagree slightly and that disagreement is recorded rather than smoothed over: the RFC 8414 authorization-server document advertises two scopes, the OIDC document and the RFC 9728 protected-resource document both advertise three. Autoura publishes no prose scope reference page, so the descriptions below are the scope names'' plain meaning and are marked as such.'
overview: 'Autoura publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Autoura API on a user''s behalf.


  Tokens are issued from https://api.autoura.com/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Autoura
provider_slug: autoura
schemes:
- flows:
  - authorizationUrl: https://api.autoura.com/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.autoura.com/api/auth/oauth2/token
  issuer: https://api.autoura.com/api/auth
  name: mcpOAuth2
  source: well-known/autoura-oauth-authorization-server.json
scope_count: 3
scope_names:
- files:read
- files:write
- offline_access
scopes:
- description: Read access to the MCP resource. No provider prose definition is published.
  flows:
  - authorizationCode
  scope: files:read
- description: Write access to the MCP resource. No provider prose definition is published.
  flows:
  - authorizationCode
  scope: files:write
- description: Refresh-token issuance, paired with the refresh_token grant type.
  flows:
  - authorizationCode
  scope: offline_access
slug: autoura-scopes
source_filename: autoura-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://api.autoura.com/api/auth/.well-known/openid-configuration\ndocs: https://api.autoura.com/api/.well-known/oauth-protected-resource\nnote: >-\n  Derived from the provider's live discovery documents, not from an OpenAPI --\n  Autoura publishes none. The three documents disagree slightly and that disagreement\n  is recorded rather than smoothed over: the RFC 8414 authorization-server document\n  advertises two scopes, the OIDC document and the RFC 9728 protected-resource\n  document both advertise three. Autoura publishes no prose scope reference page, so\n  the descriptions below are the scope names' plain meaning and are marked as such.\nschemes:\n  - name: mcpOAuth2\n    source: well-known/autoura-oauth-authorization-server.json\n    issuer: https://api.autoura.com/api/auth\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.autoura.com/api/auth/oauth2/authorize\n        tokenUrl: https://api.autoura.com/api/auth/oauth2/token\n\
  \        pkce: S256\nscopes:\n  - scope: files:read\n    description: Read access to the MCP resource. No provider prose definition is published.\n    description_source: scope name only -- Autoura publishes no scopes reference page\n    flows: [authorizationCode]\n    sources:\n      - well-known/autoura-oauth-authorization-server.json\n      - well-known/autoura-openid-configuration.json\n      - well-known/autoura-oauth-protected-resource.json\n    advertised_in_challenge: true\n    note: >-\n      This is the scope named in the WWW-Authenticate challenge returned by an\n      unauthenticated POST to https://api.autoura.com/api/mcp.\n  - scope: files:write\n    description: Write access to the MCP resource. No provider prose definition is published.\n    description_source: scope name only\n    flows: [authorizationCode]\n    sources:\n      - well-known/autoura-oauth-authorization-server.json\n      - well-known/autoura-openid-configuration.json\n      - well-known/autoura-oauth-protected-resource.json\n\
  \  - scope: offline_access\n    description: Refresh-token issuance, paired with the refresh_token grant type.\n    description_source: OIDC core semantics\n    flows: [authorizationCode]\n    sources:\n      - well-known/autoura-openid-configuration.json\n      - well-known/autoura-oauth-protected-resource.json\n    absent_from:\n      - well-known/autoura-oauth-authorization-server.json\n    note: >-\n      Present in the OIDC and protected-resource documents but NOT in the RFC 8414\n      authorization-server document, which also omits refresh_token from\n      grant_types_supported. A client that reads only the RFC 8414 document will not\n      know refresh tokens are available.\nfindings:\n  - id: scope-vocabulary-mismatch\n    severity: low\n    detail: >-\n      The scope names are files:read / files:write, which describe a file resource.\n      Nothing the MCP server actually exposes -- visit plans, preferences, venue\n      knowledge, locations -- is a file. The names look like\
  \ a framework default that\n      was never renamed for the domain, and they give an agent no way to request\n      least privilege over the surface it is really touching.\n  - id: discovery-document-drift\n    severity: low\n    detail: >-\n      Three discovery documents are served from three path roots and two of them\n      disagree on scopes_supported and grant_types_supported.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoura/refs/heads/main/scopes/autoura-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Tourism
- Tours
- Travel
- Destination
- Experience
- Digital Tourism
token_urls:
- https://api.autoura.com/api/auth/oauth2/token
---
