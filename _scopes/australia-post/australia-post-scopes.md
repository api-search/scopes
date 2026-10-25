---
api_specs:
- filename: australia-post-endpoints-api-openapi.yml
  format: yaml
  label: Australia Post Endpoints API
  slug: australia-post-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/australia-post-endpoints-api-openapi.yml
authorization_urls:
- https://welcome.auspost.com.au/authorize
description: ''
docs: https://auspost.com.au/developers/help-support/about-our-apis/
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Australia Post Scopes
name_suffix: OAuth Scopes
note: The Developer Portal documents OAuth 2.0 Client Credentials and Authorisation Code (PKCE) credential types but publishes no scope reference page; the only scope known is the one declared in the International Export Tools V3 contract.
overview: 'Australia Post publishes 1 OAuth 2.0 scope via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Australia Post API on a user''s behalf.


  Tokens are issued from https://welcome.auspost.com.au/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Australia Post
provider_slug: australia-post
schemes:
- flows:
  - flow: clientCredentials
  - authorizationUrl: https://welcome.auspost.com.au/authorize
    flow: authorizationCode
    tokenUrl: https://welcome.auspost.com.au/oauth/token
  name: OIDCSecurity
  source: openapi/australia-post-international-export-tools-v3-openapi.yml
scope_count: 1
scope_names:
- https://scopes.auspost.com.au/auth/export-tools/v3/export.read
scopes:
- description: read permissions for International Export Tools API
  flows:
  - authorizationCode
  - clientCredentials
  scope: https://scopes.auspost.com.au/auth/export-tools/v3/export.read
slug: australia-post-scopes
source_filename: australia-post-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: derived\nsource: openapi/australia-post-international-export-tools-v3-openapi.yml\nschemes:\n- name: OIDCSecurity\n  source: openapi/australia-post-international-export-tools-v3-openapi.yml\n  flows:\n  - flow: clientCredentials\n  - flow: authorizationCode\n    authorizationUrl: https://welcome.auspost.com.au/authorize\n    tokenUrl: https://welcome.auspost.com.au/oauth/token\nscopes:\n- scope: https://scopes.auspost.com.au/auth/export-tools/v3/export.read\n  description: read permissions for International Export Tools API\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/australia-post-international-export-tools-v3-openapi.yml\ndocs: https://auspost.com.au/developers/help-support/about-our-apis/\nnote: The Developer Portal documents OAuth 2.0 Client Credentials and Authorisation Code (PKCE) credential types\n  but publishes no scope reference page; the only scope known is the one declared in the International\
  \ Export Tools\n  V3 contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/scopes/australia-post-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode
tags:
- Address Validation
- Click and Collect
- Delivery
- E-Commerce
- Labels
- Location
- Logistics
- Parcel Locker
- Postal
- Postage
- Shipping
- Tracking
- Australia
token_bound: false
token_urls:
- https://welcome.auspost.com.au/oauth/token
---
