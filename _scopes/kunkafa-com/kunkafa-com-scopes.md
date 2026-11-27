---
api_specs:
- filename: kunkafa-com-account-links-api-openapi.yml
  format: yaml
  label: Kunkafa Account Links API
  slug: kunkafa-com-account-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-account-links-api-openapi.yml
- filename: kunkafa-com-articles-json-api-openapi.yml
  format: yaml
  label: Kunkafa Articles.json API
  slug: kunkafa-com-articles-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-articles-json-api-openapi.yml
- filename: kunkafa-com-authenticated-integrations-api-openapi.yml
  format: yaml
  label: Kunkafa Authenticated integrations API
  slug: kunkafa-com-authenticated-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-authenticated-integrations-api-openapi.yml
- filename: kunkafa-com-glossary-api-openapi.yml
  format: yaml
  label: Kunkafa Glossary API
  slug: kunkafa-com-glossary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-glossary-api-openapi.yml
- filename: kunkafa-com-markets-json-api-openapi.yml
  format: yaml
  label: Kunkafa Markets.json API
  slug: kunkafa-com-markets-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-markets-json-api-openapi.yml
- filename: kunkafa-com-plans-api-openapi.yml
  format: yaml
  label: Kunkafa Plans API
  slug: kunkafa-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-plans-api-openapi.yml
- filename: kunkafa-com-plans-json-api-openapi.yml
  format: yaml
  label: Kunkafa Plans.json API
  slug: kunkafa-com-plans-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-plans-json-api-openapi.yml
- filename: kunkafa-com-reports-api-openapi.yml
  format: yaml
  label: Kunkafa Reports API
  slug: kunkafa-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-reports-api-openapi.yml
- filename: kunkafa-com-sitemap-markets-xml-api-openapi.yml
  format: yaml
  label: Kunkafa Sitemap Markets.xml API
  slug: kunkafa-com-sitemap-markets-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-sitemap-markets-xml-api-openapi.yml
- filename: kunkafa-com-stats-json-api-openapi.yml
  format: yaml
  label: Kunkafa Stats.json API
  slug: kunkafa-com-stats-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-stats-json-api-openapi.yml
- filename: kunkafa-com-well-known-api-openapi.yml
  format: yaml
  label: Kunkafa .well Known API
  slug: kunkafa-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-well-known-api-openapi.yml
- filename: kunkafa-com-widgets-api-openapi.yml
  format: yaml
  label: Kunkafa Widgets API
  slug: kunkafa-com-widgets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-widgets-api-openapi.yml
authorization_urls:
- https://kunkafa.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Kunkafa Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kunkafa publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kunkafa API on a user''s behalf.


  Tokens are issued from https://kunkafa.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kunkafa
provider_slug: kunkafa-com
schemes:
- description: 'Authorization code with required PKCE. Issuer https://kunkafa.com/oauth. Request resource https://kunkafa.com/mcp for MCP or https://kunkafa.com/api/v1 for Pro or Publisher REST. Access tokens expire after 10 minutes; refresh tokens rotate and reuse revokes the grant. An MCP connection stays connected while used: it expires after 90 days without use and at most one year after approval. The same app approving again replaces its connection; asking only for access already allowed needs no second approval. Validate issuer/resource/audience; never give an agent app sign-in credentials.'
  flows:
  - authorizationUrl: https://kunkafa.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://kunkafa.com/oauth/token
  name: KunkafaOAuth
  source: openapi/kunkafa-com-openapi.json
scope_count: 6
scope_names:
- following:write
- markets:read
- outlooks:read
- performance:read
- results:read
- usage:read
scopes:
- description: Follow and unfollow markets
  flows:
  - authorizationCode
  scope: following:write
- description: List authorized markets
  flows:
  - authorizationCode
  scope: markets:read
- description: Read controlled current summaries
  flows:
  - authorizationCode
  scope: outlooks:read
- description: Read published performance
  flows:
  - authorizationCode
  scope: performance:read
- description: Read selected public results
  flows:
  - authorizationCode
  scope: results:read
- description: Check current usage
  flows:
  - authorizationCode
  scope: usage:read
slug: kunkafa-com-scopes
source_filename: kunkafa-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/kunkafa-com-openapi.json\nschemes:\n- name: KunkafaOAuth\n  source: openapi/kunkafa-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://kunkafa.com/oauth/authorize\n    tokenUrl: https://kunkafa.com/oauth/token\n  description: 'Authorization code with required PKCE. Issuer https://kunkafa.com/oauth. Request\n    resource https://kunkafa.com/mcp for MCP or https://kunkafa.com/api/v1 for Pro or Publisher\n    REST. Access tokens expire after 10 minutes; refresh tokens rotate and reuse revokes the\n    grant. An MCP connection stays connected while used: it expires after 90 days without use\n    and at most one year after approval. The same app approving again replaces its connection;\n    asking only for access already allowed needs no second approval. Validate issuer/resource/audience;\n    never give an agent app sign-in credentials.'\nscopes:\n- scope: following:write\n  description:\
  \ Follow and unfollow markets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kunkafa-com-openapi.json\n- scope: markets:read\n  description: List authorized markets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kunkafa-com-openapi.json\n- scope: outlooks:read\n  description: Read controlled current summaries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kunkafa-com-openapi.json\n- scope: performance:read\n  description: Read published performance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kunkafa-com-openapi.json\n- scope: results:read\n  description: Read selected public results\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kunkafa-com-openapi.json\n- scope: usage:read\n  description: Check current usage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kunkafa-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kunkafa-com/scopes/kunkafa-com-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Artificial Intelligence
- Finance
- Market Forecasts
- Cryptocurrency
- Predictive Analytics
- Company
token_bound: false
token_urls:
- https://kunkafa.com/oauth/token
---
