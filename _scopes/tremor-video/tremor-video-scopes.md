---
api_specs:
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP API
  slug: nexxen-dsp-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Token Service
  slug: nexxen-dsp-token-service
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Reporting API
  slug: nexxen-dsp-reporting-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Device API
  slug: nexxen-dsp-device-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Location API
  slug: nexxen-dsp-location-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
authorization_urls: []
description: ''
docs: https://www.postman.com/nexxen-api/nexxen/documentation/9md8q3a/nexxen-dsp-apis
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Tremor Video Scopes
name_suffix: OAuth Scopes
note: 'Nexxen publishes no scope reference page and no OpenAPI, so nothing here was read from a scopes document. Everything below was read out of two real sources: the OIDC metadata served by the Okta authorization server that issues Nexxen DSP API tokens, and the decoded (expired, 2022) example access token the provider itself published inside its public Postman collection. The DSP API does not ask callers for scopes — a client-credentials call to services.amobee.com/accounts/v1/api/token returns a token whose per-service entitlements are already baked into the service account.'
overview: 'Tremor Video publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tremor Video API on a user''s behalf.


  Tokens are issued from https://services.amobee.com/accounts/v1/api/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tremor Video
provider_slug: tremor-video
schemes:
- flows:
  - flow: clientCredentials
    note: The provider's own wrapper endpoint; takes client_id + client_secret in a JSON body.
    scopes: []
    tokenUrl: https://services.amobee.com/accounts/v1/api/token
  name: OAuth2ClientCredentials
  source: collections/tremor-video.postman_collection.json
scope_count: 1
scope_names:
- openid
scopes:
- description: OIDC subject identity; the only scope present on a live-issued DSP API token.
  flows:
  - clientCredentials
  scope: openid
slug: tremor-video-scopes
source_filename: tremor-video-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://amobee-platform.okta.com/oauth2/default/.well-known/openid-configuration\ndocs: https://www.postman.com/nexxen-api/nexxen/documentation/9md8q3a/nexxen-dsp-apis\nnote: >-\n  Nexxen publishes no scope reference page and no OpenAPI, so nothing here was read from a scopes\n  document. Everything below was read out of two real sources: the OIDC metadata served by the\n  Okta authorization server that issues Nexxen DSP API tokens, and the decoded (expired, 2022)\n  example access token the provider itself published inside its public Postman collection. The\n  DSP API does not ask callers for scopes — a client-credentials call to\n  services.amobee.com/accounts/v1/api/token returns a token whose per-service entitlements are\n  already baked into the service account.\nschemes:\n- name: OAuth2ClientCredentials\n  source: collections/tremor-video.postman_collection.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services.amobee.com/accounts/v1/api/token\n\
  \    scopes: []\n    note: The provider's own wrapper endpoint; takes client_id + client_secret in a JSON body.\nauthorization_server:\n  issuer: https://amobee-platform.okta.com/oauth2/default\n  vendor: Okta\n  token_endpoint: https://amobee-platform.okta.com/oauth2/default/v1/token\n  authorization_endpoint: https://amobee-platform.okta.com/oauth2/default/v1/authorize\n  introspection_endpoint: https://amobee-platform.okta.com/oauth2/default/v1/introspect\n  revocation_endpoint: https://amobee-platform.okta.com/oauth2/default/v1/revoke\n  jwks_uri: https://amobee-platform.okta.com/oauth2/default/v1/keys\n  grant_types_supported: [authorization_code, implicit, refresh_token, password, 'urn:ietf:params:oauth:grant-type:device_code']\n  client_credentials_advertised: false\n  pkce: [S256]\n  discovery_documents:\n  - well-known/tremor-video-openid-configuration.json\n  - well-known/tremor-video-oauth-authorization-server.json\nscopes:\n- scope: openid\n  description: OIDC subject identity;\
  \ the only scope present on a live-issued DSP API token.\n  flows: [clientCredentials]\n  sources: [collections/tremor-video.postman_collection.json]\n  evidence: 'scp: [\"openid\"] on the provider-published example access token'\noidc_scopes_supported:\n- {scope: openid, source: openid-configuration}\n- {scope: profile, source: openid-configuration}\n- {scope: email, source: openid-configuration}\n- {scope: address, source: openid-configuration}\n- {scope: phone, source: openid-configuration}\n- {scope: offline_access, source: openid-configuration}\n- {scope: device_sso, source: openid-configuration}\nnote_on_oidc_scopes: >-\n  These are the Okta authorization server's advertised OIDC scopes, i.e. what the identity tenant\n  supports for user sign-in. They are NOT an API permission vocabulary for the DSP API and must not\n  be read as one.\nauthorities:\n  model: >-\n    Entitlement is carried as an authorities[] claim on the issued token — a coarse per-service\n    grant, not a request-time\
  \ scope. A caller cannot narrow or elevate it; it is set on the API\n    service account when the credential is provisioned in the DSP platform.\n  source: decoded example access token published in the provider's own Postman collection\n  observed:\n  - {authority: APP_API_CAMPAIGN_MGMT, grants: Campaign Management service (/campaign/v5/api)}\n  - {authority: APP_API_REPORTING, grants: Reporting service (/reporting/v2/api)}\n  - {authority: APP_API_DEVICE, grants: Device reference service (/device/v1/api)}\n  - {authority: APP_API_LOCATION, grants: Location reference service (/location/v1/api)}\n  - {authority: APP_API_DATAMINE, grants: data-mining surface not present in the public collection}\n  - {authority: POLICY_API, grants: policy surface not present in the public collection}\n  - {authority: APP_TURN_PLATFORM, grants: legacy Turn platform (Amobee acquired Turn)}\n  - {authority: ROLE_SERVICE_ACCOUNT, grants: marks the principal as a machine account}\n  - {authority: ROLE_INTERNAL,\
  \ grants: internal role present on the published example token}\n  - {authority: Everyone, grants: default Okta group}\n  caveat: >-\n    This is one example token from one service account, published by the provider in 2022 and now\n    expired. It shows the shape and the naming of the entitlement vocabulary; it is not a complete\n    or current catalog, and two of the authorities (APP_API_DATAMINE, POLICY_API) point at services\n    that have no public documentation at all.\nprivacy_note: >-\n  The subject, email and personal-name claims carried by that example token were deliberately not\n  transcribed here, and the token itself has been redacted out of the saved collection.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/scopes/tremor-video-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Martech
- Advertising
- AdTech
- DSP
- Programmatic
- CTV
- Video Advertising
token_urls:
- https://services.amobee.com/accounts/v1/api/token
---
