---
authorization_urls: []
description: ''
docs: ''
flows:
- authorization_code
- refresh_token
kind: oauth-scopes
layout: scope
method: probed
name: Paperplane Scopes
name_suffix: OAuth Scopes
note: Read verbatim from scopes_supported in the live OIDC discovery document and the RFC 8414 metadata document served by Paperplane's own Clerk identity instance (issuer https://clerk.paperplane.ai). Paperplane publishes no scope reference page of its own — its documentation site is an unfilled GitBook starter template — so descriptions below are the standard OIDC/Clerk meanings of each scope name, marked as such, and are NOT quoted from Paperplane copy. derive-oauth-scopes.py found nothing because there is no OpenAPI in this repo to derive from; every value here came off the wire. These are end-user identity scopes for the Paperplane application, not scopes on a public developer API — Paperplane does not publish one.
overview: 'Paperplane publishes 7 OAuth 2.0 scopes via the authorization_code and refresh_token flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Paperplane API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paperplane
provider_slug: paperplane
schemes: []
scope_count: 7
scope_names:
- openid
- profile
- email
- offline_access
- public_metadata
- private_metadata
- user:org:read
scopes:
- description: Standard OIDC scope requesting an ID token.
  flows: []
  scope: openid
- description: Standard OIDC scope for basic profile claims (name, given_name, family_name, preferred_username, picture).
  flows: []
  scope: profile
- description: Standard OIDC scope for the email and email_verified claims.
  flows: []
  scope: email
- description: Standard OIDC scope requesting a refresh token for access outside an active session.
  flows: []
  scope: offline_access
- description: Clerk scope granting read access to the user's public metadata object.
  flows: []
  scope: public_metadata
- description: Clerk scope granting read access to the user's private metadata object.
  flows: []
  scope: private_metadata
- description: Clerk scope granting read access to the user's organization membership (backs the org_id claim).
  flows: []
  scope: user:org:read
slug: paperplane-scopes
source_filename: paperplane-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://clerk.paperplane.ai/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Read verbatim from scopes_supported in the live OIDC discovery document and\n  the RFC 8414 metadata document served by Paperplane's own Clerk identity\n  instance (issuer https://clerk.paperplane.ai). Paperplane publishes no scope\n  reference page of its own — its documentation site is an unfilled GitBook\n  starter template — so descriptions below are the standard OIDC/Clerk\n  meanings of each scope name, marked as such, and are NOT quoted from\n  Paperplane copy. derive-oauth-scopes.py found nothing because there is no\n  OpenAPI in this repo to derive from; every value here came off the wire.\n  These are end-user identity scopes for the Paperplane application, not\n  scopes on a public developer API — Paperplane does not publish one.\nflows:\n- authorization_code\n- refresh_token\nscope_count: 7\nscopes:\n- name: openid\n  description:\
  \ Standard OIDC scope requesting an ID token.\n  source: oidc-standard\n- name: profile\n  description: Standard OIDC scope for basic profile claims (name, given_name, family_name, preferred_username, picture).\n  source: oidc-standard\n- name: email\n  description: Standard OIDC scope for the email and email_verified claims.\n  source: oidc-standard\n- name: offline_access\n  description: Standard OIDC scope requesting a refresh token for access outside an active session.\n  source: oidc-standard\n- name: public_metadata\n  description: Clerk scope granting read access to the user's public metadata object.\n  source: clerk-platform\n- name: private_metadata\n  description: Clerk scope granting read access to the user's private metadata object.\n  source: clerk-platform\n- name: user:org:read\n  description: Clerk scope granting read access to the user's organization membership (backs the org_id claim).\n  source: clerk-platform\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperplane/refs/heads/main/scopes/paperplane-scopes.yml
summary_line: 7 scopes · authorization_code/refresh_token
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
token_bound: false
token_urls: []
---
