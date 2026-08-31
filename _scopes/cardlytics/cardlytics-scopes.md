---
api_specs:
- filename: cardlytics-adgroups-api-openapi.yml
  format: yaml
  label: Cardlytics Ad Groups API
  slug: cardlytics-adgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-adgroups-api-openapi.yml
- filename: cardlytics-ads-api-openapi.yml
  format: yaml
  label: Cardlytics Ads API
  slug: cardlytics-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-ads-api-openapi.yml
- filename: cardlytics-ads-controller-api-openapi.yml
  format: yaml
  label: Cardlytics Ads Controller API
  slug: cardlytics-ads-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-ads-controller-api-openapi.yml
- filename: cardlytics-audiencereach-api-openapi.yml
  format: yaml
  label: Cardlytics Audience Reach API
  slug: cardlytics-audiencereach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-audiencereach-api-openapi.yml
- filename: cardlytics-audiences-api-openapi.yml
  format: yaml
  label: Cardlytics Audiences API
  slug: cardlytics-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-audiences-api-openapi.yml
- filename: cardlytics-auditlogs-api-openapi.yml
  format: yaml
  label: Cardlytics Audit Logs API
  slug: cardlytics-auditlogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-auditlogs-api-openapi.yml
- filename: cardlytics-authentication-api-openapi.yml
  format: yaml
  label: Cardlytics Authentication API
  slug: cardlytics-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-authentication-api-openapi.yml
- filename: cardlytics-campaigns-api-openapi.yml
  format: yaml
  label: Cardlytics Campaigns API
  slug: cardlytics-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-campaigns-api-openapi.yml
- filename: cardlytics-customer-controller-api-openapi.yml
  format: yaml
  label: Cardlytics Customer Controller API
  slug: cardlytics-customer-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-customer-controller-api-openapi.yml
- filename: cardlytics-geo-api-openapi.yml
  format: yaml
  label: Cardlytics Geo API
  slug: cardlytics-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-geo-api-openapi.yml
- filename: cardlytics-merchants-api-openapi.yml
  format: yaml
  label: Cardlytics Merchants API
  slug: cardlytics-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-merchants-api-openapi.yml
- filename: cardlytics-offers-api-openapi.yml
  format: yaml
  label: Cardlytics Offers API
  slug: cardlytics-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-offers-api-openapi.yml
- filename: cardlytics-pricingmodels-api-openapi.yml
  format: yaml
  label: Cardlytics Pricing Models API
  slug: cardlytics-pricingmodels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-pricingmodels-api-openapi.yml
- filename: cardlytics-purchasecategories-api-openapi.yml
  format: yaml
  label: Cardlytics Purchase Categories API
  slug: cardlytics-purchasecategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-purchasecategories-api-openapi.yml
- filename: cardlytics-redemptions-api-openapi.yml
  format: yaml
  label: Cardlytics Redemptions API
  slug: cardlytics-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-redemptions-api-openapi.yml
- filename: cardlytics-reports-api-openapi.yml
  format: yaml
  label: Cardlytics Reports API
  slug: cardlytics-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-reports-api-openapi.yml
- filename: cardlytics-rewards-api-openapi.yml
  format: yaml
  label: Cardlytics Rewards API
  slug: cardlytics-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-rewards-api-openapi.yml
- filename: cardlytics-session-controller-api-openapi.yml
  format: yaml
  label: Cardlytics Session Controller API
  slug: cardlytics-session-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-session-controller-api-openapi.yml
authorization_urls:
- https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/authorize
description: ''
docs: https://docs.cardlytics.com/ads/v2/getting-started/get-session-token.html
flows:
- clientCredentials
- authorizationCode
- custom
kind: oauth-scopes
layout: scope
method: searched
name: Cardlytics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cardlytics publishes 4 OAuth 2.0 scopes via the clientCredentials, authorizationCode, and custom flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cardlytics API on a user''s behalf.


  Tokens are issued from /v1/idp/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cardlytics
provider_slug: cardlytics
schemes:
- api: Partner API
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/idp/oauth2/token
  name: oauth2
  source: openapi/cardlytics-partner-api-openapi.yml
