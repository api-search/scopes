---
api_specs:
- filename: drip-accounts-api-openapi.yml
  format: yaml
  label: Drip Accounts API
  slug: drip-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-accounts-api-openapi.yml
- filename: drip-broadcasts-api-openapi.yml
  format: yaml
  label: Drip Broadcasts API
  slug: drip-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-broadcasts-api-openapi.yml
- filename: drip-campaigns-api-openapi.yml
  format: yaml
  label: Drip Campaigns API
  slug: drip-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-campaigns-api-openapi.yml
- filename: drip-conversions-api-openapi.yml
  format: yaml
  label: Drip Conversions API
  slug: drip-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-conversions-api-openapi.yml
- filename: drip-custom-fields-api-openapi.yml
  format: yaml
  label: Drip Custom Fields API
  slug: drip-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-custom-fields-api-openapi.yml
- filename: drip-events-api-openapi.yml
  format: yaml
  label: Drip Events API
  slug: drip-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-events-api-openapi.yml
- filename: drip-forms-api-openapi.yml
  format: yaml
  label: Drip Forms API
  slug: drip-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-forms-api-openapi.yml
- filename: drip-orders-api-openapi.yml
  format: yaml
  label: Drip Orders API
  slug: drip-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-orders-api-openapi.yml
- filename: drip-shopper-activity-api-openapi.yml
  format: yaml
  label: Drip Shopper Activity API
  slug: drip-shopper-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-shopper-activity-api-openapi.yml
- filename: drip-subscribers-api-openapi.yml
  format: yaml
  label: Drip Subscribers API
  slug: drip-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-subscribers-api-openapi.yml
authorization_urls: []
description: 'Drip''s OAuth 2.0 authorization server advertises exactly two scopes. This is a coarse-grained model: `public` is the read-oriented default issued to registered applications, and `write` is the mutating grant. There is no per-resource scope (no separate subscribers/campaigns/workflows scopes), so an agent granted `write` can mutate every resource the account exposes. The API reference does not publish a scopes table of its own; these values come from the machine-readable metadata document, which is the authoritative source. Derived baseline was NOT available from the OpenAPI: the specs in openapi/ declare only HTTP basic and bearer securitySchemes, no oauth2 scheme, so derive-oauth-scopes.py found nothing to derive. Everything here is probed.'
docs: https://developer.drip.com/#oauth
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Drip Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Drip uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Drip
provider_slug: drip
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: drip-scopes
source_filename: drip-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://api.getdrip.com/.well-known/oauth-authorization-server (HTTP 200,\n  RFC 8414 authorization server metadata, probed 2026-08-13), corroborated by\n  the OAuth section of https://developer.drip.com/#oauth which shows a token\n  response carrying \"scope\": \"public\".\ndocs: https://developer.drip.com/#oauth\ndescription: >-\n  Drip's OAuth 2.0 authorization server advertises exactly two scopes. This is\n  a coarse-grained model: `public` is the read-oriented default issued to\n  registered applications, and `write` is the mutating grant. There is no\n  per-resource scope (no separate subscribers/campaigns/workflows scopes), so\n  an agent granted `write` can mutate every resource the account exposes. The\n  API reference does not publish a scopes table of its own; these values come\n  from the machine-readable metadata document, which is the authoritative\n  source.\n  Derived baseline was NOT available from the\
  \ OpenAPI: the specs in openapi/\n  declare only HTTP basic and bearer securitySchemes, no oauth2 scheme, so\n  derive-oauth-scopes.py found nothing to derive. Everything here is probed.\nauthorization_server:\n  issuer: https://api.getdrip.com\n  metadata: well-known/drip-oauth-authorization-server.json\n  authorization_endpoint: https://www.getdrip.com/oauth/authorize\n  token_endpoint: https://www.getdrip.com/oauth/token\n  registration_endpoint: https://api.getdrip.com/oauth/register\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post]\nscopes:\n  - name: public\n    description: >-\n      Default scope returned in the OAuth token response documented at\n      https://developer.drip.com/#oauth. Grants an application access to the\n      authorized Drip account through the REST API.\n    source: /.well-known/oauth-authorization-server\
  \ (scopes_supported)\n  - name: write\n    description: >-\n      Mutating access. Not broken down per resource — a single grant covering\n      every writable endpoint on the account.\n    source: /.well-known/oauth-authorization-server (scopes_supported)\nscope_count: 2\nnotes:\n  - >-\n    Drip's docs state that OAuth access tokens do not expire (\"You should only\n    have to do this once, as tokens do not expire\"), while the metadata\n    advertises refresh_token support. Long-lived non-expiring bearer tokens with\n    only two coarse scopes is the security posture an integrator should plan\n    around.\n  - >-\n    The authorization code from /oauth/authorize expires in 10 minutes per the\n    docs.\n  - >-\n    The same authorization server governs the MCP endpoint at\n    https://api.getdrip.com/mcp — see mcp/drip-mcp.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/scopes/drip-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Email Marketing
- Marketing Automation
- E-Commerce
- Customer Engagement
- Campaigns
- Workflows
token_urls: []
---
