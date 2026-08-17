---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Paperplane Scopes
name_suffix: OAuth Scopes
note: Read verbatim from scopes_supported in the live OIDC discovery document and the RFC 8414 metadata document served by Paperplane's own Clerk identity instance (issuer https://clerk.paperplane.ai). Paperplane publishes no scope reference page of its own — its documentation site is an unfilled GitBook starter template — so descriptions below are the standard OIDC/Clerk meanings of each scope name, marked as such, and are NOT quoted from Paperplane copy. derive-oauth-scopes.py found nothing because there is no OpenAPI in this repo to derive from; every value here came off the wire. These are end-user identity scopes for the Paperplane application, not scopes on a public developer API — Paperplane does not publish one.
overview: 'Paperplane uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paperplane
provider_slug: paperplane
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: paperplane-scopes
source_filename: paperplane-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://clerk.paperplane.ai/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Read verbatim from scopes_supported in the live OIDC discovery document and\n  the RFC 8414 metadata document served by Paperplane's own Clerk identity\n  instance (issuer https://clerk.paperplane.ai). Paperplane publishes no scope\n  reference page of its own — its documentation site is an unfilled GitBook\n  starter template — so descriptions below are the standard OIDC/Clerk\n  meanings of each scope name, marked as such, and are NOT quoted from\n  Paperplane copy. derive-oauth-scopes.py found nothing because there is no\n  OpenAPI in this repo to derive from; every value here came off the wire.\n  These are end-user identity scopes for the Paperplane application, not\n  scopes on a public developer API — Paperplane does not publish one.\nflows:\n- authorization_code\n- refresh_token\nscope_count: 7\nscopes:\n- name: openid\n  description:\
  \ Standard OIDC scope requesting an ID token.\n  source: oidc-standard\n- name: profile\n  description: Standard OIDC scope for basic profile claims (name, given_name, family_name, preferred_username, picture).\n  source: oidc-standard\n- name: email\n  description: Standard OIDC scope for the email and email_verified claims.\n  source: oidc-standard\n- name: offline_access\n  description: Standard OIDC scope requesting a refresh token for access outside an active session.\n  source: oidc-standard\n- name: public_metadata\n  description: Clerk scope granting read access to the user's public metadata object.\n  source: clerk-platform\n- name: private_metadata\n  description: Clerk scope granting read access to the user's private metadata object.\n  source: clerk-platform\n- name: user:org:read\n  description: Clerk scope granting read access to the user's organization membership (backs the org_id claim).\n  source: clerk-platform\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperplane/refs/heads/main/scopes/paperplane-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Sales
- CRM
- Salesforce
- Sales Automation
- Conversation Intelligence
- Note Taking
- Artificial Intelligence
- Productivity
token_urls: []
---
