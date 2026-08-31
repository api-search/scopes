---
api_specs:
- filename: videoamp-admeasurements-api-openapi.yml
  format: yaml
  label: VideoAmp Ad Measurements API
  slug: videoamp-admeasurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-admeasurements-api-openapi.yml
- filename: videoamp-audiences-api-openapi.yml
  format: yaml
  label: VideoAmp Audiences API
  slug: videoamp-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-audiences-api-openapi.yml
- filename: videoamp-campaigns-api-openapi.yml
  format: yaml
  label: VideoAmp Campaigns API
  slug: videoamp-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-campaigns-api-openapi.yml
- filename: videoamp-consents-api-openapi.yml
  format: yaml
  label: VideoAmp Consents API
  slug: videoamp-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-consents-api-openapi.yml
- filename: videoamp-content-api-openapi.yml
  format: yaml
  label: VideoAmp Content API
  slug: videoamp-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-content-api-openapi.yml
- filename: videoamp-currency-of-record-api-openapi.yml
  format: yaml
  label: VideoAmp Currency Of Record API
  slug: videoamp-currency-of-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-currency-of-record-api-openapi.yml
- filename: videoamp-datastreams-api-openapi.yml
  format: yaml
  label: VideoAmp Data Streams API
  slug: videoamp-datastreams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-datastreams-api-openapi.yml
- filename: videoamp-datastreamtypes-api-openapi.yml
  format: yaml
  label: VideoAmp Data Stream Types API
  slug: videoamp-datastreamtypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-datastreamtypes-api-openapi.yml
- filename: videoamp-inventories-api-openapi.yml
  format: yaml
  label: VideoAmp Inventories API
  slug: videoamp-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-inventories-api-openapi.yml
- filename: videoamp-library-api-openapi.yml
  format: yaml
  label: VideoAmp Library API
  slug: videoamp-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-library-api-openapi.yml
- filename: videoamp-me-api-openapi.yml
  format: yaml
  label: VideoAmp Me API
  slug: videoamp-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-me-api-openapi.yml
- filename: videoamp-plans-api-openapi.yml
  format: yaml
  label: VideoAmp Plans API
  slug: videoamp-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-plans-api-openapi.yml
- filename: videoamp-reports-api-openapi.yml
  format: yaml
  label: VideoAmp Reports API
  slug: videoamp-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-reports-api-openapi.yml
- filename: videoamp-shares-api-openapi.yml
  format: yaml
  label: VideoAmp Shares API
  slug: videoamp-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-shares-api-openapi.yml
authorization_urls:
- https://login.videoamp.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- deviceAuthorization
kind: oauth-scopes
layout: scope
method: derived
name: Videoamp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'VideoAmp publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceAuthorization flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the VideoAmp API on a user''s behalf.


  Tokens are issued from https://login.videoamp.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VideoAmp
provider_slug: videoamp
schemes:
- description: OAuth 2.0 / OIDC via VideoAmp's Auth0 tenant at https://login.videoamp.com. Verified from https://login.videoamp.com/.well-known/openid-configuration (HTTP 200) and https://api.videoamp.dev/.well-known/oauth-protected-resource/v1/mcp (HTTP 200, RFC 9728). Bearer tokens are presented in the Authorization header.
  flows:
  - authorizationUrl: https://login.videoamp.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.videoamp.com/oauth/token
  - flow: deviceAuthorization
    tokenUrl: https://login.videoamp.com/oauth/token
  name: videoampOAuth
  source: openapi/videoamp-public-api-openapi.yml
scope_count: 4
scope_names:
- email
- offline_access
- openid
- profile
scopes:
- description: Email address claim
  flows:
  - authorizationCode
  - deviceAuthorization
  scope: email
- description: Issue a refresh token
  flows:
  - authorizationCode
  - deviceAuthorization
  scope: offline_access
- description: OIDC subject identifier
  flows:
  - authorizationCode
  - deviceAuthorization
  scope: openid
- description: Basic profile claims
  flows:
  - authorizationCode
  - deviceAuthorization
  scope: profile
slug: videoamp-scopes
source_filename: videoamp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/videoamp-public-api-openapi.yml\nschemes:\n- name: videoampOAuth\n  source: openapi/videoamp-public-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.videoamp.com/authorize\n    tokenUrl: https://login.videoamp.com/oauth/token\n  - flow: deviceAuthorization\n    tokenUrl: https://login.videoamp.com/oauth/token\n  description: OAuth 2.0 / OIDC via VideoAmp's Auth0 tenant at https://login.videoamp.com. Verified\n    from https://login.videoamp.com/.well-known/openid-configuration (HTTP 200) and https://api.videoamp.dev/.well-known/oauth-protected-resource/v1/mcp\n    (HTTP 200, RFC 9728). Bearer tokens are presented in the Authorization header.\nscopes:\n- scope: email\n  description: Email address claim\n  flows:\n  - authorizationCode\n  - deviceAuthorization\n  sources:\n  - openapi/videoamp-public-api-openapi.yml\n- scope: offline_access\n  description: Issue a refresh token\n\
  \  flows:\n  - authorizationCode\n  - deviceAuthorization\n  sources:\n  - openapi/videoamp-public-api-openapi.yml\n- scope: openid\n  description: OIDC subject identifier\n  flows:\n  - authorizationCode\n  - deviceAuthorization\n  sources:\n  - openapi/videoamp-public-api-openapi.yml\n- scope: profile\n  description: Basic profile claims\n  flows:\n  - authorizationCode\n  - deviceAuthorization\n  sources:\n  - openapi/videoamp-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/scopes/videoamp-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceAuthorization
tags:
- media-measurement
- Advertising
- adtech
- tv-currency
- audience-measurement
- media-planning
- streaming
- Attribution
- data-collaboration
- MCP
- agent-native
token_urls:
- https://login.videoamp.com/oauth/token
---
