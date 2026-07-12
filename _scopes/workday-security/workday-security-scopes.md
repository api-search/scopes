---
authorization_urls:
- https://{host}/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Workday Security Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Security publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Security API on a user''s behalf.


  Tokens are issued from https://{host}/ccx/oauth2/{tenant}/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Security
provider_slug: workday-security
schemes:
- description: OAuth 2.0 authorization code flow for obtaining access tokens to Workday REST APIs.
  flows:
  - authorizationUrl: https://{host}/authorize
    flow: authorizationCode
    tokenUrl: https://{host}/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-security-authentication-openapi.yml
scope_count: 3
scope_names:
- Integration
- System
- Tenant_Non-Configurable
scopes:
- description: Access to integration resources
  flows:
  - authorizationCode
  scope: Integration
- description: Access to system-level resources
  flows:
  - authorizationCode
  scope: System
- description: Access to tenant non-configurable resources
  flows:
  - authorizationCode
  scope: Tenant_Non-Configurable
slug: workday-security-scopes
source_filename: workday-security-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-security-authentication-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/workday-security-authentication-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{host}/authorize\n    tokenUrl: https://{host}/ccx/oauth2/{tenant}/token\n  description: OAuth 2.0 authorization code flow for obtaining access tokens to Workday REST\n    APIs.\nscopes:\n- scope: Integration\n  description: Access to integration resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-security-authentication-openapi.yml\n- scope: System\n  description: Access to system-level resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-security-authentication-openapi.yml\n- scope: Tenant_Non-Configurable\n  description: Access to tenant non-configurable resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-security-authentication-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/scopes/workday-security-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Access Control
- Audit
- Authentication
- Compliance
- Enterprise
- Identity Management
- Privacy
- SAML
- Security
- SSO
token_urls:
- https://{host}/ccx/oauth2/{tenant}/token
---
