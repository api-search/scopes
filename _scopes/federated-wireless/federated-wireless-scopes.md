---
authorization_urls:
- https://federatedwireless.ai/oauth/authorize
description: Federated Wireless's only public OAuth surface is the authorization server advertised on federatedwireless.ai for its remote MCP server. It declares a single coarse scope, `mcp`. There is no published scope, permission or role reference anywhere in the public Federated Wireless surface, and no other Federated Wireless host publishes RFC 8414 or OIDC discovery metadata. The company's product APIs (Spectrum Controller external SAS API, IAM API, KPI API) are behind AWS API Gateway authentication with no anonymous discovery document, so they contribute no scope surface.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Federated Wireless Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Federated Wireless publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Federated Wireless API on a user''s behalf.


  Tokens are issued from https://federatedwireless.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Federated Wireless
provider_slug: federated-wireless
schemes:
- flows:
  - authorizationUrl: https://federatedwireless.ai/oauth/authorize
    client_authentication: none (public client)
    code_challenge_methods:
    - S256
    dynamic_client_registration: 'No RFC 7591 registration_endpoint is advertised. The server sets client_id_metadata_document_supported: true, so clients identify themselves with a client-ID metadata document URL rather than pre-registering.'
    flow: authorizationCode
    pkce: required
    refresh_tokens: true
    revocationUrl: https://federatedwireless.ai/oauth/revoke
    tokenUrl: https://federatedwireless.ai/oauth/token
  issuer: https://federatedwireless.ai
  name: FederatedWirelessMCPOAuth
  source: https://federatedwireless.ai/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the Federated Wireless MCP server at https://federatedwireless.ai/wp-json/mcp/mcp-oauth-server. Coarse single-scope model — the authorization server advertises no finer-grained read/write split, and no scope documentation is published.
  flows:
  - authorizationCode
  scope: mcp
slug: federated-wireless-scopes
source_filename: federated-wireless-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://federatedwireless.ai/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Federated Wireless's only public OAuth surface is the authorization server advertised on\n  federatedwireless.ai for its remote MCP server. It declares a single coarse scope, `mcp`. There is\n  no published scope, permission or role reference anywhere in the public Federated Wireless surface,\n  and no other Federated Wireless host publishes RFC 8414 or OIDC discovery metadata. The company's\n  product APIs (Spectrum Controller external SAS API, IAM API, KPI API) are behind AWS API Gateway\n  authentication with no anonymous discovery document, so they contribute no scope surface.\nschemes:\n- name: FederatedWirelessMCPOAuth\n  type: oauth2\n  source: https://federatedwireless.ai/.well-known/oauth-authorization-server\n  issuer: https://federatedwireless.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://federatedwireless.ai/oauth/authorize\n\
  \    tokenUrl: https://federatedwireless.ai/oauth/token\n    revocationUrl: https://federatedwireless.ai/oauth/revoke\n    pkce: required\n    code_challenge_methods: [S256]\n    refresh_tokens: true\n    client_authentication: none (public client)\n    dynamic_client_registration: >-\n      No RFC 7591 registration_endpoint is advertised. The server sets\n      client_id_metadata_document_supported: true, so clients identify themselves with a client-ID\n      metadata document URL rather than pre-registering.\nscopes:\n- scope: mcp\n  description: >-\n    Access the Federated Wireless MCP server at\n    https://federatedwireless.ai/wp-json/mcp/mcp-oauth-server. Coarse single-scope model — the\n    authorization server advertises no finer-grained read/write split, and no scope documentation is\n    published.\n  flows: [authorizationCode]\n  sources: [https://federatedwireless.ai/.well-known/oauth-authorization-server]\n  protected_resource: https://federatedwireless.ai/wp-json/mcp/mcp-oauth-server\n\
  not_applicable:\n- surface: Spectrum Controller external SAS API (spectrum-api.federatedwireless.com/v1)\n  reason: >-\n    AWS API Gateway. Anonymous requests return 403 MissingAuthenticationTokenException with no\n    WWW-Authenticate challenge and no discovery document, so no OAuth scope surface is observable.\n    Federated Wireless publishes no authentication or authorization reference for it.\n- surface: Spectrum IAM API (spectrum-iam.federatedwireless.com/v1)\n  reason: Same — 403 MissingAuthenticationTokenException, no anonymous discovery.\n- surface: SAS-CBSD interface (sas.federatedwireless.com)\n  reason: >-\n    The WInnForum SAS-CBSD protocol (WINNF-TS-0016) authenticates CBSDs with mutual TLS client\n    certificates, not OAuth. The host refuses TCP 443 from the public internet.\n- surface: 6 GHz AFC device interface (afc.federatedwireless.com)\n  reason: >-\n    The WInnForum AFC System to AFC Device interface authenticates certified devices/proxies, not\n    OAuth. The\
  \ host refuses TCP 443 from the public internet.\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - url: https://federatedwireless.ai/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://federatedwireless.ai/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://federatedwireless.ai/.well-known/openid-configuration\n    status: 404\n  - url: https://spectrum-api.federatedwireless.com/v1\n    status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federated-wireless/refs/heads/main/scopes/federated-wireless-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Spectrum
- CBRS
- Wireless
- Telecommunications
- Private 5G
- Shared Spectrum
- Spectrum Access System
- 6 GHz
- Network Planning
- RF Engineering
- Government
token_urls:
- https://federatedwireless.ai/oauth/token
---
