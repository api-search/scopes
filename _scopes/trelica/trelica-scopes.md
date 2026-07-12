---
authorization_urls:
- https://app.trelica.com/connect/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Trelica Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Trelica publishes 9 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Trelica API on a user''s behalf.


  Tokens are issued from https://app.trelica.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Trelica
provider_slug: trelica
schemes:
- description: OAuth 2.0 Client Credentials flow for server-to-server integrations
  flows:
  - flow: clientCredentials
    tokenUrl: https://app.trelica.com/connect/token
  name: OAuth2ClientCredentials
  source: openapi/trelica-rest-api-openapi.yml
- description: OAuth 2.0 Authorization Code flow for third-party developer apps
  flows:
  - authorizationUrl: https://app.trelica.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://app.trelica.com/connect/token
  name: OAuth2AuthorizationCode
  source: openapi/trelica-rest-api-openapi.yml
scope_count: 9
scope_names:
- Apps.Read
- Apps.Users.Read
- Assets.Read
- AuditLog.Read
- Contracts.Read
- People.Read
- People.Write
- Users.Read
- Workflows.Read
scopes:
- description: Read application data
  flows:
  - authorizationCode
  - clientCredentials
  scope: Apps.Read
- description: Read application user data
  flows:
  - authorizationCode
  - clientCredentials
  scope: Apps.Users.Read
- description: Read asset data
  flows:
  - authorizationCode
  - clientCredentials
  scope: Assets.Read
- description: Read audit log entries
  flows:
  - authorizationCode
  - clientCredentials
  scope: AuditLog.Read
- description: Read contract data
  flows:
  - authorizationCode
  - clientCredentials
  scope: Contracts.Read
- description: Read people data
  flows:
  - authorizationCode
  - clientCredentials
  scope: People.Read
- description: Create and update people records
  flows:
  - authorizationCode
  - clientCredentials
  scope: People.Write
- description: Read users via SCIM
  flows:
  - authorizationCode
  - clientCredentials
  scope: Users.Read
- description: Read workflow data
  flows:
  - authorizationCode
  - clientCredentials
  scope: Workflows.Read
slug: trelica-scopes
source_filename: trelica-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trelica-rest-api-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/trelica-rest-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.trelica.com/connect/token\n  description: OAuth 2.0 Client Credentials flow for server-to-server integrations\n- name: OAuth2AuthorizationCode\n  source: openapi/trelica-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.trelica.com/connect/authorize\n    tokenUrl: https://app.trelica.com/connect/token\n  description: OAuth 2.0 Authorization Code flow for third-party developer apps\nscopes:\n- scope: Apps.Read\n  description: Read application data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/trelica-rest-api-openapi.yml\n- scope: Apps.Users.Read\n  description: Read application user data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n\
  \  - openapi/trelica-rest-api-openapi.yml\n- scope: Assets.Read\n  description: Read asset data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/trelica-rest-api-openapi.yml\n- scope: AuditLog.Read\n  description: Read audit log entries\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/trelica-rest-api-openapi.yml\n- scope: Contracts.Read\n  description: Read contract data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/trelica-rest-api-openapi.yml\n- scope: People.Read\n  description: Read people data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/trelica-rest-api-openapi.yml\n- scope: People.Write\n  description: Create and update people records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/trelica-rest-api-openapi.yml\n- scope: Users.Read\n  description: Read users via SCIM\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/trelica-rest-api-openapi.yml\n- scope: Workflows.Read\n  description: Read workflow data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/trelica-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trelica/refs/heads/main/scopes/trelica-scopes.yml
summary_line: 9 scopes · clientCredentials/authorizationCode
tags:
- Contract Management
- IT Management
- License Management
- SaaS Management
- Software Asset Management
token_urls:
- https://app.trelica.com/connect/token
---
