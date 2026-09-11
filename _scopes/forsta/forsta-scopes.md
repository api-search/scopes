---
api_specs:
- filename: forsta-decipher-rest-api-openapi.yml
  format: yaml
  label: Forsta Decipher REST API
  slug: forsta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forsta/refs/heads/main/openapi/forsta-decipher-rest-api-openapi.yml
- filename: forsta-panel-management-integration-openapi.yml
  format: yaml
  label: Forsta Panel Management APIs
  slug: panel-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forsta/refs/heads/main/openapi/forsta-panel-management-integration-openapi.yml
- filename: forsta-sample-marketplace-partner-contract-openapi.yml
  format: yaml
  label: Forsta Sample Marketplace Partner APIs
  slug: sample-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forsta/refs/heads/main/openapi/forsta-sample-marketplace-partner-contract-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Forsta Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Forsta uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Forsta
provider_slug: forsta
schemes:
- description: See https://docs.aws.amazon.com/cognito/latest/developerguide/token-endpoint.html
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token/
  name: OAuth2
  source: openapi/forsta-sample-marketplace-partner-contract-openapi.yml
- description: See https://docs.aws.amazon.com/cognito/latest/developerguide/token-endpoint.html
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token/
  name: OAuth2
  source: openapi/forsta-sample-marketplace-partner-setup-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: forsta-scopes
source_filename: forsta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: derived\nsource: openapi/forsta-sample-marketplace-partner-contract-openapi.yml, openapi/forsta-sample-marketplace-partner-setup-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/forsta-sample-marketplace-partner-contract-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token/\n  description: See https://docs.aws.amazon.com/cognito/latest/developerguide/token-endpoint.html\n- name: OAuth2\n  source: openapi/forsta-sample-marketplace-partner-setup-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token/\n  description: See https://docs.aws.amazon.com/cognito/latest/developerguide/token-endpoint.html\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forsta/refs/heads/main/scopes/forsta-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Customer Insights
- Feedback
- Market Research
- Surveys
- Customer Experience
- Employee Experience
- Panel Management
- Data Collection
- Analytics
- Voice of the Customer
token_urls:
- /oauth2/token/
---
