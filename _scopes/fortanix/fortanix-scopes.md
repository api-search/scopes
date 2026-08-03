---
api_specs:
- filename: fortanix-dsm-openapi-original.json
  format: json
  label: Fortanix Data Security Manager REST API
  slug: dsm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-dsm-openapi-original.json
- filename: fortanix-ccm-openapi-original.json
  format: json
  label: Fortanix Confidential Computing Manager REST API
  slug: ccm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-ccm-openapi-original.json
- filename: fortanix-armor-key-insight-openapi-original.json
  format: json
  label: Fortanix Armor and Key Insight API
  slug: armor-key-insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-armor-key-insight-openapi-original.json
authorization_urls: []
description: ''
docs:
- name: Programmatic Access to Fortanix Armor IAM
  url: https://support.fortanix.com/docs/programmatic-access-to-fortanix-armor-iam
- name: Client Credentials Flow
  url: https://support.fortanix.com/docs/fortanix-key-insight-aws-client-credentials-flow
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Fortanix Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fortanix uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.armor.fortanix.com/api/v1/iam/session/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fortanix
provider_slug: fortanix
schemes:
- api: fortanix:armor-key-insight
  description: OAuth 2.0 client credential flow, see https://datatracker.ietf.org/doc/html/rfc6749#section-4.4.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.armor.fortanix.com/api/v1/iam/session/oauth2/token
  name: Oauth2ClientCredentials
  source: openapi/fortanix-armor-key-insight-openapi-original.json
scope_count: 0
scope_names: []
scopes: []
slug: fortanix-scopes
source_filename: fortanix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/fortanix-armor-key-insight-openapi-original.json\nschemes:\n- name: Oauth2ClientCredentials\n  source: openapi/fortanix-armor-key-insight-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.armor.fortanix.com/api/v1/iam/session/oauth2/token\n  description: OAuth 2.0 client credential flow, see https://datatracker.ietf.org/doc/html/rfc6749#section-4.4.\n  api: fortanix:armor-key-insight\nscopes: []\ndocs:\n- name: Programmatic Access to Fortanix Armor IAM\n  url: https://support.fortanix.com/docs/programmatic-access-to-fortanix-armor-iam\n- name: Client Credentials Flow\n  url: https://support.fortanix.com/docs/fortanix-key-insight-aws-client-credentials-flow\nfinding: 'Fortanix publishes NO OAuth scopes. The single oauth2 securityScheme in the\n  catalog — Oauth2ClientCredentials on the Armor / Key Insight API — declares an empty\n  scopes map, and no operation attaches a scope requirement.\
  \ The docs describe how to\n  obtain a client-credentials token (including via Okta and Auth0 as external authorization\n  servers) but publish no scope or permission reference page.'\nauthorization_model: 'Fortanix does not use scopes to express authorization anywhere\n  in its platform. DSM authorizes by GROUP MEMBERSHIP — an app or user may act on a\n  security object only if it belongs to that object''s group, with per-membership operation\n  restrictions — and by custom/external roles. CCM uses a JWT bearer token with no scope\n  claim documented. See authentication/fortanix-authentication.yml.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/scopes/fortanix-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Security
- Encryption
- Key Management
- Cryptography
- Confidential Computing
- HSM
- Data Security
- Post-Quantum
- Secrets Management
token_urls:
- https://api.armor.fortanix.com/api/v1/iam/session/oauth2/token
---
