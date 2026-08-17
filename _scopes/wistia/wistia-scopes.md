---
api_specs:
- filename: wistia-data-api-v1-openapi.yml
  format: yaml
  label: Wistia Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-data-api-v1-openapi.yml
- filename: wistia-data-api-2026-01-openapi.yml
  format: yaml
  label: Wistia Data API 2026-01
  slug: data-api-2026-01
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-data-api-2026-01-openapi.yml
- filename: wistia-data-api-modern-edge-openapi.yml
  format: yaml
  label: Wistia Data API (modern, edge)
  slug: data-api-modern-edge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-data-api-modern-edge-openapi.yml
- filename: wistia-asyncapi.yml
  format: yaml
  label: Wistia Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/asyncapi/wistia-asyncapi.yml
- filename: wistia-account-api-openapi.yml
  format: yaml
  label: Wistia Account API
  slug: wistia-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-account-api-openapi.yml
- filename: wistia-alloweddomains-api-openapi.yml
  format: yaml
  label: Wistia AllowedDomains API
  slug: wistia-alloweddomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-alloweddomains-api-openapi.yml
- filename: wistia-captions-api-openapi.yml
  format: yaml
  label: Wistia Captions API
  slug: wistia-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-captions-api-openapi.yml
- filename: wistia-channels-api-openapi.yml
  format: yaml
  label: Wistia Channels API
  slug: wistia-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-channels-api-openapi.yml
- filename: wistia-customizations-api-openapi.yml
  format: yaml
  label: Wistia Customizations API
  slug: wistia-customizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-customizations-api-openapi.yml
- filename: wistia-folders-api-openapi.yml
  format: yaml
  label: Wistia Folders API
  slug: wistia-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-folders-api-openapi.yml
- filename: wistia-medias-api-openapi.yml
  format: yaml
  label: Wistia Medias API
  slug: wistia-medias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-medias-api-openapi.yml
- filename: wistia-tags-api-openapi.yml
  format: yaml
  label: Wistia Tags API
  slug: wistia-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-tags-api-openapi.yml
- filename: wistia-tokens-api-openapi.yml
  format: yaml
  label: Wistia Tokens API
  slug: wistia-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-tokens-api-openapi.yml
- filename: wistia-webinars-api-openapi.yml
  format: yaml
  label: Wistia Webinars API
  slug: wistia-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-webinars-api-openapi.yml
