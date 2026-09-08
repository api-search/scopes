---
authorization_urls: []
description: 'Acadio''s only machine-readable scope surface is the OpenID Connect discovery document served from acadio.com — the Shopify customer-accounts authorization server scoped to Acadio''s shop. The Acadio LMS itself documents no OAuth scope model: its JWT single sign-on carries user attributes and group/credit associations rather than scopes, and the Google OAuth 2.0 integration delegates scope definition to Google. Nothing below is derived or inferred; the list is transcribed from the provider-served document.'
docs: https://acadio.instantdocsbase.com/help/google-oauth-2-dot-0-documentation
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Acadio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Acadio uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Acadio
provider_slug: acadio
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: acadio-scopes
source_filename: acadio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://acadio.com/.well-known/openid-configuration\ndocs: https://acadio.instantdocsbase.com/help/google-oauth-2-dot-0-documentation\ndescription: >-\n  Acadio's only machine-readable scope surface is the OpenID Connect discovery document served from\n  acadio.com — the Shopify customer-accounts authorization server scoped to Acadio's shop. The Acadio\n  LMS itself documents no OAuth scope model: its JWT single sign-on carries user attributes and\n  group/credit associations rather than scopes, and the Google OAuth 2.0 integration delegates scope\n  definition to Google. Nothing below is derived or inferred; the list is transcribed from the\n  provider-served document.\nauthorization_server: https://shopify.com/authentication/78091452669\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token.\n- name: email\n  description: Releases the customer's email address and email_verified\
  \ claim.\n- name: customer-account-api:full\n  description: Full access to the storefront Customer Account API for the signed-in buyer.\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP API for the signed-in buyer — the authenticated\n    counterpart to the anonymous UCP commerce MCP endpoint at https://acadio.com/api/ucp/mcp.\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\nnotes:\n- >-\n  These scopes govern the acadio.com course storefront, not the Acadio LMS platform. There is no\n  published scope reference page and no scopes documented for api.acadio.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acadio/refs/heads/main/scopes/acadio-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Education
- Learning Management System
- Professional Education
- Continuing Education
- Certification
- Exam Preparation
- SCORM
- Webhooks
- Agentic Commerce
token_urls: []
---
