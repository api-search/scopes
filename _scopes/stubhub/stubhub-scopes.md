---
api_specs:
- filename: stubhub-account-openapi.yml
  format: yaml
  label: StubHub Account API
  slug: stubhub-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-account-openapi.yml
- filename: stubhub-catalog-openapi.yml
  format: yaml
  label: StubHub Catalog API
  slug: stubhub-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-catalog-openapi.yml
- filename: stubhub-inventory-openapi.yml
  format: yaml
  label: StubHub Inventory API
  slug: stubhub-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-inventory-openapi.yml
- filename: stubhub-sales-openapi.yml
  format: yaml
  label: StubHub Sales API
  slug: stubhub-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-sales-openapi.yml
- filename: stubhub-webhooks-openapi.yml
  format: yaml
  label: StubHub Webhooks API
  slug: stubhub-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/openapi/stubhub-webhooks-openapi.yml
authorization_urls:
- https://account.stubhub.com/authorize
description: ''
docs: https://developer.stubhub.com/docs/authentication/scopes
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Stubhub Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'StubHub publishes 9 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the StubHub API on a user''s behalf.


  Tokens are issued from https://account.stubhub.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: StubHub
provider_slug: stubhub
schemes:
- description: OAuth2. All API requests must be authenticated.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.stubhub.com/oauth2/token
  - authorizationUrl: https://account.stubhub.com/authorize
    flow: authorizationCode
    tokenUrl: https://account.stubhub.com/oauth2/token
  name: oauth2
  source: openapi/stubhub-account-openapi.yml
- description: OAuth2. All API requests must be authenticated.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.stubhub.com/oauth2/token
  - authorizationUrl: https://account.stubhub.com/authorize
    flow: authorizationCode
    tokenUrl: https://account.stubhub.com/oauth2/token
  name: oauth2
  source: openapi/stubhub-catalog-openapi.yml
- description: OAuth2. All API requests must be authenticated.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.stubhub.com/oauth2/token
  - authorizationUrl: https://account.stubhub.com/authorize
    flow: authorizationCode
    tokenUrl: https://account.stubhub.com/oauth2/token
  name: oauth2
  source: openapi/stubhub-inventory-openapi.yml
- description: OAuth2. All API requests must be authenticated.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.stubhub.com/oauth2/token
  - authorizationUrl: https://account.stubhub.com/authorize
    flow: authorizationCode
    tokenUrl: https://account.stubhub.com/oauth2/token
  name: oauth2
  source: openapi/stubhub-sales-openapi.yml
- description: OAuth2. All API requests must be authenticated.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.stubhub.com/oauth2/token
  - authorizationUrl: https://account.stubhub.com/authorize
    flow: authorizationCode
    tokenUrl: https://account.stubhub.com/oauth2/token
  name: oauth2
  source: openapi/stubhub-webhooks-openapi.yml
scope_count: 9
scope_names:
- read:events
- read:payment
- read:sales
- read:sellerlistings
- read:webhooks
- write:requestedevents
- write:sales
- write:sellerlistings
- write:webhooks
scopes:
- description: Read-only access to events on the StubHub platform.
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:events
- description: Read-only access to the user's payments.
  flows:
  - authorizationCode
  scope: read:payment
- description: Read access to the user's sales.
  flows:
  - authorizationCode
  scope: read:sales
- description: Read access to the user's listings.
  flows:
  - authorizationCode
  scope: read:sellerlistings
- description: Read access to the user's webhooks.
  flows:
  - authorizationCode
  scope: read:webhooks
- description: Write access to the user's requested events.
  flows:
  - authorizationCode
  scope: write:requestedevents
- description: Write access to the user's sales (confirm and fulfill sales).
  flows:
  - authorizationCode
  scope: write:sales
- description: Write access to the user's listings (create and update listings).
  flows:
  - authorizationCode
  scope: write:sellerlistings
- description: Write access to the user's webhooks.
  flows:
  - authorizationCode
  scope: write:webhooks
slug: stubhub-scopes
source_filename: stubhub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/stubhub-account-openapi.yml, openapi/stubhub-catalog-openapi.yml, openapi/stubhub-inventory-openapi.yml, openapi/stubhub-sales-openapi.yml,\n  openapi/stubhub-webhooks-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/stubhub-account-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.stubhub.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://account.stubhub.com/authorize\n    tokenUrl: https://account.stubhub.com/oauth2/token\n  description: OAuth2. All API requests must be authenticated.\n- name: oauth2\n  source: openapi/stubhub-catalog-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.stubhub.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://account.stubhub.com/authorize\n    tokenUrl: https://account.stubhub.com/oauth2/token\n  description: OAuth2. All API requests must be authenticated.\n-\
  \ name: oauth2\n  source: openapi/stubhub-inventory-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.stubhub.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://account.stubhub.com/authorize\n    tokenUrl: https://account.stubhub.com/oauth2/token\n  description: OAuth2. All API requests must be authenticated.\n- name: oauth2\n  source: openapi/stubhub-sales-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.stubhub.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://account.stubhub.com/authorize\n    tokenUrl: https://account.stubhub.com/oauth2/token\n  description: OAuth2. All API requests must be authenticated.\n- name: oauth2\n  source: openapi/stubhub-webhooks-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.stubhub.com/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://account.stubhub.com/authorize\n    tokenUrl: https://account.stubhub.com/oauth2/token\n\
  \  description: OAuth2. All API requests must be authenticated.\nscopes:\n- scope: read:events\n  description: Read-only access to events on the StubHub platform.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n  - openapi/stubhub-inventory-openapi.yml\n  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\n- scope: read:payment\n  description: Read-only access to the user's payments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n  - openapi/stubhub-inventory-openapi.yml\n  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\n- scope: read:sales\n  description: Read access to the user's sales.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n  - openapi/stubhub-inventory-openapi.yml\n\
  \  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\n- scope: read:sellerlistings\n  description: Read access to the user's listings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n  - openapi/stubhub-inventory-openapi.yml\n  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\n- scope: read:webhooks\n  description: Read access to the user's webhooks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n  - openapi/stubhub-inventory-openapi.yml\n  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\n- scope: write:requestedevents\n  description: Write access to the user's requested events.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n  - openapi/stubhub-inventory-openapi.yml\n\
  \  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\n- scope: write:sales\n  description: Write access to the user's sales (confirm and fulfill sales).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n  - openapi/stubhub-inventory-openapi.yml\n  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\n- scope: write:sellerlistings\n  description: Write access to the user's listings (create and update listings).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n  - openapi/stubhub-inventory-openapi.yml\n  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\n- scope: write:webhooks\n  description: Write access to the user's webhooks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stubhub-account-openapi.yml\n  - openapi/stubhub-catalog-openapi.yml\n\
  \  - openapi/stubhub-inventory-openapi.yml\n  - openapi/stubhub-sales-openapi.yml\n  - openapi/stubhub-webhooks-openapi.yml\ndocs: https://developer.stubhub.com/docs/authentication/scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stubhub/refs/heads/main/scopes/stubhub-scopes.yml
summary_line: 9 scopes · clientCredentials/authorizationCode
tags:
- Company
- Marketplaces
- Tickets
- Events
- Ticketing
- Live Events
- Secondary Market
- E-commerce
- Sports
- Concerts
token_urls:
- https://account.stubhub.com/oauth2/token
---
