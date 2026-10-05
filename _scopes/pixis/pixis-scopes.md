---
authorization_urls: []
description: Every scope Pixis's authorization server advertises. Read verbatim from the `scopes_supported` array of the OIDC discovery document at auth.pixis.ai, plus the four scopes the Pixis Prism SPA actually requests.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Pixis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pixis publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pixis API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pixis
provider_slug: pixis
schemes: []
scope_count: 14
scope_names:
- openid
- profile
- email
- offline_access
- name
- given_name
- family_name
- nickname
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Request an ID token. Required to use OpenID Connect.
  flows: []
  scope: openid
- description: Basic profile claims (name, family_name, given_name, nickname, picture, and similar).
  flows: []
  scope: profile
- description: The end user's email address.
  flows: []
  scope: email
- description: Issue a refresh token so the session can be renewed without re-authentication.
  flows: []
  scope: offline_access
- description: Full name claim.
  flows: []
  scope: name
- description: Given name claim.
  flows: []
  scope: given_name
- description: Family name claim.
  flows: []
  scope: family_name
- description: Nickname claim.
  flows: []
  scope: nickname
- description: Whether the email address has been verified.
  flows: []
  scope: email_verified
- description: Profile picture URL claim.
  flows: []
  scope: picture
- description: Account creation timestamp claim.
  flows: []
  scope: created_at
- description: Linked identity-provider identities claim.
  flows: []
  scope: identities
- description: Phone number claim.
  flows: []
  scope: phone
- description: Address claim.
  flows: []
  scope: address
slug: pixis-scopes
source_filename: pixis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://auth.pixis.ai/.well-known/openid-configuration\nname: Pixis — OAuth scopes\ndescription: >-\n  Every scope Pixis's authorization server advertises. Read verbatim from the\n  `scopes_supported` array of the OIDC discovery document at auth.pixis.ai, plus the four\n  scopes the Pixis Prism SPA actually requests.\n\nimportant: >-\n  These are OpenID Connect identity/profile-claim scopes, not a Pixis resource permission\n  model. Pixis publishes no API scopes — nothing in the form `campaigns:read`,\n  `creatives:write` or similar — because it publishes no developer API. Do not read this file\n  as evidence of a scoped API authorization model; read it as evidence of an OIDC login.\n\nauthorization_server: https://auth.pixis.ai/\ndocs: null\ndocs_note: >-\n  No scopes/permissions reference page exists on any Pixis surface. pixis.ai has no developer\n  section; prism-docs.pixis.ai documents only end-user product features; the\
  \ Pixis Stoplight\n  workspace (stoplight.io workspace 104607) contains zero public projects.\n\nrequested_by_first_party_app:\n  source: https://prism.pixis.ai/assets/index-Bof3QprB.js\n  audience: https://cross-platform-prod.us.auth0.com/api/v2/\n  scopes: [openid, profile, email, offline_access]\n\nscopes:\n  - name: openid\n    kind: oidc\n    description: Request an ID token. Required to use OpenID Connect.\n    requested_by_pixis_app: true\n  - name: profile\n    kind: oidc\n    description: Basic profile claims (name, family_name, given_name, nickname, picture, and similar).\n    requested_by_pixis_app: true\n  - name: email\n    kind: oidc\n    description: The end user's email address.\n    requested_by_pixis_app: true\n  - name: offline_access\n    kind: oidc\n    description: Issue a refresh token so the session can be renewed without re-authentication.\n    requested_by_pixis_app: true\n  - name: name\n    kind: claim\n    description: Full name claim.\n    requested_by_pixis_app:\
  \ false\n  - name: given_name\n    kind: claim\n    description: Given name claim.\n    requested_by_pixis_app: false\n  - name: family_name\n    kind: claim\n    description: Family name claim.\n    requested_by_pixis_app: false\n  - name: nickname\n    kind: claim\n    description: Nickname claim.\n    requested_by_pixis_app: false\n  - name: email_verified\n    kind: claim\n    description: Whether the email address has been verified.\n    requested_by_pixis_app: false\n  - name: picture\n    kind: claim\n    description: Profile picture URL claim.\n    requested_by_pixis_app: false\n  - name: created_at\n    kind: claim\n    description: Account creation timestamp claim.\n    requested_by_pixis_app: false\n  - name: identities\n    kind: claim\n    description: Linked identity-provider identities claim.\n    requested_by_pixis_app: false\n  - name: phone\n    kind: claim\n    description: Phone number claim.\n    requested_by_pixis_app: false\n  - name: address\n    kind: claim\n \
  \   description: Address claim.\n    requested_by_pixis_app: false\n\nsummary:\n  scope_count: 14\n  api_resource_scopes: 0\n  oidc_scopes: 14\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixis/refs/heads/main/scopes/pixis-scopes.yml
summary_line: 14 scopes
tags:
- Company
- Enterprise
- Advertising
- Marketing
- Artificial Intelligence
- Generative AI
- AdTech
- Marketing Automation
token_bound: false
token_urls: []
---
