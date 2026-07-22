---
authorization_urls:
- https://io.plangrid.com/oauth/authorize
description: ''
docs: https://developer.plangrid.com/reference/oauth-scopes
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Plangrid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PlanGrid publishes 2 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the PlanGrid API on a user''s behalf.


  Tokens are issued from https://io.plangrid.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PlanGrid
provider_slug: plangrid
schemes:
- flows:
  - authorizationUrl: https://io.plangrid.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://io.plangrid.com/oauth/token
  - authorizationUrl: https://io.plangrid.com/oauth/authorize
    flow: implicit
  name: OAuth2
scope_count: 2
scope_names:
- write:projects
- read:profile
scopes:
- description: Allows the application access to view and manage project data on your behalf. This is the default scope if no scope parameter is provided with an authorization request.
  flows:
  - authorizationCode
  - implicit
  scope: write:projects
- description: Allows the application access to view the user profile, including UID, first name, last name, and email. This scope is required to access the User Profile.
  flows:
  - authorizationCode
  - implicit
  scope: read:profile
slug: plangrid-scopes
source_filename: plangrid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.plangrid.com/reference/oauth-scopes\ndocs: https://developer.plangrid.com/reference/oauth-scopes\nschemes:\n- name: OAuth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://io.plangrid.com/oauth/authorize\n    tokenUrl: https://io.plangrid.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://io.plangrid.com/oauth/authorize\nscopes:\n- scope: write:projects\n  description: >-\n    Allows the application access to view and manage project data on your behalf. This is the\n    default scope if no scope parameter is provided with an authorization request.\n  flows: [authorizationCode, implicit]\n- scope: read:profile\n  description: >-\n    Allows the application access to view the user profile, including UID, first name, last name,\n    and email. This scope is required to access the User Profile.\n  flows: [authorizationCode, implicit]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plangrid/refs/heads/main/scopes/plangrid-scopes.yml
summary_line: 2 scopes · authorizationCode/implicit
tags:
- Company
- Enterprise
- Construction
- Construction Technology
- Project Management
- Field Reports
- Documents
- RFIs
- REST API
- Autodesk
token_urls:
- https://io.plangrid.com/oauth/token
---
