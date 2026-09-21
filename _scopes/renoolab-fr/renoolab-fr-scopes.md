---
authorization_urls:
- https://mcp.renoolab.fr/authorize
description: ''
docs: https://renoolab.fr/mcp/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Renoolab Fr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RenooLab uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://mcp.renoolab.fr/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RenooLab
provider_slug: renoolab-fr
schemes:
- account_required: false
  bearer_methods:
  - header
  flows:
  - authorizationUrl: https://mcp.renoolab.fr/authorize
    client_id_metadata_document_supported: false
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256 (required per docs)
    refreshUrl: https://mcp.renoolab.fr/token
    registrationUrl: https://mcp.renoolab.fr/register
    response_modes:
    - query
    response_types:
    - code
    revocationUrl: https://mcp.renoolab.fr/token
    scopes: {}
    tokenUrl: https://mcp.renoolab.fr/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - none
  issuer: https://mcp.renoolab.fr
  name: RenooLabOAuth
  protected_resource: https://mcp.renoolab.fr
  source: well-known/renoolab-fr-oauth-authorization-server.json
  token_lifetimes:
    access_token: 1 hour
    consent_session: 10 minutes
    dynamic_client: 90 days
    refresh_token: 30 days
    revocation_browser_id: 12 months
    source: https://renoolab.fr/privacy/ §5
  type: oauth2
scope_count: 0
scope_names: []
scopes: []
slug: renoolab-fr-scopes
source_filename: renoolab-fr-scopes.yml
source_heading: OAuth Scopes
source_url: https://mcp.renoolab.fr/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://mcp.renoolab.fr/.well-known/oauth-authorization-server\ndocs: https://renoolab.fr/mcp/\nsources:\n- https://mcp.renoolab.fr/.well-known/oauth-authorization-server\n- https://mcp.renoolab.fr/.well-known/oauth-protected-resource\n- https://mcp.renoolab.fr/mcp (tools/list _meta.securitySchemes)\n- https://renoolab.fr/mcp/\n- https://renoolab.fr/privacy/ (§5 token lifetimes)\nsummary: >-\n  RenooLab runs its own OAuth 2.1 authorization server at https://mcp.renoolab.fr (RFC 8414 metadata served)\n  to protect the two write tools of its MCP server. It defines NO named scopes: the AS metadata carries no\n  scopes_supported, and both OAuth-gated tools declare {type: oauth2, scopes: []} in _meta.securitySchemes.\n  Consent is all-or-nothing at the tool-set level - the docs say the user \"accepte l'accès aux quatre outils\"\n  - and no RenooLab account is needed to grant it. The two search tools are noauth and never enter the\
  \ OAuth\n  flow. There is no OpenAPI to derive from; derive-oauth-scopes.py found no oauth2 schemes for this slug.\nschemes:\n- name: RenooLabOAuth\n  type: oauth2\n  issuer: https://mcp.renoolab.fr\n  source: well-known/renoolab-fr-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.renoolab.fr/authorize\n    tokenUrl: https://mcp.renoolab.fr/token\n    refreshUrl: https://mcp.renoolab.fr/token\n    revocationUrl: https://mcp.renoolab.fr/token\n    registrationUrl: https://mcp.renoolab.fr/register\n    pkce: S256 (required per docs)\n    response_types: [code]\n    response_modes: [query]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    client_id_metadata_document_supported: false\n    scopes: {}\n  protected_resource: https://mcp.renoolab.fr\n  bearer_methods: [header]\n  account_required: false\n  token_lifetimes:\n    access_token: 1 hour\n\
  \    refresh_token: 30 days\n    dynamic_client: 90 days\n    consent_session: 10 minutes\n    revocation_browser_id: 12 months\n    source: https://renoolab.fr/privacy/ §5\nscopes: []\nscope_count: 0\ntool_requirements:\n- {tool: rechercher_artisans, security: noauth}\n- {tool: rechercher_chantier, security: noauth}\n- {tool: contacter_artisan, security: 'oauth2, scopes: []'}\n- {tool: creer_profil_artisan, security: 'oauth2, scopes: []'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renoolab-fr/refs/heads/main/scopes/renoolab-fr-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Home Services
- Construction
- Building Trades
- Renovation
- Marketplace
- Local Services
- MCP
- A2A
- AI Agents
- Agent Skills
- France
token_urls:
- https://mcp.renoolab.fr/token
---
