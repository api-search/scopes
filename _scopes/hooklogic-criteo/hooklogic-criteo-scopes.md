---
api_specs:
- filename: hooklogic-criteo-accounts-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Accounts API
  slug: hooklogic-criteo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-accounts-api-openapi.yml
- filename: hooklogic-criteo-analytics-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Analytics API
  slug: hooklogic-criteo-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-analytics-api-openapi.yml
- filename: hooklogic-criteo-audience-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Audience API
  slug: hooklogic-criteo-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-audience-api-openapi.yml
- filename: hooklogic-criteo-balance-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Balance API
  slug: hooklogic-criteo-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-balance-api-openapi.yml
- filename: hooklogic-criteo-billing-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Billing API
  slug: hooklogic-criteo-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-billing-api-openapi.yml
- filename: hooklogic-criteo-campaign-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Campaign API
  slug: hooklogic-criteo-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-campaign-api-openapi.yml
- filename: hooklogic-criteo-catalog-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Catalog API
  slug: hooklogic-criteo-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-catalog-api-openapi.yml
- filename: hooklogic-criteo-gateway-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Gateway API
  slug: hooklogic-criteo-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-gateway-api-openapi.yml
authorization_urls:
- https://api.criteo.com/oauth2
description: ''
docs: https://developers.criteo.com/criteo-apis/docs/authorization-requests
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Hooklogic Criteo Scopes
name_suffix: OAuth Scopes
note: Scope strings below were derived from the Criteo Retail Media OpenAPI security requirements and then reconciled against the published authorization docs. Criteo does not publish a flat scope-reference table; it documents the same thing as a PERMISSION MODEL — an API application declares the "domains" it needs (Accounts, Analytics, Audience, Balance, Billing, Campaign, Catalog) at one of two permission levels, and an advertiser grants or denies them per account through the consent dashboard. The `<Domain>_Read` / `<Domain>_Manage` pairs in the spec are exactly that model expressed as OAuth2 scopes.
overview: 'HookLogic (Criteo) publishes 11 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the HookLogic (Criteo) API on a user''s behalf.


  Tokens are issued from https://api.criteo.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HookLogic (Criteo)
provider_slug: hooklogic-criteo
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  source: openapi/hooklogic-criteo-accounts-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  source: openapi/hooklogic-criteo-analytics-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  source: openapi/hooklogic-criteo-audience-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  source: openapi/hooklogic-criteo-balance-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  source: openapi/hooklogic-criteo-billing-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  source: openapi/hooklogic-criteo-campaign-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  source: openapi/hooklogic-criteo-catalog-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    tokenUrl: https://api.criteo.com/oauth2/token
  name: oauth
  source: openapi/hooklogic-criteo-gateway-api-openapi.yml
scope_count: 11
scope_names:
- RetailMedia_Accounts_Manage
- RetailMedia_Accounts_Read
- RetailMedia_Analytics_Read
- RetailMedia_Audience_Manage
- RetailMedia_Audience_Read
- RetailMedia_Balance_Manage
- RetailMedia_Balance_Read
- RetailMedia_Billing_Read
- RetailMedia_Campaign_Manage
- RetailMedia_Campaign_Read
- RetailMedia_Catalog_Manage
scopes:
- description: ''
  flows: []
  scope: RetailMedia_Accounts_Manage
- description: ''
  flows: []
  scope: RetailMedia_Accounts_Read
- description: ''
  flows: []
  scope: RetailMedia_Analytics_Read
- description: ''
  flows: []
  scope: RetailMedia_Audience_Manage
- description: ''
  flows: []
  scope: RetailMedia_Audience_Read
- description: ''
  flows: []
  scope: RetailMedia_Balance_Manage
- description: ''
  flows: []
  scope: RetailMedia_Balance_Read
- description: ''
  flows: []
  scope: RetailMedia_Billing_Read
- description: ''
  flows: []
  scope: RetailMedia_Campaign_Manage
- description: ''
  flows: []
  scope: RetailMedia_Campaign_Read
- description: ''
  flows: []
  scope: RetailMedia_Catalog_Manage
