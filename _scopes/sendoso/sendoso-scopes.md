---
api_specs:
- filename: sendoso-core-api-openapi.yml
  format: yaml
  label: Sendoso Core API
  slug: sendoso-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/openapi/sendoso-core-api-openapi.yml
- filename: sendoso-marketplace-api-openapi.yml
  format: yaml
  label: Sendoso Marketplace and SmartSend API
  slug: sendoso-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/openapi/sendoso-marketplace-api-openapi.yml
- filename: sendoso-scim-api-openapi.yml
  format: yaml
  label: Sendoso SCIM API
  slug: sendoso-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/openapi/sendoso-scim-api-openapi.yml
- filename: sendoso-webhooks-asyncapi.yml
  format: yaml
  label: Sendoso Webhooks
  slug: sendoso-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/asyncapi/sendoso-webhooks-asyncapi.yml
authorization_urls:
- https://app.sendoso.com/oauth/authorize
description: ''
docs:
- https://developer.sendoso.com/rest-api/overview/authentication
- https://developer.sendoso.com/marketplace/overview/authentication
- https://developer.sendoso.com/scim/overview/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sendoso Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sendoso publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sendoso API on a user''s behalf.


  Tokens are issued from https://app.sendoso.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sendoso
provider_slug: sendoso
schemes:
- description: 'OAuth 2.0 Authorization Code grant. Register your application by contacting developers@sendoso.com to receive a client ID and client secret. Access tokens live 7200 seconds (2 hours) and are refreshed at the same token endpoint. Tokens are sent as `Authorization: Bearer <token>`.'
  flows:
  - authorizationUrl: https://app.sendoso.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.sendoso.com/oauth/token
  name: OAuth2
  source: openapi/sendoso-core-api-openapi.yml
- description: OAuth 2.0 Authorization Code grant, same authorization server as the Core API. Marketplace operations require the `marketplace` scope; SmartSend operations require `smartsend`.
  flows:
  - authorizationUrl: https://app.sendoso.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.sendoso.com/oauth/token
  name: OAuth2
  source: openapi/sendoso-marketplace-api-openapi.yml
- description: OAuth 2.0 Authorization Code grant with `scope=scim`. SCIM requires a client id and secret specific to the SCIM API, obtained from developers@sendoso.com; Core API credentials do not work here.
  flows:
  - authorizationUrl: https://app.sendoso.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.sendoso.com/oauth/token
  name: OAuth2
  source: openapi/sendoso-scim-api-openapi.yml
scope_count: 6
scope_names:
- marketplace
- public
- scim
- smartsend
- update
- write
scopes:
- description: Access the marketplace API.
  flows:
  - authorizationCode
  scope: marketplace
- description: Access the user's basic information.
  flows:
  - authorizationCode
  scope: public
- description: Access the SCIM API.
  flows:
  - authorizationCode
  scope: scim
- description: Access the smartsend API.
  flows:
  - authorizationCode
  scope: smartsend
- description: Update the user's account details.
  flows:
  - authorizationCode
  scope: update
- description: Send gifts on the user's behalf.
  flows:
  - authorizationCode
  scope: write
slug: sendoso-scopes
source_filename: sendoso-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.sendoso.com/rest-api/overview/authentication\ndocs:\n  - https://developer.sendoso.com/rest-api/overview/authentication\n  - https://developer.sendoso.com/marketplace/overview/authentication\n  - https://developer.sendoso.com/scim/overview/authentication\nderived_from:\n  - openapi/sendoso-core-api-openapi.yml\n  - openapi/sendoso-marketplace-api-openapi.yml\n  - openapi/sendoso-scim-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/sendoso-core-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.sendoso.com/oauth/authorize\n    tokenUrl: https://app.sendoso.com/oauth/token\n  description: 'OAuth 2.0 Authorization Code grant. Register your application by contacting\n    developers@sendoso.com to receive a client ID and client secret. Access tokens live 7200\n    seconds (2 hours) and are refreshed at the same token endpoint. Tokens are sent as `Authorization:\n\
  \    Bearer <token>`.'\n- name: OAuth2\n  source: openapi/sendoso-marketplace-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.sendoso.com/oauth/authorize\n    tokenUrl: https://app.sendoso.com/oauth/token\n  description: OAuth 2.0 Authorization Code grant, same authorization server as the Core API.\n    Marketplace operations require the `marketplace` scope; SmartSend operations require `smartsend`.\n- name: OAuth2\n  source: openapi/sendoso-scim-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.sendoso.com/oauth/authorize\n    tokenUrl: https://app.sendoso.com/oauth/token\n  description: OAuth 2.0 Authorization Code grant with `scope=scim`. SCIM requires a client\n    id and secret specific to the SCIM API, obtained from developers@sendoso.com; Core API credentials\n    do not work here.\nscopes:\n- scope: marketplace\n  description: Access the marketplace API.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/sendoso-core-api-openapi.yml\n  - openapi/sendoso-marketplace-api-openapi.yml\n- scope: public\n  description: Access the user's basic information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sendoso-core-api-openapi.yml\n  - openapi/sendoso-marketplace-api-openapi.yml\n- scope: scim\n  description: Access the SCIM API.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sendoso-scim-api-openapi.yml\n- scope: smartsend\n  description: Access the smartsend API.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sendoso-core-api-openapi.yml\n  - openapi/sendoso-marketplace-api-openapi.yml\n- scope: update\n  description: Update the user's account details.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sendoso-core-api-openapi.yml\n  - openapi/sendoso-marketplace-api-openapi.yml\n- scope: write\n  description: Send gifts on the user's behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sendoso-core-api-openapi.yml\n  - openapi/sendoso-marketplace-api-openapi.yml\n\
  request_format: >-\n  Scopes are requested as a space-separated list in the `scope` parameter of the authorization\n  request, e.g. `scope=write update`. Sendoso notes the user must grant each scope\n  individually.\noperation_requirements:\n  - scope: marketplace\n    operations: [getMarketplaceProducts, sendMarketplaceProduct]\n    source: https://developer.sendoso.com/marketplace/reference/products/get-products\n  - scope: smartsend\n    operations: [getGiftRecommendations, sendRecommendation, sendMarketplaceProduct]\n    source: https://developer.sendoso.com/marketplace/reference/recommendations/get-recommendations\n    note: sendMarketplaceProduct accepts either `marketplace` or `smartsend`.\n  - scope: scim\n    operations: [scimGetUsers, scimCreateUser, scimUpdateUser]\n    source: https://developer.sendoso.com/scim/overview/authentication\nmcp_scopes:\n  resource: https://app.sendoso.com/mcp\n  source: https://app.sendoso.com/.well-known/oauth-authorization-server/mcp\n  scopes_supported:\
  \ [openid, profile, email, offline_access]\n  note: >-\n    The MCP server's authorization server advertises OIDC scopes only — none of the\n    developer-API scopes (public/write/update/marketplace/smartsend/scim) appear in its\n    metadata, so MCP authorization is coarse-grained relative to the REST API.\ngaps:\n  - >-\n    Sendoso publishes no per-operation scope table for the Core API. The five Core scopes are\n    described in prose only (\"write: allows your application to send gifts on the user's\n    behalf\"), so which scope each Core operation actually requires is not documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/scopes/sendoso-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Corporate Gifting
- Direct Mail
- Sales Engagement
- Marketing Automation
- CRM Integration
- eGifts
- Swag and Merchandise
- Fulfillment
- Employee Recognition
- Account Based Marketing
- SCIM Provisioning
- Webhook
token_urls:
- https://app.sendoso.com/oauth/token
---
