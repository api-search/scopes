---
api_specs:
- filename: tradeshift-external-api-openapi.yml
  format: yaml
  label: Tradeshift External API
  slug: tradeshift-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/openapi/tradeshift-external-api-openapi.yml
- filename: tradeshift-mcp-bridge-openapi.yml
  format: yaml
  label: Tradeshift MCP Server
  slug: tradeshift-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/openapi/tradeshift-mcp-bridge-openapi.yml
authorization_urls:
- https://go.tradeshift.com/oauth2/authorize
description: ''
docs: https://developers.tradeshift.com/docs/guides/oauth
flows:
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Tradeshift Scopes
name_suffix: OAuth Scopes
note: The Tradeshift External API OpenAPI declares no securitySchemes, so no scopes can be derived from it — the derive-oauth-scopes.py pass found zero oauth2 schemes. The scopes below are the ones Tradeshift actually publishes, anonymously, on the MCP server's RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata. They correspond one-to-one with the six MCP capability domains. Descriptions are the Tradeshift-published domain labels, not invented scope prose.
overview: 'Tradeshift publishes 7 OAuth 2.0 scopes via the clientCredentials and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tradeshift API on a user''s behalf.


  Tokens are issued from https://mcp.tradeshift.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tradeshift
provider_slug: tradeshift
schemes:
- bearer_methods_supported:
  - header
  flows:
  - flow: clientCredentials
    response_types_supported:
    - token
    tokenUrl: https://mcp.tradeshift.com/oauth/token
    token_endpoint_auth_methods_supported:
    - client_secret_post
  issuer: https://mcp.tradeshift.com
  name: TradeshiftMCPOAuth2
  resource: https://mcp.tradeshift.com/mcp
  source: https://mcp.tradeshift.com/.well-known/oauth-authorization-server
  type: oauth2
- flows:
  - authorizationUrl: https://go.tradeshift.com/oauth2/authorize
    flow: implicit
    response_types_supported:
    - token
    tokenUrl: https://api.tradeshift.com/tradeshift/auth/token
  issuer: https://api.tradeshift.com/tradeshift/
  jwks_uri: https://api.tradeshift.com/tradeshift/auth/jwks
  name: TradeshiftPlatformOAuth2
  note: The platform authorization-server metadata advertises no scopes_supported. App permissions on the Tradeshift platform are configured per app in the Developer App (the "Permissions" field on app registration) rather than declared as OAuth scope strings in a public document.
  scopes_published: false
  source: https://api.tradeshift.com/tradeshift/.well-known/oauth-authorization-server
  type: oauth2
  userinfo_endpoint: https://api.tradeshift.com/tradeshift/auth/userinfo
scope_count: 7
scope_names:
- core
- network
- documents
- company
- bfr
- askada
- all
scopes:
- description: Core services domain of the Tradeshift MCP server.
  flows:
  - clientCredentials
  scope: core
- description: Supplier network domain — connections, connection properties, network requests.
  flows:
  - clientCredentials
  scope: network
- description: Documents domain — business documents, search, validation.
  flows:
  - clientCredentials
  scope: documents
- description: Company data domain — accounts, branches, legal entities, tax identifiers.
  flows:
  - clientCredentials
  scope: company
- description: Business Firewall domain.
  flows:
  - clientCredentials
  scope: bfr
- description: AskAda AI assistant / Ada AI document intelligence domain.
  flows:
  - clientCredentials
  scope: askada
- description: All MCP capability domains.
  flows:
  - clientCredentials
  scope: all
slug: tradeshift-scopes
source_filename: tradeshift-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://mcp.tradeshift.com/.well-known/oauth-protected-resource\ndocs: https://developers.tradeshift.com/docs/guides/oauth\nnote: >-\n  The Tradeshift External API OpenAPI declares no securitySchemes, so no scopes can be derived from it — the\n  derive-oauth-scopes.py pass found zero oauth2 schemes. The scopes below are the ones Tradeshift actually publishes,\n  anonymously, on the MCP server's RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata.\n  They correspond one-to-one with the six MCP capability domains. Descriptions are the Tradeshift-published domain\n  labels, not invented scope prose.\nschemes:\n  - name: TradeshiftMCPOAuth2\n    type: oauth2\n    source: https://mcp.tradeshift.com/.well-known/oauth-authorization-server\n    issuer: https://mcp.tradeshift.com\n    resource: https://mcp.tradeshift.com/mcp\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://mcp.tradeshift.com/oauth/token\n\
  \        token_endpoint_auth_methods_supported:\n          - client_secret_post\n        response_types_supported:\n          - token\n    bearer_methods_supported:\n      - header\n  - name: TradeshiftPlatformOAuth2\n    type: oauth2\n    source: https://api.tradeshift.com/tradeshift/.well-known/oauth-authorization-server\n    issuer: https://api.tradeshift.com/tradeshift/\n    flows:\n      - flow: implicit\n        authorizationUrl: https://go.tradeshift.com/oauth2/authorize\n        tokenUrl: https://api.tradeshift.com/tradeshift/auth/token\n        response_types_supported:\n          - token\n    jwks_uri: https://api.tradeshift.com/tradeshift/auth/jwks\n    userinfo_endpoint: https://api.tradeshift.com/tradeshift/auth/userinfo\n    scopes_published: false\n    note: >-\n      The platform authorization-server metadata advertises no scopes_supported. App permissions on the Tradeshift\n      platform are configured per app in the Developer App (the \"Permissions\" field on app registration)\
  \ rather than\n      declared as OAuth scope strings in a public document.\nscopes:\n  - scope: core\n    description: Core services domain of the Tradeshift MCP server.\n    flows: [clientCredentials]\n    sources: [https://mcp.tradeshift.com/.well-known/oauth-protected-resource]\n  - scope: network\n    description: Supplier network domain — connections, connection properties, network requests.\n    flows: [clientCredentials]\n    sources: [https://mcp.tradeshift.com/.well-known/oauth-protected-resource]\n  - scope: documents\n    description: Documents domain — business documents, search, validation.\n    flows: [clientCredentials]\n    sources: [https://mcp.tradeshift.com/.well-known/oauth-protected-resource]\n  - scope: company\n    description: Company data domain — accounts, branches, legal entities, tax identifiers.\n    flows: [clientCredentials]\n    sources: [https://mcp.tradeshift.com/.well-known/oauth-protected-resource]\n  - scope: bfr\n    description: Business Firewall\
  \ domain.\n    flows: [clientCredentials]\n    sources: [https://mcp.tradeshift.com/.well-known/oauth-protected-resource]\n  - scope: askada\n    description: AskAda AI assistant / Ada AI document intelligence domain.\n    flows: [clientCredentials]\n    sources: [https://mcp.tradeshift.com/.well-known/oauth-protected-resource]\n  - scope: all\n    description: All MCP capability domains.\n    flows: [clientCredentials]\n    sources: [https://mcp.tradeshift.com/.well-known/oauth-protected-resource]\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://mcp.tradeshift.com/.well-known/oauth-protected-resource\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradeshift/refs/heads/main/scopes/tradeshift-scopes.yml
summary_line: 7 scopes · clientCredentials/implicit
tags:
- e-invoicing
- accounts-payable
- ap-automation
- procure-to-pay
- supply-chain
- b2b-commerce
- invoicing
- ubl
- peppol
- e-invoicing-compliance
- supplier-network
- business-documents
- fintech
- mcp
- agent-native
token_urls:
- https://mcp.tradeshift.com/oauth/token
- https://api.tradeshift.com/tradeshift/auth/token
---