slug: hooklogic-criteo-scopes
source_filename: hooklogic-criteo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://developers.criteo.com/criteo-apis/docs/authorization-requests\nnote: >-\n  Scope strings below were derived from the Criteo Retail Media OpenAPI security\n  requirements and then reconciled against the published authorization docs.\n  Criteo does not publish a flat scope-reference table; it documents the same\n  thing as a PERMISSION MODEL — an API application declares the \"domains\" it\n  needs (Accounts, Analytics, Audience, Balance, Billing, Campaign, Catalog) at\n  one of two permission levels, and an advertiser grants or denies them per\n  account through the consent dashboard. The `<Domain>_Read` / `<Domain>_Manage`\n  pairs in the spec are exactly that model expressed as OAuth2 scopes.\npermission_model:\n  documented_at: https://developers.criteo.com/criteo-apis/docs/authorization-requests\n  levels:\n  - name: Read-only\n    scope_suffix: _Read\n    description: >-\n      View an advertiser's data or campaign\
  \ details without making changes —\n      e.g. an app that generates campaign reports.\n  - name: Manage\n    scope_suffix: _Manage\n    description: >-\n      Modify campaigns, ad sets, or ads — e.g. an app that automates CPC\n      settings or uploads a contact list.\n  consent:\n    dashboard: https://developers.criteo.com/criteo-apis/docs/consent-url-generation\n    granted_by: [Admin, Business Manager, Technical Manager]\n    revocable: true\n    note: >-\n      Consent is granted per portfolio/account. Revocation causes previously\n      working calls to return 403.\n  applies_to_flow: authorizationCode\n  client_credentials_note: >-\n    Client-credentials applications carry application-level scopes and are\n    limited to a single data owner; no advertiser consent step applies.\nsource: openapi/hooklogic-criteo-accounts-api-openapi.yml, openapi/hooklogic-criteo-analytics-api-openapi.yml,\n  openapi/hooklogic-criteo-audience-api-openapi.yml, openapi/hooklogic-criteo-balance-api-openapi.yml,\n\
  \  openapi/hooklogic-criteo-billing-api-openapi.yml, openapi/hooklogic-criteo-campaign-api-openapi.yml,\n  openapi/hooklogic-criteo-catalog-api-openapi.yml, openapi/hooklogic-criteo-gateway-api-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/hooklogic-criteo-accounts-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n- name: oauth\n  source: openapi/hooklogic-criteo-analytics-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n- name: oauth\n  source: openapi/hooklogic-criteo-audience-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n- name: oauth\n  source: openapi/hooklogic-criteo-balance-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n- name: oauth\n  source: openapi/hooklogic-criteo-billing-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n- name: oauth\n  source: openapi/hooklogic-criteo-campaign-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n\
  - name: oauth\n  source: openapi/hooklogic-criteo-catalog-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n- name: oauth\n  source: openapi/hooklogic-criteo-gateway-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\nscopes:\n- scope: RetailMedia_Accounts_Manage\n  sources:\n  - openapi/hooklogic-criteo-accounts-api-openapi.yml\n- scope: RetailMedia_Accounts_Read\n  sources:\n  - openapi/hooklogic-criteo-accounts-api-openapi.yml\n- scope: RetailMedia_Analytics_Read\n  sources:\n  - openapi/hooklogic-criteo-analytics-api-openapi.yml\n- scope: RetailMedia_Audience_Manage\n  sources:\n  - openapi/hooklogic-criteo-audience-api-openapi.yml\n\
  - scope: RetailMedia_Audience_Read\n  sources:\n  - openapi/hooklogic-criteo-audience-api-openapi.yml\n- scope: RetailMedia_Balance_Manage\n  sources:\n  - openapi/hooklogic-criteo-balance-api-openapi.yml\n- scope: RetailMedia_Balance_Read\n  sources:\n  - openapi/hooklogic-criteo-balance-api-openapi.yml\n- scope: RetailMedia_Billing_Read\n  sources:\n  - openapi/hooklogic-criteo-billing-api-openapi.yml\n- scope: RetailMedia_Campaign_Manage\n  sources:\n  - openapi/hooklogic-criteo-campaign-api-openapi.yml\n- scope: RetailMedia_Campaign_Read\n  sources:\n  - openapi/hooklogic-criteo-campaign-api-openapi.yml\n- scope: RetailMedia_Catalog_Manage\n  sources:\n  - openapi/hooklogic-criteo-catalog-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/scopes/hooklogic-criteo-scopes.yml
summary_line: 11 scopes · clientCredentials/authorizationCode
tags:
- Company
- Commerce
- Retail Media
- Advertising
- E-Commerce
- Marketing
- Retail
token_urls:
- https://api.criteo.com/oauth2/token
---
