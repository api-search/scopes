---
api_specs:
- filename: rest.apidoc.blueconic.com
  format: yaml
  label: BlueConic REST API v2
  slug: blueconic-rest-api-v2
  spec_type: OpenAPI
  url: https://rest.apidoc.blueconic.com
authorization_urls:
- /rest/v2/oauth/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Blueconic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BlueConic publishes 27 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the BlueConic API on a user''s behalf.


  Tokens are issued from /rest/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BlueConic
provider_slug: blueconic
schemes:
- description: 'Authenticates a registered OAuth 2.0 client. The Authorization code flow and Client credentials flow are supported. Make sure to select the correct flow based on which flow the registered client supports. The client id and client secret can be found in BlueConic by opening the registered client under *Settings* > *Access management* > *Applications*.<br/>**NOTE:** When using the Authorization code flow, the redirect URL of the registered client in BlueConic must be set to `https://rest.apidoc.blueconic.com/oauth-receiver.html` and ''Send Proof Key for Code Exchange'' must be enabled.<br/><br/>To use a Bearer token for authentication, follow these steps: <br/>1. Acquire the token through authentication.<br/>2. Include the token in the request''s Authorization header as Bearer \<token\>.<br/>3. Send the request to access protected resources.<br/>4. Handle token expiration by refreshing or obtaining a new token.'
  flows:
  - flow: clientCredentials
    tokenUrl: /rest/v2/oauth/token
  - authorizationUrl: /rest/v2/oauth/authorize
    flow: authorizationCode
    tokenUrl: /rest/v2/oauth/token
  name: oauth2
  source: openapi/blueconic-rest-api-v2-openapi.yml
scope_count: 27
scope_names:
- read:audit-events
- read:channels
- read:connections
- read:content_stores
- read:dialogues
- read:group-types
- read:groups
- read:lifecycles
- read:listeners
- read:models
- read:notebooks
- read:objectives
- read:plugins
- read:profile-properties
- read:profiles
- read:roles
- read:segments
- read:timeline-event-types
- read:timeline_event_rollups
- read:url-mappings
- read:users
- write:content_stores
- write:groups
- write:models
- write:profile-properties
- write:profiles
- write:url-mappings
scopes:
- description: ''
  flows: []
  scope: read:audit-events
- description: ''
  flows: []
  scope: read:channels
- description: ''
  flows: []
  scope: read:connections
- description: ''
  flows: []
  scope: read:content_stores
- description: ''
  flows: []
  scope: read:dialogues
- description: ''
  flows: []
  scope: read:group-types
- description: ''
  flows: []
  scope: read:groups
- description: ''
  flows: []
  scope: read:lifecycles
- description: ''
  flows: []
  scope: read:listeners
- description: ''
  flows: []
  scope: read:models
- description: ''
  flows: []
  scope: read:notebooks
- description: ''
  flows: []
  scope: read:objectives
- description: ''
  flows: []
  scope: read:plugins
- description: ''
  flows: []
  scope: read:profile-properties
- description: ''
  flows: []
  scope: read:profiles
- description: ''
  flows: []
  scope: read:roles
- description: ''
  flows: []
  scope: read:segments
- description: ''
  flows: []
  scope: read:timeline-event-types
- description: ''
  flows: []
  scope: read:timeline_event_rollups
- description: ''
  flows: []
  scope: read:url-mappings
- description: ''
  flows: []
  scope: read:users
- description: ''
  flows: []
  scope: write:content_stores
- description: ''
  flows: []
  scope: write:groups
- description: ''
  flows: []
  scope: write:models
- description: ''
  flows: []
  scope: write:profile-properties
- description: ''
  flows: []
  scope: write:profiles
- description: ''
  flows: []
  scope: write:url-mappings
slug: blueconic-scopes
source_filename: blueconic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blueconic-rest-api-v2-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/blueconic-rest-api-v2-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /rest/v2/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /rest/v2/oauth/authorize\n    tokenUrl: /rest/v2/oauth/token\n  description: 'Authenticates a registered OAuth 2.0 client. The Authorization code flow and\n    Client credentials flow are supported. Make sure to select the correct flow based on which\n    flow the registered client supports. The client id and client secret can be found in BlueConic\n    by opening the registered client under *Settings* > *Access management* > *Applications*.<br/>**NOTE:**\n    When using the Authorization code flow, the redirect URL of the registered client in BlueConic\n    must be set to `https://rest.apidoc.blueconic.com/oauth-receiver.html` and ''Send Proof\n    Key for Code Exchange'' must be\
  \ enabled.<br/><br/>To use a Bearer token for authentication,\n    follow these steps: <br/>1. Acquire the token through authentication.<br/>2. Include the\n    token in the request''s Authorization header as Bearer \\<token\\>.<br/>3. Send the request\n    to access protected resources.<br/>4. Handle token expiration by refreshing or obtaining\n    a new token.'\nscopes:\n- scope: read:audit-events\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:channels\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:connections\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:content_stores\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:dialogues\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:group-types\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:groups\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:lifecycles\n \
  \ sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:listeners\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:models\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:notebooks\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:objectives\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:plugins\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:profile-properties\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:profiles\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:roles\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:segments\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:timeline-event-types\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:timeline_event_rollups\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n\
  - scope: read:url-mappings\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: read:users\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: write:content_stores\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: write:groups\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: write:models\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: write:profile-properties\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: write:profiles\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n- scope: write:url-mappings\n  sources:\n  - openapi/blueconic-rest-api-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueconic/refs/heads/main/scopes/blueconic-scopes.yml
summary_line: 27 scopes · clientCredentials/authorizationCode
tags:
- Customer Data Platform
- CDP
- Customer Profiles
- Segments
- Data Activation
- First-Party Data
- Lifecycle Stages
- Connections
- Privacy
token_urls:
- /rest/v2/oauth/token
---
