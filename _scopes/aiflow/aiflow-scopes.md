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
overview: 'aiFlow uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: aiFlow
provider_slug: aiflow
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: aiflow-scopes
source_filename: aiflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://auth.aiflow.solutions/.well-known/openid-configuration\nnote: >-\n  These are the scopes_supported advertised by the company's own Auth0 authorization server at\n  auth.aiflow.solutions, read verbatim from its discovery document. They are the standard OIDC\n  identity scopes plus offline_access — they govern sign-in to the Verata application and the claims\n  released about the signed-in user. aiFlow publishes NO API permission or scope reference, and no\n  product-specific or resource-specific scopes are advertised; a developer cannot request access to\n  any aiFlow data surface with these. Recorded as published identity scopes, not as an API\n  authorization model.\nissuer: https://auth.aiflow.solutions/\ndocs: null\ndocs_note: No scopes or permissions reference page is published on aiflow.solutions or veratainsight.com.\nscope_type: oidc-identity\napi_scopes_published: false\nscope_count: 14\nscopes:\n- name: openid\n\
  \  description: Required OIDC scope; requests an ID token for the authenticating user.\n  category: identity\n- name: profile\n  description: Releases the default profile claims (name, family_name, given_name, nickname, picture, created_at).\n  category: identity\n- name: offline_access\n  description: Requests a refresh token so the application can renew access without re-prompting the user.\n  category: session\n- name: name\n  description: Releases the user's full name claim.\n  category: identity\n- name: given_name\n  description: Releases the user's given name claim.\n  category: identity\n- name: family_name\n  description: Releases the user's family name claim.\n  category: identity\n- name: nickname\n  description: Releases the user's nickname claim.\n  category: identity\n- name: email\n  description: Releases the user's email address claim.\n  category: identity\n- name: email_verified\n  description: Releases whether the user's email address has been verified.\n  category:\
  \ identity\n- name: picture\n  description: Releases the user's profile picture URL.\n  category: identity\n- name: created_at\n  description: Releases the timestamp the user account was created.\n  category: identity\n- name: identities\n  description: Releases the linked identity-provider connections for the user.\n  category: identity\n- name: phone\n  description: Releases the user's phone number claim.\n  category: identity\n- name: address\n  description: Releases the user's address claim.\n  category: identity\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiflow/refs/heads/main/scopes/aiflow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
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
token_urls: []
---
