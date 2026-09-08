---
authorization_urls: []
description: ''
docs: https://help.expeditors.com/globalhelp/shipment_api/data_types.htm
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Expeditors International Of Washington Scopes
name_suffix: OAuth Scopes
note: The Tracking API issues a single-scope client-credentials token. Expeditors documents no scope reference page and no per-resource permissions; the docs state explicitly that "this API has only one type of token", which is why a 403 insufficient_scope "should not occur".
overview: 'Expeditors International of Washington publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Expeditors International of Washington API on a user''s behalf.


  Tokens are issued from https://api.expeditors.com/tracking/v2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Expeditors International of Washington
provider_slug: expeditors-international-of-washington
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.expeditors.com/tracking/v2/oauth2/token
  name: OAuth2ClientCredentials
  source: https://help.expeditors.com/globalhelp/shipment_api/POST_oauth2_token.htm
scope_count: 1
scope_names:
- application
scopes:
- description: Indicates the token is valid only for the Expeditors Tracking service. The only scope the API issues.
  flows:
  - clientCredentials
  scope: application
slug: expeditors-international-of-washington-scopes
source_filename: expeditors-international-of-washington-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://help.expeditors.com/globalhelp/shipment_api/POST_oauth2_token.htm\ndocs: https://help.expeditors.com/globalhelp/shipment_api/data_types.htm\nnote: >-\n  The Tracking API issues a single-scope client-credentials token. Expeditors\n  documents no scope reference page and no per-resource permissions; the docs\n  state explicitly that \"this API has only one type of token\", which is why a\n  403 insufficient_scope \"should not occur\".\nschemes:\n  - name: OAuth2ClientCredentials\n    source: https://help.expeditors.com/globalhelp/shipment_api/POST_oauth2_token.htm\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.expeditors.com/tracking/v2/oauth2/token\nscopes:\n  - scope: application\n    description: Indicates the token is valid only for the Expeditors Tracking service. The only scope the API issues.\n    flows: [clientCredentials]\n    sources: [https://help.expeditors.com/globalhelp/shipment_api/data_types.htm]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expeditors-international-of-washington/refs/heads/main/scopes/expeditors-international-of-washington-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Customs
- Freight Forwarding
- Logistics
- Supply Chain
- Warehousing
- Shipment Tracking
- Transportation
- Order Management
- Customs Brokerage
- Visibility
token_urls:
- https://api.expeditors.com/tracking/v2/oauth2/token
---
