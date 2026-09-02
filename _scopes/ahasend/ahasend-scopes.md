---
api_specs:
- filename: ahasend-accounts-api-openapi.yml
  format: yaml
  label: AhaSend Accounts API
  slug: ahasend-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-accounts-api-openapi.yml
- filename: ahasend-api-keys-api-openapi.yml
  format: yaml
  label: AhaSend API Keys API
  slug: ahasend-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-api-keys-api-openapi.yml
- filename: ahasend-domains-api-openapi.yml
  format: yaml
  label: AhaSend Domains API
  slug: ahasend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-domains-api-openapi.yml
- filename: ahasend-email-api-openapi.yml
  format: yaml
  label: AhaSend Email API
  slug: ahasend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-email-api-openapi.yml
- filename: ahasend-messages-api-openapi.yml
  format: yaml
  label: AhaSend Messages API
  slug: ahasend-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-messages-api-openapi.yml
- filename: ahasend-routes-api-openapi.yml
  format: yaml
  label: AhaSend Routes API
  slug: ahasend-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-routes-api-openapi.yml
- filename: ahasend-smtp-credentials-api-openapi.yml
  format: yaml
  label: AhaSend SMTP Credentials API
  slug: ahasend-smtp-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-smtp-credentials-api-openapi.yml
- filename: ahasend-statistics-api-openapi.yml
  format: yaml
  label: AhaSend Statistics API
  slug: ahasend-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-statistics-api-openapi.yml
- filename: ahasend-suppressions-api-openapi.yml
  format: yaml
  label: AhaSend Suppressions API
  slug: ahasend-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-suppressions-api-openapi.yml
- filename: ahasend-utility-api-openapi.yml
  format: yaml
  label: AhaSend Utility API
  slug: ahasend-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-utility-api-openapi.yml
- filename: ahasend-webhooks-api-openapi.yml
  format: yaml
  label: AhaSend Webhooks API
  slug: ahasend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-webhooks-api-openapi.yml
- filename: ahasend-sub-accounts-api-openapi.yml
  format: yaml
  label: AhaSend Sub Accounts API
  slug: ahasend-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-sub-accounts-api-openapi.yml
