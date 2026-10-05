---
authorization_urls: []
description: ''
docs: https://docs.phone.com/aboutdevenv/insidephonecomapi/apisecurity.html
flows:
- oauth2
kind: oauth-scopes
layout: scope
method: searched
name: Phone Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Phone Com publishes 4 OAuth 2.0 scopes via the oauth2 flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Phone Com API on a user''s behalf.


  Tokens are issued from https://api.phone.com/v4/oauth/access-token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Phone Com
provider_slug: phone-com
schemes: []
scope_count: 4
scope_names:
- account-owner
- extension-user
- oauth-management
- methods:ALL
scopes:
- description: Identity/permission tier granting account-owner level access across the account's resources.
  flows: []
  scope: account-owner
- description: Identity/permission tier scoped to a single extension user rather than the whole account.
  flows: []
  scope: extension-user
- description: Required for OAuth token management and API-usage endpoints (list/get/delete access tokens, API statistics, API errors).
  flows: []
  scope: oauth-management
- description: Grants access to all Phone.com API methods.
  flows: []
  scope: methods:ALL
slug: phone-com-scopes
source_filename: phone-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://apidocs.phone.com/docs/access-token\ntype: OAuthScopes\napi: phone-com-api\ndocs: https://docs.phone.com/aboutdevenv/insidephonecomapi/apisecurity.html\nflow: oauth2\ntoken_endpoint: https://api.phone.com/v4/oauth/access-token\nnotes: >-\n  Scopes are provided as a space-separated string when requesting an access\n  token and may be combined. Transcribed from the published Phone.com access\n  token documentation; no machine-readable OpenAPI is published so the\n  derive-oauth-scopes.py baseline could not be generated.\nscopes:\n- name: account-owner\n  description: Identity/permission tier granting account-owner level access across the account's resources.\n- name: extension-user\n  description: Identity/permission tier scoped to a single extension user rather than the whole account.\n- name: oauth-management\n  description: >-\n    Required for OAuth token management and API-usage endpoints (list/get/delete\n    access\
  \ tokens, API statistics, API errors).\n- name: methods:ALL\n  description: Grants access to all Phone.com API methods.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phone-com/refs/heads/main/scopes/phone-com-scopes.yml
summary_line: 4 scopes · oauth2
tags:
- Company
- VoIP
- Telephony
- Business Phone
- SMS
- Video Conferencing
- Communications
token_bound: false
token_urls:
- https://api.phone.com/v4/oauth/access-token
---
