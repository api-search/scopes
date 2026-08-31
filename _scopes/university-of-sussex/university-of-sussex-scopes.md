---
authorization_urls:
- https://okta.sussex.ac.uk/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: University Of Sussex Scopes
name_suffix: OAuth Scopes
note: These are the standard OpenID Connect scopes exposed by the org authorization server. They are not a Sussex-authored API permission model, and no institution-operated resource API publishes its own scopes. Access is gated to enrolled applications and to holders of @sussex.ac.uk credentials; there is no public developer registration.
overview: 'University of Sussex publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Sussex API on a user''s behalf.


  Tokens are issued from https://okta.sussex.ac.uk/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Sussex
provider_slug: university-of-sussex
schemes:
- flows:
  - authorizationUrl: https://okta.sussex.ac.uk/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://okta.sussex.ac.uk/oauth2/v1/token
  issuer: https://okta.sussex.ac.uk
  name: Okta OpenID Connect (Sussex tenant)
  source: https://okta.sussex.ac.uk/.well-known/openid-configuration
  x-operator: tenant
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- groups
- offline_access
scopes:
- description: Required OpenID Connect scope; requests an ID token for the authenticated Sussex account.
  flows: []
  scope: openid
- description: Basic profile claims (name, preferred_username, locale, updated_at).
  flows: []
  scope: profile
- description: The account's email address and email_verified claim.
  flows: []
  scope: email
- description: Postal address claim.
  flows: []
  scope: address
- description: Phone number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Group memberships asserted by the Sussex Okta directory.
  flows: []
  scope: groups
- description: Issues a refresh token so a client can renew access without re-prompting.
  flows: []
  scope: offline_access
slug: university-of-sussex-scopes
source_filename: university-of-sussex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# x-method: derived\n# x-source-url: https://okta.sussex.ac.uk/.well-known/openid-configuration\n# Authorship: written by API Evangelist tooling from LIVE PROBES of the URL above.\n# `x-method: derived` is the provenance-manifest vocabulary (build-provenance-manifest.py,\n# which has no `probed` term); `method: probed` below is the enrichment-pipeline vocabulary.\n# They agree: this artifact is ours, and its facts came off the wire, not off a claim.\n# University of Sussex — OAuth / OIDC scopes\n# Rebuilt 2026-08-30. The previous version listed FIGSHARE'S single `all` scope, derived\n# from Figshare's generic v2 OpenAPI, and credited it to the university. Removed.\n# The scopes below are read straight from the Sussex Okta tenant's OIDC discovery document.\ngenerated: '2026-08-30'\nmethod: probed\nsource: https://okta.sussex.ac.uk/.well-known/openid-configuration\nprovider: University of Sussex\nproviderId: university-of-sussex\n\nschemes:\n- name: Okta OpenID Connect (Sussex\
  \ tenant)\n  x-operator: tenant\n  issuer: https://okta.sussex.ac.uk\n  source: https://okta.sussex.ac.uk/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://okta.sussex.ac.uk/oauth2/v1/authorize\n    tokenUrl: https://okta.sussex.ac.uk/oauth2/v1/token\n\nscopes:\n- scope: openid\n  description: Required OpenID Connect scope; requests an ID token for the authenticated Sussex account.\n- scope: profile\n  description: Basic profile claims (name, preferred_username, locale, updated_at).\n- scope: email\n  description: The account's email address and email_verified claim.\n- scope: address\n  description: Postal address claim.\n- scope: phone\n  description: Phone number and phone_number_verified claims.\n- scope: groups\n  description: Group memberships asserted by the Sussex Okta directory.\n- scope: offline_access\n  description: Issues a refresh token so a client can renew access without re-prompting.\n\nnote: >-\n  These are the standard\
  \ OpenID Connect scopes exposed by the org authorization server. They\n  are not a Sussex-authored API permission model, and no institution-operated resource API\n  publishes its own scopes. Access is gated to enrolled applications and to holders of\n  @sussex.ac.uk credentials; there is no public developer registration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/scopes/university-of-sussex-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Public Research University
- Identity Federation
- Research Repository
- Library
- Learning Management
- Research
- Open Access
token_urls:
- https://okta.sussex.ac.uk/oauth2/v1/token
---
