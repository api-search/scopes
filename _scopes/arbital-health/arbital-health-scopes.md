---
authorization_urls:
- https://auth.arbitalhealth.com/propelauth/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Arbital Health Scopes
name_suffix: OAuth Scopes
note: Arbital Health publishes no OpenAPI, so there is no operation-level scope surface to derive. The only scopes it advertises anywhere publicly are the three standard OpenID Connect scopes in its PropelAuth discovery document. No application or resource scopes (read:contracts, write:adjudication, …) are published — any such scopes exist only inside the customer tenant.
overview: 'Arbital Health publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Arbital Health API on a user''s behalf.


  Tokens are issued from https://auth.arbitalhealth.com/propelauth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arbital Health
provider_slug: arbital-health
schemes:
- flows:
  - authorizationUrl: https://auth.arbitalhealth.com/propelauth/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.arbitalhealth.com/propelauth/oauth/token
  name: propelauth-oidc
  source: well-known/arbital-health-openid-configuration.json
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: Standard OpenID Connect scope — request an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Release the user's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Release basic profile claims (first_name, last_name, picture_url).
  flows:
  - authorizationCode
  scope: profile
slug: arbital-health-scopes
source_filename: arbital-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://auth.arbitalhealth.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Arbital Health publishes no OpenAPI, so there is no operation-level scope surface\n  to derive. The only scopes it advertises anywhere publicly are the three standard\n  OpenID Connect scopes in its PropelAuth discovery document. No application or\n  resource scopes (read:contracts, write:adjudication, …) are published — any such\n  scopes exist only inside the customer tenant.\nschemes:\n- name: propelauth-oidc\n  source: well-known/arbital-health-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.arbitalhealth.com/propelauth/oauth/authorize\n    tokenUrl: https://auth.arbitalhealth.com/propelauth/oauth/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope — request an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/arbital-health-openid-configuration.json]\n\
  - scope: email\n  description: Release the user's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/arbital-health-openid-configuration.json]\n- scope: profile\n  description: Release basic profile claims (first_name, last_name, picture_url).\n  flows: [authorizationCode]\n  sources: [well-known/arbital-health-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://auth.arbitalhealth.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbital-health/refs/heads/main/scopes/arbital-health-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Healthcare
- Health Insurance
- Value-Based Care
- Actuarial
- Claims
- Payers
- Providers
- Analytics
- Artificial Intelligence
token_urls:
- https://auth.arbitalhealth.com/propelauth/oauth/token
---
