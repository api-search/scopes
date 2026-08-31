---
api_specs:
- filename: canoe-intelligence-allocations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Allocations API
  slug: canoe-intelligence-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-allocations-api-openapi.yml
- filename: canoe-intelligence-authentication-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Authentication API
  slug: canoe-intelligence-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-authentication-api-openapi.yml
- filename: canoe-intelligence-custom-fields-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Custom Fields API
  slug: canoe-intelligence-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-custom-fields-api-openapi.yml
- filename: canoe-intelligence-documents-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Documents API
  slug: canoe-intelligence-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-documents-api-openapi.yml
- filename: canoe-intelligence-funds-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Funds API
  slug: canoe-intelligence-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-funds-api-openapi.yml
- filename: canoe-intelligence-organizations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Organizations API
  slug: canoe-intelligence-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-organizations-api-openapi.yml
- filename: canoe-intelligence-password-grant-tokens-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Password Grant Tokens API
  slug: canoe-intelligence-password-grant-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-password-grant-tokens-api-openapi.yml
- filename: canoe-intelligence-terms-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Terms API
  slug: canoe-intelligence-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-terms-api-openapi.yml
- filename: canoe-intelligence-user-api-openapi.yml
  format: yaml
  label: Canoe Intelligence User API
  slug: canoe-intelligence-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-user-api-openapi.yml
- filename: canoe-intelligence-introduction-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Introduction API
  slug: canoe-intelligence-introduction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-introduction-api-openapi.yml
authorization_urls:
- https://api.canoesoftware.com/oauth/authorize
description: ''
docs: https://api.canoesoftware.com/docs
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Canoe Intelligence Scopes
name_suffix: OAuth Scopes
note: Canoe declares OAuth 2.0 authorizationCode and clientCredentials flows but publishes NO scopes — both flows carry an empty scopes map, no operation declares a scoped security requirement, and the documentation contains no scopes or permissions reference. An access token grants "access to all other endpoints within the API"; what a caller can actually reach is decided by the Canoe services their tenant purchased and by per-user permissions, and is signalled at call time with HTTP 403. This is an accurate zero, not a harvest miss.
overview: 'Canoe Intelligence uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.canoesoftware.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Canoe Intelligence
provider_slug: canoe-intelligence
schemes:
- description: OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://api.canoesoftware.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.canoesoftware.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.canoesoftware.com/v1/tokens
  name: oauth2
  source: openapi/canoe-intelligence-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: canoe-intelligence-scopes
source_filename: canoe-intelligence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource:\n- openapi/canoe-intelligence-api-openapi.yml\n- https://api.canoesoftware.com/docs\nschemes:\n- name: oauth2\n  source: openapi/canoe-intelligence-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.canoesoftware.com/oauth/authorize\n    tokenUrl: https://api.canoesoftware.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.canoesoftware.com/v1/tokens\n  description: OAuth 2.0 authentication\nscopes: []\ndocs: https://api.canoesoftware.com/docs\nnote: Canoe declares OAuth 2.0 authorizationCode and clientCredentials flows but publishes NO scopes — both flows\n  carry an empty scopes map, no operation declares a scoped security requirement, and the documentation contains\n  no scopes or permissions reference. An access token grants \"access to all other endpoints within the API\"; what\n  a caller can actually reach is decided by the Canoe services their tenant purchased\
  \ and by per-user permissions,\n  and is signalled at call time with HTTP 403. This is an accurate zero, not a harvest miss.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/scopes/canoe-intelligence-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Alternative Investments
- Private Markets
- Document Automation
- Data Extraction
- Fund Administration
- capital-calls
- k-1-tax-documents
- Portfolio Reporting
- Financial-Services
- Fintech
- Wealth Management
- Institutional Investors
token_urls:
- https://api.canoesoftware.com/oauth/token
- https://api.canoesoftware.com/v1/tokens
---
