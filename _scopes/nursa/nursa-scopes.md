---
api_specs:
- filename: nursa-clinicians-api-openapi.yml
  format: yaml
  label: Nursa Clinicians API
  slug: nursa-clinicians-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-clinicians-api-openapi.yml
- filename: nursa-downloads-api-openapi.yml
  format: yaml
  label: Nursa Downloads API
  slug: nursa-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-downloads-api-openapi.yml
- filename: nursa-facilities-api-openapi.yml
  format: yaml
  label: Nursa Facilities API
  slug: nursa-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-facilities-api-openapi.yml
- filename: nursa-facilities-webhooks-api-openapi.yml
  format: yaml
  label: Nursa Facilities webhooks API
  slug: nursa-facilities-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-facilities-webhooks-api-openapi.yml
- filename: nursa-licenses-api-openapi.yml
  format: yaml
  label: Nursa Licenses API
  slug: nursa-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-licenses-api-openapi.yml
- filename: nursa-marketplace-api-openapi.yml
  format: yaml
  label: Nursa Marketplace API
  slug: nursa-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-marketplace-api-openapi.yml
- filename: nursa-scheduled-shifts-api-openapi.yml
  format: yaml
  label: Nursa Scheduled shifts API
  slug: nursa-scheduled-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-scheduled-shifts-api-openapi.yml
- filename: nursa-shift-reports-api-openapi.yml
  format: yaml
  label: Nursa Shift reports API
  slug: nursa-shift-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-shift-reports-api-openapi.yml
- filename: nursa-shift-requests-api-openapi.yml
  format: yaml
  label: Nursa Shift requests API
  slug: nursa-shift-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-shift-requests-api-openapi.yml
- filename: nursa-shifts-api-openapi.yml
  format: yaml
  label: Nursa Shifts API
  slug: nursa-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-shifts-api-openapi.yml
- filename: nursa-support-api-openapi.yml
  format: yaml
  label: Nursa Support API
  slug: nursa-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-support-api-openapi.yml
- filename: nursa-user-webhooks-api-openapi.yml
  format: yaml
  label: Nursa User webhooks API
  slug: nursa-user-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-user-webhooks-api-openapi.yml
- filename: nursa-webhook-logs-api-openapi.yml
  format: yaml
  label: Nursa Webhook logs API
  slug: nursa-webhook-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/openapi/nursa-webhook-logs-api-openapi.yml
authorization_urls:
- https://auth.nursa.com/oidc/authorize
description: ''
docs: https://docs.nursa.com/docs/Integration%20Guideline/Scopes/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Nursa Scopes
name_suffix: OAuth Scopes
note: 'Nursa''s OpenAPI declares no oauth2 securityScheme, so no scope is derivable from the spec — 0-working/derive-oauth-scopes.py returns "with oauth2: 0". Every scope below was read from the provider''s published Scopes reference. The OIDC discovery document advertises only the seven UserInfo/OIDC scopes in `scopes_supported`; the twenty resource scopes are documented in prose and are NOT advertised in discovery, so an OAuth client cannot enumerate them programmatically.'
overview: 'Nursa publishes 26 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nursa API on a user''s behalf.


  Tokens are issued from https://auth.nursa.com/oidc/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nursa
provider_slug: nursa
schemes:
- flows:
  - authorizationUrl: https://auth.nursa.com/oidc/authorize
    flow: authorizationCode
    tokenUrl: https://auth.nursa.com/oidc/oauth/token
  - flow: clientCredentials
    note: enabled per-application on request only
    tokenUrl: https://auth.nursa.com/oidc/oauth/token
  name: nursa-oidc
  source: https://auth.nursa.com/oidc/.well-known/openid-configuration
  type: openIdConnect
scope_count: 26
scope_names:
- openid
- profile
- email
- phone
- address
- role
- offline_access
- marketplace:write
- marketplace:read
- marketplace-policy:write
- marketplace-policy:read
- shift-requests:write
- shift-requests:read
- shift-reports:write
- shift-reports:read
- facilities:write
- facilities:read
- finances:write
- finances:read
- communication-policy:write
- communication-policy:read
- permissions:write
- permissions:read
- integrations:write
- oidc-application:write
- oidc-application:read
scopes:
- description: Returns the sub claim, which uniquely identifies the user. In an ID Token, iss, aud, exp, iat and at_hash are also present.
  flows: []
  scope: openid
