---
api_specs:
- filename: astrology-api-json-openapi.yml
  format: yaml
  label: Astrology API
  slug: astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-json-openapi.yml
- filename: astrology-api-pdf-openapi.yml
  format: yaml
  label: AstrologyAPI PDF Reports API
  slug: astrology-api-pdf
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-pdf-openapi.yml
- filename: astrology-api-palmistry-openapi.json
  format: json
  label: AstrologyAPI Palmistry API
  slug: astrology-api-palmistry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-palmistry-openapi.json
- filename: astrology-api-face-reading-openapi.yml
  format: yaml
  label: AstrologyAPI Face Reading API
  slug: astrology-api-face-reading
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-face-reading-openapi.yml
authorization_urls: []
description: The only OAuth surface AstrologyAPI operates is the MCP server. Its RFC 9728 protected-resource metadata declares exactly one scope. The REST API has no OAuth flow at all — it authenticates with HTTP Basic credentials or a wallet access token, neither of which carries scopes — so there is no scope model over the 216 REST operations. Nothing here was derived from a spec; the scope below was read from the provider's own live discovery document.
docs: https://astrologyapi.com/developers/v1/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Astrology Api Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Astrology API uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Astrology API
provider_slug: astrology-api
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: astrology-api-scopes
source_filename: astrology-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://mcp.astrologyapi.com/.well-known/oauth-protected-resource\ndocs: https://astrologyapi.com/developers/v1/mcp-server\ndescription: >-\n  The only OAuth surface AstrologyAPI operates is the MCP server. Its RFC 9728 protected-resource\n  metadata declares exactly one scope. The REST API has no OAuth flow at all — it authenticates with\n  HTTP Basic credentials or a wallet access token, neither of which carries scopes — so there is no\n  scope model over the 216 REST operations. Nothing here was derived from a spec; the scope below was\n  read from the provider's own live discovery document.\noauth_surface:\n  resource: https://mcp.astrologyapi.com/mcp\n  authorization_server_metadata: https://mcp.astrologyapi.com/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://mcp.astrologyapi.com/.well-known/oauth-protected-resource\n  bearer_methods_supported: [header]\n  grant_types_supported: [authorization_code,\
  \ client_credentials, refresh_token]\n  code_challenge_methods_supported: [S256, plain]\n  token_endpoint_auth_methods_supported: [none]\n  dynamic_client_registration: advertised\n  metadata_defect: >-\n    The authorization_servers entry in the protected-resource document, and the issuer in the\n    authorization-server document, both carry literal double-quote characters inside the value, so\n    the issuer they name is not a resolvable URL. See conformance/astrology-api-conformance.yml.\nscopes:\n  - name: offline_access\n    description: >-\n      Standard OIDC/OAuth scope requesting a refresh token so the client can obtain new access tokens\n      without the user being present. Declared in scopes_supported.\n    source: https://mcp.astrologyapi.com/.well-known/oauth-protected-resource\n    verified: probed\nscope_count: 1\nfindings:\n  - >-\n    offline_access is a token-lifetime scope, not a permission. It says the client may keep working\n    while the user is away; it says nothing\
  \ about which of the 109 advertised MCP tools the client\n    may call. There is no read/write split, no per-product scope (Vedic, Western, PDF, Vision, Chat),\n    and no way to issue an agent a credential narrower than the whole tool surface.\n  - >-\n    The REST API has no scope model whatsoever. Authorisation is by plan membership — a subscription\n    key reaches the endpoints in its package and 401s on the rest — which is a commercial boundary\n    enforced server-side, not a scope a client can request or attenuate.\n  - >-\n    A wallet access token reaches every wallet-billed endpoint including PDF generation, which is the\n    most expensive operation on the platform at up to ₹100 per report. There is no scope, no spend\n    cap, and no read-only variant, so an agent handed a token to compute a birth chart is also\n    handed the ability to bill unlimited PDF reports.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/scopes/astrology-api-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Astrology
- Horoscopes
- Zodiac
- Vedic Astrology
- Western Astrology
- Kundli
- Panchang
- Numerology
- Tarot
- Palmistry
- Human Design
- Astrocartography
- PDF Reports
- MCP
- Ephemeris
token_urls: []
---
