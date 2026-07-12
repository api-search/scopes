---
authorization_urls:
- https://authenticate.trustpilot.com/oauth/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Trustpilot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Trustpilot publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Trustpilot API on a user''s behalf.


  Tokens are issued from https://authenticate.trustpilot.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Trustpilot
provider_slug: trustpilot
schemes:
- flows:
  - authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize
    flow: authorizationCode
    tokenUrl: https://authenticate.trustpilot.com/oauth/token
  name: OAuth2
  source: openapi/trustpilot-business-units-openapi.yml
- flows:
  - authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize
    flow: authorizationCode
    tokenUrl: https://authenticate.trustpilot.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://authenticate.trustpilot.com/oauth/token
  name: OAuth2
  source: openapi/trustpilot-invitation-openapi.yml
- flows:
  - authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize
    flow: authorizationCode
    tokenUrl: https://authenticate.trustpilot.com/oauth/token
  name: OAuth2
  source: openapi/trustpilot-product-reviews-openapi.yml
- flows:
  - authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize
    flow: authorizationCode
    tokenUrl: https://authenticate.trustpilot.com/oauth/token
  name: OAuth2
  source: openapi/trustpilot-service-reviews-openapi.yml
scope_count: 4
scope_names:
- business.invitations.manage
- business.product.review.manage
- business.review.manage
- business.review.read
scopes:
- description: Manage business invitations
  flows:
  - authorizationCode
  - clientCredentials
  scope: business.invitations.manage
- description: Manage product reviews
  flows:
  - authorizationCode
  scope: business.product.review.manage
- description: Manage business reviews
  flows:
  - authorizationCode
  scope: business.review.manage
- description: Read private review data
  flows:
  - authorizationCode
  scope: business.review.read
slug: trustpilot-scopes
source_filename: trustpilot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trustpilot-business-units-openapi.yml, openapi/trustpilot-invitation-openapi.yml,\n  openapi/trustpilot-product-reviews-openapi.yml, openapi/trustpilot-service-reviews-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/trustpilot-business-units-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize\n    tokenUrl: https://authenticate.trustpilot.com/oauth/token\n- name: OAuth2\n  source: openapi/trustpilot-invitation-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize\n    tokenUrl: https://authenticate.trustpilot.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://authenticate.trustpilot.com/oauth/token\n- name: OAuth2\n  source: openapi/trustpilot-product-reviews-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://authenticate.trustpilot.com/oauth/connect/authorize\n    tokenUrl: https://authenticate.trustpilot.com/oauth/token\n- name: OAuth2\n  source: openapi/trustpilot-service-reviews-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authenticate.trustpilot.com/oauth/connect/authorize\n    tokenUrl: https://authenticate.trustpilot.com/oauth/token\nscopes:\n- scope: business.invitations.manage\n  description: Manage business invitations\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/trustpilot-invitation-openapi.yml\n- scope: business.product.review.manage\n  description: Manage product reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trustpilot-product-reviews-openapi.yml\n- scope: business.review.manage\n  description: Manage business reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trustpilot-service-reviews-openapi.yml\n- scope: business.review.read\n  description: Read private review\
  \ data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trustpilot-business-units-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/scopes/trustpilot-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Consumer Reviews
- Reviews
- Trust
- Ratings
- Business Profiles
- Product Reviews
token_urls:
- https://authenticate.trustpilot.com/oauth/token
---
