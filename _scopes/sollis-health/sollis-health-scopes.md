---
authorization_urls:
- https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sollis Health Scopes
name_suffix: OAuth Scopes
note: Not derived from an OpenAPI — Sollis Health publishes none. The OIDC scope comes from the anonymously-served Azure AD B2C discovery document; the resource scope is the value the Member Portal's public JavaScript bundle requests at token acquisition. Only scopes actually observed are listed; the full scope surface of these private APIs is not published and cannot be enumerated without credentials.
overview: 'Sollis Health publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sollis Health API on a user''s behalf.


  Tokens are issued from https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sollis Health
provider_slug: sollis-health
schemes:
- flows:
  - authorizationUrl: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/token
  name: b2c-openid-connect
  source: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration
scope_count: 2
scope_names:
- openid
- https://sollishealthprod.onmicrosoft.com/241c93c7-6f84-41cf-90ed-ba0eea2713ad/Appointment.All
scopes:
- description: Standard OpenID Connect scope; the only value advertised in the B2C user flow's scopes_supported.
  flows:
  - authorizationCode
  scope: openid
- description: Application resource scope requested by the Sollis Health Member Portal for its backend API. Registered against the sollishealthprod tenant application 241c93c7-6f84-41cf-90ed-ba0eea2713ad. Scope semantics are not documented publicly; the name indicates full access to the appointment resource.
  flows: []
  scope: https://sollishealthprod.onmicrosoft.com/241c93c7-6f84-41cf-90ed-ba0eea2713ad/Appointment.All
slug: sollis-health-scopes
source_filename: sollis-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration\nnote: >-\n  Not derived from an OpenAPI — Sollis Health publishes none. The OIDC scope comes from\n  the anonymously-served Azure AD B2C discovery document; the resource scope is the\n  value the Member Portal's public JavaScript bundle requests at token acquisition.\n  Only scopes actually observed are listed; the full scope surface of these private\n  APIs is not published and cannot be enumerated without credentials.\ndocs: null\nschemes:\n- name: b2c-openid-connect\n  source: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/authorize\n    tokenUrl: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/token\n\
  scopes:\n- scope: openid\n  description: Standard OpenID Connect scope; the only value advertised in the B2C\n    user flow's scopes_supported.\n  flows: [authorizationCode]\n  sources:\n  - https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration\n- scope: https://sollishealthprod.onmicrosoft.com/241c93c7-6f84-41cf-90ed-ba0eea2713ad/Appointment.All\n  short_name: Appointment.All\n  description: Application resource scope requested by the Sollis Health Member Portal\n    for its backend API. Registered against the sollishealthprod tenant application\n    241c93c7-6f84-41cf-90ed-ba0eea2713ad. Scope semantics are not documented publicly;\n    the name indicates full access to the appointment resource.\n  api: sollis-health:member-portal-api\n  sources:\n  - https://mp.sollishealth.com/static/js/main.bee280e8.js\ncoverage:\n  scopes_observed: 2\n  complete: false\n  complete_note: >-\n    Partial by construction. Azure AD B2C\
  \ does not enumerate application resource scopes\n    in its discovery document, and Sollis publishes no scope or permission reference,\n    so any scope not requested by the two public front-end bundles is invisible from\n    outside.\nx-evidence:\n  fetched: '2026-08-05'\n  urls:\n  - url: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration\n    http_status: 200\n  - url: https://mp.sollishealth.com/static/js/main.bee280e8.js\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sollis-health/refs/heads/main/scopes/sollis-health-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Health
- Healthcare
- Concierge Medicine
- Urgent Care
- Emergency Care
- Membership
- Telehealth
- HIPAA
token_urls:
- https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/token
---
