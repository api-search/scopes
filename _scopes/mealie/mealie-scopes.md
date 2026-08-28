---
api_specs:
- filename: mealie-openapi.json
  format: json
  label: Mealie API
  slug: mealie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealie/refs/heads/main/openapi/mealie-openapi.json
authorization_urls: []
description: ''
docs: https://docs.mealie.io/documentation/getting-started/authentication/oidc-v2/
flows:
- password
kind: oauth-scopes
layout: scope
method: searched
name: Mealie Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mealie uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mealie
provider_slug: mealie
schemes:
- flows:
  - flow: password
    tokenUrl: /api/auth/token
  name: OAuth2PasswordBearer
  source: openapi/mealie-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: mealie-scopes
source_filename: mealie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.mealie.io/documentation/getting-started/authentication/oidc-v2/\ndocs: https://docs.mealie.io/documentation/getting-started/authentication/oidc-v2/\nspec_source: openapi/mealie-openapi.json\nsummary:\n  spec_declared_scopes: 0\n  note: >-\n    The OpenAPI document declares one OAuth2 password flow with an EMPTY scopes\n    object — Mealie does not issue scoped access tokens, and an API token carries\n    the full permission set of the user who minted it. The scopes recorded below are\n    the scopes Mealie requests FROM an external identity provider when it is\n    configured as an OIDC relying party; they govern login and group mapping, not\n    API authorization. Authorization inside the API is by per-user permission flags\n    (see authentication/mealie-authentication.yml).\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/mealie-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /api/auth/token\n\
  scopes: []\noidc_relying_party_scopes:\n- scope: openid\n  required: true\n  description: Required by OIDC; identifies the authentication request.\n- scope: profile\n  required: true\n  description: Supplies the display name / username claims used to provision the Mealie user.\n- scope: email\n  required: true\n  description: >-\n    Supplies the email claim used to link the IdP identity to a Mealie account, and\n    the email_verified claim Mealie requires from v3.21.0 onward.\n- scope: groups\n  required: false\n  description: >-\n    Only when group-based access is configured; the actual scope name is whatever\n    the OIDC_GROUPS_CLAIM environment variable names.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mealie/refs/heads/main/scopes/mealie-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Recipes
- Food
- Meal Planning
- Shopping Lists
- Self-Hosted
- Open Source
- Household
- Nutrition
- Home Automation
token_urls:
- /api/auth/token
---
