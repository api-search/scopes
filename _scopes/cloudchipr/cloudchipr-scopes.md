---
api_specs:
- filename: cloudchipr-enterprise-api-openapi.yml
  format: yaml
  label: CloudChipr API
  slug: cloudchipr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/openapi/cloudchipr-enterprise-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cloudchipr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CloudChipr uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CloudChipr
provider_slug: cloudchipr
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cloudchipr-scopes
source_filename: cloudchipr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://mcp.cloudchipr.com/.well-known/oauth-protected-resource +\n  https://auth0.cloudchipr.com/.well-known/openid-configuration\nsummary: >-\n  CloudChipr's OAuth surface is the MCP server only; the REST API is apiKey-authenticated and has\n  no oauth2 securityScheme, so derive-oauth-scopes.py correctly found nothing in the spec. The\n  scopes recorded here were read from the two live discovery documents, not from the contract.\n  They are IDENTITY scopes, not API-permission scopes: the MCP protected-resource document\n  advertises exactly openid, profile, email and offline_access. There is no read/write or\n  per-resource scope vocabulary anywhere.\n\nsurfaces:\n  - name: CloudChipr MCP Server\n    endpoint: https://mcp.cloudchipr.com/mcp\n    auth: oauth2\n    resource: https://mcp.cloudchipr.com/mcp\n    audience: https://api-bff.cloudchipr.com\n    authorization_server: https://auth0.cloudchipr.com\n    issuer: https://auth0.cloudchipr.com/\n\
  \    bearer_methods_supported: [header]\n  - name: CloudChipr Enterprise API\n    base_url: https://api.cloudchipr.com\n    auth: apiKey\n    scopes: none\n    note: >-\n      Single `ApiKey` securityScheme (x-api-key header) applied per-operation. No oauth2 flow, no\n      scope vocabulary. Authorization is coarse: the docs state API keys grant \"read-only access to\n      the Cloudchipr API and your cloud resources\" - though the spec declares three mutating\n      operations under that same scheme, which is an unresolved contradiction (see notes).\n\nscopes:\n  - name: openid\n    source: mcp-protected-resource\n    type: identity\n    description: OIDC - request an ID token identifying the CloudChipr user.\n    required: true\n  - name: profile\n    source: mcp-protected-resource\n    type: identity\n    description: OIDC - basic profile claims (name, nickname, picture, updated_at).\n  - name: email\n    source: mcp-protected-resource\n    type: identity\n    description: OIDC - email\
  \ and email_verified claims.\n  - name: offline_access\n    source: mcp-protected-resource\n    type: identity\n    description: Issue a refresh token so the MCP client can hold a long-lived session.\n\nauthorization_server_scopes_supported:\n  source: https://auth0.cloudchipr.com/.well-known/openid-configuration\n  note: >-\n    The Auth0 tenant advertises the full standard OIDC claim-scope set below. This is Auth0's\n    default advertisement for the tenant, NOT a CloudChipr-defined permission model - only the four\n    scopes in `scopes:` above are the ones the MCP resource actually declares.\n  values: [openid, profile, offline_access, name, given_name, family_name, nickname, email, email_verified, picture, created_at, identities, phone, address]\n\nauthorization_model:\n  style: role-based, server-side\n  scope_granularity: none\n  notes: >-\n    Neither surface exposes a per-resource or per-action scope. What an OAuth-authenticated MCP\n    session may see is decided by the user's\
  \ CloudChipr role and organization membership\n    (\"scoped to their permissions\" - https://cloudchipr.com/mcp), not by a scope granted at consent\n    time. An agent therefore cannot request a reduced permission set: it gets whatever its human's\n    account can see.\n  agent_risk: >-\n    There is no way to grant an agent read access to Billing Explorer while withholding Live\n    Resources, and no way to down-scope a token below the user's own role.\n\nunresolved:\n  - issue: 'API keys are documented as read-only, but the spec declares three mutating operations under the same ApiKey scheme.'\n    detail: >-\n      https://docs.cloudchipr.com/docs/api-keys states \"API keys provide read-only access to the\n      Cloudchipr API and your cloud resources\", while\n      openapi/cloudchipr-enterprise-api-openapi.yml declares POST /data-sources (201 create),\n      PUT /dimensions/category-structure (204) and POST /ingest/{destinationId} - all secured by\n      `ApiKey: []`. Either the\
  \ docs statement predates the custom-data write surface or those\n      operations require an entitlement the contract does not name. Recorded, not resolved.\n    checked: '2026-09-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudchipr/refs/heads/main/scopes/cloudchipr-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Azure
- Cloud Cost Management
- Cost Optimization
- FinOps
- GCP
- Multi-Cloud
- Resource Cleanup
- Rightsizing
token_urls: []
---
