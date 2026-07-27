---
api_specs:
- filename: kore-wireless-connectivity-pro.yml
  format: yaml
  label: KORE Connectivity Pro API
  slug: kore-connectivity-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-connectivity-pro.yml
- filename: kore-wireless-supersim.yml
  format: yaml
  label: KORE Super SIM API
  slug: kore-super-sim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-supersim.yml
- filename: kore-wireless-programmable-wireless.yml
  format: yaml
  label: KORE Programmable Wireless API
  slug: kore-programmable-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-programmable-wireless.yml
- filename: kore-wireless-sms.yml
  format: yaml
  label: KORE SMS API
  slug: kore-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-sms.yml
- filename: kore-wireless-webhook.yml
  format: yaml
  label: KORE Webhook API
  slug: kore-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-webhook.yml
- filename: kore-wireless-iam.yml
  format: yaml
  label: KORE Identity and Access Management API
  slug: kore-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-iam.yml
- filename: kore-wireless-api-clients.yml
  format: yaml
  label: KORE API Clients API
  slug: kore-api-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-api-clients.yml
- filename: kore-wireless-token.yml
  format: yaml
  label: KORE Token API
  slug: kore-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-token.yml
authorization_urls: []
description: ''
docs: https://docs.korewireless.com/developers/api-management/api-clients
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Kore Wireless Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'KORE Wireless uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.korewireless.com/api-services/v1/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: KORE Wireless
provider_slug: kore-wireless
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.korewireless.com/api-services/v1/auth/token
  name: Auth
  source: openapi/kore-wireless-api-clients.yml
- description: token expiry is given in seconds
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.korewireless.com/Api/api/token
  name: Auth
  note: this spec still names the legacy developer-portal token URL; the current platform endpoint is /api-services/v1/auth/token
  source: openapi/kore-wireless-connectivity-pro.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.korewireless.com/api-services/v1/auth/token
  name: Auth
  source: openapi/kore-wireless-iam.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.korewireless.com/api-services/v1/auth/token
  name: Auth
  source: openapi/kore-wireless-programmable-wireless.yml
- description: token expiry is given in seconds
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.korewireless.com/Api/api/token
  name: Auth
  note: legacy developer-portal token URL, as with ConnectivityPro
  source: openapi/kore-wireless-sms.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.korewireless.com/api-services/v1/auth/token
  name: OAuth
  source: openapi/kore-wireless-supersim.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.korewireless.com/api-services/v1/auth/token
  name: Auth
  source: openapi/kore-wireless-webhook.yml
