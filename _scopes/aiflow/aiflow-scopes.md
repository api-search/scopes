---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Aiflow Scopes
name_suffix: OAuth Scopes
note: These are the scopes_supported advertised by the company's own Auth0 authorization server at auth.aiflow.solutions, read verbatim from its discovery document. They are the standard OIDC identity scopes plus offline_access — they govern sign-in to the Verata application and the claims released about the signed-in user. aiFlow publishes NO API permission or scope reference, and no product-specific or resource-specific scopes are advertised; a developer cannot request access to any aiFlow data surface with these. Recorded as published identity scopes, not as an API authorization model.
overview: 'aiFlow publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the aiFlow API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: aiFlow
provider_slug: aiflow
schemes: []
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- name
- given_name
- family_name
- nickname
- email
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Required OIDC scope; requests an ID token for the authenticating user.
  flows: []
  scope: openid
- description: Releases the default profile claims (name, family_name, given_name, nickname, picture, created_at).
  flows: []
  scope: profile
- description: Requests a refresh token so the application can renew access without re-prompting the user.
  flows: []
  scope: offline_access
- description: Releases the user's full name claim.
  flows: []
  scope: name
- description: Releases the user's given name claim.
  flows: []
  scope: given_name
- description: Releases the user's family name claim.
  flows: []
  scope: family_name
- description: Releases the user's nickname claim.
  flows: []
  scope: nickname
- description: Releases the user's email address claim.
  flows: []
  scope: email
- description: Releases whether the user's email address has been verified.
  flows: []
  scope: email_verified
- description: Releases the user's profile picture URL.
  flows: []
  scope: picture
- description: Releases the timestamp the user account was created.
  flows: []
  scope: created_at
- description: Releases the linked identity-provider connections for the user.
  flows: []
  scope: identities
- description: Releases the user's phone number claim.
  flows: []
  scope: phone
- description: Releases the user's address claim.
  flows: []
  scope: address
slug: aiflow-scopes
source_filename: aiflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://auth.aiflow.solutions/.well-known/openid-configuration\nnote: >-\n  These are the scopes_supported advertised by the company's own Auth0 authorization server at\n  auth.aiflow.solutions, read verbatim from its discovery document. They are the standard OIDC\n  identity scopes plus offline_access — they govern sign-in to the Verata application and the claims\n  released about the signed-in user. aiFlow publishes NO API permission or scope reference, and no\n  product-specific or resource-specific scopes are advertised; a developer cannot request access to\n  any aiFlow data surface with these. Recorded as published identity scopes, not as an API\n  authorization model.\nissuer: https://auth.aiflow.solutions/\ndocs: null\ndocs_note: No scopes or permissions reference page is published on aiflow.solutions or veratainsight.com.\nscope_type: oidc-identity\napi_scopes_published: false\nscope_count: 14\nscopes:\n- name: openid\n\
  \  description: Required OIDC scope; requests an ID token for the authenticating user.\n  category: identity\n- name: profile\n  description: Releases the default profile claims (name, family_name, given_name, nickname, picture, created_at).\n  category: identity\n- name: offline_access\n  description: Requests a refresh token so the application can renew access without re-prompting the user.\n  category: session\n- name: name\n  description: Releases the user's full name claim.\n  category: identity\n- name: given_name\n  description: Releases the user's given name claim.\n  category: identity\n- name: family_name\n  description: Releases the user's family name claim.\n  category: identity\n- name: nickname\n  description: Releases the user's nickname claim.\n  category: identity\n- name: email\n  description: Releases the user's email address claim.\n  category: identity\n- name: email_verified\n  description: Releases whether the user's email address has been verified.\n  category:\
  \ identity\n- name: picture\n  description: Releases the user's profile picture URL.\n  category: identity\n- name: created_at\n  description: Releases the timestamp the user account was created.\n  category: identity\n- name: identities\n  description: Releases the linked identity-provider connections for the user.\n  category: identity\n- name: phone\n  description: Releases the user's phone number claim.\n  category: identity\n- name: address\n  description: Releases the user's address claim.\n  category: identity\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiflow/refs/heads/main/scopes/aiflow-scopes.yml
summary_line: 14 scopes
tags:
- Company
- Executive Search
- Private Equity
- Talent Intelligence
- People Data
- Company Data
- Market Intelligence
- Artificial Intelligence
- Y Combinator
- No Public API
token_bound: false
token_urls: []
---
