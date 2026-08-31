---
api_specs:
- filename: blng-user-api-openapi.yml
  format: yaml
  label: BLNG User API
  slug: blng-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-user-api-openapi.yml
- filename: blng-billing-api-openapi.yml
  format: yaml
  label: BLNG Billing API
  slug: blng-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-billing-api-openapi.yml
- filename: blng-chat-prompts-api-openapi.yml
  format: yaml
  label: Blng Chat Prompts API
  slug: blng-chat-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-chat-prompts-api-openapi.yml
- filename: blng-composite-api-openapi.yml
  format: yaml
  label: Blng Composite API
  slug: blng-composite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-composite-api-openapi.yml
- filename: blng-design-journey-api-openapi.yml
  format: yaml
  label: Blng Design Journey API
  slug: blng-design-journey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-design-journey-api-openapi.yml
- filename: blng-invitation-api-openapi.yml
  format: yaml
  label: Blng Invitation API
  slug: blng-invitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-invitation-api-openapi.yml
- filename: blng-journeys-api-openapi.yml
  format: yaml
  label: Blng Journeys API
  slug: blng-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-journeys-api-openapi.yml
- filename: blng-organization-api-openapi.yml
  format: yaml
  label: Blng Organization API
  slug: blng-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-organization-api-openapi.yml
- filename: blng-prompts-api-openapi.yml
  format: yaml
  label: Blng Prompts API
  slug: blng-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-prompts-api-openapi.yml
- filename: blng-subscription-api-openapi.yml
  format: yaml
  label: Blng Subscription API
  slug: blng-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-subscription-api-openapi.yml
- filename: blng-user-subscription-api-openapi.yml
  format: yaml
  label: Blng User Subscription API
  slug: blng-user-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-user-subscription-api-openapi.yml
- filename: blng-user-tooltip-api-openapi.yml
  format: yaml
  label: Blng User Tooltip API
  slug: blng-user-tooltip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-user-tooltip-api-openapi.yml
- filename: blng-webhook-api-openapi.yml
  format: yaml
  label: Blng Webhook API
  slug: blng-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-webhook-api-openapi.yml
- filename: blng-workspace-api-openapi.yml
  format: yaml
  label: Blng Workspace API
  slug: blng-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-workspace-api-openapi.yml
authorization_urls:
- https://auth.app.blng.ai/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Blng Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Blng publishes 4 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Blng API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blng
provider_slug: blng
schemes:
- description: Cognito authorization code flow for users
  flows:
  - authorizationUrl: https://auth.app.blng.ai/oauth2/authorize
    flow: implicit
  name: cognitoUserAuth
  source: openapi/blng-billing-api-openapi.yml
- description: Cognito authorization code flow for users
  flows:
  - authorizationUrl: https://auth.app.blng.ai/oauth2/authorize
    flow: implicit
  name: cognitoUserAuth
  source: openapi/blng-journey-api-openapi.yml
- description: Cognito authorization code flow for users
  flows:
  - authorizationUrl: https://auth.app.blng.ai/oauth2/authorize
    flow: implicit
  name: cognitoUserAuth
  source: openapi/blng-user-api-openapi.yml
scope_count: 4
scope_names:
- aws.cognito.signin.user.admin
- email
- openid
- profile
scopes:
- description: aws.cognito.signin.user.admin
  flows:
  - implicit
  scope: aws.cognito.signin.user.admin
- description: email
  flows:
  - implicit
  scope: email
- description: openid
  flows:
  - implicit
  scope: openid
- description: profile
  flows:
  - implicit
  scope: profile
slug: blng-scopes
source_filename: blng-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/blng-billing-api-openapi.yml, openapi/blng-journey-api-openapi.yml, openapi/blng-user-api-openapi.yml\nschemes:\n- name: cognitoUserAuth\n  source: openapi/blng-billing-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.app.blng.ai/oauth2/authorize\n  description: Cognito authorization code flow for users\n- name: cognitoUserAuth\n  source: openapi/blng-journey-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.app.blng.ai/oauth2/authorize\n  description: Cognito authorization code flow for users\n- name: cognitoUserAuth\n  source: openapi/blng-user-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.app.blng.ai/oauth2/authorize\n  description: Cognito authorization code flow for users\nscopes:\n- scope: aws.cognito.signin.user.admin\n  description: aws.cognito.signin.user.admin\n  flows:\n  - implicit\n  sources:\n  - openapi/blng-billing-api-openapi.yml\n\
  \  - openapi/blng-journey-api-openapi.yml\n  - openapi/blng-user-api-openapi.yml\n- scope: email\n  description: email\n  flows:\n  - implicit\n  sources:\n  - openapi/blng-billing-api-openapi.yml\n  - openapi/blng-journey-api-openapi.yml\n  - openapi/blng-user-api-openapi.yml\n- scope: openid\n  description: openid\n  flows:\n  - implicit\n  sources:\n  - openapi/blng-billing-api-openapi.yml\n  - openapi/blng-journey-api-openapi.yml\n  - openapi/blng-user-api-openapi.yml\n- scope: profile\n  description: profile\n  flows:\n  - implicit\n  sources:\n  - openapi/blng-billing-api-openapi.yml\n  - openapi/blng-journey-api-openapi.yml\n  - openapi/blng-user-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/scopes/blng-scopes.yml
summary_line: 4 scopes · implicit
tags:
- Company
- Jewelry
- Generative AI
- Design
- Creative Tools
- Rendering
- Marketing
- Retail
- 3D Models
- Image-Generation
- Workspaces
- Billing
- OpenAPI
- AWS Cognito
token_urls: []
---
