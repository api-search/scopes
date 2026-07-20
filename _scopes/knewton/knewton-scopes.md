---
authorization_urls: []
description: ''
docs: https://dev.knewton.com/implementation/authentication-and-authorization/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Knewton Scopes
name_suffix: OAuth Scopes
note: Knewton runs an OAuth 2.0 client_credentials flow but does NOT publish a permission scope registry. The OAuth `scope` parameter is overloaded to carry the external ID of the user account the returned tokens should be associated with, not a permission string. The real permission surface is the account `entitlements` list, captured below and in authentication/knewton-authentication.yml. No scope values are invented here.
overview: 'Knewton uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.knewton.com/v0/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Knewton
provider_slug: knewton
schemes:
- flows:
  - flow: clientCredentials
    grant_types:
    - client_credentials
    - refresh_token
    tokenUrl: https://api.knewton.com/v0/oauth/token
  name: OAuth2ClientCredentials
scope_count: 0
scope_names: []
scopes: []
slug: knewton-scopes
source_filename: knewton-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://dev.knewton.com/reference/authentication/\ndocs: https://dev.knewton.com/implementation/authentication-and-authorization/\nnote: Knewton runs an OAuth 2.0 client_credentials flow but does NOT publish a permission\n  scope registry. The OAuth `scope` parameter is overloaded to carry the external ID of the\n  user account the returned tokens should be associated with, not a permission string. The\n  real permission surface is the account `entitlements` list, captured below and in\n  authentication/knewton-authentication.yml. No scope values are invented here.\nscope_parameter:\n  present: true\n  semantics: external-user-id\n  description: The external ID of a previously created user account to be associated with\n    the returned tokens.\n  example_form: scope=user_601726\n  source: https://dev.knewton.com/reference/authentication/\nschemes:\n- name: OAuth2ClientCredentials\n  flows:\n  - flow: clientCredentials\n  \
  \  tokenUrl: https://api.knewton.com/v0/oauth/token\n    grant_types:\n    - client_credentials\n    - refresh_token\nscopes: []\nentitlements:\n- name: all\n  description: Full entitlement set.\n- name: knerd\n  description: Internal Knewton entitlement.\n- name: partner_admin\n  description: Partner administrator; required for account, learning-instance and goal\n    write operations.\n- name: partner_inventory_access\n  description: Access to the partner content inventory.\n- name: partner_graph_update\n  description: Update an existing knowledge graph.\n- name: partner_graph_ingest\n  description: Ingest a new knowledge graph.\n- name: partner_graph_validate\n  description: Validate a knowledge graph.\n- name: create_learning_instance\n  description: Create learning instances.\nentitlements_source: https://dev.knewton.com/reference/accounts/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knewton/refs/heads/main/scopes/knewton-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer
- Education
- EdTech
- Adaptive Learning
- Learning Analytics
- Machine Learning
- Recommendations
- Courseware
- Higher Education
token_urls:
- https://api.knewton.com/v0/oauth/token
---
