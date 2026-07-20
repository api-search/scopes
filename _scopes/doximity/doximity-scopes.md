---
api_specs:
- filename: doximity-oauth-openapi.yml
  format: yaml
  label: Doximity OAuth & OpenID Connect API
  slug: doximity-oauth-openid-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doximity/refs/heads/main/openapi/doximity-oauth-openapi.yml
authorization_urls:
- https://auth.doximity.com/oauth/authorize
description: ''
docs: https://www.doximity.com/developers/documentation
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Doximity Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Doximity publishes 21 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Doximity API on a user''s behalf.


  Tokens are issued from https://auth.doximity.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Doximity
provider_slug: doximity
schemes:
- flows:
  - authorizationUrl: https://auth.doximity.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.doximity.com/oauth/token
  name: doximityOAuth
  source: https://auth.doximity.com/.well-known/openid-configuration
  type: oauth2
scope_count: 21
scope_names:
- openid
- profile:read:basic
- profile:read:email
- profile:read:dialer_phone
- profile:read:experience
- profile:read:office
- profile:read:permissions
- profile:read:private_contact
- search
- dialer
- docsgpt:access
- hipaa:identified
- jobs:read
- colleagues:read
- colleagues:write
- login_context:inferred
- sessions:linked
- activities:read:cards
- activities:read:comments
- activities:read:likes
- activities:write:likes
scopes:
- description: Enables the OpenID Connect id_token to be returned. Default scope, always supported.
  flows:
  - authorizationCode
  scope: openid
- description: Grants access to name, given_name, family_name, middle_name, credentials, profile_photo_url, and specialty.
  flows:
  - authorizationCode
  scope: profile:read:basic
- description: Read the member's email address.
  flows:
  - authorizationCode
  scope: profile:read:email
- description: Read the member's Doximity Dialer phone number.
  flows:
  - authorizationCode
  scope: profile:read:dialer_phone
- description: Read the member's professional experience.
  flows:
  - authorizationCode
  scope: profile:read:experience
- description: Read the member's office information.
  flows:
  - authorizationCode
  scope: profile:read:office
- description: Read the member's permissions.
  flows:
  - authorizationCode
  scope: profile:read:permissions
- description: Read the member's private contact information.
  flows:
  - authorizationCode
  scope: profile:read:private_contact
- description: Search the Doximity member directory.
  flows:
  - authorizationCode
  scope: search
- description: Access to Doximity Dialer functionality.
  flows:
  - authorizationCode
  scope: dialer
- description: Access to DocsGPT.
  flows:
  - authorizationCode
  scope: docsgpt:access
- description: Access identified data under HIPAA.
  flows:
  - authorizationCode
  scope: hipaa:identified
- description: Read job data.
  flows:
  - authorizationCode
  scope: jobs:read
- description: Read the member's colleagues.
  flows:
  - authorizationCode
  scope: colleagues:read
- description: Modify the member's colleagues.
  flows:
  - authorizationCode
  scope: colleagues:write
- description: Access inferred login context.
  flows:
  - authorizationCode
  scope: login_context:inferred
- description: Access linked sessions.
  flows:
  - authorizationCode
  scope: sessions:linked
- description: Read activity cards.
  flows:
  - authorizationCode
  scope: activities:read:cards
- description: Read activity comments.
  flows:
  - authorizationCode
  scope: activities:read:comments
- description: Read activity likes.
  flows:
  - authorizationCode
  scope: activities:read:likes
- description: Write activity likes.
  flows:
  - authorizationCode
  scope: activities:write:likes
slug: doximity-scopes
source_filename: doximity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.doximity.com/.well-known/openid-configuration\ndocs: https://www.doximity.com/developers/documentation\nschemes:\n- name: doximityOAuth\n  type: oauth2\n  source: https://auth.doximity.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.doximity.com/oauth/authorize\n    tokenUrl: https://auth.doximity.com/oauth/token\nscopes:\n- scope: openid\n  description: Enables the OpenID Connect id_token to be returned. Default scope, always supported.\n  flows: [authorizationCode]\n- scope: profile:read:basic\n  description: Grants access to name, given_name, family_name, middle_name, credentials, profile_photo_url, and specialty.\n  flows: [authorizationCode]\n- scope: profile:read:email\n  description: Read the member's email address.\n  flows: [authorizationCode]\n- scope: profile:read:dialer_phone\n  description: Read the member's Doximity Dialer phone number.\n\
  \  flows: [authorizationCode]\n- scope: profile:read:experience\n  description: Read the member's professional experience.\n  flows: [authorizationCode]\n- scope: profile:read:office\n  description: Read the member's office information.\n  flows: [authorizationCode]\n- scope: profile:read:permissions\n  description: Read the member's permissions.\n  flows: [authorizationCode]\n- scope: profile:read:private_contact\n  description: Read the member's private contact information.\n  flows: [authorizationCode]\n- scope: search\n  description: Search the Doximity member directory.\n  flows: [authorizationCode]\n- scope: dialer\n  description: Access to Doximity Dialer functionality.\n  flows: [authorizationCode]\n- scope: docsgpt:access\n  description: Access to DocsGPT.\n  flows: [authorizationCode]\n- scope: hipaa:identified\n  description: Access identified data under HIPAA.\n  flows: [authorizationCode]\n- scope: jobs:read\n  description: Read job data.\n  flows: [authorizationCode]\n- scope:\
  \ colleagues:read\n  description: Read the member's colleagues.\n  flows: [authorizationCode]\n- scope: colleagues:write\n  description: Modify the member's colleagues.\n  flows: [authorizationCode]\n- scope: login_context:inferred\n  description: Access inferred login context.\n  flows: [authorizationCode]\n- scope: sessions:linked\n  description: Access linked sessions.\n  flows: [authorizationCode]\n- scope: activities:read:cards\n  description: Read activity cards.\n  flows: [authorizationCode]\n- scope: activities:read:comments\n  description: Read activity comments.\n  flows: [authorizationCode]\n- scope: activities:read:likes\n  description: Read activity likes.\n  flows: [authorizationCode]\n- scope: activities:write:likes\n  description: Write activity likes.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doximity/refs/heads/main/scopes/doximity-scopes.yml
summary_line: 21 scopes · authorizationCode
tags:
- Company
- Healthtech
- Identity
- OAuth
- OpenID Connect
- Authentication
- Physician Network
- Healthcare
- SSO
- Verification
token_urls:
- https://auth.doximity.com/oauth/token
---