authorization_urls: []
description: 'Wistia''s OAuth 2.0 authorization surface publishes its scopes in machine-readable form: `scopes_supported` appears in both the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata at api.wistia.com, and the same names are documented in prose on the OAuth2 guide. Two of the seven live scopes (`project:write` and `all:delegate_to_contact_permissions`) are advertised by the metadata but are NOT described on the docs page — recorded here from the metadata with that gap noted rather than invented. Note that OAuth scopes are a separate axis from API-token PERMISSIONS: a Wistia API access token is issued with one of a small set of permission tiers, which is what the API reference cites per-operation. Both are captured below.'
docs: https://docs.wistia.com/docs/authenticating-with-oauth2
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Wistia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wistia uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wistia
provider_slug: wistia
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: wistia-scopes
source_filename: wistia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://api.wistia.com/.well-known/oauth-authorization-server (live RFC 8414 metadata),\n  https://api.wistia.com/.well-known/oauth-protected-resource,\n  https://docs.wistia.com/docs/authenticating-with-oauth2\ndocs: https://docs.wistia.com/docs/authenticating-with-oauth2\ndescription: >-\n  Wistia's OAuth 2.0 authorization surface publishes its scopes in machine-readable form:\n  `scopes_supported` appears in both the RFC 8414 authorization-server metadata and the RFC 9728\n  protected-resource metadata at api.wistia.com, and the same names are documented in prose on the\n  OAuth2 guide. Two of the seven live scopes (`project:write` and\n  `all:delegate_to_contact_permissions`) are advertised by the metadata but are NOT described on the\n  docs page — recorded here from the metadata with that gap noted rather than invented.\n  Note that OAuth scopes are a separate axis from API-token PERMISSIONS: a Wistia API access\
  \ token\n  is issued with one of a small set of permission tiers, which is what the API reference cites\n  per-operation. Both are captured below.\nauthorization_server:\n  issuer: https://api.wistia.com\n  authorization_endpoint: https://api.wistia.com/oauth/authorize\n  token_endpoint: https://api.wistia.com/oauth/token\n  revocation_endpoint: https://api.wistia.com/oauth/revoke\n  introspection_endpoint: https://api.wistia.com/oauth/introspect\n  registration_endpoint: https://api.wistia.com/oauth/register\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  code_challenge_methods_supported:\n  - S256\nscope_count: 7\nscopes:\n- name: all:all\n  description: Anything you can do with the Wistia API is allowed.\n  documented: true\n  sources:\n  - well-known/wistia-oauth-authorization-server.json\n  - https://docs.wistia.com/docs/authenticating-with-oauth2\n- name: all:read\n  description: All requests for data are allowed, but no changes can\
  \ be made.\n  documented: true\n  sources:\n  - well-known/wistia-oauth-authorization-server.json\n  - https://docs.wistia.com/docs/authenticating-with-oauth2\n- name: media:read\n  description: >-\n    All requests for media and project data are allowed. Extends to customization and captions\n    data.\n  documented: true\n  sources:\n  - well-known/wistia-oauth-authorization-server.json\n  - https://docs.wistia.com/docs/authenticating-with-oauth2\n- name: media:upload\n  description: >-\n    Uploading via the API is allowed, as well as fetching data about a single media by hashed ID\n    (medias#show).\n  documented: true\n  sources:\n  - well-known/wistia-oauth-authorization-server.json\n  - https://docs.wistia.com/docs/authenticating-with-oauth2\n- name: stats:read\n  description: All requests for stats data are allowed.\n  documented: true\n  sources:\n  - well-known/wistia-oauth-authorization-server.json\n  - https://docs.wistia.com/docs/authenticating-with-oauth2\n- name: project:write\n\
  \  description: null\n  documented: false\n  note: >-\n    Advertised in scopes_supported by the live authorization-server and protected-resource\n    metadata but absent from the \"Available Scopes\" section of the OAuth2 guide. Name implies\n    write access to projects/folders; no provider description exists to quote, so none is\n    asserted here.\n  sources:\n  - well-known/wistia-oauth-authorization-server.json\n  - well-known/wistia-oauth-protected-resource.json\n- name: all:delegate_to_contact_permissions\n  description: null\n  documented: false\n  note: >-\n    Advertised in scopes_supported but undocumented on the OAuth2 guide. It IS referenced in the\n    API reference: the List Folders operation says that for tokens scoped to a specific user\n    (`all:delegate_to_contact_permissions`), results are limited to the folders that user can see\n    in their content library. So the scope narrows a token to one contact's effective permissions.\n  sources:\n  - well-known/wistia-oauth-authorization-server.json\n\
  \  - https://docs.wistia.com/reference/get_folders\ntoken_permissions:\n  note: >-\n    Distinct from OAuth scopes. Every operation in the API reference states which API-token\n    permission it requires. These four strings are quoted verbatim from the reference pages\n    indexed by https://docs.wistia.com/llms.txt.\n  tiers:\n  - name: Read all folder and media data\n    kind: read\n  - name: Read, update & delete anything\n    kind: write\n  - name: Read detailed stats\n    kind: stats\n  - name: (any scope allowed)\n    kind: unrestricted\n    note: Used by operations such as Get Account Usage that any token may call.\nagent_auth:\n  note: >-\n    The authorization-server metadata carries a non-standard `agent_auth` block aimed at\n    autonomous clients, pointing at a human/agent-readable onboarding document.\n  skill: https://api.wistia.com/auth.md\n  registration_types_supported:\n  - oauth_dynamic_client_registration\n  identity_types_supported:\n  - user_delegated\n  - application\n\
  \  credential_types_supported:\n  - client_secret\n  - pkce\n  - bearer_token\navailability:\n  note: >-\n    The OAuth2 guide states OAuth2 \"is not yet available for all accounts\" and that customers must\n    contact Wistia to have it enabled — the discovery metadata is public, the grant is gated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/scopes/wistia-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Video Hosting
- Video Marketing
- Video Analytics
- Lead Generation
- Webinars
- B2B Marketing
- Video Captions
- Localization
- MCP
- Media Management
token_urls: []
---
