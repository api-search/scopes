---
authorization_urls: []
description: ''
docs: https://help.alteryx.com/current/en/server/api-overview/alteryx-server-api-v3/server-api-configuration-and-authorization.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Alteryx Scopes
name_suffix: OAuth Scopes
note: Alteryx Server API v3 uses an OAuth 2.0 client_credentials flow with an API Access Key and Secret from the user's Server profile, and access is governed by Server roles (e.g. admin enablement) rather than OAuth scopes; no scopes are documented (https://help.alteryx.com/current/en/server/api-overview/alteryx-server-api-v3/server-api-configuration-and-authorization.html).
overview: 'Alteryx uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{serverHostname}/webapi/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alteryx
provider_slug: alteryx
schemes:
- description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained from the Server User Interface under the Keys section.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{serverHostname}/webapi/oauth2/token
  name: oauth2
  source: openapi/alteryx-server-api-v3.yml
scope_count: 0
scope_names: []
scopes: []
slug: alteryx-scopes
source_filename: alteryx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alteryx-server-api-v3.yml\ndocs: https://help.alteryx.com/current/en/server/api-overview/alteryx-server-api-v3/server-api-configuration-and-authorization.html\nnote: Alteryx Server API v3 uses an OAuth 2.0 client_credentials flow with an API\n  Access Key and Secret from the user's Server profile, and access is governed by\n  Server roles (e.g. admin enablement) rather than OAuth scopes; no scopes are documented\n  (https://help.alteryx.com/current/en/server/api-overview/alteryx-server-api-v3/server-api-configuration-and-authorization.html).\nschemes:\n- name: oauth2\n  source: openapi/alteryx-server-api-v3.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{serverHostname}/webapi/oauth2/token\n  description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained\n    from the Server User Interface under the Keys section.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/scopes/alteryx-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
token_urls:
- https://{serverHostname}/webapi/oauth2/token
---
