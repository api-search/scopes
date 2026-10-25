---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Uptake Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Uptake publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Uptake API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Uptake
provider_slug: uptake
schemes: []
scope_count: 7
scope_names:
- openid
- email
- profile
- address
- phone
- offline_access
- groups
scopes:
- description: Required OIDC scope; requests an ID token.
  flows: []
  scope: openid
- description: Release the user's email address and email_verified claim.
  flows: []
  scope: email
- description: Release standard profile claims (name, given_name, family_name, locale, zoneinfo, updated_at).
  flows: []
  scope: profile
- description: Release the user's address claim.
  flows: []
  scope: address
- description: Release phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Issue a refresh token.
  flows: []
  scope: offline_access
- description: Release the user's Okta group memberships — the claim Uptake tenancy/role mapping is most likely to key on.
  flows: []
  scope: groups
slug: uptake-scopes
source_filename: uptake-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://start.uptake.com/.well-known/openid-configuration\ndocs: null\nsummary: 'Uptake publishes no OpenAPI and no scope reference page, so these scopes come from the only anonymous, machine-readable auth metadata the estate\n  serves: the OIDC discovery and RFC 8414 authorization-server metadata documents on Uptake''s Okta tenant at start.uptake.com. IMPORTANT — these are IDENTITY\n  scopes, not Uptake product-API scopes. The okta.* set is Okta''s own org-management scope vocabulary, present because the tenant fronts the Okta management\n  API; it does not describe access to Uptake Fleet, Radar, Compass, Fusion or Scout data. No Uptake product scope vocabulary is published anywhere we could\n  reach.'\nissuer: https://start.uptake.com\nscope_sets:\n- id: oidc-standard\n  origin: OpenID Connect discovery document\n  applies_to: Sign-in to the Uptake platform (fleet.uptake.com) via Uptake's Okta tenant\n  source_url: https://start.uptake.com/.well-known/openid-configuration\n\
  \  http_status: 200\n  scopes:\n  - name: openid\n    description: Required OIDC scope; requests an ID token.\n  - name: email\n    description: Release the user's email address and email_verified claim.\n  - name: profile\n    description: Release standard profile claims (name, given_name, family_name, locale, zoneinfo, updated_at).\n  - name: address\n    description: Release the user's address claim.\n  - name: phone\n    description: Release phone_number and phone_number_verified claims.\n  - name: offline_access\n    description: Issue a refresh token.\n  - name: groups\n    description: Release the user's Okta group memberships — the claim Uptake tenancy/role mapping is most likely to key on.\n- id: okta-management\n  origin: RFC 8414 authorization-server metadata\n  applies_to: The Okta management API on Uptake's tenant, NOT the Uptake product API. Recorded for completeness and for the auth-clarity signal; do not\n    read this as an Uptake data-access scope vocabulary.\n  source_url:\
  \ https://start.uptake.com/.well-known/oauth-authorization-server\n  http_status: 200\n  scope_count: 80\n  vendor_vocabulary: okta\n  scopes_sample:\n  - okta.users.read\n  - okta.users.manage\n  - okta.groups.read\n  - okta.groups.manage\n  - okta.apps.read\n  - okta.apps.manage\n  - okta.clients.register\n  - okta.policies.read\n  - okta.logs.read\n  - okta.events.read\n  - okta.sessions.manage\n  - okta.trustedOrigins.manage\n  - okta.rateLimits.read\n  - okta.apiTokens.manage\n  full_list_file: well-known/uptake-oauth-authorization-server.json\nproduct_api_scopes:\n  published: false\n  note: api.uptake.com and api.common.uptake.com return 403 ForbiddenException to every anonymous request with no WWW-Authenticate challenge, so no scope,\n    realm or audience is advertised. The retired developer portal (developer.uptake.com) now 404s. Nothing to record without credentials.\ngaps_for_provider:\n- Publish the Uptake Platform API scope/permission reference at a public URL.\n- Return\
  \ a WWW-Authenticate challenge on the gateway so the auth model is discoverable without a support ticket.\nchecked: '2026-08-05'\nscopes:\n- name: openid\n  description: Required OIDC scope; requests an ID token.\n  set: oidc-standard\n- name: email\n  description: Release the user's email address and email_verified claim.\n  set: oidc-standard\n- name: profile\n  description: Release standard profile claims (name, given_name, family_name, locale, zoneinfo, updated_at).\n  set: oidc-standard\n- name: address\n  description: Release the user's address claim.\n  set: oidc-standard\n- name: phone\n  description: Release phone_number and phone_number_verified claims.\n  set: oidc-standard\n- name: offline_access\n  description: Issue a refresh token.\n  set: oidc-standard\n- name: groups\n  description: Release the user's Okta group memberships — the claim Uptake tenancy/role mapping is most likely to key on.\n  set: oidc-standard\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptake/refs/heads/main/scopes/uptake-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Industrial AI
- Predictive Maintenance
- Asset Performance Management
- Fleet Management
- Telematics
- Machine Learning
- Industrial IoT
- Industrial
token_bound: false
token_urls: []
---
