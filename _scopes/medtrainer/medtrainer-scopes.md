---
api_specs:
- filename: medtrainer-public-api-openapi.json
  format: json
  label: MedTrainer Public API
  slug: medtrainer-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/openapi/medtrainer-public-api-openapi.json
authorization_urls: []
description: ''
docs: https://api.medtrainer.com/docs#section/Getting-started
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Medtrainer Scopes
name_suffix: OAuth Scopes
note: The MedTrainer Public API itself declares NO oauth2 security scheme — it authenticates with an X-API-Key header or an opaque bearer token, and therefore has no scope surface at all. An API key is scoped by the permissions of the API key group created in the platform, and those permissions are not published. The scopes below were read from two live OAuth/OIDC discovery documents on other MedTrainer hosts and are recorded so the platform's real authorization surface is not lost — they do NOT govern api.medtrainer.com.
overview: 'MedTrainer uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MedTrainer
provider_slug: medtrainer
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: medtrainer-scopes
source_filename: medtrainer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  https://auth.medtrainer.com/.well-known/openid-configuration;\n  https://medtrainer.com/.well-known/oauth-authorization-server\ndocs: https://api.medtrainer.com/docs#section/Getting-started\nnote: >-\n  The MedTrainer Public API itself declares NO oauth2 security scheme — it authenticates with an\n  X-API-Key header or an opaque bearer token, and therefore has no scope surface at all. An API\n  key is scoped by the permissions of the API key group created in the platform, and those\n  permissions are not published. The scopes below were read from two live OAuth/OIDC discovery\n  documents on other MedTrainer hosts and are recorded so the platform's real authorization\n  surface is not lost — they do NOT govern api.medtrainer.com.\nsurfaces:\n- surface: platform identity provider\n  issuer: https://auth.medtrainer.com/\n  protocol: OpenID Connect\n  scopes:\n  - name: openid\n    description: Standard OIDC scope requesting\
  \ an ID token.\n  - name: profile\n    description: Standard OIDC profile claims.\n  - name: email\n    description: Standard OIDC email claim.\n  - name: email_verified\n  - name: name\n  - name: given_name\n  - name: family_name\n  - name: nickname\n  - name: picture\n  - name: phone\n  - name: address\n  - name: created_at\n  - name: identities\n  - name: offline_access\n    description: Requests a refresh token.\n- surface: MCP server (medtrainer.com WordPress)\n  issuer: https://medtrainer.com\n  protocol: OAuth 2.0 (RFC 8414 + RFC 9728)\n  scopes:\n  - name: mcp\n    description: The only scope advertised for the MedTrainer MCP protected resource at /wp-json/mcp/mcp-oauth-server.\n- surface: MedTrainer Public API\n  issuer: null\n  protocol: api-key / bearer\n  scopes: []\n  note: 'No OAuth scopes. Authorization is per-API-key-group and is configured in the platform UI, not published.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/scopes/medtrainer-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Compliance
- Credentialing
- Learning Management
- Provider Directory
- FHIR
- HL7
- Training
- Risk Management
- SaaS
token_urls: []
---
