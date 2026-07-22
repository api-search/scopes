---
api_specs:
- filename: the-mobile-first-company-allo-openapi.json
  format: json
  label: Allo API
  slug: allo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-mobile-first-company/refs/heads/main/openapi/the-mobile-first-company-allo-openapi.json
authorization_urls: []
description: ''
docs: https://help.withallo.com/en/v2/api-reference/guides/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: The Mobile First Company Scopes
name_suffix: OAuth Scopes
note: Scopes are attached to Allo API keys (created in Settings > API) and to OAuth clients / the MCP server. The 19 scopes below are advertised verbatim in the OAuth authorization-server metadata; WEBHOOKS_READ_WRITE, BILLING and PARTNER are documented in the API-key scope reference / partner endpoints but are not listed in scopes_supported.
overview: 'The Mobile First Company uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Mobile First Company
provider_slug: the-mobile-first-company
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: the-mobile-first-company-scopes
source_filename: the-mobile-first-company-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://help.withallo.com/en/v2/api-reference/guides/authentication\nsource: >-\n  https://api.withallo.com/.well-known/oauth-authorization-server (scopes_supported)\n  + Allo API-key scope reference (authentication guide) + partner endpoint scope\n  requirements in openapi/the-mobile-first-company-allo-openapi.json\napi: Allo API\noauth:\n  issuer: https://api.withallo.com\n  authorization_endpoint: https://api.withallo.com/v1/oauth/authorize\n  token_endpoint: https://api.withallo.com/v1/oauth/token\n  revocation_endpoint: https://api.withallo.com/v1/oauth/revoke\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_post\nnote: >-\n  Scopes are attached to Allo API keys (created in Settings > API) and to OAuth\n  clients / the MCP server. The 19 scopes below are advertised\
  \ verbatim in the\n  OAuth authorization-server metadata; WEBHOOKS_READ_WRITE, BILLING and PARTNER\n  are documented in the API-key scope reference / partner endpoints but are not\n  listed in scopes_supported.\nscopes:\n- name: CONVERSATIONS_READ\n  source: oauth-metadata\n  description: Read calls, SMS, and conversation history.\n- name: CONVERSATIONS_WRITE\n  source: oauth-metadata\n  description: Write / mutate conversation items (e.g. update summaries, mark read/archived).\n- name: CONTACTS_READ\n  source: oauth-metadata\n  description: Read contact information.\n- name: CONTACTS_READ_WRITE\n  source: oauth-metadata\n  description: Read and write contact information.\n- name: SMS_SEND\n  source: oauth-metadata\n  description: Send SMS and MMS messages.\n- name: DIALING_QUEUE_READ_WRITE\n  source: oauth-metadata\n  description: Manage Power Dialer queues.\n- name: PHONE_NUMBERS_READ\n  source: oauth-metadata\n  description: List phone numbers and their capabilities.\n- name: TAGS_READ\n\
  \  source: oauth-metadata\n  description: List available tags.\n- name: TAGS_WRITE\n  source: oauth-metadata\n  description: Add and remove tags on conversation items.\n- name: USERS_READ\n  source: oauth-metadata\n  description: List team members and their roles.\n- name: CRM_READ\n  source: oauth-metadata\n  description: Read CRM people, companies, and deals.\n- name: CRM_WRITE\n  source: oauth-metadata\n  description: Create and update CRM people, companies, and deals.\n- name: CRM_DELETE\n  source: oauth-metadata\n  description: Delete CRM records (e.g. deals).\n- name: SUMMARY_TEMPLATES_READ\n  source: oauth-metadata\n  description: Read call summary templates.\n- name: SUMMARY_TEMPLATES_WRITE\n  source: oauth-metadata\n  description: Create, update, and delete call summary templates.\n- name: NOTES_READ\n  source: oauth-metadata\n  description: Read notes.\n- name: NOTES_WRITE\n  source: oauth-metadata\n  description: Create and update notes.\n- name: THREADS_READ\n  source: oauth-metadata\n\
  \  description: Read message threads.\n- name: THREADS_WRITE\n  source: oauth-metadata\n  description: Write / mutate message threads.\n- name: WEBHOOKS_READ_WRITE\n  source: docs\n  description: Create and manage webhook configurations.\n- name: BILLING\n  source: docs\n  description: Access billing and subscription information.\n- name: PARTNER\n  source: docs\n  description: >-\n    Reseller / partner scope required to provision and manage Allo accounts for\n    your customers (POST/GET/DELETE /v2/api/partner/accounts).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-mobile-first-company/refs/heads/main/scopes/the-mobile-first-company-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Communication
- Telephony
- Voice
- SMS
- CRM
- Artificial Intelligence
- MCP
- Webhooks
- Small Business
token_urls: []
---
