---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V3 API
  slug: identity-security-cloud-v3-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v3/identity-security-cloud-v-3-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V2024 API
  slug: identity-security-cloud-v2024-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v2024/identity-security-cloud-v-2024-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V2025 API
  slug: identity-security-cloud-v2025-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v2025/identity-security-cloud-v-2025-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud Beta API
  slug: identity-security-cloud-beta-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/beta/identity-security-cloud-beta-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint IdentityIQ SCIM API
  slug: identityiq-scim-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/iiq/identityiq-scim-rest-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V2026 API
  slug: identity-security-cloud-v2026-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v2026/identity-security-cloud-v-2026-api/
authorization_urls:
- https://{tenant}.identitynow.com/oauth/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Sailpoint Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SailPoint publishes 11 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the SailPoint API on a user''s behalf.


  Tokens are issued from https://{tenant}.api.identitynow.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SailPoint
provider_slug: sailpoint
schemes:
- description: OAuth 2.0 authentication. Use client credentials or authorization code flow to obtain access tokens.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.api.identitynow.com/oauth/token
  - authorizationUrl: https://{tenant}.identitynow.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{tenant}.api.identitynow.com/oauth/token
  name: oauth2
  source: openapi/identity-security-cloud-v3.yml
scope_count: 11
scope_names:
- idn:access-profile:manage
- idn:access-profile:read
- idn:certification:manage
- idn:certification:read
- idn:entitlement:read
- idn:identity-profile:manage
- idn:identity-profile:read
- idn:identity:read
- idn:role-unchecked:manage
- idn:role-unchecked:read
- idn:sources:read
scopes:
- description: Manage access profiles
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:access-profile:manage
- description: Read access profiles
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:access-profile:read
- description: Manage certifications
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:certification:manage
- description: Read certifications
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:certification:read
- description: Read entitlements
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:entitlement:read
- description: Manage identity profiles
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:identity-profile:manage
- description: Read identity profiles
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:identity-profile:read
- description: Read identity information
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:identity:read
- description: Manage roles
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:role-unchecked:manage
- description: Read roles
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:role-unchecked:read
- description: Read sources
  flows:
  - authorizationCode
  - clientCredentials
  scope: idn:sources:read
slug: sailpoint-scopes
source_filename: sailpoint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/identity-security-cloud-v3.yml\nschemes:\n- name: oauth2\n  source: openapi/identity-security-cloud-v3.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.api.identitynow.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.identitynow.com/oauth/authorize\n    tokenUrl: https://{tenant}.api.identitynow.com/oauth/token\n  description: OAuth 2.0 authentication. Use client credentials or authorization code flow to\n    obtain access tokens.\nscopes:\n- scope: idn:access-profile:manage\n  description: Manage access profiles\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- scope: idn:access-profile:read\n  description: Read access profiles\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- scope: idn:certification:manage\n  description: Manage\
  \ certifications\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- scope: idn:certification:read\n  description: Read certifications\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- scope: idn:entitlement:read\n  description: Read entitlements\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- scope: idn:identity-profile:manage\n  description: Manage identity profiles\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- scope: idn:identity-profile:read\n  description: Read identity profiles\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- scope: idn:identity:read\n  description: Read identity information\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n\
  \  - openapi/identity-security-cloud-v3.yml\n- scope: idn:role-unchecked:manage\n  description: Manage roles\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- scope: idn:role-unchecked:read\n  description: Read roles\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n- scope: idn:sources:read\n  description: Read sources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/identity-security-cloud-v3.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sailpoint/refs/heads/main/scopes/sailpoint-scopes.yml
summary_line: 11 scopes · clientCredentials/authorizationCode
tags:
- Access Governance
- Compliance
- IAM
- Identity Management
- Identity Security
- Security
token_urls:
- https://{tenant}.api.identitynow.com/oauth/token
---
