---
api_specs:
- filename: zoopla-products-api-openapi.yml
  format: yaml
  label: Zoopla Products API
  slug: zoopla-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/openapi/zoopla-products-api-openapi.yml
- filename: zoopla-rest-endpoints-api-openapi.yml
  format: yaml
  label: Zoopla REST Endpoints API
  slug: zoopla-rest-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/openapi/zoopla-rest-endpoints-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.zoopla.co.uk/pages/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Zoopla Scopes
name_suffix: OAuth Scopes
note: 'Zoopla publishes no scopes reference page. The authentication guide documents only `scope=api/api_access` on the token request for the activation APIs; the two lead scopes appear in the Leads contract and are not named anywhere in prose. The split is worth noting: leads use resource-scoped strings (leads/list:applicant-leads, leads/list:appraisal-leads) while both activation APIs — including the two operations that spend money — share one coarse api/api_access scope, so scope alone cannot separate reading an activation history from buying a product.'
overview: 'Zoopla publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoopla API on a user''s behalf.


  Tokens are issued from https://services-auth.services.zoopla.co.uk/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoopla
provider_slug: zoopla
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token
  name: OAuth2
  source: openapi/zoopla-leads-api-openapi.json
- description: This API uses OAuth 2 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token
  name: oAuthSample
  source: openapi/zoopla-premium-listing-activations-openapi.json
- description: This API uses OAuth 2 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token
  name: oAuthSample
  source: openapi/zoopla-weekly-featured-property-activations-openapi.json
scope_count: 3
scope_names:
- api/api_access
- leads/list:applicant-leads
- leads/list:appraisal-leads
scopes:
- description: access to the API
  flows:
  - clientCredentials
  scope: api/api_access
- description: Grants read access to applicant lead lists
  flows:
  - clientCredentials
  scope: leads/list:applicant-leads
- description: Grants read access to appraisal lead lists
  flows:
  - clientCredentials
  scope: leads/list:appraisal-leads
slug: zoopla-scopes
source_filename: zoopla-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\ndocs: https://developers.zoopla.co.uk/pages/authentication\nsource: openapi/zoopla-leads-api-openapi.json, openapi/zoopla-premium-listing-activations-openapi.json,\n  openapi/zoopla-weekly-featured-property-activations-openapi.json, https://developers.zoopla.co.uk/pages/authentication\nnote: >-\n  Zoopla publishes no scopes reference page. The authentication guide documents\n  only `scope=api/api_access` on the token request for the activation APIs; the\n  two lead scopes appear in the Leads contract and are not named anywhere in\n  prose. The split is worth noting: leads use resource-scoped strings\n  (leads/list:applicant-leads, leads/list:appraisal-leads) while both activation\n  APIs — including the two operations that spend money — share one coarse\n  api/api_access scope, so scope alone cannot separate reading an activation\n  history from buying a product.\nschemes:\n- name: OAuth2\n  source: openapi/zoopla-leads-api-openapi.json\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token\n- name: oAuthSample\n  source: openapi/zoopla-premium-listing-activations-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token\n  description: This API uses OAuth 2 with the client credentials grant flow.\n- name: oAuthSample\n  source: openapi/zoopla-weekly-featured-property-activations-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token\n  description: This API uses OAuth 2 with the client credentials grant flow.\nscopes:\n- scope: api/api_access\n  description: access to the API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zoopla-premium-listing-activations-openapi.json\n  - openapi/zoopla-weekly-featured-property-activations-openapi.json\n- scope: leads/list:applicant-leads\n  description: Grants read access to applicant\
  \ lead lists\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zoopla-leads-api-openapi.json\n- scope: leads/list:appraisal-leads\n  description: Grants read access to appraisal lead lists\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zoopla-leads-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/scopes/zoopla-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Property Portal
- PropTech
- Rentals
- Estate Agents
- Leads
- CRM Integration
token_urls:
- https://services-auth.services.zoopla.co.uk/oauth2/token
---
