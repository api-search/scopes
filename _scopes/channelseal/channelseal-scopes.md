---
api_specs:
- filename: channelseal-platform-api-openapi.yml
  format: yaml
  label: ChannelSeal Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-platform-api-openapi.yml
- filename: channelseal-api-discovery-service-api-openapi.yml
  format: yaml
  label: ChannelSeal API Discovery Service API
  slug: api-discovery-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-api-discovery-service-api-openapi.yml
- filename: channelseal-api-catalog-api-openapi.yml
  format: yaml
  label: ChannelSeal API Catalog API
  slug: api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-api-catalog-api-openapi.yml
- filename: channelseal-data-classification-api-openapi.yml
  format: yaml
  label: ChannelSeal Data Classification API
  slug: data-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-data-classification-api-openapi.yml
authorization_urls: []
description: 'The OpenAPI declares a single oauth2 clientCredentials scheme (security_auth) with an EMPTY scopes map, and no operation carries a security[] requirement, so the derived baseline had zero scopes. The docs'' Authentication section publishes four coarse scopes requested at the Auth0 token endpoint with audience https://api.channelseal.com; the provider''s own OpenTelemetry collector integration (github.com/channelseal/integrations) requests a fifth, import:telemetry, against audience https://telemetry.channelseal.com. Scope-to-operation mapping is not published; the docs'' 403 example shows the server naming a required scope in the problem detail ("Required scope: ''admin''").'
docs: https://docs.channelseal.com/api-reference#available-scopes
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Channelseal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ChannelSeal publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ChannelSeal API on a user''s behalf.


  Tokens are issued from https://dev-channelseal.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ChannelSeal
provider_slug: channelseal
schemes:
- flows:
  - audience: https://api.channelseal.com
    discovery: well-known/channelseal-auth0-oauth-authorization-server.json
    flow: clientCredentials
    issuer: https://dev-channelseal.us.auth0.com/
    tokenUrl: https://dev-channelseal.us.auth0.com/oauth/token
  name: security_auth
  source: openapi/channelseal-api-schemas-openapi.yml
scope_count: 5
scope_names:
- read
- write
- delete
- admin
- import:telemetry
scopes:
- description: Read access to resources
  flows:
  - clientCredentials
  scope: read
- description: Create and update resources
  flows:
  - clientCredentials
  scope: write
- description: Delete resources
  flows:
  - clientCredentials
  scope: delete
- description: Full administrative access
  flows:
  - clientCredentials
  scope: admin
- description: Export OTLP logs/traces of HTTP API traffic into ChannelSeal via the OpenTelemetry Collector otlphttp exporter (audience https://telemetry.channelseal.com)
  flows:
  - clientCredentials
  scope: import:telemetry
slug: channelseal-scopes
source_filename: channelseal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: openapi/channelseal-api-schemas-openapi.yml\ndocs: https://docs.channelseal.com/api-reference#available-scopes\ndescription: >-\n  The OpenAPI declares a single oauth2 clientCredentials scheme (security_auth) with an EMPTY scopes map,\n  and no operation carries a security[] requirement, so the derived baseline had zero scopes. The docs'\n  Authentication section publishes four coarse scopes requested at the Auth0 token endpoint with\n  audience https://api.channelseal.com; the provider's own OpenTelemetry collector integration\n  (github.com/channelseal/integrations) requests a fifth, import:telemetry, against audience\n  https://telemetry.channelseal.com. Scope-to-operation mapping is not published; the docs' 403 example\n  shows the server naming a required scope in the problem detail (\"Required scope: 'admin'\").\nschemes:\n- name: security_auth\n  source: openapi/channelseal-api-schemas-openapi.yml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://dev-channelseal.us.auth0.com/oauth/token\n    audience: https://api.channelseal.com\n    issuer: https://dev-channelseal.us.auth0.com/\n    discovery: well-known/channelseal-auth0-oauth-authorization-server.json\nscopes:\n- scope: read\n  description: Read access to resources\n  flows: [clientCredentials]\n  sources: [https://docs.channelseal.com/api-reference#available-scopes]\n- scope: write\n  description: Create and update resources\n  flows: [clientCredentials]\n  sources: [https://docs.channelseal.com/api-reference#available-scopes]\n- scope: delete\n  description: Delete resources\n  flows: [clientCredentials]\n  sources: [https://docs.channelseal.com/api-reference#available-scopes]\n- scope: admin\n  description: Full administrative access\n  flows: [clientCredentials]\n  sources: [https://docs.channelseal.com/api-reference#available-scopes]\n- scope: import:telemetry\n  description: Export OTLP logs/traces of HTTP API traffic into ChannelSeal\
  \ via the OpenTelemetry Collector otlphttp exporter (audience https://telemetry.channelseal.com)\n  flows: [clientCredentials]\n  sources: [https://github.com/channelseal/integrations/blob/main/otlp-collector/otel-collector-config.yaml]\nnotes:\n- Multiple scopes are space-separated in the token request (\"scope=read write delete\").\n- The docs' example token request sends client_id/client_secret in a JSON body to the Auth0 /oauth/token endpoint; the JavaScript example sends them as URL-encoded form fields with a JSON content-type header — the two examples disagree.\n- The docs portal itself (Zudoku) signs users in against the same Auth0 tenant with scopes openid profile email custom_scope; that is portal login, not an API scope set.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/scopes/channelseal-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Company
- API Security
- AI Agents
- MCP
- Data Classification
- API Discovery
- Non-Human Identity
- Sensitive Data
- Observability
- OpenTelemetry
- Governance
token_urls:
- https://dev-channelseal.us.auth0.com/oauth/token
---