authorization_urls: []
description: ''
docs: https://ahasend.com/docs/api-reference/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ahasend Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AhaSend uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AhaSend
provider_slug: ahasend
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ahasend-scopes
source_filename: ahasend-scopes.yml
source_heading: OAuth Scopes
source_url: https://ahasend.com/docs/api-reference/scopes.md
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://ahasend.com/docs/api-reference/scopes\ndocs: https://ahasend.com/docs/api-reference/scopes\nsources:\n  - https://ahasend.com/docs/api-reference/scopes.md\n  - https://ahasend.com/docs/security/scoped-credentials.md\n  - https://ahasend.com/docs/api-reference/sub-accounts/overview.md\n  - openapi/_original/ahasend-openapi-v2.yaml\nprovider: AhaSend\nproviderId: ahasend\nscheme: api-key-scopes\noauth2: false\nscheme_note: >-\n  IMPORTANT — these are NOT OAuth 2.0 scopes. AhaSend declares a single `BearerAuth` HTTP bearer\n  scheme in its OpenAPI and no oauth2 flow anywhere. What it does publish is a granular\n  authorization model attached to each API key, and the OpenAPI carries those role names as the\n  VALUES of its per-operation security requirements — the contract's own words: \"Non-empty\n  Security Requirement values are AhaSend API-key roles. Roles listed within one requirement\n  object are jointly required;\
  \ separate requirement objects are alternatives.\" The file is filed\n  under scopes/ because that is what the model is; the label OAuthScopes on the apis.yml pointer\n  is the catalog's canonical string, not a claim that AhaSend runs OAuth.\noidc:\n  supported: true\n  role: relying-party\n  note: >-\n    AhaSend supports OpenID Connect SSO (with PKCE and multi-domain support) for DASHBOARD login\n    on the Max plan. It consumes a customer's identity provider; it does not issue OAuth tokens\n    for its API.\n  docs: https://ahasend.com/docs/security/sso.md\nscope_kinds:\n  - kind: static\n    description: Fixed account-level permissions, e.g. accounts:read, domains:write.\n  - kind: global\n    description: Ends with :all, covering every domain in the account, e.g. messages:send:all.\n  - kind: domain-specific\n    description: Restricted to one domain, e.g. messages:send:{example.com}.\n  - kind: wildcard\n    value: '*'\n    description: Grants everything. AhaSend advises using it\
  \ only for development and testing.\nscope_count: 51\nscopes:\n  - {name: 'accounts:read', description: Read account information}\n  - {name: 'accounts:write', description: Update account settings}\n  - {name: 'accounts:billing', description: Access billing information}\n  - {name: 'accounts:members:read', description: View account members}\n  - {name: 'accounts:members:add', description: Add new account members}\n  - {name: 'accounts:members:update', description: Update member permissions}\n  - {name: 'accounts:members:remove', description: Remove account members}\n  - {name: 'domains:read', description: List and view domain information}\n  - {name: 'domains:write', description: Add and update domains}\n  - {name: 'domains:delete:{domain}', description: Delete a specific domain, kind: domain-specific, note: Domain deletion has no global form — a :all scope cannot delete a domain.}\n  - {name: 'messages:send:all', description: Send messages from any domain, kind: global}\n  - {name: 'messages:send:{domain}',\
  \ description: Send messages from a specific domain, kind: domain-specific}\n  - {name: 'messages:cancel:all', description: Cancel messages from any domain, kind: global}\n  - {name: 'messages:cancel:{domain}', description: Cancel messages from a specific domain, kind: domain-specific}\n  - {name: 'messages:read:all', description: Read messages from any domain, kind: global}\n  - {name: 'messages:read:{domain}', description: Read messages from a specific domain, kind: domain-specific}\n  - {name: 'webhooks:read:all', description: Read webhooks for all domains, kind: global}\n  - {name: 'webhooks:write:all', description: Create/update webhooks for all domains, kind: global}\n  - {name: 'webhooks:delete:all', description: Delete webhooks for all domains, kind: global}\n  - {name: 'webhooks:read:{domain}', description: Read webhooks for a specific domain, kind: domain-specific}\n  - {name: 'webhooks:write:{domain}', description: Create/update webhooks for a specific domain, kind: domain-specific}\n\
  \  - {name: 'webhooks:delete:{domain}', description: Delete webhooks for a specific domain, kind: domain-specific}\n  - {name: 'routes:read:all', description: Read routes for all domains, kind: global}\n  - {name: 'routes:write:all', description: Create/update routes for all domains, kind: global}\n  - {name: 'routes:delete:all', description: Delete routes for all domains, kind: global}\n  - {name: 'routes:read:{domain}', description: Read routes for a specific domain, kind: domain-specific}\n  - {name: 'routes:write:{domain}', description: Create/update routes for a specific domain, kind: domain-specific}\n  - {name: 'routes:delete:{domain}', description: Delete routes for a specific domain, kind: domain-specific}\n  - {name: 'smtp-credentials:read:all', description: Read SMTP credentials for all domains, kind: global}\n  - {name: 'smtp-credentials:write:all', description: Create/update SMTP credentials for all domains, kind: global}\n  - {name: 'smtp-credentials:delete:all', description:\
  \ Delete SMTP credentials for all domains, kind: global}\n  - {name: 'smtp-credentials:read:{domain}', description: Read SMTP credentials for a specific domain, kind: domain-specific}\n  - {name: 'smtp-credentials:write:{domain}', description: Create/update SMTP credentials for a specific domain, kind: domain-specific}\n  - {name: 'smtp-credentials:delete:{domain}', description: Delete SMTP credentials for a specific domain, kind: domain-specific}\n  - {name: 'suppressions:read', description: View suppression lists}\n  - {name: 'suppressions:write', description: Add suppressions}\n  - {name: 'suppressions:delete', description: Remove specific suppressions}\n  - {name: 'suppressions:wipe', description: Clear the entire suppression list, note: Separated from suppressions:delete on purpose — the wipe is irreversible.}\n  - {name: 'api-keys:read', description: List and view API keys}\n  - {name: 'api-keys:write', description: Create and update API keys}\n  - {name: 'api-keys:delete', description:\
  \ Delete API keys}\n  - {name: 'sub-accounts:read', description: List and read sub accounts under the parent}\n  - {name: 'sub-accounts:write', description: Create and update sub accounts}\n  - {name: 'sub-accounts:delete', description: Soft-delete sub accounts}\n  - {name: 'sub-accounts:suspend', description: Suspend and unsuspend sub accounts}\n  - {name: 'sub-accounts:usage', description: Read per-sub-account usage and allocated cost}\n  - {name: 'sub-account-api-keys:read', description: List and read API keys owned by sub accounts}\n  - {name: 'sub-account-api-keys:write', description: Create and update API keys owned by sub accounts}\n  - {name: 'sub-account-api-keys:delete', description: Delete API keys owned by sub accounts}\n  - {name: 'statistics-transactional:read:all', description: Read statistics for all domains, kind: global}\n  - {name: 'statistics-transactional:read:{domain}', description: Read statistics for a specific domain, kind: domain-specific}\nenforcement_notes:\n\
  \  - >-\n    Scopes are enforced per operation and, for domain-scoped keys, per resource — a route or\n    webhook is authorized against the domain it belongs to, not just against the caller.\n  - >-\n    Sub-account API keys are managed only with PARENT credentials holding the relevant\n    sub-account-api-keys:* scope. A sub account's own credentials cannot create or manage its\n    nested keys.\n  - >-\n    Scopes compose with IP allow lists: a key outside its allow list is rejected on every\n    endpoint regardless of the scopes it holds.\n  - >-\n    A scope failure and an IP-allow-list failure both return HTTP 403 with a free-text message\n    and no machine-distinguishable marker.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/scopes/ahasend-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhook
token_urls: []
---
