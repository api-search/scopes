---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Kevala Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kevala uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kevala
provider_slug: kevala
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: kevala-scopes
source_filename: kevala-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: >-\n  https://app.kevala.com/ authorize redirect (observed 2026-08-23) +\n  https://kevalaanalytics.auth0.com/.well-known/openid-configuration (HTTP 200)\ndocs: null\nprovider: Auth0\nauthorization_server: https://kevalaanalytics.auth0.com/\naudience: https://api.kevala.com\nsummary: >-\n  Only the standard OpenID Connect scope set is discoverable. Kevala's Auth0 tenant publishes\n  scopes_supported in its OIDC discovery document, and the platform application requests\n  \"openid profile email offline_access\" when it authorizes for the api.kevala.com audience.\n  API-resource scopes (permissions attached to the https://api.kevala.com API in Auth0) are NOT\n  published anonymously and cannot be enumerated without credentials — do not assume the OIDC list\n  below describes what the DER API authorizes.\nscopes:\n- name: openid\n  description: OpenID Connect authentication; requested by the Kevala platform application.\n  requested_by_platform:\
  \ true\n- name: profile\n  description: Basic profile claims; requested by the Kevala platform application.\n  requested_by_platform: true\n- name: email\n  description: Email address claim; requested by the Kevala platform application.\n  requested_by_platform: true\n- name: offline_access\n  description: Refresh-token issuance; requested by the Kevala platform application.\n  requested_by_platform: true\n- name: name\n  description: Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\n- name: given_name\n  description: Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\n- name: family_name\n  description: Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\n- name: nickname\n  description: Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\n- name: email_verified\n  description: Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\n- name: picture\n  description:\
  \ Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\n- name: created_at\n  description: Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\n- name: identities\n  description: Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\n- name: phone\n  description: Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\n- name: address\n  description: Advertised in the tenant's scopes_supported.\n  requested_by_platform: false\napi_resource_scopes:\n  published: false\n  note: >-\n    No resource-server permission list is published. The gated OpenAPI at\n    https://api.kevala.com/der/openapi/ would carry them; it returns 403 to anonymous callers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevala/refs/heads/main/scopes/kevala-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Energy
- Electricity
- Electric Grid
- Grid Analytics
- Distributed Energy Resources
- Utilities
- Geospatial
- Analytics
- Carbon Accounting
- Electric Vehicles
- Sustainability
token_urls: []
---
