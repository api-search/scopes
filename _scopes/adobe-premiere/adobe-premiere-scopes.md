---
api_specs:
- filename: adobe-premiere-elements-api-openapi.yml
  format: yaml
  label: Adobe Premiere Pro Elements API
  slug: adobe-premiere-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/openapi/adobe-premiere-elements-api-openapi.yml
- filename: adobe-premiere-libraries-api-openapi.yml
  format: yaml
  label: Adobe Premiere Pro Libraries API
  slug: adobe-premiere-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/openapi/adobe-premiere-libraries-api-openapi.yml
- filename: adobe-premiere-representations-api-openapi.yml
  format: yaml
  label: Adobe Premiere Pro Representations API
  slug: adobe-premiere-representations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/openapi/adobe-premiere-representations-api-openapi.yml
- filename: adobe-premiere-cc-libraries-api-openapi.json
  format: json
  label: Adobe Creative Cloud Libraries API
  slug: adobe-creative-cloud-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/openapi/adobe-premiere-cc-libraries-api-openapi.json
authorization_urls:
- https://ims-na1.adobelogin.com/ims/authorize/v2
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Adobe Premiere Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adobe Premiere Pro publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adobe Premiere Pro API on a user''s behalf.


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
  source: openapi/adobe-premiere-elements-api-openapi.yml
- flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  source: openapi/adobe-premiere-libraries-api-openapi.yml
- flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  source: openapi/adobe-premiere-representations-api-openapi.yml
scope_count: 4
scope_names:
- creative_sdk
- openid
- profile
- AdobeID
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
- description: Core Adobe Identity Management System scope required alongside openid for an authorization-code flow against Adobe IMS.
  flows:
  - authorizationCode
  scope: AdobeID
slug: adobe-premiere-scopes
source_filename: adobe-premiere-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: openapi/adobe-premiere-elements-api-openapi.yml, openapi/adobe-premiere-libraries-api-openapi.yml,\n  openapi/adobe-premiere-representations-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/adobe-premiere-elements-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n- name: oauth2\n  source: openapi/adobe-premiere-libraries-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n- name: oauth2\n  source: openapi/adobe-premiere-representations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\nscopes:\n- scope: creative_sdk\n\
  \  description: Access Creative Cloud Libraries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-premiere-elements-api-openapi.yml\n  - openapi/adobe-premiere-libraries-api-openapi.yml\n  - openapi/adobe-premiere-representations-api-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-premiere-elements-api-openapi.yml\n  - openapi/adobe-premiere-libraries-api-openapi.yml\n  - openapi/adobe-premiere-representations-api-openapi.yml\n- scope: profile\n  description: User profile access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-premiere-elements-api-openapi.yml\n  - openapi/adobe-premiere-libraries-api-openapi.yml\n  - openapi/adobe-premiere-representations-api-openapi.yml\n- scope: AdobeID\n  description: >-\n    Core Adobe Identity Management System scope required alongside openid for an authorization-code\n    flow against Adobe IMS.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - https://developer.adobe.com/creative-cloud-libraries/docs/integrate/setup/oauth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/scopes/adobe-premiere-scopes.yml
summary_line: 4 scopes · authorizationCode
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
