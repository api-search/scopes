---
api_specs:
- filename: fanaura-com-careers-api-openapi.yml
  format: yaml
  label: Fanaura Careers API
  slug: fanaura-com-careers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-careers-api-openapi.yml
- filename: fanaura-com-demo-api-openapi.yml
  format: yaml
  label: Fanaura Demo API
  slug: fanaura-com-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-demo-api-openapi.yml
- filename: fanaura-com-legal-api-openapi.yml
  format: yaml
  label: Fanaura Legal API
  slug: fanaura-com-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-legal-api-openapi.yml
- filename: fanaura-com-llms-full-txt-api-openapi.yml
  format: yaml
  label: Fanaura Llms Full.txt API
  slug: fanaura-com-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-llms-full-txt-api-openapi.yml
- filename: fanaura-com-llms-txt-api-openapi.yml
  format: yaml
  label: Fanaura Llms.txt API
  slug: fanaura-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-llms-txt-api-openapi.yml
- filename: fanaura-com-mcp-api-openapi.yml
  format: yaml
  label: Fanaura MCP API
  slug: fanaura-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-mcp-api-openapi.yml
- filename: fanaura-com-openapi-json-api-openapi.yml
  format: yaml
  label: Fanaura Openapi.json API
  slug: fanaura-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-openapi-json-api-openapi.yml
- filename: fanaura-com-privacy-policy-txt-api-openapi.yml
  format: yaml
  label: Fanaura Privacy Policy.txt API
  slug: fanaura-com-privacy-policy-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-privacy-policy-txt-api-openapi.yml
- filename: fanaura-com-revalidate-api-openapi.yml
  format: yaml
  label: Fanaura Revalidate API
  slug: fanaura-com-revalidate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-revalidate-api-openapi.yml
- filename: fanaura-com-sitemap-xml-api-openapi.yml
  format: yaml
  label: Fanaura Sitemap.xml API
  slug: fanaura-com-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-sitemap-xml-api-openapi.yml
- filename: fanaura-com-well-known-api-openapi.yml
  format: yaml
  label: Fanaura .well Known API
  slug: fanaura-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-well-known-api-openapi.yml
authorization_urls:
- https://app.fanaura.com/oauth/mcp/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Fanaura Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fanaura publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fanaura API on a user''s behalf.


  Tokens are issued from https://app.fanaura.com/api/oauth/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fanaura
provider_slug: fanaura-com
schemes:
- description: OAuth 2.0 for https://app.fanaura.com/mcp. Authorization code with PKCE (S256). Request only the scope the task needs. Do not request every scope in this list.
  flows:
  - authorizationUrl: https://app.fanaura.com/oauth/mcp/authorize
    flow: authorizationCode
    tokenUrl: https://app.fanaura.com/api/oauth/mcp/token
  name: fanauraMcpOAuth
  source: openapi/fanaura-com-openapi.json
scope_count: 3
scope_names:
- audience:read
- journeys:read
- journeys:write
scopes:
- description: Read contacts, timelines, and audience totals on the signed-in account.
  flows:
  - authorizationCode
  scope: audience:read
- description: Read journeys, keywords, destinations, and publish state on the signed-in account.
  flows:
  - authorizationCode
  scope: journeys:read
- description: Create and edit journeys on the signed-in account. Publishing still requires an active membership and a connected Instagram account.
  flows:
  - authorizationCode
  scope: journeys:write
slug: fanaura-com-scopes
source_filename: fanaura-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fanaura-com-openapi.json\nschemes:\n- name: fanauraMcpOAuth\n  source: openapi/fanaura-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.fanaura.com/oauth/mcp/authorize\n    tokenUrl: https://app.fanaura.com/api/oauth/mcp/token\n  description: OAuth 2.0 for https://app.fanaura.com/mcp. Authorization code with PKCE (S256).\n    Request only the scope the task needs. Do not request every scope in this list.\nscopes:\n- scope: audience:read\n  description: Read contacts, timelines, and audience totals on the signed-in account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fanaura-com-openapi.json\n- scope: journeys:read\n  description: Read journeys, keywords, destinations, and publish state on the signed-in account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fanaura-com-openapi.json\n- scope: journeys:write\n  description: Create and edit journeys on the\
  \ signed-in account. Publishing still requires\n    an active membership and a connected Instagram account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fanaura-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fanaura-com/scopes/fanaura-com-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Instagram DM automation
- Music marketing
- Release marketing
- Business marketing
token_bound: false
token_urls:
- https://app.fanaura.com/api/oauth/mcp/token
---
