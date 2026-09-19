---
api_specs:
- filename: google-vault-exports-api-openapi.yml
  format: yaml
  label: Google Vault Exports API
  slug: google-vault-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-exports-api-openapi.yml
- filename: google-vault-heldaccounts-api-openapi.yml
  format: yaml
  label: Google Vault HeldAccounts API
  slug: google-vault-heldaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-heldaccounts-api-openapi.yml
- filename: google-vault-holds-api-openapi.yml
  format: yaml
  label: Google Vault Holds API
  slug: google-vault-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-holds-api-openapi.yml
- filename: google-vault-matters-api-openapi.yml
  format: yaml
  label: Google Vault Matters API
  slug: google-vault-matters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-matters-api-openapi.yml
- filename: google-vault-operations-api-openapi.yml
  format: yaml
  label: Google Vault Operations API
  slug: google-vault-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-operations-api-openapi.yml
- filename: google-vault-saved-queries-api-openapi.yml
  format: yaml
  label: Google Vault Saved Queries API
  slug: google-vault-saved-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/openapi/google-vault-saved-queries-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: https://developers.google.com/workspace/vault/auth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Vault Scopes
name_suffix: OAuth Scopes
note: Google publishes exactly two OAuth 2.0 scopes for the Vault API and no more. The docs page names them and their descriptions but does not say which method needs which — so the per-method binding below was read from the provider's own Discovery document (id vault:v1, revision 20260905), where every one of the 33 methods carries its own scopes[] array. Descriptions are the provider's verbatim strings from that document.
overview: 'Google Vault publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Vault API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Vault
provider_slug: google-vault
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: googleOAuth
  source: openapi/*.yml + discovery/google-vault-discovery-v1.json
  type: oauth2
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/ediscovery
- https://www.googleapis.com/auth/ediscovery.readonly
scopes:
- description: Manage your eDiscovery data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/ediscovery
- description: View your eDiscovery data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/ediscovery.readonly
slug: google-vault-scopes
source_filename: google-vault-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://developers.google.com/workspace/vault/auth\ndocs: https://developers.google.com/workspace/vault/auth\nreferences:\n  - https://developers.google.com/workspace/vault/auth\n  - https://developers.google.com/identity/protocols/oauth2/scopes#vault\n  - discovery/google-vault-discovery-v1.json\nnote: >-\n  Google publishes exactly two OAuth 2.0 scopes for the Vault API and no more. The docs page\n  names them and their descriptions but does not say which method needs which — so the\n  per-method binding below was read from the provider's own Discovery document\n  (id vault:v1, revision 20260905), where every one of the 33 methods carries its own\n  scopes[] array. Descriptions are the provider's verbatim strings from that document.\nschemes:\n  - name: googleOAuth\n    type: oauth2\n    source: openapi/*.yml + discovery/google-vault-discovery-v1.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n  - scope: https://www.googleapis.com/auth/ediscovery\n    description: Manage your eDiscovery data\n    sensitivity: not-published\n    grants: read+write\n    method_count: 33\n    flows: [authorizationCode]\n    sources:\n      - https://developers.google.com/workspace/vault/auth\n      - discovery/google-vault-discovery-v1.json\n  - scope: https://www.googleapis.com/auth/ediscovery.readonly\n    description: View your eDiscovery data\n    sensitivity: not-published\n    grants: read\n    method_count: 11\n    flows: [authorizationCode]\n    sources:\n      - https://developers.google.com/workspace/vault/auth\n      - discovery/google-vault-discovery-v1.json\nscope_bindings:\n  - scope_set: [https://www.googleapis.com/auth/ediscovery]\n    kind: write-only\n    count: 22\n    methods:\n      - vault.matters.addPermissions\n      - vault.matters.close\n      - vault.matters.count\n\
  \      - vault.matters.create\n      - vault.matters.delete\n      - vault.matters.exports.create\n      - vault.matters.exports.delete\n      - vault.matters.holds.accounts.create\n      - vault.matters.holds.accounts.delete\n      - vault.matters.holds.addHeldAccounts\n      - vault.matters.holds.create\n      - vault.matters.holds.delete\n      - vault.matters.holds.removeHeldAccounts\n      - vault.matters.holds.update\n      - vault.matters.removePermissions\n      - vault.matters.reopen\n      - vault.matters.savedQueries.create\n      - vault.matters.savedQueries.delete\n      - vault.matters.undelete\n      - vault.matters.update\n      - vault.operations.cancel\n      - vault.operations.delete\n    note: >-\n      vault.matters.count is a read-shaped operation (it returns search counts) that Google\n      nonetheless gates behind the full ediscovery scope — a read-only token cannot call it.\n  - scope_set:\n      - https://www.googleapis.com/auth/ediscovery\n      - https://www.googleapis.com/auth/ediscovery.readonly\n\
  \    kind: read\n    count: 11\n    methods:\n      - vault.matters.exports.get\n      - vault.matters.exports.list\n      - vault.matters.get\n      - vault.matters.holds.accounts.list\n      - vault.matters.holds.get\n      - vault.matters.holds.list\n      - vault.matters.list\n      - vault.matters.savedQueries.get\n      - vault.matters.savedQueries.list\n      - vault.operations.get\n      - vault.operations.list\nleast_privilege:\n  guidance: >-\n    Google's own wording on the scopes page: \"choose the most narrowly focused scope possible\n    and avoid requesting scopes that your app doesn't require.\" An agent that only reads\n    matters, holds, saved queries, exports and operations needs ediscovery.readonly alone.\n  read_only_sufficient_for: 11\n  requires_full_scope: 22\n  sensitivity_note: >-\n    Google's master OAuth 2.0 scopes page lists both Vault scopes with a description only and\n    attaches no Sensitive/Restricted label to either, so no sensitivity class is asserted\
  \ here.\n    Checked 2026-09-12 against https://developers.google.com/identity/protocols/oauth2/scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-vault/refs/heads/main/scopes/google-vault-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- eDiscovery
- Legal Hold
- Information Governance
- Compliance
- Archiving
- Retention
- Google Workspace
- Audit
token_urls:
- https://oauth2.googleapis.com/token
---