scope_count: 0
scope_names: []
scopes: []
slug: kore-wireless-scopes
source_filename: kore-wireless-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/kore-wireless-api-clients.yml, openapi/kore-wireless-connectivity-pro.yml,\n  openapi/kore-wireless-iam.yml, openapi/kore-wireless-programmable-wireless.yml,\n  openapi/kore-wireless-sms.yml, openapi/kore-wireless-supersim.yml, openapi/kore-wireless-webhook.yml\ndocs: https://docs.korewireless.com/developers/api-management/api-clients\nauth_docs: https://docs.korewireless.com/developers/api-management/auth\nmodel:\n  style: client-bound resource scopes, not string scopes in the authorization request\n  description: >-\n    KORE does not publish a string scope vocabulary (no read:sims / write:fleets\n    style identifiers), and no oauth2 flow in any of the eight OpenAPI documents\n    declares a scopes map — every declared clientCredentials flow has an empty\n    scopes object. Scope is instead bound to the API Client at creation time in the\n    console: you pick a Client Type, then select the Global Resources and Products\n\
  \    the client may reach, each with an access level. Those selections are minted\n    into the access token as structured claims, so the token — not the request —\n    carries the grant. Changing a client's scope requires re-authorizing to obtain a\n    new token; previously issued tokens keep their original scopes until they expire.\n  selection_surface: https://build.korewireless.com/clients/list\n  token_claim_shape: |\n    \"scopes\": {\n      \"globalResources\": [\n        {\"resourceName\": \"API Clients\", \"access\": [\"Read\", \"Write\", \"Modify\", \"Delete\"]}\n      ]\n    }\n  claim_source: sample access token published at https://docs.korewireless.com/developers/api-management/auth\nclient_types:\n- name: Admin\n  grants: global resources and product resources\n  who_can_create: Account Owner, Account Admin\n- name: Standard\n  grants: product resources only\n  who_can_create: Account Owner, Account Admin, Developer\nscope_dimensions:\n- dimension: globalResources\n  description:\
  \ account-wide resources the client may manage. The documented example\n    is \"API Clients\", which lets a client manage API Clients through the API.\n  known_values: [API Clients]\n  note: KORE does not publish the full enumeration of global resource names.\n- dimension: products\n  description: the KORE products the client may call. Product selection is what makes\n    a client's token valid against ConnectivityPro, Super SIM, Programmable Wireless,\n    SMS, Webhook or IAM.\n  known_values: [ConnectivityPro / OmniSIM, Super SIM, Programmable Wireless, SMS,\n    Webhook, IAM]\n  note: read from the eight published API surfaces; KORE does not publish the\n    console's product enumeration as a reference table.\naccess_levels: [Read, Write, Modify, Delete]\ntoken:\n  endpoint: https://api.korewireless.com/api-services/v1/auth/token\n  grant_type: client_credentials\n  response_scope_field: scope\n  observed_scope_value: email\n  expiry_options: [1 hour, 24 hours, 30 days, 24 months]\n\
  \  rotation_rule: changing Token Expiry Time, Client Type, Global Resources or Products\n    requires re-authorizing to mint a new token\nschemes:\n- name: Auth\n  source: openapi/kore-wireless-api-clients.yml\n  flows:\n  - {flow: clientCredentials, tokenUrl: 'https://api.korewireless.com/api-services/v1/auth/token'}\n- name: Auth\n  source: openapi/kore-wireless-connectivity-pro.yml\n  description: token expiry is given in seconds\n  flows:\n  - {flow: clientCredentials, tokenUrl: 'https://api.korewireless.com/Api/api/token'}\n  note: this spec still names the legacy developer-portal token URL; the current\n    platform endpoint is /api-services/v1/auth/token\n- name: Auth\n  source: openapi/kore-wireless-iam.yml\n  flows:\n  - {flow: clientCredentials, tokenUrl: 'https://api.korewireless.com/api-services/v1/auth/token'}\n- name: Auth\n  source: openapi/kore-wireless-programmable-wireless.yml\n  flows:\n  - {flow: clientCredentials, tokenUrl: 'https://api.korewireless.com/api-services/v1/auth/token'}\n\
  - name: Auth\n  source: openapi/kore-wireless-sms.yml\n  description: token expiry is given in seconds\n  flows:\n  - {flow: clientCredentials, tokenUrl: 'https://api.korewireless.com/Api/api/token'}\n  note: legacy developer-portal token URL, as with ConnectivityPro\n- name: OAuth\n  source: openapi/kore-wireless-supersim.yml\n  flows:\n  - {flow: clientCredentials, tokenUrl: 'https://api.korewireless.com/api-services/v1/auth/token'}\n- name: Auth\n  source: openapi/kore-wireless-webhook.yml\n  flows:\n  - {flow: clientCredentials, tokenUrl: 'https://api.korewireless.com/api-services/v1/auth/token'}\nscopes: []\nscopes_note: >-\n  Intentionally empty. No named OAuth scope string is published by KORE anywhere —\n  not in the specs, not in the docs, not in a scopes reference page. Filling this\n  list would mean inventing scope identifiers. The real grant model is the\n  scope_dimensions block above.\ngaps_for_provider:\n- publish the enumeration of Global Resources and Products selectable\
  \ on an API Client\n- declare the scopes map on each oauth2 securityScheme in the OpenAPI documents\n- apply per-operation security requirements so a consumer can compute the minimum\n  client scope for a given call\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/scopes/kore-wireless-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Telecommunications
- United States
- IoT
- eSIM
- Connectivity
- MVNO
- SIM Management
- Roaming
- Messaging
- SMS
- Device Management
- Network APIs
token_urls:
- https://api.korewireless.com/api-services/v1/auth/token
- https://api.korewireless.com/Api/api/token
---
