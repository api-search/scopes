---
api_specs:
- filename: saperly-api-token-registry-api-openapi.yml
  format: yaml
  label: Saperly API Token Registry API
  slug: saperly-api-token-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-api-token-registry-api-openapi.yml
- filename: saperly-assistant-api-openapi.yml
  format: yaml
  label: Saperly Assistant API
  slug: saperly-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-assistant-api-openapi.yml
- filename: saperly-connections-api-openapi.yml
  format: yaml
  label: Saperly Connections API
  slug: saperly-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-connections-api-openapi.yml
- filename: saperly-consent-api-openapi.yml
  format: yaml
  label: Saperly Consent API
  slug: saperly-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-consent-api-openapi.yml
- filename: saperly-customvoices-api-openapi.yml
  format: yaml
  label: Saperly Custom Voices API
  slug: saperly-customvoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-customvoices-api-openapi.yml
- filename: saperly-health-api-openapi.yml
  format: yaml
  label: Saperly Health API
  slug: saperly-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-health-api-openapi.yml
- filename: saperly-keys-api-openapi.yml
  format: yaml
  label: Saperly Keys API
  slug: saperly-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-keys-api-openapi.yml
- filename: saperly-languages-api-openapi.yml
  format: yaml
  label: Saperly Languages API
  slug: saperly-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-languages-api-openapi.yml
- filename: saperly-messaging-api-openapi.yml
  format: yaml
  label: Saperly Messaging API
  slug: saperly-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-messaging-api-openapi.yml
- filename: saperly-numbers-api-openapi.yml
  format: yaml
  label: Saperly Numbers API
  slug: saperly-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-numbers-api-openapi.yml
- filename: saperly-pricing-api-openapi.yml
  format: yaml
  label: Saperly Pricing API
  slug: saperly-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-pricing-api-openapi.yml
- filename: saperly-usage-api-openapi.yml
  format: yaml
  label: Saperly Usage API
  slug: saperly-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-usage-api-openapi.yml
- filename: saperly-voice-api-openapi.yml
  format: yaml
  label: Saperly Voice API
  slug: saperly-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-voice-api-openapi.yml
- filename: saperly-voices-api-openapi.yml
  format: yaml
  label: Saperly Voices API
  slug: saperly-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-voices-api-openapi.yml
- filename: saperly-workspace-api-openapi.yml
  format: yaml
  label: Saperly Workspace API
  slug: saperly-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-workspace-api-openapi.yml
- filename: saperly-workspace-invitations-api-openapi.yml
  format: yaml
  label: Saperly Workspace Invitations API
  slug: saperly-workspace-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-workspace-invitations-api-openapi.yml
authorization_urls: []
description: 'Saperly has two scope vocabularies: the coarse read/write/admin grant carried by a scoped sap_sk_ API key (bounded further by an optional number allow-list and spend cap), and the OpenID scopes the MCP OAuth 2.1 authorization server at https://saperly.com advertises.'
docs: https://saperly.com/docs/guides/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Saperly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Saperly publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Saperly API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Saperly
provider_slug: saperly
schemes: []
scope_count: 7
scope_names:
- read
- write
- admin
- openid
- profile
- email
- offline_access
scopes:
- description: list and read resources (numbers, connections, messages, calls, usage, consent)
  flows: []
  scope: read
- description: mutating actions — place calls, send SMS, provision/release numbers, record consent, write connections
  flows: []
  scope: write
- description: everything write allows, plus minting, listing, and revoking child keys (keys:admin)
  flows: []
  scope: admin
- description: OpenID Connect identity scope advertised by the MCP OAuth authorization server
  flows: []
  scope: openid
- description: advertised by the MCP OAuth authorization server
  flows: []
  scope: profile
- description: advertised by the MCP OAuth authorization server
  flows: []
  scope: email
- description: refresh-token access (grant_types_supported includes refresh_token)
  flows: []
  scope: offline_access
slug: saperly-scopes
source_filename: saperly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: https://saperly.com/docs/guides/authentication (API-key scope grants); https://saperly.com/.well-known/oauth-authorization-server\n  (MCP OAuth scopes_supported, probed 2026-10-07)\ndocs: https://saperly.com/docs/guides/authentication\ndescription: 'Saperly has two scope vocabularies: the coarse read/write/admin grant carried by a scoped sap_sk_\n  API key (bounded further by an optional number allow-list and spend cap), and the OpenID scopes the MCP OAuth\n  2.1 authorization server at https://saperly.com advertises.'\nscopes:\n- scope: read\n  name: read\n  description: list and read resources (numbers, connections, messages, calls, usage, consent)\n  issuer: api-key grant\n- scope: write\n  name: write\n  description: mutating actions — place calls, send SMS, provision/release numbers, record consent, write connections\n  issuer: api-key grant\n- scope: admin\n  name: admin\n  description: everything write allows, plus minting,\
  \ listing, and revoking child keys (keys:admin)\n  issuer: api-key grant\n- scope: openid\n  name: openid\n  description: OpenID Connect identity scope advertised by the MCP OAuth authorization server\n  issuer: https://saperly.com\n- scope: profile\n  name: profile\n  description: advertised by the MCP OAuth authorization server\n  issuer: https://saperly.com\n- scope: email\n  name: email\n  description: advertised by the MCP OAuth authorization server\n  issuer: https://saperly.com\n- scope: offline_access\n  name: offline_access\n  description: refresh-token access (grant_types_supported includes refresh_token)\n  issuer: https://saperly.com\ngrant_bounds:\n  numberScope: optional allow-list of number ids; number-scoped actions are restricted to exactly those numbers\n  spendLimitCents: hard spend cap in cents enforced at reserve time\n  spendLimitResetPeriod: '''monthly'' (resets at the UTC month boundary) or null for a lifetime cap'\n  child_keys: a key with admin can mint child\
  \ keys whose scopes, allow-list and cap may not exceed its own grant\n    (enforced server-side)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/scopes/saperly-scopes.yml
summary_line: 7 scopes
tags:
- Telephony
- Voice
- SMS
- Phone Numbers
- AI Agents
- Consent
- Compliance
- MCP
- Messaging
- Communications
token_bound: false
token_urls: []
---
