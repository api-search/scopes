---
authorization_urls: []
description: ''
docs: https://dash.plotly.com/plotly-cloud/sign-in
flows:
- authorization_code
- refresh_token
- device_code
- client_credentials
kind: oauth-scopes
layout: scope
method: probed
name: Plotly Scopes
name_suffix: OAuth Scopes
note: 'Read directly from the Plotly Cloud authorization server''s own discovery documents (RFC 8414 and OpenID Connect Discovery), both fetched 2026-08-26. Plotly publishes no scopes reference page and declares no product- or resource-specific scopes: the advertised set is the standard OIDC quartet only. That is the finding - the Dash Docs MCP server is protected by authentication rather than by scoped authorization.'
overview: 'Plotly publishes 4 OAuth 2.0 scopes via the authorization_code, refresh_token, device_code, and client_credentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Plotly API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Plotly
provider_slug: plotly
schemes:
- flows:
  - authorization_code
  - refresh_token
  - device_code
  - client_credentials
  issuer: https://signin.cloud.plotly.com
  name: PlotlyCloudOAuth
  source: https://signin.cloud.plotly.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect - request an ID token identifying the end user.
  flows: []
  scope: openid
- description: Access the end user's default profile claims.
  flows: []
  scope: profile
- description: Access the end user's email address claim.
  flows: []
  scope: email
- description: Issue a refresh token so the client can act without the user present.
  flows: []
  scope: offline_access
slug: plotly-scopes
source_filename: plotly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://signin.cloud.plotly.com/.well-known/openid-configuration\ndocs: https://dash.plotly.com/plotly-cloud/sign-in\nnote: >-\n  Read directly from the Plotly Cloud authorization server's own discovery documents (RFC 8414\n  and OpenID Connect Discovery), both fetched 2026-08-26. Plotly publishes no scopes reference\n  page and declares no product- or resource-specific scopes: the advertised set is the standard\n  OIDC quartet only. That is the finding - the Dash Docs MCP server is protected by\n  authentication rather than by scoped authorization.\nschemes:\n- name: PlotlyCloudOAuth\n  source: https://signin.cloud.plotly.com/.well-known/oauth-authorization-server\n  issuer: https://signin.cloud.plotly.com\n  flows:\n  - authorization_code\n  - refresh_token\n  - device_code\n  - client_credentials\nscopes:\n- name: openid\n  description: OpenID Connect - request an ID token identifying the end user.\n  standard: true\n- name:\
  \ profile\n  description: Access the end user's default profile claims.\n  standard: true\n- name: email\n  description: Access the end user's email address claim.\n  standard: true\n- name: offline_access\n  description: Issue a refresh token so the client can act without the user present.\n  standard: true\nscope_count: 4\nproduct_specific_scopes: 0\nx-evidence:\n- url: https://signin.cloud.plotly.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-26'\n- url: https://signin.cloud.plotly.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plotly/refs/heads/main/scopes/plotly-scopes.yml
summary_line: 4 scopes · authorization_code/refresh_token/device_code/client_credentials
tags:
- Company
- Data Visualization
- Analytics
- Data Apps
- Business Intelligence
- Open Source
- Python
- JavaScript
- Charts
- Dashboards
- Developer Tools
- MCP
token_bound: false
token_urls: []
---
