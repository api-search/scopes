---
api_specs:
- filename: coderbuds-com-openapi-generated.yml
  format: yaml
  label: Coderbuds API
  slug: coderbuds-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderbuds-com/openapi/_ae-authored/coderbuds-com-openapi-generated.yml
authorization_urls: []
description: ''
docs: https://coderbuds.com/docs/api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Coderbuds Scopes
name_suffix: OAuth Scopes
note: The REST API uses API-token permissions rather than OAuth scopes. Only the read permission is documented as relevant; "Granting more permissions does not unlock anything here — every endpoint on this page is a GET." The MCP server's OAuth scope set is not documented on https://coderbuds.com/docs/mcp.
overview: 'Coderbuds publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coderbuds API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coderbuds
provider_slug: coderbuds-com
schemes: []
scope_count: 1
scope_names:
- read
scopes:
- description: Required and sufficient for every /api/v1 endpoint. A token without it is rejected with 403; mint a new token with read checked, permissions cannot be added to an existing token.
  flows: []
  scope: read
slug: coderbuds-com-scopes
source_filename: coderbuds-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coderbuds.com/docs/api\ndocs: https://coderbuds.com/docs/api\nnote: The REST API uses API-token permissions rather than OAuth scopes. Only the read permission is documented as relevant; \"Granting more permissions does not unlock anything here — every endpoint on this page is a GET.\" The MCP server's OAuth scope set is not documented on https://coderbuds.com/docs/mcp.\nscopes:\n- name: read\n  kind: api-token-permission\n  description: Required and sufficient for every /api/v1 endpoint. A token without it is rejected with 403; mint a new token with read checked, permissions cannot be added to an existing token.\n"
source_yaml_url: https://artifacts.apis.io/coderbuds-com/scopes/coderbuds-com-scopes.yml
summary_line: 1 scope
tags:
- Company
- DORA Metrics
- Engineering Metrics
- Developer Productivity
- Code Review
- AI Agents
- MCP
- Software Engineering Intelligence
token_bound: false
token_urls: []
---
