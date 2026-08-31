---
api_specs:
- filename: carmd-openapi.yml
  format: yaml
  label: CarMD Vehicle API
  slug: carmd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carmd/refs/heads/main/openapi/carmd-openapi.yml
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes CarMD's domain advertises. These come from the customer-accounts authorization server discovery document served at carmd.com/.well-known/openid-configuration (identical body is served at /.well-known/oauth-authorization-server). The authorization server is Shopify's customer-accounts issuer for CarMD's store (issuer https://shopify.com/authentication/93440671876); the scopes govern shopper identity and the customer-account APIs for the CarMD storefront. The CarMD Vehicle API on api.carmd.com does not use OAuth — and could not be probed at all, because that host refused connections.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Carmd Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CarMD uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CarMD
provider_slug: carmd
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: carmd-scopes
source_filename: carmd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://carmd.com/.well-known/openid-configuration\nprovider: CarMD\nproviderId: carmd\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes CarMD's domain advertises. These come from the customer-accounts\n  authorization server discovery document served at carmd.com/.well-known/openid-configuration (identical\n  body is served at /.well-known/oauth-authorization-server). The authorization server is Shopify's\n  customer-accounts issuer for CarMD's store (issuer https://shopify.com/authentication/93440671876); the\n  scopes govern shopper identity and the customer-account APIs for the CarMD storefront. The CarMD Vehicle\n  API on api.carmd.com does not use OAuth — and could not be probed at all, because that host refused\n  connections.\nauthorization_server:\n  issuer: https://shopify.com/authentication/93440671876\n  authorization_endpoint: https://shopify.com/authentication/93440671876/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/93440671876/oauth/token\n\
  \  jwks_uri: https://shopify.com/authentication/93440671876/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/93440671876/logout\n  grant_types_supported:\n    - authorization_code\n    - refresh_token\n    - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  response_types_supported:\n    - code\n  code_challenge_methods_supported:\n    - S256\n  token_endpoint_auth_methods_supported:\n    - client_secret_basic\n    - client_secret_post\n  id_token_signing_alg_values_supported:\n    - RS256\nscope_count: 4\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope; requests an ID token identifying the shopper.\n  - name: email\n    description: Releases the shopper's email address and email_verified claim.\n  - name: 'customer-account-api:full'\n    description: Full access to the customer-account API for the authenticated shopper.\n  - name: 'customer-account-mcp-api:full'\n    description: >-\n      Full access to the customer-account MCP\
  \ API for the authenticated shopper — the authenticated\n      counterpart to the anonymous UCP commerce MCP endpoint at https://carmd.com/api/ucp/mcp.\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\ndocs: null\ndocs_note: CarMD publishes no scope reference page of its own; the scope list is machine-read from its discovery document.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carmd/refs/heads/main/scopes/carmd-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Automobiles
- Cars
- Diagnostics
- Vehicles
- Automotive
- OBD-II
- Agentic Commerce
- MCP
- E-Commerce
token_urls: []
---
