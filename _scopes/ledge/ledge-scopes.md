---
api_specs:
- filename: ledge-api-openapi.yml
  format: yaml
  label: Ledge API
  slug: ledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledge/refs/heads/main/openapi/ledge-api-openapi.yml
authorization_urls: []
description: Ledge authorizes API calls with OAuth 2.0 client_credentials but publishes NO named OAuth scopes. The documented token request sends only grant_type, client_id, client_secret and audience — there is no scope parameter — and the token response returns access_token, token_type and expires_in with no scope claim. Authorization is instead enforced by a role-based fine-grained permissions model. The empty scopes[] below is a verified absence, not a gap in this capture.
docs: https://docs.ledge.co/api-reference/fundamentals/fine-grained-permissions
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Ledge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ledge uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://goledge.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ledge
provider_slug: ledge
schemes:
- description: Obtain a client ID and generate a client secret on the Ledge Developers page (https://app.goledge.io/developers), then request an access token from the Ledge Auth0 tenant using the client_credentials grant.
  flows:
  - flow: clientCredentials
    scopes: []
    tokenUrl: https://goledge.us.auth0.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/ledge-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: ledge-scopes
source_filename: ledge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  openapi/ledge-api-openapi.yml (oauth2 securityScheme) plus a search of the\n  Ledge documentation for a scopes or permissions reference:\n  https://docs.ledge.co/api-reference/fundamentals/authentication and\n  https://docs.ledge.co/api-reference/fundamentals/fine-grained-permissions.\ndocs: https://docs.ledge.co/api-reference/fundamentals/fine-grained-permissions\ndescription: >-\n  Ledge authorizes API calls with OAuth 2.0 client_credentials but publishes NO\n  named OAuth scopes. The documented token request sends only grant_type,\n  client_id, client_secret and audience — there is no scope parameter — and the\n  token response returns access_token, token_type and expires_in with no scope\n  claim. Authorization is instead enforced by a role-based fine-grained\n  permissions model. The empty scopes[] below is a verified absence, not a gap\n  in this capture.\nscopes_published: false\nscopes: []\nauthorization_model:\n\
  \  type: role-based fine-grained permissions\n  description: >-\n    Administrators can define permissions that fit their organization's specific\n    needs with role-based access, based on either built-in or custom roles.\n  builtin_roles:\n  - name: Administrator\n    access: Full access to all resources; user management control\n  - name: Full member\n    access: Full access to all resources\n  - name: View-only\n    access: Read-only access to all resources\n  custom_roles:\n    supported: true\n    description: Custom roles can be used to allow, or deny, access to specific resources.\n  enforcement: >-\n    A denied resource returns HTTP 403 — \"The request was rejected for security\n    reasons, contact Ledge for assistance.\"\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/ledge-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://goledge.us.auth0.com/oauth/token\n    scopes: []\n  description: >-\n    Obtain a client ID and generate a client\
  \ secret on the Ledge Developers page\n    (https://app.goledge.io/developers), then request an access token from the\n    Ledge Auth0 tenant using the client_credentials grant.\nidentity_provider_scopes:\n  note: >-\n    The underlying Auth0 tenant advertises the standard OIDC scopes below in its\n    discovery document (well-known/ledge-openid-configuration.json). These are\n    Auth0 platform defaults for interactive sign-in, NOT Ledge API authorization\n    scopes, and must not be read as a Ledge permission model.\n  source: https://goledge.us.auth0.com/.well-known/openid-configuration\n  scopes_supported:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\ndetail: authentication/ledge-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledge/refs/heads/main/scopes/ledge-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Fintech
- Accounting
- Reconciliation
- Financial Close
- Payment Operations
- Transaction Matching
- Cash Application
- Journal Entries
- AI Agents
- ERP Integration
- Finance Automation
token_urls:
- https://goledge.us.auth0.com/oauth/token
---
