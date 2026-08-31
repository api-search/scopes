---
authorization_urls:
- https://id.uh.live/realms/uhlive/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
- deviceCode
- password
- refreshToken
- tokenExchange
- jwtBearer
- uma
- ciba
kind: oauth-scopes
layout: scope
method: probed
name: Allo Media Scopes
name_suffix: OAuth Scopes
note: 'This is the most interesting thing recovered from Allo-Media in this pass. The developer documentation states only that you exchange a client_id and client_secret for a token; it never mentions scopes at all. The realm''s discovery document exposes a per-product scope model that the docs are silent about, including one scope — `voip-callapi` — for a surface that has no public documentation page whatsoever. Because these come from `scopes_supported` on the realm, they are the scopes the AUTHORIZATION SERVER can issue, not necessarily the scopes any given client is granted or that a given API enforces. Product mappings below are marked with an honest confidence: the names map onto documented product surfaces one-for-one, but no provider documentation confirms the binding.'
overview: 'Allo-Media publishes 19 OAuth 2.0 scopes via the clientCredentials, authorizationCode, deviceCode, password, refreshToken, tokenExchange, jwtBearer, uma, and ciba flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allo-Media API on a user''s behalf.


  Tokens are issued from https://id.uh.live/realms/uhlive/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allo-Media
provider_slug: allo-media
schemes:
- discovery: https://id.uh.live/realms/uhlive/.well-known/openid-configuration
  flows:
  - documented: true
    flow: clientCredentials
    note: the only flow the provider's developer docs describe
    tokenUrl: https://id.uh.live/realms/uhlive/protocol/openid-connect/token
  - authorizationUrl: https://id.uh.live/realms/uhlive/protocol/openid-connect/auth
    documented: false
    flow: authorizationCode
    note: Advertised by the realm but not documented for API consumers; presumably serves the WebApp/Scribr human login rather than API integrations.
    tokenUrl: https://id.uh.live/realms/uhlive/protocol/openid-connect/token
  - deviceAuthorizationUrl: https://id.uh.live/realms/uhlive/protocol/openid-connect/auth/device
    documented: false
    flow: deviceCode
  - documented: false
    flow: password
    note: Resource-owner password grant is still enabled on the realm. It is deprecated in OAuth 2.1 and generally should be off; flagged as an observation, not an exploit.
  - documented: false
    flow: refreshToken
  - documented: false
    flow: tokenExchange
    grant: urn:ietf:params:oauth:grant-type:token-exchange
  - documented: false
    flow: jwtBearer
    grant: urn:ietf:params:oauth:grant-type:jwt-bearer
  - documented: false
    flow: uma
    grant: urn:ietf:params:oauth:grant-type:uma-ticket
  - backchannel_authentication_endpoint: https://id.uh.live/realms/uhlive/protocol/openid-connect/ext/ciba/auth
    documented: false
    flow: ciba
    grant: urn:openid:params:grant-type:ciba
  issuer: https://id.uh.live/realms/uhlive
  jwks_uri: https://id.uh.live/realms/uhlive/protocol/openid-connect/certs
  name: uhlive_keycloak_realm
  type: openIdConnect
scope_count: 19
scope_names:
- activate
- stream-h2h
- stream-h2h-v2
- stream-h2b
- voip-callapi
- scribr
- service_account
- app_metadata
- basic
- openid
- profile
- email
- address
- phone
- roles
- web-origins
- offline_access
- acr
- microprofile-jwt
scopes:
- description: Access to the Activate API — the read-only REST surface over processed calls at https://activate.uh.live.
  flows: []
  scope: activate
- description: Access to the Stream API for humans (real-time human-to-human transcription over WebSocket) — protocol V1.
  flows: []
  scope: stream-h2h
- description: Access to the Stream API for humans, protocol V2 — the current version.
  flows: []
  scope: stream-h2h-v2
- description: Access to the Stream API for voicebots (human-to-bot, MRCP/WebSocket).
  flows: []
  scope: stream-h2b
- description: A VoIP / call API scope with no corresponding public documentation page.
  flows: []
  scope: voip-callapi
- description: Access to Scribr, the hosted search interface over calls and transcripts.
  flows: []
  scope: scribr
- description: Machine/service-account identity scope (Keycloak client credentials).
  flows: []
  scope: service_account
- description: Application metadata claims.
  flows: []
  scope: app_metadata
- description: Keycloak built-in basic claims scope.
  flows: []
  scope: basic