- description: Returns basic profile claims — name, nickname, picture.
  flows: []
  scope: profile
- description: Returns the email claim.
  flows: []
  scope: email
- description: Returns the phone_number claim.
  flows: []
  scope: phone
- description: Returns the address claim — an object with city and state.
  flows: []
  scope: address
- description: Returns the role claim; NURSE_USER or FACILITY_USER.
  flows: []
  scope: role
- description: Returns a refresh_token from the Get Token endpoint.
  flows: []
  scope: offline_access
- description: User allows your application to post and update shifts on their behalf.
  flows: []
  scope: marketplace:write
- description: User allows your application to read shifts on their behalf.
  flows: []
  scope: marketplace:read
- description: User allows your application to manage shift policy on their behalf.
  flows: []
  scope: marketplace-policy:write
- description: User allows your application to read shift policy on their behalf.
  flows: []
  scope: marketplace-policy:read
- description: User allows your application to manage shift requests on their behalf.
  flows: []
  scope: shift-requests:write
- description: User allows your application to read shift requests on their behalf.
  flows: []
  scope: shift-requests:read
- description: User allows your application to manage shift reports on their behalf.
  flows: []
  scope: shift-reports:write
- description: User allows your application to read shift reports on their behalf.
  flows: []
  scope: shift-reports:read
- description: User allows your application to manage the facility profile on their behalf.
  flows: []
  scope: facilities:write
- description: User allows your application to read the facility profile on their behalf.
  flows: []
  scope: facilities:read
- description: User allows your application to manage the facility's financial information on their behalf.
  flows: []
  scope: finances:write
- description: User allows your application to read the facility's financial information on their behalf.
  flows: []
  scope: finances:read
- description: User allows your application to manage the communication policy on their behalf.
  flows: []
  scope: communication-policy:write
- description: User allows your application to read the communication policy on their behalf.
  flows: []
  scope: communication-policy:read
- description: User allows your application to manage the user permissions under an organization on their behalf.
  flows: []
  scope: permissions:write
- description: User allows your application to read the user permissions under an organization on their behalf.
  flows: []
  scope: permissions:read
- description: User allows your application to manage the integration settings of the organization on their behalf.
  flows: []
  scope: integrations:write
- description: User allows your application to manage the OpenID Connect applications of the organization on their behalf.
  flows: []
  scope: oidc-application:write
- description: User allows your application to read the OpenID Connect applications of the organization on their behalf.
  flows: []
  scope: oidc-application:read
