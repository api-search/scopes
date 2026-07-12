---
authorization_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Defender Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Defender publishes 1 OAuth 2.0 scope via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Defender API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Defender
provider_slug: microsoft-defender
schemes:
- description: OAuth 2.0 authentication using Microsoft Entra ID (Azure AD). Supports both application-level and delegated permissions.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-defender-for-endpoint-api-openapi.yml
scope_count: 1
scope_names:
- https://api.security.microsoft.com/.default
scopes:
- description: Default scope for application permissions
  flows:
  - authorizationCode
  - clientCredentials
  scope: https://api.security.microsoft.com/.default
slug: microsoft-defender-scopes
source_filename: microsoft-defender-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-defender-for-endpoint-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-defender-for-endpoint-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: OAuth 2.0 authentication using Microsoft Entra ID (Azure AD). Supports both application-level\n    and delegated permissions.\nscopes:\n- scope: https://api.security.microsoft.com/.default\n  description: Default scope for application permissions\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/microsoft-defender-for-endpoint-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-defender/refs/heads/main/scopes/microsoft-defender-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode
tags: []
token_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
