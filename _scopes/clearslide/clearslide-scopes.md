---
api_specs:
- filename: clearslide-insights-api-openapi.yml
  format: yaml
  label: ClearSlide Insights API
  slug: clearslide-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-insights-api-openapi.yml
- filename: clearslide-links-api-openapi.yml
  format: yaml
  label: ClearSlide Links API
  slug: clearslide-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-links-api-openapi.yml
- filename: clearslide-meetings-api-openapi.yml
  format: yaml
  label: ClearSlide Meetings API
  slug: clearslide-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-meetings-api-openapi.yml
- filename: clearslide-presentations-api-openapi.yml
  format: yaml
  label: ClearSlide Presentations API
  slug: clearslide-presentations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-presentations-api-openapi.yml
- filename: clearslide-upload-api-openapi.yml
  format: yaml
  label: ClearSlide Upload API
  slug: clearslide-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-upload-api-openapi.yml
- filename: clearslide-users-api-openapi.yml
  format: yaml
  label: ClearSlide Users API
  slug: clearslide-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-users-api-openapi.yml
authorization_urls:
- https://oauth.platform.clearslide.com/oauth/authorize
description: ''
docs: https://developer.clearslide.com/docs/oauth-20
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Clearslide Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ClearSlide publishes 2 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClearSlide API on a user''s behalf.


  Tokens are issued from https://oauth.platform.clearslide.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClearSlide
provider_slug: clearslide
schemes:
- authorization_server: https://oauth.platform.clearslide.com
  correction: A `password` (Resource Owner Password Credentials) flow was recorded in the prior round. It is not documented on either of ClearSlide's published OAuth pages and has been removed.
  description: ClearSlide supports the OAuth 2.0 Authorization Code grant (RFC 6749 §4.1) and refresh_token grant. Register a client redirect URL with apisupport@clearslide.com to receive a client id and client secret.
  flows:
  - authorizationUrl: https://oauth.platform.clearslide.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://oauth.platform.clearslide.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://oauth.platform.clearslide.com/oauth/token
  name: oauth2
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to ClearSlide resources.
  flows:
  - authorizationCode
  - refreshToken
  scope: read
- description: Write access to ClearSlide resources.
  flows:
  - authorizationCode
  - refreshToken
  scope: write
slug: clearslide-scopes
source_filename: clearslide-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.platform.clearslide.com/oauth2.html and https://developer.clearslide.com/docs/oauth-20\ndocs: https://developer.clearslide.com/docs/oauth-20\nscope_count: 2\ngranularity: coarse\nschemes:\n- name: oauth2\n  authorization_server: https://oauth.platform.clearslide.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.platform.clearslide.com/oauth/authorize\n    tokenUrl: https://oauth.platform.clearslide.com/oauth/token\n  - flow: refreshToken\n    tokenUrl: https://oauth.platform.clearslide.com/oauth/token\n  description: >-\n    ClearSlide supports the OAuth 2.0 Authorization Code grant (RFC 6749 §4.1) and refresh_token\n    grant. Register a client redirect URL with apisupport@clearslide.com to receive a client id\n    and client secret.\n  correction: >-\n    A `password` (Resource Owner Password Credentials) flow was recorded in the prior round. It is\n    not documented on either\
  \ of ClearSlide's published OAuth pages and has been removed.\nscopes:\n- scope: read\n  description: Read access to ClearSlide resources.\n  flows: [authorizationCode, refreshToken]\n  observed_in: token response \"scope\":\"read write\"\n  sources:\n  - https://docs.platform.clearslide.com/oauth2.html\n- scope: write\n  description: Write access to ClearSlide resources.\n  flows: [authorizationCode, refreshToken]\n  observed_in: token response \"scope\":\"read write\"\n  sources:\n  - https://docs.platform.clearslide.com/oauth2.html\nscope_to_operation:\n  published: false\n  note: >-\n    ClearSlide publishes no mapping from scope to operation. The Swagger document declares no\n    securityDefinitions and no per-operation security, so which scope any given call requires is\n    undocumented. The mapping below is our reading of read-vs-write semantics, not a provider\n    statement.\n  inferred:\n  - scope: read\n    operations: [GET /presentations, GET /insights, GET /users, \"GET /upload/{uploadID}\"\
  , GET /meeting/scheduled]\n  - scope: write\n    operations: [POST /links, POST /upload, POST /meeting/scheduled, \"PUT /meeting/scheduled/{inviteMailVid}\"]\nfindings:\n- >-\n  Two scopes cover the entire platform. The same `write` scope that creates a trackable link also\n  covers SCIM user and group provisioning — creating, deactivating and deleting directory users —\n  so a token issued for content sharing carries directory-administration authority.\n- >-\n  No scope is documented for the SCIM surface at all, despite it being the highest-privilege\n  surface ClearSlide exposes.\ngaps:\n- No scope reference page exists on the developer portal.\n- No incremental or step-up authorisation is documented.\n- No way for a consumer to request a reduced scope for a narrow integration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/scopes/clearslide-scopes.yml
summary_line: 2 scopes · authorizationCode/refreshToken
tags:
- Company
- Sales Engagement
- Sales Enablement
- Content Management
- Presentations
- Analytics
- Meetings
- CRM
- OAuth
- SCIM
token_urls:
- https://oauth.platform.clearslide.com/oauth/token
---
