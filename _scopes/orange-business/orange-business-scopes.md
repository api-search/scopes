---
api_specs:
- filename: orange-business-live-objects-openapi.json
  format: json
  label: Orange Business Live Objects API
  slug: orange-business-live-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-live-objects-openapi.json
- filename: orange-business-check-device-swap-api-openapi.yml
  format: yaml
  label: Orange Business Check Device Swap API
  slug: orange-business-check-device-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-check-device-swap-api-openapi.yml
- filename: orange-business-check-sim-swap-api-openapi.yml
  format: yaml
  label: Orange Business Check SIM swap API
  slug: orange-business-check-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-check-sim-swap-api-openapi.yml
- filename: orange-business-device-reachability-status-api-openapi.yml
  format: yaml
  label: Orange Business Device reachability status API
  slug: orange-business-device-reachability-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-reachability-status-api-openapi.yml
- filename: orange-business-geofencing-subscriptions-api-openapi.yml
  format: yaml
  label: Orange Business Geofencing subscriptions API
  slug: orange-business-geofencing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-geofencing-subscriptions-api-openapi.yml
- filename: orange-business-location-retrieval-api-openapi.yml
  format: yaml
  label: Orange Business Location retrieval API
  slug: orange-business-location-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-location-retrieval-api-openapi.yml
- filename: orange-business-location-verification-api-openapi.yml
  format: yaml
  label: Orange Business Location verification API
  slug: orange-business-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-location-verification-api-openapi.yml
- filename: orange-business-match-api-openapi.yml
  format: yaml
  label: Orange Business Match API
  slug: orange-business-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-match-api-openapi.yml
- filename: orange-business-phone-number-share-api-openapi.yml
  format: yaml
  label: Orange Business Phone number share API
  slug: orange-business-phone-number-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-phone-number-share-api-openapi.yml
- filename: orange-business-phone-number-verify-api-openapi.yml
  format: yaml
  label: Orange Business Phone number verify API
  slug: orange-business-phone-number-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-phone-number-verify-api-openapi.yml
- filename: orange-business-population-density-data-api-openapi.yml
  format: yaml
  label: Orange Business Population Density Data API
  slug: orange-business-population-density-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-population-density-data-api-openapi.yml
- filename: orange-business-qos-sessions-api-openapi.yml
  format: yaml
  label: Orange Business QoS Sessions API
  slug: orange-business-qos-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-qos-sessions-api-openapi.yml
- filename: orange-business-retrieve-device-swap-date-api-openapi.yml
  format: yaml
  label: Orange Business Retrieve Device Swap Date API
  slug: orange-business-retrieve-device-swap-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-retrieve-device-swap-date-api-openapi.yml
- filename: orange-business-retrieve-sim-swap-date-api-openapi.yml
  format: yaml
  label: Orange Business Retrieve SIM swap date API
  slug: orange-business-retrieve-sim-swap-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-retrieve-sim-swap-date-api-openapi.yml
- filename: orange-business-roaming-status-retrieval-api-openapi.yml
  format: yaml
  label: Orange Business Roaming status retrieval API
  slug: orange-business-roaming-status-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-roaming-status-retrieval-api-openapi.yml
authorization_urls:
- https://liveobjects.orange-business.com/api/v1/oauth2/authorize
description: ''
docs:
- https://liveobjects.orange-business.com/doc/html/lo_manual_v2.html
- https://docs.developer.orange.com/network-apis/practical-guides/api-authentication/backend-flow
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Orange Business Scopes
name_suffix: OAuth Scopes
note: 'The 23 scopes below are Live Objects API-key roles, declared verbatim in the Live Objects OpenAPI OAuth2.0 authorizationCode flow and enforced per operation ("Restricted to API keys with at least one of the following roles: ..."). They pair R/W by domain — DATA, DEVICE, USER, API_KEY, BUS, BUS_CONFIG, CAMPAIGN, DATA_PROCESSING, BOOTSTRAP, SETTINGS — plus two connection-mode roles (DEVICE_ACCESS, CONNECTOR_ACCESS) and one read-only audit role (LOGS_R). The CAMARA Network APIs on api.orange.com do NOT use named scopes. Their authorization is purpose-bound instead: the scope string is `openid dpv:<dpvValue> <technicalParameter>`, carrying a W3C Data Privacy Vocabulary purpose value rather than an API permission. There is no scope list to enumerate for that estate — the vocabulary is DPV''s, not Orange''s.'
overview: 'Orange Business publishes 23 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Orange Business API on a user''s behalf.


  Tokens are issued from https://liveobjects.orange-business.com/api/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Orange Business
