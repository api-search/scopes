---
api_specs:
- filename: reliance-jio-jiomeet-platform-openapi.yml
  format: yaml
  label: JioMeet Platform Server API
  slug: jiomeet-platform-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jiomeet-platform-openapi.yml
- filename: reliance-jio-jiomeet-oauth-openapi.yml
  format: yaml
  label: JioMeet Platform OAuth API
  slug: jiomeet-platform-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jiomeet-oauth-openapi.yml
- filename: reliance-jio-jioevents-platform-openapi.yml
  format: yaml
  label: JioEvents Platform Server API
  slug: jioevents-platform-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jioevents-platform-openapi.yml
authorization_urls:
- https://jiomeetpro.jio.com/oauth2/authorize
description: 'OAuth 2.0 authorization-code scopes for the JioMeet Platform OAuth API. These scopes are documented on Jio''s OAuth integration guide, NOT in the machine-readable spec - the harvested OpenAPI models the OAuth API with plain http basic / http bearer security schemes and declares no oauth2 flow object, so the scope list exists only in prose. Scope is nevertheless returned at runtime: the token response carries a `scope` field described as "the permissions that are granted to the access token". This applies to the user-authorized JioMeet surface only; the JioMeet Platform Server API and the JioEvents Platform Server API are app-credential JWT surfaces with no scope model at all.'
docs: https://dev.jiomeet.com/docs/quick-start/integrate_using_oauth_client
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Reliance Jio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Reliance Jio publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Reliance Jio API on a user''s behalf.


  Tokens are issued from https://jiomeetpro.jio.com/api/oauth2/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Reliance Jio
provider_slug: reliance-jio
schemes:
- documented_only: true
  flows:
  - authorizationUrl: https://jiomeetpro.jio.com/oauth2/authorize
    flow: authorizationCode
    refresh_supported: true
    tokenUrl: https://jiomeetpro.jio.com/api/oauth2/v2/token
    token_endpoint_auth: HTTP Basic (clientId as username, clientSecret as password)
  name: oauth2-authorization-code
  source: https://dev.jiomeet.com/docs/quick-start/integrate_using_oauth_client
scope_count: 6
scope_names:
- user:read
- meeting:create
- meeting:read
- meeting:update
- meeting:delete
- meeting:join
scopes:
- description: Access to user profile information.
  flows: []
  scope: user:read
- description: Create new meetings.
  flows: []
  scope: meeting:create
- description: View meeting details and participants.
  flows: []
  scope: meeting:read
- description: Modify meeting information.
  flows: []
  scope: meeting:update
- description: Remove existing meetings.
  flows: []
  scope: meeting:delete
- description: Access the JioMeet Web SDK for meeting participation.
  flows: []
  scope: meeting:join
slug: reliance-jio-scopes
source_filename: reliance-jio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://dev.jiomeet.com/docs/quick-start/integrate_using_oauth_client\ndocs: https://dev.jiomeet.com/docs/quick-start/integrate_using_oauth_client\ndescription: >-\n  OAuth 2.0 authorization-code scopes for the JioMeet Platform OAuth API. These scopes\n  are documented on Jio's OAuth integration guide, NOT in the machine-readable spec -\n  the harvested OpenAPI models the OAuth API with plain http basic / http bearer\n  security schemes and declares no oauth2 flow object, so the scope list exists only in\n  prose. Scope is nevertheless returned at runtime: the token response carries a `scope`\n  field described as \"the permissions that are granted to the access token\".\n  This applies to the user-authorized JioMeet surface only; the JioMeet Platform Server\n  API and the JioEvents Platform Server API are app-credential JWT surfaces with no\n  scope model at all.\nspec_declares_oauth2_scheme: false\nschemes:\n  - name: oauth2-authorization-code\n\
  \    documented_only: true\n    source: https://dev.jiomeet.com/docs/quick-start/integrate_using_oauth_client\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://jiomeetpro.jio.com/oauth2/authorize\n        tokenUrl: https://jiomeetpro.jio.com/api/oauth2/v2/token\n        token_endpoint_auth: HTTP Basic (clientId as username, clientSecret as password)\n        refresh_supported: true\nscopes:\n  - scope: user:read\n    group: user\n    description: Access to user profile information.\n    operations: ['GET /api/my_profile']\n  - scope: meeting:create\n    group: meeting\n    description: Create new meetings.\n    operations: ['POST /api/meeting']\n  - scope: meeting:read\n    group: meeting\n    description: View meeting details and participants.\n    operations: ['GET /api/meeting/meetingDetails/{meetingId}', 'GET /api/meeting/{userId}']\n  - scope: meeting:update\n    group: meeting\n    description: Modify meeting information.\n    operations: ['PUT /api/meeting/meetingDetails/{meetingId}']\n\
  \  - scope: meeting:delete\n    group: meeting\n    description: Remove existing meetings.\n    operations: ['POST /api/meeting/cancel/{meetingId}']\n  - scope: meeting:join\n    group: meeting\n    description: Access the JioMeet Web SDK for meeting participation.\ntoken_lifetimes:\n  authorization_code: 5 minutes\n  access_token: 1 day\n  refresh_token: 60 days\nredirect_uri_rules:\n  - HTTPS required; plain HTTP rejected.\n  - Raw IP addresses not allowed.\n  - >-\n    Must not contain the query parameters sessionId, token, success, redirect_uri or\n    clientId.\n  - No wildcards, fragments or prohibited special characters.\n  - Must match a URL registered on the OAuth application.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/scopes/reliance-jio-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Telecommunications
- India
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- CPaaS
- Messaging
- Voice
- IoT
- Broadband
- 5G
- BSS
- OSS
- Standards
- Video Conferencing
token_urls:
- https://jiomeetpro.jio.com/api/oauth2/v2/token
---
