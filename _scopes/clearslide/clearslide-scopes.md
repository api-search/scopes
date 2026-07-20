---
api_specs:
- filename: clearslide-openapi.yml
  format: yaml
  label: ClearSlide Platform API
  slug: clearslide-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-openapi.yml
authorization_urls:
- https://oauth.platform.clearslide.com/oauth/authorize
description: ''
docs: https://developer.clearslide.com/docs/oauth-20
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: searched
name: Clearslide Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ClearSlide publishes 2 OAuth 2.0 scopes via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClearSlide API on a user''s behalf.


  Tokens are issued from https://oauth.platform.clearslide.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClearSlide
provider_slug: clearslide
schemes:
- description: ClearSlide supports OAuth 2.0 Authorization Code (RFC 6749 §4.1) and Resource Owner Password Credentials (RFC 6749 §4.3) grants. Register a client redirect URL with apisupport@clearslide.com to receive a client id and client secret.
  flows:
  - authorizationUrl: https://oauth.platform.clearslide.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://oauth.platform.clearslide.com/oauth/token
  - flow: password
    tokenUrl: https://oauth.platform.clearslide.com/oauth/token
  name: oauth2
  source: openapi/clearslide-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to ClearSlide resources
  flows:
  - authorizationCode
  - password
  scope: read
- description: Write access to ClearSlide resources
  flows:
  - authorizationCode
  - password
  scope: write
slug: clearslide-scopes
source_filename: clearslide-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/clearslide-openapi.yml\ndocs: https://developer.clearslide.com/docs/oauth-20\nschemes:\n- name: oauth2\n  source: openapi/clearslide-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.platform.clearslide.com/oauth/authorize\n    tokenUrl: https://oauth.platform.clearslide.com/oauth/token\n  - flow: password\n    tokenUrl: https://oauth.platform.clearslide.com/oauth/token\n  description: ClearSlide supports OAuth 2.0 Authorization Code (RFC 6749 §4.1) and Resource\n    Owner Password Credentials (RFC 6749 §4.3) grants. Register a client redirect URL with apisupport@clearslide.com\n    to receive a client id and client secret.\nscopes:\n- scope: read\n  description: Read access to ClearSlide resources\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/clearslide-openapi.yml\n- scope: write\n  description: Write access to ClearSlide resources\n  flows:\n  - authorizationCode\n\
  \  - password\n  sources:\n  - openapi/clearslide-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/scopes/clearslide-scopes.yml
summary_line: 2 scopes · authorizationCode/password
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
