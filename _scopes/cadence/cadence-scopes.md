---
authorization_urls: []
description: The only OAuth 2.0 / OpenID Connect scope surface Cadence Design Systems publishes anonymously. It is served by Cadence Online Support (support.cadence.com), a Salesforce Experience Cloud tenant acting as an OpenID Provider with issuer https://support.cadence.com. The scope list below is read verbatim from that discovery document.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cadence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cadence Design Systems uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cadence Design Systems
provider_slug: cadence
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cadence-scopes
source_filename: cadence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://support.cadence.com/.well-known/openid-configuration\ndescription: >-\n  The only OAuth 2.0 / OpenID Connect scope surface Cadence Design Systems\n  publishes anonymously. It is served by Cadence Online Support\n  (support.cadence.com), a Salesforce Experience Cloud tenant acting as an\n  OpenID Provider with issuer https://support.cadence.com. The scope list below\n  is read verbatim from that discovery document.\nhonesty_note: >-\n  These are the Salesforce platform scope names the tenant advertises, not a\n  Cadence-designed API permission model. They govern OIDC/OAuth clients\n  authenticating against the Cadence support portal — not the Orion or MMDS\n  APIs, which authenticate with an account-issued token and have no published\n  scope surface at all (see authentication/cadence-authentication.yml).\ndocs: null\ndocs_note: >-\n  Cadence publishes no scopes/permissions reference page. This artifact records\n  the\
  \ machine-readable discovery document instead, which is stronger evidence\n  than prose but weaker in coverage — no per-scope description is published.\n\nissuer: https://support.cadence.com\nendpoints:\n  authorization: https://support.cadence.com/services/oauth2/authorize\n  token: https://support.cadence.com/services/oauth2/token\n  userinfo: https://support.cadence.com/services/oauth2/userinfo\n  revocation: https://support.cadence.com/services/oauth2/revoke\n  introspection: https://support.cadence.com/services/oauth2/introspect\n  registration: https://support.cadence.com/services/oauth2/register\n  end_session: https://support.cadence.com/services/auth/idp/oidc/logout\n  jwks: https://support.cadence.com/id/keys\ngrant_and_client_support:\n  response_types_supported: [code, token, token id_token]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, private_key_jwt]\n  id_token_signing_alg_values_supported: [RS256]\n  dpop_signing_alg_values_supported:\
  \ [RS256, RS384, RS512, ES256, ES384, ES512, EdDSA]\n  subject_types_supported: [public]\n  dynamic_client_registration: true\n\nscopes:\n  - {name: openid, description: null}\n  - {name: profile, description: null}\n  - {name: email, description: null}\n  - {name: address, description: null}\n  - {name: phone, description: null}\n  - {name: id, description: null}\n  - {name: api, description: null}\n  - {name: web, description: null}\n  - {name: full, description: null}\n  - {name: lightning, description: null}\n  - {name: visualforce, description: null}\n  - {name: content, description: null}\n  - {name: refresh_token, description: null}\n  - {name: offline_access, description: null}\n  - {name: custom_permissions, description: null}\n  - {name: chatter_api, description: null}\n  - {name: chatbot_api, description: null}\n  - {name: interaction_api, description: null}\n  - {name: wave_api, description: null}\n  - {name: eclair_api, description: null}\n  - {name: pardot_api, description:\
  \ null}\n  - {name: scrt_api, description: null}\n  - {name: sfap_api, description: null}\n  - {name: einstein_gpt_api, description: null}\n  - {name: mcp_api, description: null}\n  - {name: user_registration_api, description: null}\n  - {name: pwdless_login_api, description: null}\n  - {name: forgot_password, description: null}\n  - {name: data_cloud_user_claims, description: null}\n  - {name: cdp_api, description: null}\n  - {name: cdp_query_api, description: null}\n  - {name: cdp_profile_api, description: null}\n  - {name: cdp_ingest_api, description: null}\n  - {name: cdp_segment_api, description: null}\n  - {name: cdp_identityresolution_api, description: null}\n  - {name: cdp_calculated_insight_api, description: null}\nscope_count: 36\ndescription_coverage: >-\n  0 of 36 scopes carry a published description — the discovery document lists\n  names only and Cadence publishes no scope reference page.\n\nclaims_supported:\n  - active\n  - address\n  - email\n  - email_verified\n  - family_name\n\
  \  - given_name\n  - is_app_installed\n  - language\n  - locale\n  - name\n  - nickname\n  - organization_id\n  - phone_number\n  - phone_number_verified\n  - photos\n  - picture\n  - preferred_username\n  - profile\n  - sub\n  - updated_at\n  - urls\n  - user_id\n  - user_type\n  - zoneinfo\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadence/refs/heads/main/scopes/cadence-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Electronic Design Automation
- EDA
- Semiconductors
- Chip Design
- IC Design
- PCB Design
- Software
- Company
token_urls: []
---
