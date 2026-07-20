---
api_specs:
- filename: lithium-care-conversation-api-v2-openapi.json
  format: json
  label: Khoros Care API
  slug: care
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/openapi/lithium-care-conversation-api-v2-openapi.json
- filename: lithium-marketing-conversations-openapi.json
  format: json
  label: Khoros Marketing API
  slug: marketing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/openapi/lithium-marketing-conversations-openapi.json
- filename: lithium-flow-flow-rest-api-openapi.json
  format: json
  label: Khoros Flow API
  slug: flow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/openapi/lithium-flow-flow-rest-api-openapi.json
authorization_urls:
- https://login.spredfast.com/v3/oauth/authorize
description: 'Khoros Marketing is the only product in the Lithium/Khoros surface with an OAuth 2.0 authorization server, and it publishes a single coarse scope. There is no granular read/write or per-resource scope model: `all` grants read/write across every endpoint. Access is narrowed by the tenant headers (x-sf-company-id, x-sf-initiative, x-sf-user-email) and by the permissions of the authorizing user, not by scope.'
docs: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lithium Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lithium publishes 1 OAuth 2.0 scope via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lithium API on a user''s behalf.


  Tokens are issued from https://example.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lithium
provider_slug: lithium
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  source: openapi/lithium-marketing-beta-analytics-api-openapi.json
- flows:
  - authorizationUrl: https://login.spredfast.com/v3/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.spredfast.com/v3/oauth/token
  name: oauth2
  source: openapi/lithium-marketing-conversations-api-v1-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  source: openapi/lithium-marketing-conversations-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  source: openapi/lithium-marketing-crm-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  source: openapi/lithium-marketing-introspection-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  source: openapi/lithium-marketing-labelsets-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  source: openapi/lithium-marketing-notification-service-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  source: openapi/lithium-marketing-stream-api-openapi.json
scope_count: 1
scope_names:
- all
scopes:
- description: Read/write access for all endpoints.
  flows:
  - authorizationCode
  scope: all
slug: lithium-scopes
source_filename: lithium-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lithium-marketing-beta-analytics-api-openapi.json, openapi/lithium-marketing-conversations-api-v1-openapi.json,\n  openapi/lithium-marketing-conversations-openapi.json, openapi/lithium-marketing-crm-openapi.json,\n  openapi/lithium-marketing-introspection-api-openapi.json, openapi/lithium-marketing-labelsets-api-openapi.json,\n  openapi/lithium-marketing-notification-service-openapi.json, openapi/lithium-marketing-stream-api-openapi.json\nschemes:\n- name: sec0\n  source: openapi/lithium-marketing-beta-analytics-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n- name: oauth2\n  source: openapi/lithium-marketing-conversations-api-v1-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.spredfast.com/v3/oauth/authorize\n    tokenUrl: https://login.spredfast.com/v3/oauth/token\n- name: sec0\n  source: openapi/lithium-marketing-conversations-openapi.json\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n- name: sec0\n  source: openapi/lithium-marketing-crm-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n- name: sec0\n  source: openapi/lithium-marketing-introspection-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n- name: sec0\n  source: openapi/lithium-marketing-labelsets-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n- name: sec0\n  source: openapi/lithium-marketing-notification-service-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n- name: sec0\n  source: openapi/lithium-marketing-stream-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\nscopes:\n- scope: all\n  description: Read/write access for all endpoints.\n  flows:\n  -\
  \ authorizationCode\n  sources:\n  - openapi/lithium-marketing-conversations-api-v1-openapi.json\n\ndocs: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api\nintrospection_endpoint: https://api.spredfast.com/v2/whoami\ndescription: >-\n  Khoros Marketing is the only product in the Lithium/Khoros surface with an OAuth 2.0\n  authorization server, and it publishes a single coarse scope. There is no granular\n  read/write or per-resource scope model: `all` grants read/write across every endpoint.\n  Access is narrowed by the tenant headers (x-sf-company-id, x-sf-initiative,\n  x-sf-user-email) and by the permissions of the authorizing user, not by scope.\n\nscope_model:\n  granularity: coarse\n  scope_count: 1\n  least_privilege_supported: false\n  note: >-\n    An agent or integration cannot be issued a read-only Khoros Marketing token. Any token\n    that works is a read/write token for all endpoints the user can reach.\n\ncaveats:\n  - >-\n\
  \    The clientCredentials schemes on seven Marketing definitions carry an empty scopes map\n    and the placeholder tokenUrl https://example.com/oauth2/token (a ReadMe API-designer\n    default). They are not evidence of a second, scopeless authorization server.\n  - >-\n    Khoros Care, Khoros Flow and Khoros Community do not use OAuth 2.0 and therefore have\n    no scope surface — see ../authentication/lithium-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithium/refs/heads/main/scopes/lithium-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode
tags:
- Company
- Martech
- Community
- Social Media
- Customer Engagement
- Customer Support
- Chatbots
- Messaging
- Analytics
- Marketing
token_urls:
- https://example.com/oauth2/token
- https://login.spredfast.com/v3/oauth/token
---
