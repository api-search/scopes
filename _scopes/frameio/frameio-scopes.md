---
api_specs:
- filename: frameio-v4-openapi.json
  format: json
  label: Frame.io V4 API
  slug: frameio-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-v4-openapi.json
authorization_urls:
- https://ims-na1.adobelogin.com/ims/authorize/v2
description: ''
docs: https://next.developer.frame.io/platform/v4/docs/guides/authentication/overview
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Frameio Scopes
name_suffix: OAuth Scopes
note: Frame.io delegates auth to Adobe IMS; scopes are coarse Adobe IMS scopes (not fine-grained Frame.io read/write scopes). Server-to-server default scope set is "openid AdobeID frame.s2s.all"; user flows use "openid email profile offline_access additional_info.roles".
overview: 'Frame.io publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Frame.io API on a user''s behalf.


  Tokens are issued from https://ims-na1.adobelogin.com/ims/token/v3.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Frame.io
provider_slug: frameio
schemes:
- description: 'For more information, see: https://developer.adobe.com/frameio'
  flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: OAuth2
  source: openapi/frameio-v4-openapi.json
- description: 'For more information, see: https://developer.adobe.com/frameio'
  flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: bearer
  source: openapi/frameio-v4-openapi.json
- description: Server to server authentication flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: s2s_auth
  source: openapi/frameio-v4-openapi.json
scope_count: 6
scope_names:
- AdobeID
- additional_info.roles
- frame.s2s.all
- offline_access
- openid
- profile
scopes:
- description: Adobe ID
  flows:
  - clientCredentials
  scope: AdobeID
- description: Adobe Commerce Admin
  flows:
  - authorizationCode
  scope: additional_info.roles
- description: Frame.io Server to Server access
  flows:
  - clientCredentials
  scope: frame.s2s.all
- description: Maintain access to the data the user had consented to for refresh tokens
  flows:
  - authorizationCode
  scope: offline_access
- description: Sign in a user
  flows:
  - authorizationCode
  - clientCredentials
  scope: openid
- description: Read the user's basic information
  flows:
  - authorizationCode
  scope: profile
slug: frameio-scopes
source_filename: frameio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/frameio-v4-openapi.json\ndocs: https://next.developer.frame.io/platform/v4/docs/guides/authentication/overview\nnote: Frame.io delegates auth to Adobe IMS; scopes are coarse Adobe IMS scopes (not\n  fine-grained Frame.io read/write scopes). Server-to-server default scope set is\n  \"openid AdobeID frame.s2s.all\"; user flows use \"openid email profile offline_access\n  additional_info.roles\".\nschemes:\n- name: OAuth2\n  source: openapi/frameio-v4-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n  description: 'For more information, see: https://developer.adobe.com/frameio'\n- name: bearer\n  source: openapi/frameio-v4-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n\
  \  description: 'For more information, see: https://developer.adobe.com/frameio'\n- name: s2s_auth\n  source: openapi/frameio-v4-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n  description: Server to server authentication flow\nscopes:\n- scope: AdobeID\n  description: Adobe ID\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/frameio-v4-openapi.json\n- scope: additional_info.roles\n  description: Adobe Commerce Admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/frameio-v4-openapi.json\n- scope: frame.s2s.all\n  description: Frame.io Server to Server access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/frameio-v4-openapi.json\n- scope: offline_access\n  description: Maintain access to the data the user had consented to for refresh tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/frameio-v4-openapi.json\n- scope: openid\n  description: Sign in a user\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/frameio-v4-openapi.json\n- scope: profile\n  description: Read the user's basic information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/frameio-v4-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/scopes/frameio-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Company
- Media
- Video
- Collaboration
- Review and Approval
- Media Production
- Adobe
- Content
token_urls:
- https://ims-na1.adobelogin.com/ims/token/v3
---
