---
api_specs:
- filename: istreamplanet-audit-operations-for-organization-api-openapi.yml
  format: yaml
  label: iStreamPlanet Audit Operations for Organization API
  slug: istreamplanet-audit-operations-for-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-audit-operations-for-organization-api-openapi.yml
- filename: istreamplanet-available-sources-api-openapi.yml
  format: yaml
  label: iStreamPlanet Available Sources API
  slug: istreamplanet-available-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-available-sources-api-openapi.yml
- filename: istreamplanet-channel-operations-for-organization-api-openapi.yml
  format: yaml
  label: iStreamPlanet Channel Operations for Organization API
  slug: istreamplanet-channel-operations-for-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-channel-operations-for-organization-api-openapi.yml
- filename: istreamplanet-channels-api-openapi.yml
  format: yaml
  label: iStreamPlanet Channels API
  slug: istreamplanet-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-channels-api-openapi.yml
- filename: istreamplanet-channels-for-organization-api-openapi.yml
  format: yaml
  label: iStreamPlanet Channels for Organization API
  slug: istreamplanet-channels-for-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-channels-for-organization-api-openapi.yml
- filename: istreamplanet-deprecated-live2vod-api-openapi.yml
  format: yaml
  label: iStreamPlanet Deprecated Live2VOD API
  slug: istreamplanet-deprecated-live2vod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-deprecated-live2vod-api-openapi.yml
- filename: istreamplanet-live2vod-for-organization-api-openapi.yml
  format: yaml
  label: iStreamPlanet Live2VOD for Organization API
  slug: istreamplanet-live2vod-for-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-live2vod-for-organization-api-openapi.yml
- filename: istreamplanet-organizations-api-openapi.yml
  format: yaml
  label: iStreamPlanet Organizations API
  slug: istreamplanet-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-organizations-api-openapi.yml
- filename: istreamplanet-source-previews-api-openapi.yml
  format: yaml
  label: iStreamPlanet Source Previews API
  slug: istreamplanet-source-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-source-previews-api-openapi.yml
- filename: istreamplanet-transcoder-telemetry-api-openapi.yml
  format: yaml
  label: iStreamPlanet Transcoder Telemetry API
  slug: istreamplanet-transcoder-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-transcoder-telemetry-api-openapi.yml
authorization_urls:
- https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Istreamplanet Scopes
name_suffix: OAuth Scopes
note: 'Both oauth2 securitySchemes declare `scopes: null`, and no scopes/permissions reference page was found in the API reference (https://api.istreamplanet.com/docs) or the iStreamPlanet Developer Portal (https://istreamlabs.github.io/docs/guide/). The only scope names in the contract are the two the spec''s x-cli-config extension tells Restish to request on the authorization-code flow; they are WBD Okta token scopes, not per-resource API permissions.'
overview: 'iStreamPlanet publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the iStreamPlanet API on a user''s behalf.


  Tokens are issued from https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: iStreamPlanet
provider_slug: istreamplanet
schemes:
- flows:
  - authorizationUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/authorize
    flow: authorizationCode
    tokenUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token
  name: authcode
  source: openapi/istreamplanet-aventus-channels-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token
  name: m2m
  source: openapi/istreamplanet-aventus-channels-openapi.yml
scope_count: 2
scope_names:
- offline_access
- Groups
scopes:
- description: Requested by the CLI auto-configuration (x-cli-config.params.scopes "offline_access,Groups"); standard OIDC scope for a refresh token.
  flows: []
  scope: offline_access
- description: Requested by the CLI auto-configuration (x-cli-config.params.scopes "offline_access,Groups"); no further description is published.
  flows: []
  scope: Groups
slug: istreamplanet-scopes
source_filename: istreamplanet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/istreamplanet-aventus-channels-openapi.yml\nnote: 'Both oauth2 securitySchemes declare `scopes: null`, and no scopes/permissions reference page was found in the API reference (https://api.istreamplanet.com/docs) or the iStreamPlanet Developer Portal (https://istreamlabs.github.io/docs/guide/). The only scope names in the contract are the two the spec''s x-cli-config extension tells Restish to request on the authorization-code flow; they are WBD Okta token scopes, not per-resource API permissions.'\nschemes:\n- name: authcode\n  source: openapi/istreamplanet-aventus-channels-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/authorize\n    tokenUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token\n- name: m2m\n  source: openapi/istreamplanet-aventus-channels-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token\n\
  scopes:\n- name: offline_access\n  scheme: authcode\n  description: Requested by the CLI auto-configuration (x-cli-config.params.scopes \"offline_access,Groups\"); standard OIDC scope for a refresh token.\n  source: openapi/_original/istreamplanet-aventus-channels-openapi.json#/x-cli-config\n- name: Groups\n  scheme: authcode\n  description: Requested by the CLI auto-configuration (x-cli-config.params.scopes \"offline_access,Groups\"); no further description is published.\n  source: openapi/_original/istreamplanet-aventus-channels-openapi.json#/x-cli-config\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/scopes/istreamplanet-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Company
- Video Streaming
- Live Streaming
- Media
- Cloud Video
- Spectral
- API Governance
token_bound: false
token_urls:
- https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token
---
