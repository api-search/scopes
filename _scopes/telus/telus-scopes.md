---
api_specs:
- filename: telus-insights-location-api.postman_collection.json
  format: json
  label: TELUS Insights Location API
  slug: telus-insights-location-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/telus/refs/heads/main/collections/telus-insights-location-api.postman_collection.json
authorization_urls: []
description: 'The only OAuth 2.0 surface TELUS documents publicly is the Insights Location API''s client- credentials grant. TELUS does document that a `scope` parameter is sent on the token request, but it does not publish any scope VALUES: the documentation tells the consumer to copy oauth_client_id, oauth_client_secret, oauth_token_endpoint, oauth_grant_type and oauth_scope from the "My Account" page of the TELUS Insights Portal after onboarding. There is therefore a real scope parameter with a per-customer, unpublished value — recorded here as an honest empty registry rather than an invented one. The TELUS Health CHR Enterprise API has no scopes at all: it authenticates with a self-signed RS512 JWT and, per its own documentation, an API Consumer provides "unrestricted access to your organization''s CHR data" (there is no scoping layer).'
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Telus Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TELUS uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TELUS
provider_slug: telus
schemes:
- api: TELUS Insights Location API
  flows:
  - flow: clientCredentials
    scopeParameterSupported: true
    tokenUrl: null
    tokenUrlPublished: false
  name: InsightsOAuth2ClientCredentials
  source: collections/telus-insights-location-api.postman_collection.json
  type: oauth2
scope_count: 0
scope_names: []
scopes: []
slug: telus-scopes
source_filename: telus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://docs.insights.telus.com/ — \"Introduction - API Integrations\" and \"Getting Started - Authentication\"\ndescription: >-\n  The only OAuth 2.0 surface TELUS documents publicly is the Insights Location API's client-\n  credentials grant. TELUS does document that a `scope` parameter is sent on the token request, but\n  it does not publish any scope VALUES: the documentation tells the consumer to copy\n  oauth_client_id, oauth_client_secret, oauth_token_endpoint, oauth_grant_type and oauth_scope from\n  the \"My Account\" page of the TELUS Insights Portal after onboarding. There is therefore a real\n  scope parameter with a per-customer, unpublished value — recorded here as an honest empty\n  registry rather than an invented one. The TELUS Health CHR Enterprise API has no scopes at all:\n  it authenticates with a self-signed RS512 JWT and, per its own documentation, an API Consumer\n  provides \"unrestricted access to\
  \ your organization's CHR data\" (there is no scoping layer).\nschemes:\n- name: InsightsOAuth2ClientCredentials\n  api: TELUS Insights Location API\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    tokenUrlPublished: false\n    scopeParameterSupported: true\n  source: collections/telus-insights-location-api.postman_collection.json\nscopes: []\nscopes_published: false\nscopes_note: >-\n  Zero scope values are published anonymously. Do not assume a scope string — request the\n  oauth_scope value with the credentials issued through the Insights Portal ticket process.\nno_scope_surfaces:\n- api: TELUS Health CHR Enterprise API\n  reason: >-\n    Self-signed JWT bearer (RS512); authorization is all-or-nothing per API Consumer, not scoped.\n  source: https://help.inputhealth.com/en/articles/6483229-creating-api-consumers\nrelated:\n  authentication: authentication/telus-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telus/refs/heads/main/scopes/telus-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Telecommunications
- Canada
- Mobile Network Operator
- Broadband
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- Location Intelligence
- IoT
- 5G
- Healthcare
- Electronic Medical Records
- GraphQL
- Webhooks
- Geospatial
token_urls: []
---
