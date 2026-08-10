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
overview: 'Uptake uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Uptake
provider_slug: uptake
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: uptake-scopes
source_filename: uptake-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://start.uptake.com/.well-known/openid-configuration\ndocs: null\nsummary: >-\n  Uptake publishes no OpenAPI and no scope reference page, so these scopes come\n  from the only anonymous, machine-readable auth metadata the estate serves: the\n  OIDC discovery and RFC 8414 authorization-server metadata documents on Uptake's\n  Okta tenant at start.uptake.com. IMPORTANT — these are IDENTITY scopes, not\n  Uptake product-API scopes. The okta.* set is Okta's own org-management scope\n  vocabulary, present because the tenant fronts the Okta management API; it does\n  not describe access to Uptake Fleet, Radar, Compass, Fusion or Scout data. No\n  Uptake product scope vocabulary is published anywhere we could reach.\nissuer: https://start.uptake.com\nscope_sets:\n- id: oidc-standard\n  origin: OpenID Connect discovery document\n  applies_to: Sign-in to the Uptake platform (fleet.uptake.com) via Uptake's Okta tenant\n  source_url:\
  \ https://start.uptake.com/.well-known/openid-configuration\n  http_status: 200\n  scopes:\n  - name: openid\n    description: Required OIDC scope; requests an ID token.\n  - name: email\n    description: Release the user's email address and email_verified claim.\n  - name: profile\n    description: Release standard profile claims (name, given_name, family_name, locale, zoneinfo, updated_at).\n  - name: address\n    description: Release the user's address claim.\n  - name: phone\n    description: Release phone_number and phone_number_verified claims.\n  - name: offline_access\n    description: Issue a refresh token.\n  - name: groups\n    description: Release the user's Okta group memberships — the claim Uptake tenancy/role mapping is most likely to key on.\n- id: okta-management\n  origin: RFC 8414 authorization-server metadata\n  applies_to: >-\n    The Okta management API on Uptake's tenant, NOT the Uptake product API.\n    Recorded for completeness and for the auth-clarity signal;\
  \ do not read this\n    as an Uptake data-access scope vocabulary.\n  source_url: https://start.uptake.com/.well-known/oauth-authorization-server\n  http_status: 200\n  scope_count: 80\n  vendor_vocabulary: okta\n  scopes_sample:\n  - okta.users.read\n  - okta.users.manage\n  - okta.groups.read\n  - okta.groups.manage\n  - okta.apps.read\n  - okta.apps.manage\n  - okta.clients.register\n  - okta.policies.read\n  - okta.logs.read\n  - okta.events.read\n  - okta.sessions.manage\n  - okta.trustedOrigins.manage\n  - okta.rateLimits.read\n  - okta.apiTokens.manage\n  full_list_file: well-known/uptake-oauth-authorization-server.json\nproduct_api_scopes:\n  published: false\n  note: >-\n    api.uptake.com and api.common.uptake.com return 403 ForbiddenException to every\n    anonymous request with no WWW-Authenticate challenge, so no scope, realm or\n    audience is advertised. The retired developer portal (developer.uptake.com)\n    now 404s. Nothing to record without credentials.\ngaps_for_provider:\n\
  - Publish the Uptake Platform API scope/permission reference at a public URL.\n- Return a WWW-Authenticate challenge on the gateway so the auth model is discoverable without a support ticket.\nchecked: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptake/refs/heads/main/scopes/uptake-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Industrial AI
- Predictive Maintenance
- Asset Performance Management
- Fleet Management
- Telematics
- Machine Learning
- Industrial IoT
token_urls: []
---
