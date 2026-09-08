---
api_specs:
- filename: archer-daniels-midland-commodities-api-openapi.yml
  format: yaml
  label: Archer Daniels Midland Commodities API
  slug: archer-daniels-midland-commodities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/openapi/archer-daniels-midland-commodities-api-openapi.yml
- filename: archer-daniels-midland-locations-api-openapi.yml
  format: yaml
  label: Archer Daniels Midland Locations API
  slug: archer-daniels-midland-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/openapi/archer-daniels-midland-locations-api-openapi.yml
- filename: archer-daniels-midland-products-api-openapi.yml
  format: yaml
  label: Archer Daniels Midland Products API
  slug: archer-daniels-midland-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/openapi/archer-daniels-midland-products-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Archer Daniels Midland Scopes
name_suffix: OAuth Scopes
note: 'These scopes are not read from an ADM API product — ADM publishes no developer portal and no API reference. They are read verbatim from the OpenID Connect discovery document ADM''s own www.adm.com host serves (HTTP 200, application/json, 2026-09-04). The issuer is https://www.adm.com/ and the endpoints sit under /api/episerver/connect/, i.e. this is the Optimizely (Episerver) CMS authorization server that fronts adm.com itself. Recorded because it is a real, first-party, machine-readable authorization surface on the company''s domain; NOT because ADM sells API access under these scopes. The three OpenAPI documents in openapi/ are API-Evangelist-authored (x-generated-from: documentation) and declare an apiKey scheme, not OAuth, so nothing here was derived from them.'
overview: 'Archer Daniels Midland uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: archer-daniels-midland-scopes
source_filename: archer-daniels-midland-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://www.adm.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  These scopes are not read from an ADM API product — ADM publishes no developer portal and no API\n  reference. They are read verbatim from the OpenID Connect discovery document ADM's own\n  www.adm.com host serves (HTTP 200, application/json, 2026-09-04). The issuer is\n  https://www.adm.com/ and the endpoints sit under /api/episerver/connect/, i.e. this is the\n  Optimizely (Episerver) CMS authorization server that fronts adm.com itself. Recorded because it\n  is a real, first-party, machine-readable authorization surface on the company's domain; NOT\n  because ADM sells API access under these scopes. The three OpenAPI documents in openapi/ are\n  API-Evangelist-authored (x-generated-from: documentation) and declare an apiKey scheme, not\n  OAuth, so nothing here was derived from them.\nprovider_metadata:\n  issuer: https://www.adm.com/\n  authorization_endpoint:\
  \ https://www.adm.com/api/episerver/connect/authorize\n  token_endpoint: https://www.adm.com/api/episerver/connect/token\n  userinfo_endpoint: https://www.adm.com/api/episerver/connect/userinfo\n  end_session_endpoint: https://www.adm.com/api/episerver/connect/logout\n  jwks_uri: https://www.adm.com/.well-known/jwks\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\nscope_count: 5\nscopes:\n- name: openid\n  description: OpenID Connect — request an ID token for the authenticated subject.\n  source: scopes_supported in the published discovery document\n- name: offline_access\n  description: Issue a refresh token so the client can renew access without the user present.\n  source: scopes_supported in the published discovery document\n- name: profile\n  description: Access the subject's profile claims.\n  source:\
  \ scopes_supported in the published discovery document\n- name: email\n  description: Access the subject's email claim.\n  source: scopes_supported in the published discovery document\n- name: roles\n  description: Access the subject's role claim, used by the CMS for content authorization.\n  source: scopes_supported in the published discovery document\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/scopes/archer-daniels-midland-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
token_urls: []
---