- api: Campaign Build API
  flows:
  - authorizationUrl: https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/token
  name: oauth2-cognito
  source: openapi/cardlytics-campaign-build-api-openapi.yml
- api: Publisher API v2
  flows:
  - flow: custom
    note: POST a JSON body with scopes[] (plus sourceCustomerId for customer-level scopes); the response returns a sessionToken sent on later calls as the X-CDLX-Session-Token header.
    tokenUrl: /v2/session/startSession
  name: session-token
  source: https://docs.cardlytics.com/ads/v2/getting-started/get-session-token.html
scope_count: 4
scope_names:
- openid
- read
- api:institution
- api:customer
scopes:
- description: openid
  flows:
  - authorizationCode
  - clientCredentials
  scope: openid
- description: Declared on Campaign Build API operation security requirements.
  flows: []
  scope: read
- description: Institution-level access. Create or update the institution's customer, account and card data, and send Cardlytics transaction information. Used for server-side Data API onboarding; no customer context required.
  flows:
  - custom
  scope: api:institution
- description: Customer-level access, on behalf of one end customer. Requires a sourceCustomerId on the startSession request. Grants targeted ad access, customer profile reads, and event logging for that customer's session.
  flows:
  - custom
  scope: api:customer
slug: cardlytics-scopes
source_filename: cardlytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/cardlytics-campaign-build-api-openapi.yml, openapi/cardlytics-partner-api-openapi.yml\ndocs: https://docs.cardlytics.com/ads/v2/getting-started/get-session-token.html\nnotes: >-\n  Two scope vocabularies exist and they are unrelated. The OpenAPI-declared\n  OAuth 2.0 schemes (partner API, campaign build API) declare only `openid`,\n  which is an OIDC marker rather than a permission model — Cardlytics states\n  that \"API scopes\" exist as an authorization control for partners but does not\n  publish their names. The Publisher API v2 session token carries a genuine,\n  documented two-scope model (api:institution, api:customer) requested in the\n  startSession body and encoded into a `scope` claim.\nschemes:\n- name: oauth2\n  source: openapi/cardlytics-partner-api-openapi.yml\n  api: Partner API\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/idp/oauth2/token\n- name: oauth2-cognito\n  source: openapi/cardlytics-campaign-build-api-openapi.yml\n\
  \  api: Campaign Build API\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/token\n- name: session-token\n  source: https://docs.cardlytics.com/ads/v2/getting-started/get-session-token.html\n  api: Publisher API v2\n  flows:\n  - flow: custom\n    tokenUrl: /v2/session/startSession\n    note: >-\n      POST a JSON body with scopes[] (plus sourceCustomerId for customer-level\n      scopes); the response returns a sessionToken sent on later calls as the\n      X-CDLX-Session-Token header.\nscopes:\n- scope: openid\n  description: openid\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cardlytics-campaign-build-api-openapi.yml\n  - openapi/cardlytics-partner-api-openapi.yml\n- scope: read\n  description: Declared on Campaign Build API operation security requirements.\n  sources:\n\
  \  - openapi/cardlytics-campaign-build-api-openapi.yml\n- scope: api:institution\n  description: >-\n    Institution-level access. Create or update the institution's customer,\n    account and card data, and send Cardlytics transaction information. Used for\n    server-side Data API onboarding; no customer context required.\n  apis:\n  - Data APIs\n  flows:\n  - custom\n  sources:\n  - https://docs.cardlytics.com/ads/v2/getting-started/get-session-token.html\n- scope: api:customer\n  description: >-\n    Customer-level access, on behalf of one end customer. Requires a\n    sourceCustomerId on the startSession request. Grants targeted ad access,\n    customer profile reads, and event logging for that customer's session.\n  apis:\n  - Ads\n  - Customer Profile APIs\n  - Events APIs\n  flows:\n  - custom\n  sources:\n  - https://docs.cardlytics.com/ads/v2/getting-started/get-session-token.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/scopes/cardlytics-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode/custom
tags:
- Company
- Advertising
- Commerce Media
- Card-Linked Offers
- Purchase Intelligence
- Financial-Services
- Loyalty and Rewards
- Marketing
- Banking
- Retail Media
- Attribution
- Offers
token_urls:
- /v1/idp/oauth2/token
- https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/token
- /v2/session/startSession
---
