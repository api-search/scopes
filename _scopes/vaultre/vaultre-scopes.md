---
api_specs:
- filename: vaultre-api-v1-3-openapi.yml
  format: yaml
  label: VaultRE API
  slug: vaultre-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/openapi/vaultre-api-v1-3-openapi.yml
- filename: vaultre-api-v1-3-openapi.yml
  format: yaml
  label: VaultRE Integrator API
  slug: vaultre-integrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/openapi/vaultre-api-v1-3-openapi.yml
- filename: vaultre-aggregator-api-v1-0-openapi.yml
  format: yaml
  label: VaultRE Aggregator API
  slug: vaultre-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/openapi/vaultre-aggregator-api-v1-0-openapi.yml
authorization_urls: []
description: ''
docs:
- https://docs.api.vaultre.com.au/oauth.html
- https://docs.api.vaultre.com.au/guide.html
- https://docs.api.vaultre.com.au/basics.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Vaultre Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'VaultRE uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VaultRE
provider_slug: vaultre
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: vaultre-scopes
source_filename: vaultre-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://docs.api.vaultre.com.au/oauth.html\ndocs:\n- https://docs.api.vaultre.com.au/oauth.html\n- https://docs.api.vaultre.com.au/guide.html\n- https://docs.api.vaultre.com.au/basics.html\nspec_declares_oauth2: false\nspec_note: >-\n  None of the four harvested OpenAPI documents declares an oauth2 securityScheme —\n  running 0-working/derive-oauth-scopes.py against this repo yields nothing. The OAuth\n  surface exists only in the documentation, so this file is searched rather than derived.\nmodel:\n  authorization_model: >-\n    Scopes are chosen by the VaultRE customer, not requested by the integrator. When an\n    agency grants an integrator access (Office Integrations > Third-Party Access >\n    Create Token, or by completing the OAuth flow) it selects the set of scopes applied\n    to that token. There is no `scope` request parameter in the authorization URL and no\n    incremental-consent mechanism: the client cannot\
  \ ask for a permission, it can only\n    read what it was given.\n  revocation: The customer can delete/revoke the token at any time from inside their VaultRE account.\n  token_cardinality: One access token per customer account; an integrator serving many agencies holds many tokens.\nscopes_documented: false\nscopes: []\nscopes_note: >-\n  VaultRE publishes no scope vocabulary. The scope names are discoverable only at\n  runtime, with live credentials, from the two endpoints below. No scope names were\n  invented here — an empty list is the honest and complete result of this search.\ndiscovery_endpoints:\n- operationId: getTokenScopes\n  path: GET /scopes\n  summary: Retrieve a list of granted scopes for this bearer token\n  auth: customer access token\n  response: array of strings\n  source: openapi/vaultre-api-v1-3-openapi.yml\n- operationId: getIntegratorScopes\n  path: GET /integrator/scopes\n  summary: Retrieve a list of possible scopes for your API key\n  auth: integrator HS512 JWT\n\
  \  note: >-\n    This is the closest thing to a published scope registry — the full vocabulary\n    available to an integrator's key — but it is authenticated, so the vocabulary cannot\n    be captured anonymously.\n  source: openapi/vaultre-api-v1-3-openapi.yml\nflows:\n- flow: authorizationCode\n  style: OAuth2-style (not RFC 6749 conformant — see conformance/vaultre-conformance.yml)\n  token_type: third-party / office-account token\n  authorizationUrl: https://login.vaultre.com.au/cgi-bin/clientvault/oauth-authorize.cgi\n  tokenUrl: https://login.vaultre.com.au/cgi-bin/clientvault/integrations/oauthexchange.cgi\n  parameters: [client_id, redirect_uri, response_type=code, state]\n  note: Account-level access; only a system-admin user can complete this flow.\n- flow: authorizationCode\n  style: OAuth2-style\n  token_type: user/person-level token\n  authorizationUrl: https://login.vaultre.com.au/cgi-bin/clientvault/oauth-authorize-user.cgi\n  tokenUrl: https://login.vaultre.com.au/cgi-bin/clientvault/integrations/oauthexchange.cgi\n\
  \  parameters: [client_id, redirect_uri, response_type=code, state]\nconstraints:\n  authorization_code_ttl_seconds: 60\n  exchange: Server-side only — CORS blocks a browser-side exchange.\n  redirect_uris: >-\n    Matched literally, including any query string. Every variant (including each\n    parameter value) must be pre-registered; prefix matching is not supported.\n  client_id_issuance: Out of band, by emailing api@vaultre.com.au. Different value from the API key.\n  dynamic_client_registration: false\n  refresh_tokens: not documented\n  cancel_behaviour: 'Redirects to redirect_uri with ?reason=User%20denied%20request'\n  success_behaviour: 'Redirects to redirect_uri with ?reason=success&code=<code>'\n  exchange_response: '{\"token\": \"<token>\", \"message\": \"Token generated successfully\"}'\nrelated:\n  authentication: authentication/vaultre-authentication.yml\n  conformance: conformance/vaultre-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/scopes/vaultre-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Real Estate
- Australia
- New Zealand
- PropTech
- CRM
- Property Listings
- Property Management
- Rentals
- Commercial Real Estate
- Webhooks
token_urls: []
---
