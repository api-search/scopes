---
api_specs:
- filename: tigera-apis-api-openapi.yml
  format: yaml
  label: Tigera APIS API
  slug: tigera-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-apis-api-openapi.yml
- filename: tigera-projectcalicoorg-api-openapi.yml
  format: yaml
  label: Tigera Projectcalico Org API
  slug: tigera-projectcalicoorg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-projectcalicoorg-api-openapi.yml
- filename: tigera-projectcalicoorg-v3-api-openapi.yml
  format: yaml
  label: Tigera Projectcalico Org V3 API
  slug: tigera-projectcalicoorg-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-projectcalicoorg-v3-api-openapi.yml
- filename: tigera-version-api-openapi.yml
  format: yaml
  label: Tigera Version API
  slug: tigera-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-version-api-openapi.yml
authorization_urls:
- https://www.tigera.io/oauth/authorize
description: Tigera's only public OAuth surface is the authorization server advertised on www.tigera.io for its remote MCP server. It declares a single coarse scope, `mcp`. There is no published scope or permission reference in the Tigera documentation, and no other Tigera or Calico Cloud host publishes RFC 8414 or OIDC discovery metadata. The Calico API itself has no OAuth surface — it is a Kubernetes aggregated API server and delegates authentication and authorization to the cluster's own authenticators and RBAC.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Tigera Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tigera publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tigera API on a user''s behalf.


  Tokens are issued from https://www.tigera.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tigera
provider_slug: tigera
schemes:
- flows:
  - authorizationUrl: https://www.tigera.io/oauth/authorize
    client_authentication: none (public client)
    code_challenge_methods:
    - S256
    dynamic_client_registration: 'No RFC 7591 registration_endpoint. The server advertises client_id_metadata_document_supported: true, so clients identify themselves with a client-ID metadata document URL rather than pre-registering.'
    flow: authorizationCode
    pkce: required
    refresh_tokens: true
    revocationUrl: https://www.tigera.io/oauth/revoke
    tokenUrl: https://www.tigera.io/oauth/token
  issuer: https://www.tigera.io
  name: TigeraMCPOAuth
  source: https://www.tigera.io/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the Tigera MCP server at https://www.tigera.io/wp-json/mcp/mcp-oauth-server. Coarse, single-scope model — the authorization server advertises no finer-grained read/write split.
  flows:
  - authorizationCode
  scope: mcp
slug: tigera-scopes
source_filename: tigera-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://www.tigera.io/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Tigera's only public OAuth surface is the authorization server advertised on www.tigera.io for\n  its remote MCP server. It declares a single coarse scope, `mcp`. There is no published scope\n  or permission reference in the Tigera documentation, and no other Tigera or Calico Cloud host\n  publishes RFC 8414 or OIDC discovery metadata. The Calico API itself has no OAuth surface — it\n  is a Kubernetes aggregated API server and delegates authentication and authorization to the\n  cluster's own authenticators and RBAC.\nschemes:\n- name: TigeraMCPOAuth\n  type: oauth2\n  source: https://www.tigera.io/.well-known/oauth-authorization-server\n  issuer: https://www.tigera.io\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.tigera.io/oauth/authorize\n    tokenUrl: https://www.tigera.io/oauth/token\n    revocationUrl:\
  \ https://www.tigera.io/oauth/revoke\n    pkce: required\n    code_challenge_methods: [S256]\n    refresh_tokens: true\n    client_authentication: none (public client)\n    dynamic_client_registration: >-\n      No RFC 7591 registration_endpoint. The server advertises\n      client_id_metadata_document_supported: true, so clients identify themselves with a\n      client-ID metadata document URL rather than pre-registering.\nscopes:\n- scope: mcp\n  description: >-\n    Access the Tigera MCP server at https://www.tigera.io/wp-json/mcp/mcp-oauth-server. Coarse,\n    single-scope model — the authorization server advertises no finer-grained read/write split.\n  flows: [authorizationCode]\n  sources: [https://www.tigera.io/.well-known/oauth-authorization-server]\n  protected_resource: https://www.tigera.io/wp-json/mcp/mcp-oauth-server\nnot_applicable:\n- surface: Calico API (projectcalico.org/v3)\n  reason: >-\n    The published Swagger 2.0 definition declares no securityDefinitions. Authentication\
  \ and\n    authorization are the host cluster's — bearer tokens, client certificates or kubeconfig\n    credentials, authorized by Kubernetes RBAC on projectcalico.org resources plus Calico's own\n    tier-scoped policy RBAC. There is no OAuth scope surface to record.\n- surface: Calico Cloud Usage API\n  reason: Organization-scoped read-only API keys, not OAuth. No scopes are published.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://www.tigera.io/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://www.tigera.io/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://www.tigera.io/.well-known/openid-configuration\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/scopes/tigera-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Kubernetes
- Networking
- Network Security
- Container Security
- Cloud-Native
- Observability
- Microsegmentation
- Zero Trust
- eBPF
- Open-Source
token_urls:
- https://www.tigera.io/oauth/token
---
