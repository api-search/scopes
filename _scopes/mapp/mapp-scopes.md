---
api_specs:
- filename: mapp-engage-openapi.yml
  format: yaml
  label: Mapp Engage API
  slug: engage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-engage-openapi.yml
- filename: mapp-intelligence-analytics-openapi.yml
  format: yaml
  label: Mapp Intelligence Analytics API
  slug: intelligence-analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-intelligence-analytics-openapi.yml
- filename: mapp-product-catalog-openapi.yml
  format: yaml
  label: Mapp Product Catalog Public API
  slug: product-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-product-catalog-openapi.yml
- filename: mapp-fashion-openapi.yml
  format: yaml
  label: Mapp Fashion API
  slug: fashion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-fashion-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.mapp.com/apidocs/how-to-grant-access-to-the-intelligence-analytics-api
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Mapp Scopes
name_suffix: OAuth Scopes
note: Mapp has almost no scope surface. The Analytics API OpenAPI declares a single scope, "mapp.intelligence-api", on its clientCredentials scheme — and the current documentation explicitly tells integrators NOT to send a scope parameter at all, because earlier versions required one and the current token endpoint rejects it. Treat the declared scope as vestigial. The only other scope published anywhere in the Mapp estate is "mcp", advertised by https://mapp.com/.well-known/oauth-authorization-server for the WordPress MCP endpoint. Engage (HTTP Basic) and Product Catalog (bearer JWT) have no scope model; authorisation there is by system-user role and per-account feature enablement.
overview: 'Mapp Marketing Cloud publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mapp Marketing Cloud API on a user''s behalf.


  Tokens are issued from https://auth.mapp.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mapp Marketing Cloud
provider_slug: mapp
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.mapp.com/oauth2/token
  name: oauth_security_scheme
  source: openapi/mapp-intelligence-analytics-openapi.yml
scope_count: 2
scope_names:
- mapp.intelligence-api
- mcp
scopes:
- description: Declared on the Analytics API oauth2 scheme. Documentation instructs clients not to send a scope parameter.
  flows:
  - clientCredentials
  scope: mapp.intelligence-api
- description: The only scope the mapp.com MCP authorization server advertises.
  flows:
  - authorizationCode
  scope: mcp
slug: mapp-scopes
source_filename: mapp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/mapp-intelligence-analytics-openapi.yml\nschemes:\n- name: oauth_security_scheme\n  source: openapi/mapp-intelligence-analytics-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.mapp.com/oauth2/token\nscopes:\n- scope: mapp.intelligence-api\n  api: mapp:intelligence-analytics\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/mapp-intelligence-analytics-openapi.yml\n  description: Declared on the Analytics API oauth2 scheme. Documentation instructs clients not to send a scope\n    parameter.\n  status: vestigial\n- scope: mcp\n  api: mapp.com MCP endpoint\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/mapp-oauth-authorization-server.json\n  - well-known/mapp-oauth-protected-resource.json\n  description: The only scope the mapp.com MCP authorization server advertises.\ndocs: https://docs.mapp.com/apidocs/how-to-grant-access-to-the-intelligence-analytics-api\nnote: Mapp\
  \ has almost no scope surface. The Analytics API OpenAPI declares a single scope, \"mapp.intelligence-api\",\n  on its clientCredentials scheme — and the current documentation explicitly tells integrators NOT to send a scope\n  parameter at all, because earlier versions required one and the current token endpoint rejects it. Treat the declared\n  scope as vestigial. The only other scope published anywhere in the Mapp estate is \"mcp\", advertised by https://mapp.com/.well-known/oauth-authorization-server\n  for the WordPress MCP endpoint. Engage (HTTP Basic) and Product Catalog (bearer JWT) have no scope model; authorisation\n  there is by system-user role and per-account feature enablement.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/scopes/mapp-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Marketing
- Marketing Automation
- Email
- Analytics
- Customer Data
- Personalization
- Push Notifications
- SMS
- E-Commerce
- Digital Analytics
- Recommendations
token_urls:
- https://auth.mapp.com/oauth2/token
---
