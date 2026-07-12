---
authorization_urls:
- https://cognitoforms.com/api-connection
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cognito Forms Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cognito Forms publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cognito Forms API on a user''s behalf.


  Tokens are issued from https://cognitoforms.com/admin/oauthtoken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cognito Forms
provider_slug: cognito-forms
schemes:
- flows:
  - authorizationUrl: https://cognitoforms.com/api-connection
    flow: authorizationCode
    tokenUrl: https://cognitoforms.com/admin/oauthtoken
  name: oauth2Auth
  source: openapi/cognito-forms-openapi.yml
scope_count: 1
scope_names:
- admin
scopes:
- description: Full administrative access
  flows:
  - authorizationCode
  scope: admin
slug: cognito-forms-scopes
source_filename: cognito-forms-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cognito-forms-openapi.yml\nschemes:\n- name: oauth2Auth\n  source: openapi/cognito-forms-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cognitoforms.com/api-connection\n    tokenUrl: https://cognitoforms.com/admin/oauthtoken\nscopes:\n- scope: admin\n  description: Full administrative access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cognito-forms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognito-forms/refs/heads/main/scopes/cognito-forms-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Forms
- Form Builder
- Form Entries
- Workflow Automation
- Data Collection
- OData
token_urls:
- https://cognitoforms.com/admin/oauthtoken
---
