---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Credly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Credly publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Credly API on a user''s behalf.


  Tokens are issued from https://api.credly.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Credly
provider_slug: credly
schemes:
- description: OAuth 2.0 client_credentials grant. Tokens are short-lived (2 hours) and sent as a Bearer token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.credly.com/oauth/token
  name: oauth2
  source: openapi/credly-openapi.yml
scope_count: 3
scope_names:
- issue
- read
- workforce
scopes:
- description: Issue and manage badges.
  flows:
  - clientCredentials
  scope: issue
- description: Read access to organization resources.
  flows:
  - clientCredentials
  scope: read
- description: Access to employee/workforce data.
  flows:
  - clientCredentials
  scope: workforce
slug: credly-scopes
source_filename: credly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/credly-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/credly-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.credly.com/oauth/token\n  description: OAuth 2.0 client_credentials grant. Tokens are short-lived (2 hours) and sent\n    as a Bearer token.\nscopes:\n- scope: issue\n  description: Issue and manage badges.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/credly-openapi.yml\n- scope: read\n  description: Read access to organization resources.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/credly-openapi.yml\n- scope: workforce\n  description: Access to employee/workforce data.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/credly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/scopes/credly-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Digital Credentials
- Open Badges
- Badging
- Certifications
- Verifiable Credentials
- Pearson
token_urls:
- https://api.credly.com/oauth/token
---