provider_slug: orange-business
schemes:
- flows:
  - authorizationUrl: https://liveobjects.orange-business.com/api/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://liveobjects.orange-business.com/api/v1/oauth2/token
  name: OAuth2.0
  source: openapi/orange-business-live-objects-openapi.json
scope_count: 23
scope_names:
- API_KEY_R
- API_KEY_W
- BOOTSTRAP_R
- BOOTSTRAP_W
- BUS_CONFIG_R
- BUS_CONFIG_W
- BUS_R
- BUS_W
- CAMPAIGN_R
- CAMPAIGN_W
- CONNECTOR_ACCESS
- DATA_PROCESSING_R
- DATA_PROCESSING_W
- DATA_R
- DATA_W
- DEVICE_ACCESS
- DEVICE_R
- DEVICE_W
- LOGS_R
- SETTINGS_R
- SETTINGS_W
- USER_R
- USER_W
scopes:
- description: Read parameters and status of an API key.
  flows:
  - authorizationCode
  scope: API_KEY_R
- description: Create, modify, disable an API key.
  flows:
  - authorizationCode
  scope: API_KEY_W
- description: Read parameters and status of the LwM2M Bootstrap configurations and entries.
  flows:
  - authorizationCode
  scope: BOOTSTRAP_R
- description: Create ans modify LwM2M Bootstrap configurations and entries.
  flows:
  - authorizationCode
  scope: BOOTSTRAP_W
- description: Read config parameters of a FIFO queue.
  flows:
  - authorizationCode
  scope: BUS_CONFIG_R
- description: Create, modify a FIFO queue.
  flows:
  - authorizationCode
  scope: BUS_CONFIG_W
- description: Read data on the Live Objects bus. Minimum permission for the API key of an application collecting data on Live Objects in MQTT(s).
  flows:
  - authorizationCode
  scope: BUS_R
- description: Publish data on the Live Objects bus.
  flows:
  - authorizationCode
  scope: BUS_W
- description: Read parameters and status of a massive deployment campaign on your Device Fleet.
  flows:
  - authorizationCode
  scope: CAMPAIGN_R
- description: Create, modify a campaign on your Device Fleet.
  flows:
  - authorizationCode
  scope: CAMPAIGN_W
- description: Role to set on a external connector API key to allow only MQTT external connector mode
  flows:
  - authorizationCode
  scope: CONNECTOR_ACCESS
- description: Read parameters and status of an event processing rule or a Data decoder.
  flows:
  - authorizationCode
  scope: DATA_PROCESSING_R
- description: Create, modify, disable an event processing rule or a Data decoder.
  flows:
  - authorizationCode
  scope: DATA_PROCESSING_W
- description: Read the data collected by the Store Service or search into this data using the Search Service.
  flows:
  - authorizationCode
  scope: DATA_R
- description: Insert a data record to the Store Service. Minimum permission required for the API key of a device pushing data to Live Objects in HTTPS.
  flows:
  - authorizationCode
  scope: DATA_W
- description: Role to set on a Device API key to allow only MQTT Device mode
  flows:
  - authorizationCode
  scope: DEVICE_ACCESS
- description: Read parameters and status of a Device management.
  flows:
  - authorizationCode
  scope: DEVICE_R
- description: Create, modify, disable a Device management, send command, modify config, update resource of a Device.
  flows:
  - authorizationCode
  scope: DEVICE_W
- description: Read the logs collected by the Audit Log service. This right allows users to use the Audit Log service as debugging tool.
  flows:
  - authorizationCode
  scope: LOGS_R
- description: Read the tenant account custom settings.
  flows:
  - authorizationCode
  scope: SETTINGS_R
- description: Create, modify tenant account custom settings.
  flows:
  - authorizationCode
  scope: SETTINGS_W
- description: Read parameters and status of a user.
  flows:
  - authorizationCode
  scope: USER_R
- description: Create, modify, disable a user.
  flows:
  - authorizationCode
  scope: USER_W
