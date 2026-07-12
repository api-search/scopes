---
authorization_urls:
- https://ims-na1.adobelogin.com/ims/authorize/v2
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Adobe Premiere Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adobe Premiere Pro publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adobe Premiere Pro API on a user''s behalf.


  Tokens are issued from https://ims-na1.adobelogin.com/ims/token/v3.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
schemes:
- flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  source: openapi/adobe-premiere-creative-cloud-libraries-openapi.yml
scope_count: 3
scope_names:
- creative_sdk
- openid
- profile
scopes:
- description: Access Creative Cloud Libraries
  flows:
  - authorizationCode
  scope: creative_sdk
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: User profile access
  flows:
  - authorizationCode
  scope: profile
slug: adobe-premiere-scopes
source_filename: adobe-premiere-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-premiere-creative-cloud-libraries-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/adobe-premiere-creative-cloud-libraries-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\nscopes:\n- scope: creative_sdk\n  description: Access Creative Cloud Libraries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-premiere-creative-cloud-libraries-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-premiere-creative-cloud-libraries-openapi.yml\n- scope: profile\n  description: User profile access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-premiere-creative-cloud-libraries-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/scopes/adobe-premiere-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
token_urls:
- https://ims-na1.adobelogin.com/ims/token/v3
---
