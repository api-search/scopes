---
api_specs:
- filename: QuantcastDeveloperAPI.postman_collection.json
  format: json
  label: Quantcast Platform GraphQL API
  slug: quantcast-platform-graphql-api
  spec_type: Postman
  url: https://developers.quantcast.com/docs/QuantcastDeveloperAPI.postman_collection.json
authorization_urls: []
description: ''
docs: https://developers.quantcast.com/docs/get-started/authentication/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Quantcast Scopes
name_suffix: OAuth Scopes
note: 'Quantcast publishes no OpenAPI, so derive-oauth-scopes.py has nothing to read. These scopes were taken verbatim from the token request the authentication guide prints, and from the sample token response on the same page which echoes back "scope": "read_reports api_access". Quantcast publishes no separate scopes/permissions reference page; the two scopes below are the complete published set. Fine-grained authorization on the platform is expressed through Roles / AccountAction on the GraphQL Role object, not through OAuth scopes.'
overview: 'Quantcast publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Quantcast API on a user''s behalf.


  Tokens are issued from https://auth.quantcast.com/oauth2/default/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Quantcast
provider_slug: quantcast
schemes:
- flows:
  - flow: clientCredentials
    source: https://developers.quantcast.com/docs/get-started/authentication/
    tokenUrl: https://auth.quantcast.com/oauth2/default/v1/token
  name: QuantcastPlatformOAuth2
scope_count: 2
scope_names:
- api_access
- read_reports
scopes:
- description: Grants the client credential access to the Quantcast Platform APIs. Sent in the documented token request and echoed in the token response.
  flows:
  - clientCredentials
  scope: api_access
- description: Grants read access to reporting data — the accountMetricsReport and availableBreakdownsAndMetrics queries in the GraphQL API and the legacy REST Reporting API report endpoint.
  flows:
  - clientCredentials
  scope: read_reports
slug: quantcast-scopes
source_filename: quantcast-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.quantcast.com/docs/get-started/authentication/\ndocs: https://developers.quantcast.com/docs/get-started/authentication/\nnote: >-\n  Quantcast publishes no OpenAPI, so derive-oauth-scopes.py has nothing to\n  read. These scopes were taken verbatim from the token request the\n  authentication guide prints, and from the sample token response on the same\n  page which echoes back \"scope\": \"read_reports api_access\". Quantcast\n  publishes no separate scopes/permissions reference page; the two scopes\n  below are the complete published set. Fine-grained authorization on the\n  platform is expressed through Roles / AccountAction on the GraphQL Role\n  object, not through OAuth scopes.\nschemes:\n- name: QuantcastPlatformOAuth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.quantcast.com/oauth2/default/v1/token\n    source: https://developers.quantcast.com/docs/get-started/authentication/\n\
  scopes:\n- scope: api_access\n  description: >-\n    Grants the client credential access to the Quantcast Platform APIs. Sent\n    in the documented token request and echoed in the token response.\n  flows: [clientCredentials]\n  sources: [https://developers.quantcast.com/docs/get-started/authentication/]\n- scope: read_reports\n  description: >-\n    Grants read access to reporting data — the accountMetricsReport and\n    availableBreakdownsAndMetrics queries in the GraphQL API and the legacy\n    REST Reporting API report endpoint.\n  flows: [clientCredentials]\n  sources: [https://developers.quantcast.com/docs/get-started/authentication/]\nrelated:\n  okta_org_server_scopes:\n    source: well-known/quantcast-openid-configuration.json\n    scopes: [openid, email, profile, address, phone, offline_access, groups]\n    note: >-\n      These are the standard OIDC scopes advertised by the Okta org\n      authorization server at auth.quantcast.com. They govern platform user\n      sign-in,\
  \ NOT the Quantcast Platform API. Recorded for completeness;\n      do not request them for API access.\n  permission_model:\n    note: >-\n      Effective API permissions follow the calling user. API credentials are\n      themselves platform users: an Owner has all permissions over every\n      account, while Members and Supply Managers must be assigned to\n      individual accounts through the Platform UI before the API will return\n      their resources.\n    source: https://developers.quantcast.com/docs/get-started/understanding-the-domain/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantcast/refs/heads/main/scopes/quantcast-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Advertising
- AdTech
- Programmatic Advertising
- Demand-Side Platform
- DSP
- Audience Measurement
- Audience Intelligence
- Consent Management
- CMP
- Privacy
- GraphQL
- Conversion Tracking
- CTV
- Video Advertising
- Display Advertising
- Artificial Intelligence
- Audience Graph
token_urls:
- https://auth.quantcast.com/oauth2/default/v1/token
---
