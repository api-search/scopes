---
authorization_urls: []
description: ''
docs: https://features.scnd.com/v2.0/superadmin/oauth
flows:
- clientCredentials
- password
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Scnd Scopes
name_suffix: OAuth Scopes
note: Second's OAuth authorized-apps model exposes a coarse two-level permission ("scope") selection rather than a fine-grained named-scope catalog. An authorized app is granted one or both of the permissions below at registration. No further per-resource scope reference is published in the docs.
overview: 'Second (scnd) publishes 2 OAuth 2.0 scopes via the clientCredentials, password, and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Second (scnd) API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Second (scnd)
provider_slug: scnd
schemes:
- flows:
  - clientCredentials
  - password
  - authorizationCode
  name: OAuth2
scope_count: 2
scope_names:
- private
- admin
scopes:
- description: Access to all frontend endpoints where a user auth is required.
  flows:
  - password
  - authorizationCode
  scope: private
- description: Access to all backend endpoints where an admin (super-admin) auth is required.
  flows:
  - clientCredentials
  - password
  - authorizationCode
  scope: admin
slug: scnd-scopes
source_filename: scnd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://features.scnd.com/v2.0/superadmin/oauth\ndocs: https://features.scnd.com/v2.0/superadmin/oauth\nnote: >-\n  Second's OAuth authorized-apps model exposes a coarse two-level permission\n  (\"scope\") selection rather than a fine-grained named-scope catalog. An\n  authorized app is granted one or both of the permissions below at registration.\n  No further per-resource scope reference is published in the docs.\nschemes:\n- name: OAuth2\n  flows: [clientCredentials, password, authorizationCode]\nscopes:\n- scope: private\n  description: Access to all frontend endpoints where a user auth is required.\n  flows: [password, authorizationCode]\n- scope: admin\n  description: Access to all backend endpoints where an admin (super-admin) auth is required.\n  flows: [clientCredentials, password, authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scnd/refs/heads/main/scopes/scnd-scopes.yml
summary_line: 2 scopes · clientCredentials/password/authorizationCode
tags:
- Company
- Marketplace
- Services
- Vendor Management
- Payments
- OAuth
- SaaS
- Procurement
token_urls: []
---
