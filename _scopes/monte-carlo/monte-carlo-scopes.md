---
api_specs:
- filename: monte-carlo-graph-ql-api-openapi.yml
  format: yaml
  label: Monte Carlo Graph QL API
  slug: monte-carlo-graph-ql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monte-carlo/refs/heads/main/openapi/monte-carlo-graph-ql-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.getmontecarlo.com/docs/api-authentication#authenticating-with-oauth-client-credentials
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Monte Carlo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Monte Carlo publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Monte Carlo API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Monte Carlo
provider_slug: monte-carlo
schemes: []
scope_count: 6
scope_names:
- https://api.getmontecarlo.com/access
- https://instance.getmontecarlo.com/{instance_id}
- offline_access
- openid
- profile
- email
scopes:
- description: API access scope requested in the client-credentials grant.
  flows: []
  scope: https://api.getmontecarlo.com/access
- description: Instance-routing scope naming the deployment (e.g. us1, eu1); requested together with the access scope.
  flows: []
  scope: https://instance.getmontecarlo.com/{instance_id}
- description: Only scope advertised by the MCP protected-resource metadata; issues refresh tokens.
  flows: []
  scope: offline_access
- description: Advertised by auth.getmontecarlo.com.
  flows: []
  scope: openid
- description: Advertised by auth.getmontecarlo.com.
  flows: []
  scope: profile
- description: Advertised by auth.getmontecarlo.com.
  flows: []
  scope: email
slug: monte-carlo-scopes
source_filename: monte-carlo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: https://docs.getmontecarlo.com/docs/api-authentication\ndocs: https://docs.getmontecarlo.com/docs/api-authentication#authenticating-with-oauth-client-credentials\nauthorization_servers:\n- issuer: https://auth.getmontecarlo.com\n  metadata: https://auth.getmontecarlo.com/.well-known/oauth-authorization-server\n- token_url: https://api.getmontecarlo.com/oauth2/token\n  note: Token URL shown for OAuth client-credentials clients of the GraphQL API.\nscopes:\n- scope: https://api.getmontecarlo.com/access\n  api: monte-carlo:graphql-api\n  description: API access scope requested in the client-credentials grant.\n- scope: https://instance.getmontecarlo.com/{instance_id}\n  api: monte-carlo:graphql-api\n  description: Instance-routing scope naming the deployment (e.g. us1, eu1); requested together with the access scope.\n- scope: offline_access\n  api: monte-carlo:mcp-server\n  description: Only scope advertised by the MCP protected-resource\
  \ metadata; issues refresh tokens.\n- scope: openid\n  api: auth\n  description: Advertised by auth.getmontecarlo.com.\n- scope: profile\n  api: auth\n  description: Advertised by auth.getmontecarlo.com.\n- scope: email\n  api: auth\n  description: Advertised by auth.getmontecarlo.com.\npermissions_note: >-\n  Fine-grained access is governed by Monte Carlo roles and authorization groups rather than OAuth scopes\n  (e.g. lineage/read; MCP requires Editor or above). See https://docs.getmontecarlo.com/docs/authorization.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monte-carlo/refs/heads/main/scopes/monte-carlo-scopes.yml
summary_line: 6 scopes
tags:
- Data Observability
- Data Quality
- Data Reliability
- Data Lake
- Data Warehouse
- Lineage
- Monitoring
- AI Observability
token_urls: []
---
