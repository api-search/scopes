---
api_specs:
- filename: impact-brand-account-v14-openapi.yml
  format: yaml
  label: Impact Brand API
  slug: brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-brand-account-v14-openapi.yml
- filename: impact-partner-account-v16-openapi.yml
  format: yaml
  label: Impact Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-partner-account-v16-openapi.yml
- filename: impact-agency-advertisers-v3-openapi.yml
  format: yaml
  label: Impact Agency API
  slug: agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-agency-advertisers-v3-openapi.yml
- filename: impact-brand-advocate-account-v13-openapi.yml
  format: yaml
  label: Impact Advocate API
  slug: advocate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/openapi/impact-brand-advocate-account-v13-openapi.yml
authorization_urls: []
description: The OAuth 2.1 scopes impact.com publishes for its MCP server, and the scoped-token model that governs REST API access.
docs:
  mcp: https://integrations.impact.com/ai-solutions/mcp-quick-start
  migrate_to_scoped_tokens: https://help.impact.com/other/reference-documentation/api-access-tokens-and-changelog/migrate-to-scoped-tokens
  scoped_token_best_practices: https://help.impact.com/other/reference-documentation/api-access-tokens-and-changelog/scoped-tokens-best-practices
  scoped_tokens: https://integrations.impact.com/rest-apis/api-quick-start/create-an-api-key
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Impact Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Impact uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Impact
provider_slug: impact
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: impact-scopes
source_filename: impact-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Impact OAuth Scopes and Token Scoping\ndescription: The OAuth 2.1 scopes impact.com publishes for its MCP server, and the scoped-token\n  model that governs REST API access.\ngenerated: '2026-08-13'\nmethod: probed\nsource: https://app.impact.com/.well-known/oauth-protected-resource\ndocs:\n  mcp: https://integrations.impact.com/ai-solutions/mcp-quick-start\n  scoped_tokens: https://integrations.impact.com/rest-apis/api-quick-start/create-an-api-key\n  scoped_token_best_practices: https://help.impact.com/other/reference-documentation/api-access-tokens-and-changelog/scoped-tokens-best-practices\n  migrate_to_scoped_tokens: https://help.impact.com/other/reference-documentation/api-access-tokens-and-changelog/migrate-to-scoped-tokens\noauth:\n  issuer: https://app.impact.com\n  protected_resource: https://mcp.impact.com/mcp\n  metadata_url: https://app.impact.com/.well-known/oauth-protected-resource\n  http_status: 200\n  probed: '2026-08-13'\n  bearer_methods_supported:\
  \ [header]\n  scopes:\n    - name: mcp:read\n      description: Read access through the MCP server, further constrained by the consenting\n        user's own platform permissions.\n    - name: mcp:write\n      description: Write access through the MCP server (creating campaigns, updating settings,\n        managing partners, creating tracking links), further constrained by the consenting\n        user's own platform permissions.\n    - name: openid\n      description: Advertised by the OpenID Connect discovery document as the only supported\n        OIDC scope.\n      source: https://app.impact.com/.well-known/openid-configuration\nrest_token_scoping:\n  model: scoped access tokens\n  since: April 2025\n  granularity: API category toggle plus per-endpoint selection\n  enforcement_status: 403\n  enumerable: false\n  note: The REST scope vocabulary is not published as a machine-readable list. Scopes are\n    chosen from category and endpoint toggles inside the impact.com UI when a token\
  \ is minted,\n    so the full scope set can only be enumerated from an authenticated account. No OpenAPI\n    document declares an oauth2 securityScheme with a scopes map.\n  categories_observed_from_published_endpoint_groups:\n    - Accounts\n    - Actions\n    - Action Inquiries\n    - Ads\n    - Call Data\n    - Catalogs\n    - Clicks\n    - Contacts\n    - Contracts\n    - Conversions\n    - Deals\n    - Exception Lists\n    - Invoices\n    - Jobs\n    - Notes\n    - Partners\n    - Partner Groups\n    - Programs\n    - Promo Codes\n    - Promo Code Exception Lists\n    - Reports\n    - Routing Rules\n    - Submissions\n    - Tasks\n    - Tracking Links\n    - Tracking Value Requests\n  categories_note: Derived from the tag/endpoint groups in the 69 published OpenAPI documents,\n    not from a published scope registry. Treat as the shape of the scope surface, not as\n    literal scope strings.\nfindings:\n  - Only the MCP surface has a published, machine-readable scope vocabulary,\
  \ and it is exactly\n    two scopes - mcp:read and mcp:write - covering every one of the fifteen documented tools.\n  - The REST surface has genuinely fine-grained scoping but publishes no scope registry, so an\n    integrator cannot request or document least-privilege access without logging in.\nprovider_action: Publish the scoped-token category and endpoint vocabulary as data, and declare\n  it as an oauth2 or apiKey securityScheme with a scopes map in the OpenAPI documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impact/refs/heads/main/scopes/impact-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Affiliate
- Partnerships
- Performance Marketing
- Commission
- Tracking
- Creator Economy
- Partner Management
- Referral
- Attribution
- Payouts
- Marketing
- Advertising
- MCP
- Agents
token_urls: []
---
