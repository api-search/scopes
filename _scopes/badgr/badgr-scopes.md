---
api_specs:
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Issuers API
  slug: badgr-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr BadgeClasses API
  slug: badgr-badgeclasses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Assertions (Awarded Badges) API
  slug: badgr-assertions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Backpack API
  slug: badgr-backpack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Collections API
  slug: badgr-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Users API
  slug: badgr-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Authentication API
  slug: badgr-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
authorization_urls:
- https://api.badgr.io/o/authorize
description: ''
docs: ''
flows:
- password
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Badgr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Badgr publishes 3 OAuth 2.0 scopes via the password and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Badgr API on a user''s behalf.


  Tokens are issued from https://api.badgr.io/o/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Badgr
provider_slug: badgr
schemes:
- flows:
  - flow: password
    tokenUrl: https://api.badgr.io/o/token
  - authorizationUrl: https://api.badgr.io/o/authorize
    flow: authorizationCode
    tokenUrl: https://api.badgr.io/o/token
  name: OAuth2
  source: openapi/badgr-openapi.yml
scope_count: 3
scope_names:
- rw:backpack
- rw:issuer
- rw:profile
scopes:
- description: Read and write the earner backpack and collections
  flows:
  - authorizationCode
  - password
  scope: rw:backpack
- description: Read and write issuers, badge classes, and assertions
  flows:
  - authorizationCode
  - password
  scope: rw:issuer
- description: Read and write the user profile
  flows:
  - authorizationCode
  - password
  scope: rw:profile
slug: badgr-scopes
source_filename: badgr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/badgr-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/badgr-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.badgr.io/o/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.badgr.io/o/authorize\n    tokenUrl: https://api.badgr.io/o/token\nscopes:\n- scope: rw:backpack\n  description: Read and write the earner backpack and collections\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/badgr-openapi.yml\n- scope: rw:issuer\n  description: Read and write issuers, badge classes, and assertions\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/badgr-openapi.yml\n- scope: rw:profile\n  description: Read and write the user profile\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/badgr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/scopes/badgr-scopes.yml
summary_line: 3 scopes · password/authorizationCode
tags:
- Digital Badges
- Open Badges
- Micro-Credentials
- Credentialing
- Verifiable Credentials
- Education
- Open Source
token_urls:
- https://api.badgr.io/o/token
---