- description: OIDC required scope.
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: address
- description: ''
  flows: []
  scope: phone
- description: ''
  flows: []
  scope: roles
- description: ''
  flows: []
  scope: web-origins
- description: ''
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: acr
- description: ''
  flows: []
  scope: microprofile-jwt
slug: allo-media-scopes
source_filename: allo-media-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://id.uh.live/realms/uhlive/.well-known/openid-configuration\nartifact: well-known/allo-media-openid-configuration.json\ndocs: null\ndocs_note: >-\n  The provider publishes NO scopes or permissions reference page. Every scope\n  below was read from the live OIDC discovery document of the Keycloak realm the\n  provider's own documentation names as its token endpoint — not from\n  documentation, and not derived from an OpenAPI (there is none).\nnote: >-\n  This is the most interesting thing recovered from Allo-Media in this pass. The\n  developer documentation states only that you exchange a client_id and\n  client_secret for a token; it never mentions scopes at all. The realm's\n  discovery document exposes a per-product scope model that the docs are silent\n  about, including one scope — `voip-callapi` — for a surface that has no public\n  documentation page whatsoever.\n  Because these come from `scopes_supported` on the\
  \ realm, they are the scopes the\n  AUTHORIZATION SERVER can issue, not necessarily the scopes any given client is\n  granted or that a given API enforces. Product mappings below are marked with an\n  honest confidence: the names map onto documented product surfaces\n  one-for-one, but no provider documentation confirms the binding.\nschemes:\n- name: uhlive_keycloak_realm\n  type: openIdConnect\n  issuer: https://id.uh.live/realms/uhlive\n  discovery: https://id.uh.live/realms/uhlive/.well-known/openid-configuration\n  jwks_uri: https://id.uh.live/realms/uhlive/protocol/openid-connect/certs\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.uh.live/realms/uhlive/protocol/openid-connect/token\n    documented: true\n    note: the only flow the provider's developer docs describe\n  - flow: authorizationCode\n    authorizationUrl: https://id.uh.live/realms/uhlive/protocol/openid-connect/auth\n    tokenUrl: https://id.uh.live/realms/uhlive/protocol/openid-connect/token\n    documented:\
  \ false\n    note: >-\n      Advertised by the realm but not documented for API consumers; presumably\n      serves the WebApp/Scribr human login rather than API integrations.\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://id.uh.live/realms/uhlive/protocol/openid-connect/auth/device\n    documented: false\n  - flow: password\n    documented: false\n    note: >-\n      Resource-owner password grant is still enabled on the realm. It is\n      deprecated in OAuth 2.1 and generally should be off; flagged as an\n      observation, not an exploit.\n  - flow: refreshToken\n    documented: false\n  - flow: tokenExchange\n    grant: urn:ietf:params:oauth:grant-type:token-exchange\n    documented: false\n  - flow: jwtBearer\n    grant: urn:ietf:params:oauth:grant-type:jwt-bearer\n    documented: false\n  - flow: uma\n    grant: urn:ietf:params:oauth:grant-type:uma-ticket\n    documented: false\n  - flow: ciba\n    grant: urn:openid:params:grant-type:ciba\n    backchannel_authentication_endpoint:\
  \ https://id.uh.live/realms/uhlive/protocol/openid-connect/ext/ciba/auth\n    documented: false\nscopes:\n- scope: activate\n  description: >-\n    Access to the Activate API — the read-only REST surface over processed calls\n    at https://activate.uh.live.\n  product: Allo-Media Activate API\n  api: allo-media-activate-api\n  confidence: high\n  sources: [well-known/allo-media-openid-configuration.json]\n- scope: stream-h2h\n  description: >-\n    Access to the Stream API for humans (real-time human-to-human transcription\n    over WebSocket) — protocol V1.\n  product: Allo-Media Stream API for Humans\n  api: allo-media-stream-api-humans\n  confidence: high\n  sources: [well-known/allo-media-openid-configuration.json]\n- scope: stream-h2h-v2\n  description: >-\n    Access to the Stream API for humans, protocol V2 — the current version.\n  product: Allo-Media Stream API for Humans\n  api: allo-media-stream-api-humans\n  confidence: high\n  note: >-\n    A separate scope per protocol version.\
  \ That is real evidence the V1/V2 split\n    is enforced at the authorization server, so a V1 client's token will not\n    simply work against V2 — a migration detail the deprecation docs do not\n    mention.\n  sources: [well-known/allo-media-openid-configuration.json]\n- scope: stream-h2b\n  description: >-\n    Access to the Stream API for voicebots (human-to-bot, MRCP/WebSocket).\n  product: Allo-Media Stream API for Voicebots\n  api: allo-media-stream-api-voicebots\n  confidence: high\n  sources: [well-known/allo-media-openid-configuration.json]\n- scope: voip-callapi\n  description: >-\n    A VoIP / call API scope with no corresponding public documentation page.\n  product: unknown\n  confidence: low\n  note: >-\n    The only scope that does not map onto a documented product. There is no\n    \"call API\" or VoIP section anywhere in the documentation sitemap. Recorded as\n    an undocumented surface rather than guessed at — this is a real question to\n    put to the provider, not\
  \ a finding to publish as a product.\n  sources: [well-known/allo-media-openid-configuration.json]\n- scope: scribr\n  description: >-\n    Access to Scribr, the hosted search interface over calls and transcripts.\n  product: Scribr\n  confidence: high\n  note: >-\n    Scribr is documented as a product UI with its own search syntax; the scope\n    suggests it is served by an API behind the realm, though no Scribr API is\n    documented.\n  sources: [well-known/allo-media-openid-configuration.json]\n- scope: service_account\n  description: Machine/service-account identity scope (Keycloak client credentials).\n  category: platform\n  confidence: medium\n  sources: [well-known/allo-media-openid-configuration.json]\n- scope: app_metadata\n  description: Application metadata claims.\n  category: platform\n  confidence: medium\n  sources: [well-known/allo-media-openid-configuration.json]\n- scope: basic\n  description: Keycloak built-in basic claims scope.\n  category: standard\n  confidence:\
  \ high\n  sources: [well-known/allo-media-openid-configuration.json]\n- scope: openid\n  description: OIDC required scope.\n  category: standard\n  confidence: high\n- scope: profile\n  category: standard\n- scope: email\n  category: standard\n- scope: address\n  category: standard\n- scope: phone\n  category: standard\n- scope: roles\n  category: standard\n- scope: web-origins\n  category: standard\n- scope: offline_access\n  category: standard\n- scope: acr\n  category: standard\n- scope: microprofile-jwt\n  category: standard\nsummary:\n  scopes_total: 19\n  product_scopes: 6\n  platform_scopes: 2\n  standard_oidc_scopes: 11\n  documented_by_provider: 0\n  undocumented_product_surfaces: 1\nx-security-posture:\n  note: >-\n    Read from the same discovery document. This realm is configured well above the\n    baseline, which is worth recording because it contrasts sharply with the\n    provider's thin API documentation.\n  pkce: [plain, S256]\n  pkce_note: >-\n    S256 supported; `plain`\
  \ is also still advertised, which is the weaker option\n    OAuth 2.1 removes.\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  mtls_client_auth: true\n  mtls_bound_access_tokens: true\n  dpop: true\n  dpop_algs: [PS384, RS384, EdDSA, ES384, ES256, RS256, ES512, PS256, PS512, RS512]\n  introspection_endpoint: https://id.uh.live/realms/uhlive/protocol/openid-connect/token/introspect\n  revocation_endpoint: https://id.uh.live/realms/uhlive/protocol/openid-connect/revoke\n  dynamic_client_registration_endpoint: https://id.uh.live/realms/uhlive/clients-registrations/openid-connect\n  assessment: >-\n    mTLS-bound access tokens, DPoP, private_key_jwt and a dynamic client\n    registration endpoint are all advertised — capabilities most catalogued\n    providers do not offer. They are also Keycloak defaults, so their presence\n    proves the platform supports them, not that Allo-Media requires\
  \ or documents\n    them. The gap here is documentation, not capability: a customer reading the\n    developer docs would never learn that sender-constrained tokens are an option.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allo-media/refs/heads/main/scopes/allo-media-scopes.yml
summary_line: 19 scopes · clientCredentials/authorizationCode/deviceCode/password/refreshToken/tokenExchange/jwtBearer/uma/ciba
tags:
- Company
- Ai Data
- Speech Recognition
- Speech To Text
- Conversation Intelligence
- Call Tracking
- Voice AI
- Natural Language Processing
- Call Analytics
- Contact Center
- Speech Analytics
- Transcription
- France
token_urls:
- https://id.uh.live/realms/uhlive/protocol/openid-connect/token
---
