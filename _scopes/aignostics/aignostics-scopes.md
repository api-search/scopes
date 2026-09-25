---
api_specs:
- filename: aignostics-public-api-openapi.yml
  format: yaml
  label: Aignostics Public API
  slug: aignostics-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aignostics/refs/heads/main/openapi/aignostics-public-api-openapi.yml
authorization_urls:
- https://aignostics-platform.eu.auth0.com/authorize
description: ''
docs: https://aignostics.readthedocs.io/en/latest/get_started_api.html
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Aignostics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aignostics uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://aignostics-platform.eu.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aignostics
provider_slug: aignostics
schemes:
- declared_scopes: 0
  flows:
  - authorizationUrl: https://aignostics-platform.eu.auth0.com/authorize
    flow: authorizationCode
    tokenUrl: https://aignostics-platform.eu.auth0.com/oauth/token
  - audience: https://aignostics-platform-samia
    flow: deviceCode
    requested_scope: offline_access
    source: https://aignostics.readthedocs.io/en/latest/get_started_api.html
    tokenUrl: https://aignostics-platform.eu.auth0.com/oauth/token
  name: OAuth2AuthorizationCodeBearer
  source: openapi/aignostics-platform-api-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: aignostics-scopes
source_filename: aignostics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: >-\n  openapi/aignostics-platform-api-openapi.json,\n  https://aignostics-platform.eu.auth0.com/.well-known/openid-configuration,\n  https://aignostics.readthedocs.io/en/latest/get_started_api.html\ndocs: https://aignostics.readthedocs.io/en/latest/get_started_api.html\napi: Aignostics Platform API\nsummary: >-\n  The API declares OAuth 2.0 but publishes no API scopes. The securityScheme's scopes object is\n  empty, no operation carries a security requirement naming a scope, and no scope or permission\n  reference page exists in the documentation. Authorization is not expressed as scopes at all - it is\n  evaluated server-side from the caller's organization membership and from the grant/share-token\n  graph, which is why 15 distinct 403 variants exist in the contract while zero scopes do.\nscheme_scopes: []\nscopes: []\nschemes:\n- name: OAuth2AuthorizationCodeBearer\n  source: openapi/aignostics-platform-api-openapi.json\n\
  \  declared_scopes: 0\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://aignostics-platform.eu.auth0.com/authorize\n    tokenUrl: https://aignostics-platform.eu.auth0.com/oauth/token\n  - flow: deviceCode\n    tokenUrl: https://aignostics-platform.eu.auth0.com/oauth/token\n    requested_scope: offline_access\n    audience: https://aignostics-platform-samia\n    source: https://aignostics.readthedocs.io/en/latest/get_started_api.html\nidentity_scopes:\n  note: >-\n    These are the OIDC scopes the Auth0 tenant advertises. They govern the identity token, NOT access\n    to any Platform API resource, and are listed here only so the distinction is on the record.\n  source: https://aignostics-platform.eu.auth0.com/.well-known/openid-configuration\n  supported:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\nauthorization_model:\n\
  \  style: relationship-based (Zanzibar-shaped)\n  primitives:\n    resource_types: [run, item, output_artifact, share_token]\n    subject_types: [user, organization_admin, organization_user, share_token]\n    relations: [owner, editor, viewer]\n  creatable_through_api: [viewer]\n  note: >-\n    The access surface that scopes would normally cover is instead exposed as first-class API\n    resources - /v1/access/grants and /v1/access/share-tokens - which is a more expressive model than\n    scopes, and is auditable and revocable at runtime. The cost is that a bearer token carries no\n    intrinsic limit: an agent holding a user token can do everything that user can do, including\n    submitting billable runs, and there is no way to mint a read-only token for it. A share token is\n    the nearest equivalent, and it only covers reading an already-existing run.\ngaps:\n- id: no-least-privilege-token\n  detail: >-\n    With zero scopes, a delegated agent cannot be given a narrower credential\
  \ than the human it acts\n    for. Defining even two scopes - read and submit - would let an integrator hand an autonomous\n    client a token that cannot incur GPU cost.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aignostics/refs/heads/main/scopes/aignostics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Health
- Healthcare
- Life Sciences
- Pathology
- Medical Imaging
- Digital Pathology
- Oncology
- Biotechnology
- Research
- Germany
token_urls:
- https://aignostics-platform.eu.auth0.com/oauth/token
---
