---
authorization_urls:
- https://app.accelerant.ai/api/auth/oidc/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Accelerant Scopes
name_suffix: OAuth Scopes
note: Scopes taken verbatim from the scopes_supported array of the Accelerant Risk Exchange platform OpenID Connect discovery document. These are the standard OIDC identity scopes the platform advertises for anonymous discovery; any resource/API scopes for the Member API surface at api.accelerant.ai are not published anonymously and would require the gated developer documentation to enumerate. No scopes have been invented.
overview: 'Accelerant publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Accelerant API on a user''s behalf.


  Tokens are issued from https://app.accelerant.ai/api/auth/oidc/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Accelerant
provider_slug: accelerant
schemes:
- flows:
  - authorizationUrl: https://app.accelerant.ai/api/auth/oidc/authorize
    flow: authorizationCode
    tokenUrl: https://app.accelerant.ai/api/auth/oidc/token
  name: AccelerantPlatformOIDC
  source: well-known/accelerant-openid-configuration.json
scope_count: 4
scope_names:
- openid
- profile
- name
- email
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the authenticated Accelerant platform user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated user's default profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the authenticated user's name claim.
  flows:
  - authorizationCode
  scope: name
- description: Access to the authenticated user's email claim.
  flows:
  - authorizationCode
  scope: email
slug: accelerant-scopes
source_filename: accelerant-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://app.accelerant.ai/.well-known/openid-configuration\nnote: 'Scopes taken verbatim from the scopes_supported array of the Accelerant Risk\n  Exchange platform OpenID Connect discovery document. These are the standard OIDC\n  identity scopes the platform advertises for anonymous discovery; any resource/API\n  scopes for the Member API surface at api.accelerant.ai are not published anonymously\n  and would require the gated developer documentation to enumerate. No scopes have\n  been invented.'\nschemes:\n- name: AccelerantPlatformOIDC\n  source: well-known/accelerant-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.accelerant.ai/api/auth/oidc/authorize\n    tokenUrl: https://app.accelerant.ai/api/auth/oidc/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope requesting an ID token for the authenticated\n    Accelerant platform user.\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - well-known/accelerant-openid-configuration.json\n- scope: profile\n  description: Access to the authenticated user's default profile claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/accelerant-openid-configuration.json\n- scope: name\n  description: Access to the authenticated user's name claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/accelerant-openid-configuration.json\n- scope: email\n  description: Access to the authenticated user's email claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/accelerant-openid-configuration.json\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://app.accelerant.ai/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelerant/refs/heads/main/scopes/accelerant-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Insurance
- Insurtech
- Specialty Insurance
- Underwriting
- Risk Management
- Reinsurance
- Marketplace
- Risk Scoring
- Financial-Services
- Artificial Intelligence
token_urls:
- https://app.accelerant.ai/api/auth/oidc/token
---