slug: orange-business-scopes
source_filename: orange-business-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: openapi/orange-business-live-objects-openapi.json\nschemes:\n- name: OAuth2.0\n  source: openapi/orange-business-live-objects-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://liveobjects.orange-business.com/api/v1/oauth2/authorize\n    tokenUrl: https://liveobjects.orange-business.com/api/v1/oauth2/token\nscopes:\n- scope: API_KEY_R\n  description: Read parameters and status of an API key.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: API_KEY_W\n  description: Create, modify, disable an API key.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: BOOTSTRAP_R\n  description: Read parameters and status of the LwM2M Bootstrap configurations and entries.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: BOOTSTRAP_W\n\
  \  description: Create ans modify LwM2M Bootstrap configurations and entries.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: BUS_CONFIG_R\n  description: Read config parameters of a FIFO queue.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: BUS_CONFIG_W\n  description: Create, modify a FIFO queue.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: BUS_R\n  description: Read data on the Live Objects bus. Minimum permission for the API key of an application collecting\n    data on Live Objects in MQTT(s).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: BUS_W\n  description: Publish data on the Live Objects bus.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: CAMPAIGN_R\n  description:\
  \ Read parameters and status of a massive deployment campaign on your Device Fleet.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: CAMPAIGN_W\n  description: Create, modify a campaign on your Device Fleet.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: CONNECTOR_ACCESS\n  description: Role to set on a external connector API key to allow only MQTT external connector mode\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: DATA_PROCESSING_R\n  description: Read parameters and status of an event processing rule or a Data decoder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: DATA_PROCESSING_W\n  description: Create, modify, disable an event processing rule or a Data decoder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n\
  - scope: DATA_R\n  description: Read the data collected by the Store Service or search into this data using the Search Service.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: DATA_W\n  description: Insert a data record to the Store Service. Minimum permission required for the API key of a\n    device pushing data to Live Objects in HTTPS.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: DEVICE_ACCESS\n  description: Role to set on a Device API key to allow only MQTT Device mode\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: DEVICE_R\n  description: Read parameters and status of a Device management.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: DEVICE_W\n  description: Create, modify, disable a Device management, send command, modify config,\
  \ update resource of\n    a Device.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: LOGS_R\n  description: Read the logs collected by the Audit Log service. This right allows users to use the Audit Log\n    service as debugging tool.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: SETTINGS_R\n  description: Read the tenant account custom settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: SETTINGS_W\n  description: Create, modify tenant account custom settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: USER_R\n  description: Read parameters and status of a user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- scope: USER_W\n  description: Create, modify, disable a user.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\ndocs:\n- https://liveobjects.orange-business.com/doc/html/lo_manual_v2.html\n- https://docs.developer.orange.com/network-apis/practical-guides/api-authentication/backend-flow\nnote: 'The 23 scopes below are Live Objects API-key roles, declared verbatim in the Live Objects OpenAPI OAuth2.0\n  authorizationCode flow and enforced per operation (\"Restricted to API keys with at least one of the following\n  roles: ...\"). They pair R/W by domain — DATA, DEVICE, USER, API_KEY, BUS, BUS_CONFIG, CAMPAIGN, DATA_PROCESSING,\n  BOOTSTRAP, SETTINGS — plus two connection-mode roles (DEVICE_ACCESS, CONNECTOR_ACCESS) and one read-only\n  audit role (LOGS_R).\n\n\n  The CAMARA Network APIs on api.orange.com do NOT use named scopes. Their authorization is purpose-bound instead:\n  the scope string is `openid dpv:<dpvValue> <technicalParameter>`, carrying a W3C Data Privacy Vocabulary\n  purpose value rather than\
  \ an API permission. There is no scope list to enumerate for that estate — the vocabulary\n  is DPV''s, not Orange''s.'\ncamara_scope_model:\n  style: purpose-bound (W3C DPV)\n  form: openid dpv:<dpvValue> <technicalParameter>\n  source: https://docs.developer.orange.com/network-apis/practical-guides/api-authentication/backend-flow\n  named_scopes: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/scopes/orange-business-scopes.yml
summary_line: 23 scopes · authorizationCode
tags:
- 5G
- Artificial Intelligence
- B2B
- CAMARA
- Cloud
- Communications
- Cybersecurity
- Developer Platform
- Digital Workplace
- Enterprise
- France
- IoT
- Identity
- Mobile Money
- Network APIs
- Open Gateway
- Orange
- Payments
- SD-WAN
- SMS
- SASE
- Telco
- Voice
token_urls:
- https://liveobjects.orange-business.com/api/v1/oauth2/token
---
