---
api_specs:
- filename: eliq-auth-api-openapi.yaml
  format: yaml
  label: Eliq Auth API
  slug: auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-auth-api-openapi.yaml
- filename: eliq-data-management-api-openapi.json
  format: json
  label: Eliq Data Management API
  slug: data-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-data-management-api-openapi.json
- filename: eliq-insights-api-openapi.yaml
  format: yaml
  label: Eliq Insights API
  slug: insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-insights-api-openapi.yaml
- filename: eliq-intelligence-api-openapi.json
  format: json
  label: Eliq Intelligence API
  slug: intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-intelligence-api-openapi.json
authorization_urls: []
description: ''
docs: https://developer.eliq.com/doc/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Eliq Scopes
name_suffix: OAuth Scopes
note: Eliq does NOT publish a scope reference page. The scopes below are the ones the provider's own documentation and Auth API contract show by name in request examples and token-claim examples — they are transcribed, not enumerated from a catalogue, and the real per-client scope set is only visible inside the Client Admin Portal. `scopes_supported` is absent from the OIDC discovery document too. NO SCOPE HERE WAS INVENTED and this list is not claimed to be complete.
overview: 'Eliq uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Eliq
provider_slug: eliq
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: eliq-scopes
source_filename: eliq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# Eliq OAuth scopes — transcribed from the provider's auth documentation. Not a complete catalogue.\ngenerated: '2026-09-06'\nmethod: searched\nsource: https://developer.eliq.com/doc/authentication, openapi/eliq-auth-api-openapi.yaml\ndocs: https://developer.eliq.com/doc/authentication\nprovider: Eliq\nproviderId: eliq\nmodel: OAuth 2.0 scopes, space-delimited, optional on the token request. When `scope` is omitted the token receives\n  the scopes configured for that client.\nscope_reference_published: false\nnote: Eliq does NOT publish a scope reference page. The scopes below are the ones the provider's own documentation\n  and Auth API contract show by name in request examples and token-claim examples — they are transcribed, not enumerated\n  from a catalogue, and the real per-client scope set is only visible inside the Client Admin Portal. `scopes_supported`\n  is absent from the OIDC discovery document too. NO SCOPE HERE WAS INVENTED and this list is not claimed to be\n\
  \  complete.\nscope_count: 4\nscopes:\n- name: insights.read\n  description: Read access to the Eliq Insights API.\n  evidence: https://developer.eliq.com/doc/authentication (delegated token example)\n- name: insights.write\n  description: Write access to the Eliq Insights API.\n  evidence: https://developer.eliq.com/doc/authentication (delegated token example)\n- name: data.read\n  description: Read access to Eliq data.\n  evidence: https://developer.eliq.com/doc/authentication (token claims table, `scope` claim example)\n- name: data.write\n  description: Write access to Eliq data.\n  evidence: https://developer.eliq.com/doc/authentication (token claims table, `scope` claim example)\naudiences:\n- name: data-management-api\n  description: Eliq Data Management API\n- name: insights-api\n  description: Eliq Insights API\naccess_types:\n- name: application\n  description: App (machine-to-machine) token\n- name: delegated\n  description: Token issued on behalf of a named subject\ndiscovery:\n\
  \  scopes_supported_published: false\n  url: https://auth-api.eliq.com/.well-known/openid-configuration\n  note: The discovery document carries issuer and jwks_uri only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/scopes/eliq-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Utilities
- Analytics
- Sustainability
- Energy Data
- Smart Meter
- Disaggregation
- Forecasting
- Segmentation
- Consumption
- Tariffs
- Insights
token_urls: []
---
