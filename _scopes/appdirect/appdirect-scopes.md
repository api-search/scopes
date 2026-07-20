---
api_specs:
- filename: appdirect-companies-openapi-original.yml
  format: yaml
  label: AppDirect Companies / Marketplace API
  slug: appdirect-companies-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdirect/refs/heads/main/openapi/appdirect-companies-openapi-original.yml
- filename: appdirect-devsai-openapi-original.json
  format: json
  label: AppDirect Devs.ai API
  slug: appdirect-devsai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdirect/refs/heads/main/openapi/appdirect-devsai-openapi-original.json
authorization_urls:
- https://{marketplaceURL}/oauth2/authorize
description: ''
docs: https://developer.appdirect.com/user-guides/api-usage/api-auth/scopes
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Appdirect Scopes
name_suffix: OAuth Scopes
note: AppDirect OAuth 2.0 scopes correspond to marketplace user roles. Role scopes are used with the Authorization Code / Implicit / Password grant types (user-level); the ROLE_PARTNER_READ / ROLE_PARTNER scopes are used with the Client Credentials grant (system-level). openid/profile/email are OIDC scopes.
overview: 'AppDirect publishes 15 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AppDirect API on a user''s behalf.


  Tokens are issued from https://{marketplaceURL}/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AppDirect
provider_slug: appdirect
schemes:
- flows:
  - authorizationUrl: https://{marketplaceURL}/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://{marketplaceURL}/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://{marketplaceURL}/oauth2/token
  name: OAuth2
  source: https://developer.appdirect.com/user-guides/api-usage/api-auth
scope_count: 15
scope_names:
- ROLE_USER
- ROLE_BILLING_ADMIN
- ROLE_SYS_ADMIN
- ROLE_RESELLER
- ROLE_SALES_SUPPORT
- ROLE_CHANNEL_SUPPORT
- ROLE_CHANNEL_PRODUCT_SUPPORT
- ROLE_CHANNEL_ADMIN
- ROLE_CORPORATE_ADMIN
- ROLE_DEVELOPER
- ROLE_PARTNER_READ
- ROLE_PARTNER
- openid
- profile
- email
scopes:
- description: Allows access as an end user in the company associated with an API call.
  flows: []
  scope: ROLE_USER
- description: Allows access as a Billing Admin for the company associated with an API call.
  flows: []
  scope: ROLE_BILLING_ADMIN
- description: Allows access as a Company Admin for the company associated with an API call.
  flows: []
  scope: ROLE_SYS_ADMIN
- description: Allows access as a Reseller for the company associated with an API call.
  flows: []
  scope: ROLE_RESELLER
- description: Allows access as a Sales Support agent for the marketplace.
  flows: []
  scope: ROLE_SALES_SUPPORT
- description: Allows access as a Customer Support agent for the marketplace.
  flows: []
  scope: ROLE_CHANNEL_SUPPORT
- description: Allows access as a Product Support agent for the marketplace.
  flows: []
  scope: ROLE_CHANNEL_PRODUCT_SUPPORT
- description: Allows access as a Marketplace Manager for the marketplace.
  flows: []
  scope: ROLE_CHANNEL_ADMIN
- description: Allows access as a Network Manager for the marketplace.
  flows: []
  scope: ROLE_CORPORATE_ADMIN
- description: Allows access as a Developer for the user associated with an API call.
  flows: []
  scope: ROLE_DEVELOPER
- description: Allows access to read all marketplace data.
  flows: []
  scope: ROLE_PARTNER_READ
- description: Allows access to read and write all marketplace data.
  flows: []
  scope: ROLE_PARTNER
- description: Requests that the ID token be returned from the token endpoint for SSO (OIDC).
  flows: []
  scope: openid
- description: API client can retrieve user profile information like name (OIDC).
  flows: []
  scope: profile
- description: API client can retrieve a user's email address (OIDC).
  flows: []
  scope: email
slug: appdirect-scopes
source_filename: appdirect-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developer.appdirect.com/user-guides/api-usage/api-auth/scopes\ndocs: https://developer.appdirect.com/user-guides/api-usage/api-auth/scopes\nnote: >-\n  AppDirect OAuth 2.0 scopes correspond to marketplace user roles. Role scopes are\n  used with the Authorization Code / Implicit / Password grant types (user-level);\n  the ROLE_PARTNER_READ / ROLE_PARTNER scopes are used with the Client Credentials\n  grant (system-level). openid/profile/email are OIDC scopes.\nschemes:\n- name: OAuth2\n  source: https://developer.appdirect.com/user-guides/api-usage/api-auth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{marketplaceURL}/oauth2/authorize\n    tokenUrl: https://{marketplaceURL}/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://{marketplaceURL}/oauth2/token\nscopes:\n- scope: ROLE_USER\n  description: Allows access as an end user in the company associated with an API call.\n  grant_types:\
  \ [authorizationCode, implicit, password]\n- scope: ROLE_BILLING_ADMIN\n  description: Allows access as a Billing Admin for the company associated with an API call.\n  grant_types: [authorizationCode, implicit, password]\n- scope: ROLE_SYS_ADMIN\n  description: Allows access as a Company Admin for the company associated with an API call.\n  grant_types: [authorizationCode, implicit, password]\n- scope: ROLE_RESELLER\n  description: Allows access as a Reseller for the company associated with an API call.\n  grant_types: [authorizationCode, implicit, password]\n- scope: ROLE_SALES_SUPPORT\n  description: Allows access as a Sales Support agent for the marketplace.\n  grant_types: [authorizationCode, implicit, password]\n- scope: ROLE_CHANNEL_SUPPORT\n  description: Allows access as a Customer Support agent for the marketplace.\n  grant_types: [authorizationCode, implicit, password]\n- scope: ROLE_CHANNEL_PRODUCT_SUPPORT\n  description: Allows access as a Product Support agent for the marketplace.\n\
  \  grant_types: [authorizationCode, implicit, password]\n- scope: ROLE_CHANNEL_ADMIN\n  description: Allows access as a Marketplace Manager for the marketplace.\n  grant_types: [authorizationCode, implicit, password]\n- scope: ROLE_CORPORATE_ADMIN\n  description: Allows access as a Network Manager for the marketplace.\n  grant_types: [authorizationCode, implicit, password]\n- scope: ROLE_DEVELOPER\n  description: Allows access as a Developer for the user associated with an API call.\n  grant_types: [authorizationCode, implicit, password]\n- scope: ROLE_PARTNER_READ\n  description: Allows access to read all marketplace data.\n  grant_types: [clientCredentials]\n- scope: ROLE_PARTNER\n  description: Allows access to read and write all marketplace data.\n  grant_types: [clientCredentials]\n- scope: openid\n  description: Requests that the ID token be returned from the token endpoint for SSO (OIDC).\n  grant_types: [authorizationCode, implicit, password]\n- scope: profile\n  description: API\
  \ client can retrieve user profile information like name (OIDC).\n  grant_types: [authorizationCode, implicit, password]\n- scope: email\n  description: API client can retrieve a user's email address (OIDC).\n  grant_types: [authorizationCode, implicit, password]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appdirect/refs/heads/main/scopes/appdirect-scopes.yml
summary_line: 15 scopes · authorizationCode/clientCredentials
tags:
- Company
- Commerce
- Subscription Commerce
- Marketplace
- Billing
- Reseller
- Cloud Distribution
- Webhooks
- OAuth
token_urls:
- https://{marketplaceURL}/oauth2/token
---
