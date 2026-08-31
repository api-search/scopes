---
api_specs:
- filename: nexar-citystream-live-feed-api-v4-api-openapi.yml
  format: yaml
  label: Nexar CityStream™ Live Feed API V4 API
  slug: nexar-citystream-live-feed-api-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-citystream-live-feed-api-v4-api-openapi.yml
- filename: nexar-get-a-collection-of-road-signs-api-openapi.yml
  format: yaml
  label: Nexar Get a collection of road signs API
  slug: nexar-get-a-collection-of-road-signs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-a-collection-of-road-signs-api-openapi.yml
- filename: nexar-get-a-collection-of-work-zones-api-openapi.yml
  format: yaml
  label: Nexar Get a collection of work zones API
  slug: nexar-get-a-collection-of-work-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-a-collection-of-work-zones-api-openapi.yml
- filename: nexar-get-a-specific-work-zone-api-openapi.yml
  format: yaml
  label: Nexar Get a specific work zone API
  slug: nexar-get-a-specific-work-zone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-a-specific-work-zone-api-openapi.yml
- filename: nexar-get-the-details-of-a-specific-road-sign-api-openapi.yml
  format: yaml
  label: Nexar Get the details of a specific road sign API
  slug: nexar-get-the-details-of-a-specific-road-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-the-details-of-a-specific-road-sign-api-openapi.yml
- filename: nexar-virtualcam-api-api-openapi.yml
  format: yaml
  label: Nexar VirtualCam API
  slug: nexar-virtualcam-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-virtualcam-api-api-openapi.yml
authorization_urls:
- https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/authorize
description: ''
docs: https://developer.getnexar.com/access
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nexar Scopes
name_suffix: OAuth Scopes
note: 'The four published OpenAPI documents declare only an apiKey scheme named `Bearer` in the Authorization header, so derive-oauth-scopes.py found no oauth2 flows in the contract. The real authorization model is OAuth 2.0 Authorization Code + PKCE against Nexar''s own Okta tenant: the portal mints a per-API access token and the scope strings it requests are hard-coded in the portal bundle, one set per CityStream product. The Okta authorization-server metadata (saved under well-known/) advertises only the standard OIDC scopes; these product scopes are custom and are granted through Okta group membership, which is also what gates the documentation route for each API.'
overview: 'Nexar publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nexar API on a user''s behalf.


  Tokens are issued from https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nexar
provider_slug: nexar
schemes:
- flows:
  - authorizationUrl: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/authorize
    flow: authorizationCode
    introspectionUrl: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/introspect
    pkce: S256
    revocationUrl: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/revoke
    tokenUrl: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/token
  issuer: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7
  name: Okta OAuth 2.0
  refresh: https://external.getnexar.com/dev-portal/refresh-token
  type: oauth2
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/nexar-virtualcam-openapi.yml
  - openapi/nexar-livefeed-openapi.yml
  - openapi/nexar-workzones-openapi.yml
  - openapi/nexar-roadinventory-openapi.yml
  type: apiKey
scope_count: 4
scope_names:
- frame:get
- image:get
- detection:find
- detection:get
scopes:
- description: Read road frames.
  flows:
  - authorizationCode
  scope: frame:get
- description: Read the image bytes behind a frame or a detection evidence frame.
  flows:
  - authorizationCode
  scope: image:get
- description: Search a collection of detections.
  flows:
  - authorizationCode
  scope: detection:find
- description: Read a single detection in full.
  flows:
  - authorizationCode
  scope: detection:get
slug: nexar-scopes
source_filename: nexar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://developer.getnexar.com/static/js/main.821ebbae.js (the Developers Portal application bundle)\ndocs: https://developer.getnexar.com/access\nnote: 'The four published OpenAPI documents declare only an apiKey scheme named `Bearer` in the Authorization header,\n  so derive-oauth-scopes.py found no oauth2 flows in the contract. The real authorization model is OAuth 2.0 Authorization\n  Code + PKCE against Nexar''s own Okta tenant: the portal mints a per-API access token and the scope strings it\n  requests are hard-coded in the portal bundle, one set per CityStream product. The Okta authorization-server metadata\n  (saved under well-known/) advertises only the standard OIDC scopes; these product scopes are custom and are granted\n  through Okta group membership, which is also what gates the documentation route for each API.'\nschemes:\n- name: Okta OAuth 2.0\n  type: oauth2\n  issuer: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7\n\
  \  flows:\n  - flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/authorize\n    tokenUrl: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/token\n    revocationUrl: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/revoke\n    introspectionUrl: https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/introspect\n  refresh: https://external.getnexar.com/dev-portal/refresh-token\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/nexar-virtualcam-openapi.yml\n  - openapi/nexar-livefeed-openapi.yml\n  - openapi/nexar-workzones-openapi.yml\n  - openapi/nexar-roadinventory-openapi.yml\nscopes:\n- scope: frame:get\n  description: Read road frames.\n  apis:\n  - CityStream VirtualCam API\n  flows:\n  - authorizationCode\n- scope: image:get\n  description: Read the image bytes behind a frame or a detection evidence frame.\n  apis:\n  - CityStream VirtualCam API\n  - CityStream\
  \ Live Feed API\n  - CityStream Work Zones API\n  - CityStream Road Inventory API\n  flows:\n  - authorizationCode\n- scope: detection:find\n  description: Search a collection of detections.\n  apis:\n  - CityStream Live Feed API\n  - CityStream Work Zones API\n  - CityStream Road Inventory API\n  flows:\n  - authorizationCode\n- scope: detection:get\n  description: Read a single detection in full.\n  apis:\n  - CityStream Live Feed API\n  - CityStream Work Zones API\n  - CityStream Road Inventory API\n  flows:\n  - authorizationCode\nstandard_oidc_scopes:\n- openid\n- profile\n- email\n- address\n- phone\n- offline_access\n- device_sso\nokta_groups_gate: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/scopes/nexar-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Mapping
- Geospatial
- Transportation
- Computer Vision
- Autonomous Vehicles
- Smart Cities
- Imagery
- Road Data
- Machine Learning
token_urls:
- https://nexar.okta.com/oauth2/aus3qkg89t55hJZsT4x7/v1/token
---