slug: nursa-scopes
source_filename: nursa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://docs.nursa.com/docs/Integration%20Guideline/Scopes/\ndocs: https://docs.nursa.com/docs/Integration%20Guideline/Scopes/\ndiscovery: well-known/nursa-openid-configuration.json\nnote: >-\n  Nursa's OpenAPI declares no oauth2 securityScheme, so no scope is derivable from the spec —\n  0-working/derive-oauth-scopes.py returns \"with oauth2: 0\". Every scope below was read from the\n  provider's published Scopes reference. The OIDC discovery document advertises only the seven\n  UserInfo/OIDC scopes in `scopes_supported`; the twenty resource scopes are documented in prose\n  and are NOT advertised in discovery, so an OAuth client cannot enumerate them programmatically.\nschemes:\n- name: nursa-oidc\n  type: openIdConnect\n  source: https://auth.nursa.com/oidc/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.nursa.com/oidc/authorize\n    tokenUrl: https://auth.nursa.com/oidc/oauth/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://auth.nursa.com/oidc/oauth/token\n    note: enabled per-application on request only\nenforcement:\n  granted: HTTP 2xx\n  missing_scope: HTTP 403 Forbidden Resource\n  consent: >-\n    Scopes are requested in the `scope` parameter of the authorization request; the authorization\n    server may show a consent screen and the user may deny all or part of the request. The granted\n    set lands in the access token's `scope` claim.\nscopes:\n- scope: openid\n  description: Returns the sub claim, which uniquely identifies the user. In an ID Token, iss, aud, exp, iat and at_hash are also present.\n  category: openid\n  advertised_in_discovery: true\n- scope: profile\n  description: Returns basic profile claims — name, nickname, picture.\n  category: openid\n  advertised_in_discovery: true\n- scope: email\n  description: Returns the email claim.\n  category: openid\n  advertised_in_discovery: true\n- scope: phone\n  description: Returns the phone_number\
  \ claim.\n  category: openid\n  advertised_in_discovery: true\n- scope: address\n  description: Returns the address claim — an object with city and state.\n  category: openid\n  advertised_in_discovery: true\n- scope: role\n  description: Returns the role claim; NURSE_USER or FACILITY_USER.\n  category: openid\n  advertised_in_discovery: true\n- scope: offline_access\n  description: Returns a refresh_token from the Get Token endpoint.\n  category: openid\n  advertised_in_discovery: true\n- scope: marketplace:write\n  name: Post Shifts\n  description: User allows your application to post and update shifts on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: marketplace:read\n  name: View Posted Shifts\n  description: User allows your application to read shifts on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: marketplace-policy:write\n  name: Manage Shift Policy\n  description: User allows your application to manage shift policy\
  \ on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: marketplace-policy:read\n  name: View Shift Policy\n  description: User allows your application to read shift policy on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: shift-requests:write\n  name: Manage Shift Requests\n  description: User allows your application to manage shift requests on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: shift-requests:read\n  name: View Shift Requests\n  description: User allows your application to read shift requests on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: shift-reports:write\n  name: Manage Shift Reports\n  description: User allows your application to manage shift reports on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: shift-reports:read\n  name: View Shift Reports\n  description: User allows your application to read shift reports\
  \ on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: facilities:write\n  name: Manage Facility Profile\n  description: User allows your application to manage the facility profile on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: facilities:read\n  name: View Facility Profile\n  description: User allows your application to read the facility profile on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: finances:write\n  name: Manage Financial Information\n  description: User allows your application to manage the facility's financial information on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: finances:read\n  name: View Financial Information\n  description: User allows your application to read the facility's financial information on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: communication-policy:write\n  name: Manage Communication\
  \ Policy\n  description: User allows your application to manage the communication policy on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: communication-policy:read\n  name: View Communication Policy\n  description: User allows your application to read the communication policy on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: permissions:write\n  name: Manage Permissions\n  description: User allows your application to manage the user permissions under an organization on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: permissions:read\n  name: View Permissions\n  description: User allows your application to read the user permissions under an organization on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: integrations:write\n  name: Manage Integrations\n  description: User allows your application to manage the integration settings of the organization on their\
  \ behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: oidc-application:write\n  name: Manage OIDC Applications\n  description: User allows your application to manage the OpenID Connect applications of the organization on their behalf.\n  category: resource\n  advertised_in_discovery: false\n- scope: oidc-application:read\n  name: View OIDC Applications\n  description: User allows your application to read the OpenID Connect applications of the organization on their behalf.\n  category: resource\n  advertised_in_discovery: false\ncoverage:\n  total: 27\n  openid: 7\n  resource: 20\n  read_write_pairs: 9\n  write_only: 1\ngaps:\n- >-\n  No operation-to-scope binding is published anywhere machine-readable. The docs say \"The API\n  documentation will define which scopes will be requested for each endpoint\", but the OpenAPI's\n  only security requirement is `public-api: []` — an empty scope array on all 40 operations. An\n  agent or client cannot compute least privilege\
  \ from the contract.\n- >-\n  `integrations:write` has no matching `integrations:read`, unlike every other resource family.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - url: https://docs.nursa.com/docs/Integration%20Guideline/Scopes/\n    status: 200\n  - url: https://auth.nursa.com/oidc/.well-known/openid-configuration\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nursa/refs/heads/main/scopes/nursa-scopes.yml
summary_line: 26 scopes · authorizationCode/clientCredentials
tags:
- Company
- Healthcare
- Health
- Staffing
- Nursing
- Marketplace
- Workforce Management
- Scheduling
- Human Resources
- Per Diem
- Shifts
- Webhook
token_urls:
- https://auth.nursa.com/oidc/oauth/token
---
