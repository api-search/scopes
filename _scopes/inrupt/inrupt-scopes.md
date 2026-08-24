---
api_specs:
- filename: inrupt-notification-openapi.yaml
  format: yaml
  label: Inrupt Change Notifications API (ESS Notification Delivery Service)
  slug: notification-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/openapi/inrupt-notification-openapi.yaml
authorization_urls: []
description: ''
docs: https://docs.inrupt.com/guides/authentication-in-solid
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Inrupt Scopes
name_suffix: OAuth Scopes
note: 'Inrupt''s Solid OpenID Provider advertises three scopes and no resource-level permission scopes. This is by design and is the most important thing to understand about authorizing against ESS: authorization is NOT carried in the OAuth scope. A token grants an identity (the WebID); what that identity may read or write is decided separately by Access Control Policies on the resource and by Access Grants, which are W3C Verifiable Credentials issued by the data subject. There is therefore no scope reference page to enumerate, and the absence of granular scopes is not a documentation gap.'
overview: 'Inrupt uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Inrupt
provider_slug: inrupt
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: inrupt-scopes
source_filename: inrupt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://login.inrupt.com/.well-known/openid-configuration\ndocs: https://docs.inrupt.com/guides/authentication-in-solid\nissuer: https://login.inrupt.com\nnote: >-\n  Inrupt's Solid OpenID Provider advertises three scopes and no resource-level permission scopes.\n  This is by design and is the most important thing to understand about authorizing against ESS:\n  authorization is NOT carried in the OAuth scope. A token grants an identity (the WebID); what that\n  identity may read or write is decided separately by Access Control Policies on the resource and by\n  Access Grants, which are W3C Verifiable Credentials issued by the data subject. There is therefore\n  no scope reference page to enumerate, and the absence of granular scopes is not a documentation gap.\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token.\n  required: true\n- name: offline_access\n  description: Requests a refresh\
  \ token so a session can be restored without re-authenticating.\n- name: webid\n  description: >-\n    Solid-OIDC scope requesting the webid claim, which binds the token to the user's WebID URI. Present\n    in both scopes_supported and claims_supported.\nauthorization_model:\n  identity_scopes: OAuth/OIDC scopes above\n  resource_authorization:\n  - mechanism: Access Control Policy (ACP)\n    docs: https://docs.inrupt.com/security/authorization/acp\n    description: Policies on the Access Control Resource attached to each Pod resource.\n  - mechanism: Access Requests and Access Grants\n    docs: https://docs.inrupt.com/security/authorization/access-requests-grants\n    description: >-\n      Verifiable Credentials issued by the data subject naming grantee, resource, access modes and\n      purpose, with expiry and revocation. As of ESS 3.0 a grant acts as a receipt checked server-side.\n  access_modes:\n  - read\n  - write\n  - append\n  - control\n  mcp_restriction: >-\n    The MCP Resource\
  \ Service currently supports only the read access mode for requestAccess and\n    hasMatchingAccessGrant.\ntoken_endpoint_auth_methods:\n- client_secret_basic\n- client_secret_post\ngrant_types:\n- authorization_code\n- refresh_token\n- client_credentials\npkce:\n- plain\n- S256\ndpop_signing_algs:\n- RS256\n- ES256\ndynamic_client_registration: https://login.inrupt.com/registration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/scopes/inrupt-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Solid
- Personal Data Stores
- Decentralized Identity
- Data Privacy
- Access Control
- Verifiable Credentials
- Linked Data
- RDF
- Consent Management
- Data Wallets
- Agent Infrastructure
- Model Context Protocol
- Enterprise Software
token_urls: []
---
