---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Human Longevity Scopes
name_suffix: OAuth Scopes
note: These are the scopes_supported values Human Longevity's own OpenID Connect discovery document advertises for the HLI client-portal authorization server. They are the standard OIDC scope set plus Auth0's per-claim scopes; there are NO product or API scopes, because Human Longevity publishes no API for a third party to be authorized against. No scope reference page exists on the provider's site — this artifact is derived entirely from the machine-readable discovery document.
overview: 'Human Longevity publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Human Longevity API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Human Longevity
provider_slug: human-longevity
schemes: []
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- address
- phone
- email
- email_verified
- name
- given_name
- family_name
- nickname
- picture
- created_at
- identities
scopes:
- description: Standard OIDC scope requesting an ID token for the authenticated client.
  flows: []
  scope: openid
- description: Standard OIDC scope releasing the basic profile claim set.
  flows: []
  scope: profile
- description: Standard OIDC scope requesting a refresh token.
  flows: []
  scope: offline_access
- description: Standard OIDC scope releasing the address claim.
  flows: []
  scope: address
- description: Standard OIDC scope releasing phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Releases the email claim.
  flows: []
  scope: email
- description: Releases the email_verified claim.
  flows: []
  scope: email_verified
- description: Releases the name claim.
  flows: []
  scope: name
- description: Releases the given_name claim.
  flows: []
  scope: given_name
- description: Releases the family_name claim.
  flows: []
  scope: family_name
- description: Releases the nickname claim.
  flows: []
  scope: nickname
- description: Releases the picture claim.
  flows: []
  scope: picture
- description: Releases the Auth0 created_at claim for the user record.
  flows: []
  scope: created_at
- description: Releases the Auth0 identities array (linked identity providers) for the user.
  flows: []
  scope: identities
slug: human-longevity-scopes
source_filename: human-longevity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://auth.humanlongevity.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes_supported values Human Longevity's own OpenID Connect discovery document\n  advertises for the HLI client-portal authorization server. They are the standard OIDC scope set\n  plus Auth0's per-claim scopes; there are NO product or API scopes, because Human Longevity\n  publishes no API for a third party to be authorized against. No scope reference page exists on the\n  provider's site — this artifact is derived entirely from the machine-readable discovery document.\nauthorization_server: https://auth.humanlongevity.com/\ndocs: null\ndocs_note: No published scopes/permissions reference page was found on humanlongevity.com.\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token for the authenticated client.\n  standard: openid-connect-core\n- name: profile\n  description: Standard OIDC scope releasing the\
  \ basic profile claim set.\n  standard: openid-connect-core\n- name: offline_access\n  description: Standard OIDC scope requesting a refresh token.\n  standard: openid-connect-core\n- name: address\n  description: Standard OIDC scope releasing the address claim.\n  standard: openid-connect-core\n- name: phone\n  description: Standard OIDC scope releasing phone_number and phone_number_verified claims.\n  standard: openid-connect-core\n- name: email\n  description: Releases the email claim.\n- name: email_verified\n  description: Releases the email_verified claim.\n- name: name\n  description: Releases the name claim.\n- name: given_name\n  description: Releases the given_name claim.\n- name: family_name\n  description: Releases the family_name claim.\n- name: nickname\n  description: Releases the nickname claim.\n- name: picture\n  description: Releases the picture claim.\n- name: created_at\n  description: Releases the Auth0 created_at claim for the user record.\n- name: identities\n \
  \ description: Releases the Auth0 identities array (linked identity providers) for the user.\nscope_count: 14\nproduct_scope_count: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/human-longevity/refs/heads/main/scopes/human-longevity-scopes.yml
summary_line: 14 scopes
tags:
- Company
- Health
- Healthcare
- Genomics
- Precision Medicine
- Diagnostics
- Artificial Intelligence
- Longevity
- Life Sciences
- Medical Imaging
token_bound: false
token_urls: []
---
