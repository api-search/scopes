---
api_specs:
- filename: experian-address-validation-api-openapi.yml
  format: yaml
  label: Experian Address Validation API
  slug: experian-address-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-address-validation-api-openapi.yml
- filename: experian-bulk-address-api-openapi.yml
  format: yaml
  label: Experian Bulk Address API
  slug: experian-bulk-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-address-api-openapi.yml
- filename: experian-bulk-email-api-openapi.yml
  format: yaml
  label: Experian Bulk Email API
  slug: experian-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-email-api-openapi.yml
- filename: experian-bulk-phone-api-openapi.yml
  format: yaml
  label: Experian Bulk Phone API
  slug: experian-bulk-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-phone-api-openapi.yml
- filename: experian-email-validation-api-openapi.yml
  format: yaml
  label: Experian Email Validation API
  slug: experian-email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-email-validation-api-openapi.yml
- filename: experian-enrichment-api-openapi.yml
  format: yaml
  label: Experian Enrichment API
  slug: experian-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-enrichment-api-openapi.yml
- filename: experian-identity-append-usa-only-api-openapi.yml
  format: yaml
  label: Experian Identity Append (USA only) API
  slug: experian-identity-append-usa-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-identity-append-usa-only-api-openapi.yml
- filename: experian-phone-validation-api-openapi.yml
  format: yaml
  label: Experian Phone Validation API
  slug: experian-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-phone-validation-api-openapi.yml
