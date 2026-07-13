---
api_specs:
- filename: aweber-openapi.yml
  format: yaml
  label: AWeber REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-openapi.yml
authorization_urls:
- https://auth.aweber.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Aweber Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AWeber publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AWeber API on a user''s behalf.


  Tokens are issued from https://auth.aweber.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AWeber
provider_slug: aweber
schemes:
- flows:
  - authorizationUrl: https://auth.aweber.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.aweber.com/oauth2/token
  name: OAuth2
  source: openapi/aweber-openapi.yml
scope_count: 9
scope_names:
- account.read
- email.read
- email.write
- landing-page.read
- landing-page.write
- list.read
- list.write
- subscriber.read
- subscriber.write
scopes:
- description: Read account information
  flows:
  - authorizationCode
  scope: account.read
- description: Read broadcasts and campaigns
  flows:
  - authorizationCode
  scope: email.read
- description: Manage broadcasts and campaigns
  flows:
  - authorizationCode
  scope: email.write
- description: Read landing pages
  flows:
  - authorizationCode
  scope: landing-page.read
- description: Manage landing pages
  flows:
  - authorizationCode
  scope: landing-page.write
- description: Read lists
  flows:
  - authorizationCode
  scope: list.read
- description: Manage lists
  flows:
  - authorizationCode
  scope: list.write
- description: Read subscribers
  flows:
  - authorizationCode
  scope: subscriber.read
- description: Manage subscribers
  flows:
  - authorizationCode
  scope: subscriber.write
slug: aweber-scopes
source_filename: aweber-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aweber-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/aweber-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.aweber.com/oauth2/authorize\n    tokenUrl: https://auth.aweber.com/oauth2/token\nscopes:\n- scope: account.read\n  description: Read account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aweber-openapi.yml\n- scope: email.read\n  description: Read broadcasts and campaigns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aweber-openapi.yml\n- scope: email.write\n  description: Manage broadcasts and campaigns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aweber-openapi.yml\n- scope: landing-page.read\n  description: Read landing pages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aweber-openapi.yml\n- scope: landing-page.write\n  description: Manage landing pages\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/aweber-openapi.yml\n- scope: list.read\n  description: Read lists\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aweber-openapi.yml\n- scope: list.write\n  description: Manage lists\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aweber-openapi.yml\n- scope: subscriber.read\n  description: Read subscribers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aweber-openapi.yml\n- scope: subscriber.write\n  description: Manage subscribers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aweber-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/scopes/aweber-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Email Marketing
- Marketing Automation
- Email
- Newsletters
- Subscribers
- Campaigns
- Landing Pages
token_urls:
- https://auth.aweber.com/oauth2/token
---
