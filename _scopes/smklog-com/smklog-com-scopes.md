---
api_specs:
- filename: smklog-com-openapi.yml
  format: yaml
  label: SMKlog Quote API
  slug: smklog-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smklog-com/refs/heads/main/openapi/smklog-com-openapi.yml
authorization_urls: []
description: The OpenAPI declares no securitySchemes (0-working/derive-oauth-scopes.py found nothing to derive), because the API is open; OAuth exists only as an optional rate-limit tier. The RFC 8414 metadata publishes one scope, quote, one grant (client_credentials) and two token-endpoint auth methods. Registration is manual by email; there is no authorization endpoint, no user identity and no dynamic client registration.
docs: https://smklog.com/auth.md
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Smklog Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SMKlog publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SMKlog API on a user''s behalf.


  Tokens are issued from https://quote-api.smklog.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SMKlog
provider_slug: smklog-com
schemes:
- flows:
  - flow: clientCredentials
    scopes:
      quote: Raise the per-client hourly quote bucket on POST /quote (and the shared MCP bucket)
    tokenUrl: https://quote-api.smklog.com/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
  issuer: https://quote-api.smklog.com
  name: SMKlog client_credentials
  registration:
    dynamic_client_registration: false
    method: manual_email
    note: '"credentials are issued manually and the secret is shown exactly once" — auth.md'
    uri: mailto:info@smklog.com
  revocation: operator-initiated by email; "existing tokens die with the client" — auth.md
  source: https://quote-api.smklog.com/.well-known/oauth-authorization-server
  token:
    bearer_methods:
    - header
    format: opaque bearer, prefix smk_at_
    lifetime: one hour (auth.md)
  type: oauth2
scope_count: 1
scope_names:
- quote
scopes:
- description: The only published scope. Grants a dedicated hourly rate-limit bucket for quoting; it adds no user identity and no payment powers ("purchases still happen on smklog.com behind the human consent gates, whoever holds the token").
  flows:
  - clientCredentials
  scope: quote
slug: smklog-com-scopes
source_filename: smklog-com-scopes.yml
source_heading: OAuth Scopes
source_url: https://quote-api.smklog.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://quote-api.smklog.com/.well-known/oauth-authorization-server\ndocs: https://smklog.com/auth.md\nsources:\n- https://quote-api.smklog.com/.well-known/oauth-authorization-server\n- https://smklog.com/.well-known/oauth-authorization-server\n- https://quote-api.smklog.com/.well-known/oauth-protected-resource\n- https://smklog.com/auth.md\ndescription: >-\n  The OpenAPI declares no securitySchemes (0-working/derive-oauth-scopes.py found nothing to derive), because the\n  API is open; OAuth exists only as an optional rate-limit tier. The RFC 8414 metadata publishes one scope,\n  quote, one grant (client_credentials) and two token-endpoint auth methods. Registration is manual by email;\n  there is no authorization endpoint, no user identity and no dynamic client registration.\nschemes:\n- name: SMKlog client_credentials\n  type: oauth2\n  source: https://quote-api.smklog.com/.well-known/oauth-authorization-server\n  issuer:\
  \ https://quote-api.smklog.com\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://quote-api.smklog.com/oauth/token\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    scopes: {quote: 'Raise the per-client hourly quote bucket on POST /quote (and the shared MCP bucket)'}\n  token:\n    format: opaque bearer, prefix smk_at_\n    lifetime: one hour (auth.md)\n    bearer_methods: [header]\n  registration:\n    method: manual_email\n    uri: mailto:info@smklog.com\n    dynamic_client_registration: false\n    note: '\"credentials are issued manually and the secret is shown exactly once\" — auth.md'\n  revocation: 'operator-initiated by email; \"existing tokens die with the client\" — auth.md'\nscopes:\n- scope: quote\n  description: The only published scope. Grants a dedicated hourly rate-limit bucket for quoting; it adds no user identity and no payment powers (\"purchases still happen on smklog.com behind the human consent gates, whoever holds the token\"\
  ).\n  flows: [clientCredentials]\n  sources: [https://quote-api.smklog.com/.well-known/oauth-authorization-server, https://smklog.com/auth.md]\nobserved:\n- 'POST /oauth/token grant_type=client_credentials without credentials -> 401 {\"error\":\"invalid_client\"} (2026-09-19)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smklog-com/refs/heads/main/scopes/smklog-com-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Shipping
- Logistics
- Parcel Shipping
- shipping-rates
- Shipping Labels
- E-Commerce
- Agents
- MCP
- A2A
token_urls:
- https://quote-api.smklog.com/oauth/token
---