- filename: experian-reverse-phone-append-usa-only-api-openapi.yml
  format: yaml
  label: Experian Reverse Phone Append (USA only) API
  slug: experian-reverse-phone-append-usa-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-reverse-phone-append-usa-only-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.experian.com/tutorials/oauth-20-tutorial
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Experian Scopes
name_suffix: OAuth Scopes
note: 'Experian publishes no API scope reference — no page names a scope that grants access to a product. What it does serve is discovery metadata on ten hosts, and the scopes_supported arrays in those documents are the only authoritative scope data that exists publicly. They say something worth recording: on the Global Developer Platform, the ONLY supported scope is `openid`. Access to a product is not expressed as a scope at all — it is granted per application in the Developer Portal and enforced server-side, so an access token carries no readable statement of what it may do. On the Aperture side, entitlement is carried entirely by the Auth-Token header plus per-integration domain and IP allowlists, with the standard OIDC profile scopes available from the Okta issuer for user authentication only. In short: scope-based authorization is effectively absent from Experian''s public API surface, and that is a finding, not a gap in the search.'
overview: 'Experian uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Experian
provider_slug: experian
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: experian-scopes
source_filename: experian-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: the OAuth/OIDC discovery documents fetched in this pass and saved verbatim under well-known/\ndocs: https://developer.experian.com/tutorials/oauth-20-tutorial\nnote: 'Experian publishes no API scope reference — no page names a scope that grants access to a\n  product. What it does serve is discovery metadata on ten hosts, and the scopes_supported arrays in\n  those documents are the only authoritative scope data that exists publicly. They say something\n  worth recording: on the Global Developer Platform, the ONLY supported scope is `openid`. Access to a\n  product is not expressed as a scope at all — it is granted per application in the Developer Portal\n  and enforced server-side, so an access token carries no readable statement of what it may do. On\n  the Aperture side, entitlement is carried entirely by the Auth-Token header plus per-integration\n  domain and IP allowlists, with the standard OIDC profile scopes available\
  \ from the Okta issuer for\n  user authentication only. In short: scope-based authorization is effectively absent from\n  Experian''s public API surface, and that is a finding, not a gap in the search.'\nmodel: no product scopes published; entitlement is out-of-band\nissuers:\n- issuer: https://sso.experianaperture.io\n  platform: Experian Data Quality (Aperture) SSO\n  vendor: Okta\n  document: well-known/experian-sso-openid-configuration.json\n  scopes_supported:\n  - openid\n  - email\n  - profile\n  - address\n  - phone\n  - offline_access\n  - groups\n  scope_note: Standard OIDC profile scopes only. None of them grants access to an Aperture API\n    product; they describe the authenticated user.\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  -\
  \ private_key_jwt\n  - none\n  pkce: [S256]\n  admin_scopes_note: 'The oauth-authorization-server document additionally advertises ~80 okta.*\n    administrative scopes (okta.users.manage, okta.apps.manage, okta.apiTokens.manage and so on).\n    These are the Okta tenant management API''s own scopes, exposed because the issuer is an Okta org\n    authorization server — they are not Experian API scopes and are not grantable to an ordinary\n    integration. Recorded here so a reader does not mistake them for an Experian product surface.'\n- issuer: https://us-api.experian.com\n  platform: Experian Global Developer Platform (US production)\n  document: well-known/experian-us-api-openid-configuration.json\n  scopes_supported: [openid]\n  grant_types_supported: [password]\n  token_endpoint_auth_methods_supported: [client_secret_post, none]\n  pkce: null\n- issuer: https://sandbox-us-api.experian.com\n  platform: Experian Global Developer Platform (US sandbox)\n  document: well-known/experian-sandbox-us-api-openid-configuration.json\n\
  \  scopes_supported: [openid]\n  grant_types_supported: [password]\n- issuer: https://uk-api.experian.com\n  platform: Experian Global Developer Platform (UK production)\n  document: well-known/experian-uk-api-openid-configuration.json\n  scopes_supported: [openid]\n  grant_types_supported: [password]\n- issuer: https://sandbox-uk-api.experian.com\n  platform: Experian Global Developer Platform (UK sandbox)\n  document: well-known/experian-sandbox-uk-api-openid-configuration.json\n  scopes_supported: [openid]\n  grant_types_supported: [password]\n- issuer: https://eu-api.experian.com\n  platform: Experian Global Developer Platform (EMEA production)\n  document: well-known/experian-eu-api-openid-configuration.json\n  scopes_supported: [openid]\n  grant_types_supported: [password]\n- issuer: https://sandbox-eu-api.experian.com\n  platform: Experian Global Developer Platform (EMEA sandbox)\n  document: well-known/experian-sandbox-eu-api-openid-configuration.json\n  scopes_supported: [openid]\n\
  \  grant_types_supported: [password]\n- issuer: https://sandbox-in-api.experian.com\n  platform: Experian Global Developer Platform (India sandbox)\n  document: well-known/experian-sandbox-in-api-openid-configuration.json\n  scopes_supported: [openid]\n  grant_types_supported: [password]\n- issuer: https://api.experian.com.au\n  platform: Experian Global Developer Platform (Australia production)\n  document: well-known/experian-api-au-openid-configuration.json\n  scopes_supported: [openid]\n  grant_types_supported: [password]\n- issuer: https://sandbox-api.experian.com.au\n  platform: Experian Global Developer Platform (Australia sandbox)\n  document: well-known/experian-sandbox-api-au-openid-configuration.json\n  scopes_supported: [openid]\n  grant_types_supported: [password]\n- issuer: https://sandbox-api.experian.com.sg\n  platform: Experian Global Developer Platform (Singapore sandbox)\n  document: well-known/experian-sandbox-api-sg-openid-configuration.json\n  scopes_supported: [openid]\n\
  \  grant_types_supported: [password]\nscopes: []\nscopes_note: The scopes[] list is deliberately empty. No Experian product scope exists to record, and\n  listing the OIDC profile scopes or the Okta admin scopes here would misrepresent them as API\n  permissions.\nagent_readiness_implication: 'An agent holding an Experian access token cannot determine from the\n  token, or from any discovery document, which products it may call. It finds out by calling and\n  reading the 403. The published 403 causes confirm this is the intended design — \"the token is valid,\n  but it is associated with another product or you have insufficient credits.\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/scopes/experian-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Credit Bureau
- Credit Reporting
- Identity Verification
- Fraud Prevention
- Data Quality
- Address Validation
- Email Validation
- Phone Validation
- Data Enrichment
- Financial-Services
- Risk Management
token_urls: []
---
