---
api_specs:
- filename: attentive-v1-openapi.yaml
  format: yaml
  label: Attentive API
  slug: attentive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-v1-openapi.yaml
- filename: attentive-v2-openapi.yaml
  format: yaml
  label: Attentive API V2
  slug: attentive-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-v2-openapi.yaml
authorization_urls:
- https://ui-devel.attentivemobile.com/integrations/oauth-install?client_id={clientId}&redirect_uri={redirectUri}&scope={scope}
description: ''
docs: https://docs.attentive.com/docs/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Attentive Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Attentive publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Attentive API on a user''s behalf.


  Tokens are issued from https://api.attentivemobile.com/v1/authorization-codes/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Attentive
provider_slug: attentive
schemes:
- description: This API uses OAuth 2 with the authorization code grant flow. [More info](https://docs.attentivemobile.com/pages/authentication/)
  flows:
  - authorizationUrl: https://ui-devel.attentivemobile.com/integrations/oauth-install?client_id={clientId}&redirect_uri={redirectUri}&scope={scope}
    flow: authorizationCode
    tokenUrl: https://api.attentivemobile.com/v1/authorization-codes/tokens
  name: OAuthFlow
  source: openapi/attentive-v1-openapi.yaml
- description: This API uses OAuth 2 with the authorization code grant flow. [More info](https://docs.attentivemobile.com/pages/authentication/)
  flows:
  - authorizationUrl: https://ui-devel.attentivemobile.com/integrations/oauth-install?client_id={clientId}&redirect_uri={redirectUri}&scope={scope}
    flow: authorizationCode
    tokenUrl: https://api.attentivemobile.com/v1/authorization-codes/tokens
  name: OAuthFlow
  source: openapi/attentive-v2-openapi.yaml
scope_count: 14
scope_names:
- attributes:write
- ecommerce:write
- events:write
- identity:write
- offers:write
- privacy_requests:read
- privacy_requests:write
- product_catalogs:read
- product_catalogs:write
- segments:read
- segments:write
- subscriptions:read
- subscriptions:write
- webhooks:write
scopes:
- description: read and write custom attributes
  flows:
  - authorizationCode
  scope: attributes:write
- description: read and write ecommerce events
  flows:
  - authorizationCode
  scope: ecommerce:write
- description: read and write custom events
  flows:
  - authorizationCode
  scope: events:write
- description: read and write identity resolution (client/custom user identifiers)
  flows: []
  scope: identity:write
- description: read and write offers / coupon-pool discount codes
  flows: []
  scope: offers:write
- description: read privacy (CCPA) deletion requests
  flows: []
  scope: privacy_requests:read
- description: create privacy (CCPA) deletion requests
  flows: []
  scope: privacy_requests:write
- description: read product catalog uploads
  flows: []
  scope: product_catalogs:read
- description: upload and manage the product catalog
  flows: []
  scope: product_catalogs:write
- description: read segments
  flows:
  - authorizationCode
  scope: segments:read
- description: read and write segments
  flows:
  - authorizationCode
  scope: segments:write
- description: read subscriptions and subscription eligibility
  flows: []
  scope: subscriptions:read
- description: read and write subscriptions
  flows:
  - authorizationCode
  scope: subscriptions:write
- description: create and manage webhook subscriptions
  flows: []
  scope: webhooks:write
slug: attentive-scopes
source_filename: attentive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/attentive-v1-openapi.yaml, openapi/attentive-v2-openapi.yaml\ndocs: https://docs.attentive.com/docs/authentication\nschemes:\n- name: OAuthFlow\n  source: openapi/attentive-v1-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ui-devel.attentivemobile.com/integrations/oauth-install?client_id={clientId}&redirect_uri={redirectUri}&scope={scope}\n    tokenUrl: https://api.attentivemobile.com/v1/authorization-codes/tokens\n  description: This API uses OAuth 2 with the authorization code grant flow. [More\n    info](https://docs.attentivemobile.com/pages/authentication/)\n- name: OAuthFlow\n  source: openapi/attentive-v2-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ui-devel.attentivemobile.com/integrations/oauth-install?client_id={clientId}&redirect_uri={redirectUri}&scope={scope}\n    tokenUrl: https://api.attentivemobile.com/v1/authorization-codes/tokens\n\
  \  description: This API uses OAuth 2 with the authorization code grant flow. [More\n    info](https://docs.attentivemobile.com/pages/authentication/)\nscopes:\n- scope: attributes:write\n  description: read and write custom attributes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\n- scope: ecommerce:write\n  description: read and write ecommerce events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\n- scope: events:write\n  description: read and write custom events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\n- scope: identity:write\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  description: read and write identity resolution (client/custom user identifiers)\n- scope: offers:write\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  description: read\
  \ and write offers / coupon-pool discount codes\n- scope: privacy_requests:read\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  description: read privacy (CCPA) deletion requests\n- scope: privacy_requests:write\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  description: create privacy (CCPA) deletion requests\n- scope: product_catalogs:read\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  description: read product catalog uploads\n- scope: product_catalogs:write\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  description: upload and manage the product catalog\n- scope: segments:read\n  description: read segments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\n- scope: segments:write\n  description: read and write segments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\n- scope: subscriptions:read\n  sources:\n \
  \ - openapi/attentive-v1-openapi.yaml\n  description: read subscriptions and subscription eligibility\n- scope: subscriptions:write\n  description: read and write subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\n- scope: webhooks:write\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  description: create and manage webhook subscriptions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/scopes/attentive-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Company
- Martech
- SMS Marketing
- Email Marketing
- Ecommerce
- Marketing Automation
- Subscribers
- Webhooks
- Customer Engagement
token_urls:
- https://api.attentivemobile.com/v1/authorization-codes/tokens
---
