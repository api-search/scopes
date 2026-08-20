---
api_specs:
- filename: outline-accessrequests-api-openapi.yml
  format: yaml
  label: Outline AccessRequests API
  slug: outline-accessrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-accessrequests-api-openapi.yml
- filename: outline-attachments-api-openapi.yml
  format: yaml
  label: Outline Attachments API
  slug: outline-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-attachments-api-openapi.yml
- filename: outline-auth-api-openapi.yml
  format: yaml
  label: Outline Auth API
  slug: outline-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-auth-api-openapi.yml
- filename: outline-collections-api-openapi.yml
  format: yaml
  label: Outline Collections API
  slug: outline-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-collections-api-openapi.yml
- filename: outline-comments-api-openapi.yml
  format: yaml
  label: Outline Comments API
  slug: outline-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-comments-api-openapi.yml
- filename: outline-dataattributes-api-openapi.yml
  format: yaml
  label: Outline DataAttributes API
  slug: outline-dataattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-dataattributes-api-openapi.yml
- filename: outline-documents-api-openapi.yml
  format: yaml
  label: Outline Documents API
  slug: outline-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-documents-api-openapi.yml
- filename: outline-events-api-openapi.yml
  format: yaml
  label: Outline Events API
  slug: outline-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-events-api-openapi.yml
- filename: outline-fileoperations-api-openapi.yml
  format: yaml
  label: Outline FileOperations API
  slug: outline-fileoperations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-fileoperations-api-openapi.yml
- filename: outline-groups-api-openapi.yml
  format: yaml
  label: Outline Groups API
  slug: outline-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-groups-api-openapi.yml
- filename: outline-oauthauthentications-api-openapi.yml
  format: yaml
  label: Outline OAuthAuthentications API
  slug: outline-oauthauthentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-oauthauthentications-api-openapi.yml
- filename: outline-oauthclients-api-openapi.yml
  format: yaml
  label: Outline OAuthClients API
  slug: outline-oauthclients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-oauthclients-api-openapi.yml
- filename: outline-revisions-api-openapi.yml
  format: yaml
  label: Outline Revisions API
  slug: outline-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-revisions-api-openapi.yml
- filename: outline-shares-api-openapi.yml
  format: yaml
  label: Outline Shares API
  slug: outline-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-shares-api-openapi.yml
- filename: outline-stars-api-openapi.yml
  format: yaml
  label: Outline Stars API
  slug: outline-stars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-stars-api-openapi.yml
- filename: outline-templates-api-openapi.yml
  format: yaml
  label: Outline Templates API
  slug: outline-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-templates-api-openapi.yml
- filename: outline-users-api-openapi.yml
  format: yaml
  label: Outline Users API
  slug: outline-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-users-api-openapi.yml
- filename: outline-views-api-openapi.yml
  format: yaml
  label: Outline Views API
  slug: outline-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-views-api-openapi.yml
authorization_urls:
- https://app.getoutline.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Outline Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Outline publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Outline API on a user''s behalf.


  Tokens are issued from https://app.getoutline.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Outline
provider_slug: outline
schemes:
- flows:
  - authorizationUrl: https://app.getoutline.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.getoutline.com/oauth/token
  name: OAuth2
  source: openapi/outline-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access
  flows:
  - authorizationCode
  scope: read
- description: Write access
  flows:
  - authorizationCode
  scope: write
slug: outline-scopes
source_filename: outline-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/outline-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/outline-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.getoutline.com/oauth/authorize\n    tokenUrl: https://app.getoutline.com/oauth/token\nscopes:\n- scope: read\n  description: Read access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outline-openapi.yml\n- scope: write\n  description: Write access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outline-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/scopes/outline-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Knowledge Base
- Wiki
- Documents
- Collaboration
- Open-Source
- Team
token_urls:
- https://app.getoutline.com/oauth/token
---
