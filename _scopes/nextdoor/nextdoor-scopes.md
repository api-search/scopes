---
api_specs:
- filename: nextdoor-openapi.yml
  format: yaml
  label: Nextdoor
  slug: nextdoor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-openapi.yml
authorization_urls:
- https://auth.nextdoor.com/v3/authorize
description: ''
docs: https://developer.nextdoor.com/reference/sharing-get-authorization-code
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nextdoor Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nextdoor publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nextdoor API on a user''s behalf.


  Tokens are issued from https://auth.nextdoor.com/v3/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nextdoor
provider_slug: nextdoor
schemes:
- description: 'Nextdoor uses OAuth-based access tokens to authorize API

    requests. Refer to developer.nextdoor.com for token issuance

    and required scopes.'
  flows:
  - authorizationUrl: https://auth.nextdoor.com/v3/authorize
    flow: authorizationCode
    tokenUrl: https://auth.nextdoor.com/v3/token
  name: oauth2
  source: openapi/nextdoor-openapi.yml
scope_count: 11
scope_names:
- openid
- publish_api
- post:write
- post:read
- comment:write
- profile:read
- agency.boundary:read
- profile
- entity_page:claim
- article:write
- cms_api
scopes:
- description: Always include this scope in the authorization request.
  flows: []
  scope: openid
- description: Super scope covering all Publish API features (posts, comments, profile, and agency boundary access).
  flows: []
  scope: publish_api
- description: Create, delete, or edit posts.
  flows: []
  scope: post:write
- description: Read post data.
  flows: []
  scope: post:read
- description: Create, delete, or edit comments.
  flows: []
  scope: comment:write
- description: Get information on the authenticated user (unique user identifier, name, profile picture, etc.). Required by the /me endpoint.
  flows: []
  scope: profile:read
- description: Create geo-targeted agency posts.
  flows: []
  scope: agency.boundary:read
- description: Use only the /me and /me/profiles endpoints for user verification purposes.
  flows: []
  scope: profile
- description: Allows partners to claim pages on Nextdoor (CMS partner flow).
  flows: []
  scope: entity_page:claim
- description: Allows partners to create, update, and delete news articles (CMS partner flow).
  flows: []
  scope: article:write
- description: Scope included in the CMS partner default scope parameter; no further description documented.
  flows: []
  scope: cms_api
slug: nextdoor-scopes
source_filename: nextdoor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/nextdoor-openapi.yml\ndocs: https://developer.nextdoor.com/reference/sharing-get-authorization-code\nschemes:\n- name: oauth2\n  source: openapi/nextdoor-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.nextdoor.com/v3/authorize\n    tokenUrl: https://auth.nextdoor.com/v3/token\n  description: |-\n    Nextdoor uses OAuth-based access tokens to authorize API\n    requests. Refer to developer.nextdoor.com for token issuance\n    and required scopes.\nscopes:\n- scope: openid\n  description: Always include this scope in the authorization request.\n  sources:\n  - https://developer.nextdoor.com/reference/sharing-get-authorization-code\n- scope: publish_api\n  description: Super scope covering all Publish API features (posts, comments,\n    profile, and agency boundary access).\n  sources:\n  - https://developer.nextdoor.com/reference/sharing-get-authorization-code\n- scope: post:write\n\
  \  description: Create, delete, or edit posts.\n  sources:\n  - https://developer.nextdoor.com/reference/sharing-get-authorization-code\n- scope: post:read\n  description: Read post data.\n  sources:\n  - https://developer.nextdoor.com/reference/sharing-get-authorization-code\n- scope: comment:write\n  description: Create, delete, or edit comments.\n  sources:\n  - https://developer.nextdoor.com/reference/sharing-get-authorization-code\n- scope: profile:read\n  description: Get information on the authenticated user (unique user identifier,\n    name, profile picture, etc.). Required by the /me endpoint.\n  sources:\n  - https://developer.nextdoor.com/reference/sharing-get-authorization-code\n  - https://developer.nextdoor.com/reference/me-1\n- scope: agency.boundary:read\n  description: Create geo-targeted agency posts.\n  sources:\n  - https://developer.nextdoor.com/reference/sharing-get-authorization-code\n- scope: profile\n  description: Use only the /me and /me/profiles endpoints for\
  \ user verification\n    purposes.\n  sources:\n  - https://developer.nextdoor.com/reference/sharing-get-authorization-code\n  - https://developer.nextdoor.com/docs/how-to-verify-the-user-using-nextdoor\n- scope: entity_page:claim\n  description: Allows partners to claim pages on Nextdoor (CMS partner flow).\n  sources:\n  - https://developer.nextdoor.com/reference/user-authentication-and-authorization\n- scope: article:write\n  description: Allows partners to create, update, and delete news articles (CMS\n    partner flow).\n  sources:\n  - https://developer.nextdoor.com/reference/user-authentication-and-authorization\n- scope: cms_api\n  description: Scope included in the CMS partner default scope parameter; no\n    further description documented.\n  sources:\n  - https://developer.nextdoor.com/reference/user-authentication-and-authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/scopes/nextdoor-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Social
- Local
- Advertising
- Community
- Sharing
token_urls:
- https://auth.nextdoor.com/v3/token
---
