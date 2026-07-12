---
authorization_urls: []
description: ''
docs: https://developers.deliverect.com/docs/getting-started
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Deliverect Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Deliverect publishes 7 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deliverect API on a user''s behalf.


  Tokens are issued from https://api.deliverect.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deliverect
provider_slug: deliverect
schemes:
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-channel-api-openapi-original.yml
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-commerce-api-openapi-original.yml
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-crm-api-openapi-original.yml
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-dispatch-api-openapi-original.yml
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-gift-cards-api-openapi-original.yml
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-kds-api-openapi-original.yml
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-loyalty-api-openapi-original.yml
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-pay-api-openapi-original.yml
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-pos-api-openapi-original.yml
- description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret at POST /oauth/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.deliverect.com/oauth/token
  name: oauth2
  source: openapi/deliverect-store-api-openapi-original.yml
scope_count: 7
scope_names:
- genericChannel:{channel_scope}
- genericPOS
- store
- genericFulfillment
- genericKDS
- payments
- genericCommerce
scopes:
- description: All endpoints within the Channel API.
  flows: []
  scope: genericChannel:{channel_scope}
- description: All endpoints within the POS + Store API.
  flows: []
  scope: genericPOS
- description: All endpoints within the Store API.
  flows: []
  scope: store
- description: All endpoints within the Dispatch API.
  flows: []
  scope: genericFulfillment
- description: All endpoints within the KDS API.
  flows: []
  scope: genericKDS
- description: All endpoints within the DPAY (Pay) API.
  flows: []
  scope: payments
- description: All endpoints within the Commerce API.
  flows: []
  scope: genericCommerce
slug: deliverect-scopes
source_filename: deliverect-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://developers.deliverect.com/docs/getting-started\nsource: openapi/deliverect-channel-api-openapi-original.yml, openapi/deliverect-commerce-api-openapi-original.yml,\n  openapi/deliverect-crm-api-openapi-original.yml, openapi/deliverect-dispatch-api-openapi-original.yml,\n  openapi/deliverect-gift-cards-api-openapi-original.yml, openapi/deliverect-kds-api-openapi-original.yml,\n  openapi/deliverect-loyalty-api-openapi-original.yml, openapi/deliverect-pay-api-openapi-original.yml,\n  openapi/deliverect-pos-api-openapi-original.yml, openapi/deliverect-store-api-openapi-original.yml\nschemes:\n- name: oauth2\n  source: openapi/deliverect-channel-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n- name: oauth2\n\
  \  source: openapi/deliverect-commerce-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n- name: oauth2\n  source: openapi/deliverect-crm-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n- name: oauth2\n  source: openapi/deliverect-dispatch-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n- name: oauth2\n  source: openapi/deliverect-gift-cards-api-openapi-original.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n- name: oauth2\n  source: openapi/deliverect-kds-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n- name: oauth2\n  source: openapi/deliverect-loyalty-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n- name: oauth2\n  source: openapi/deliverect-pay-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n- name: oauth2\n  source: openapi/deliverect-pos-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\n- name: oauth2\n  source: openapi/deliverect-store-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.deliverect.com/oauth/token\n  description: OAuth 2.0 machine-to-machine client-credentials. Exchange client_id/client_secret\n    at POST /oauth/token for a Bearer access_token.\nscopes:\n- scope: genericChannel:{channel_scope}\n  description: All endpoints within the Channel API.\n  sources:\n  - https://developers.deliverect.com/docs/getting-started\n\
  - scope: genericPOS\n  description: All endpoints within the POS + Store API.\n  sources:\n  - https://developers.deliverect.com/docs/getting-started\n- scope: store\n  description: All endpoints within the Store API.\n  sources:\n  - https://developers.deliverect.com/docs/getting-started\n- scope: genericFulfillment\n  description: All endpoints within the Dispatch API.\n  sources:\n  - https://developers.deliverect.com/docs/getting-started\n- scope: genericKDS\n  description: All endpoints within the KDS API.\n  sources:\n  - https://developers.deliverect.com/docs/getting-started\n- scope: payments\n  description: All endpoints within the DPAY (Pay) API.\n  sources:\n  - https://developers.deliverect.com/docs/getting-started\n- scope: genericCommerce\n  description: All endpoints within the Commerce API.\n  sources:\n  - https://developers.deliverect.com/docs/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/scopes/deliverect-scopes.yml
summary_line: 7 scopes · clientCredentials
tags:
- Restaurant
- Delivery
- Online Ordering
- Point of Sale
- Order Management
- Integration
token_urls:
- https://api.deliverect.com/oauth/token
---
