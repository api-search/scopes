---
api_specs:
- filename: peking-collections-api-openapi.yml
  format: yaml
  label: Peking University Collections API
  slug: peking-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/openapi/peking-collections-api-openapi.yml
- filename: peking-communities-api-openapi.yml
  format: yaml
  label: Peking University Communities API
  slug: peking-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/openapi/peking-communities-api-openapi.yml
- filename: peking-harvesting-api-openapi.yml
  format: yaml
  label: Peking University Harvesting API
  slug: peking-harvesting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/openapi/peking-harvesting-api-openapi.yml
- filename: peking-items-api-openapi.yml
  format: yaml
  label: Peking University Items API
  slug: peking-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/openapi/peking-items-api-openapi.yml
- filename: peking-status-api-openapi.yml
  format: yaml
  label: Peking University Status API
  slug: peking-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/openapi/peking-status-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Peking Scopes
name_suffix: OAuth Scopes
note: No OAuth scope vocabulary is published by Peking University. The IAAA unified authentication service exposes an OAuth authorization page (HTTP 200) but no discovery document — /.well-known/openid-configuration was not served on any PKU host probed on 2026-08-19 — and client registration is an internal, approval-gated process. The federated surface uses SAML attribute release, not OAuth scopes; the attribute authority is declared in the IdP metadata and its released attribute set is negotiated per service provider through CARSI rather than published. Nothing is asserted here that was not observed. This file records an absence.
overview: 'Peking University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Peking University
provider_slug: peking
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: peking-scopes
source_filename: peking-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: https://iaaa.pku.edu.cn/iaaa/oauth.jsp\nx-operator: institution\nnote: >-\n  No OAuth scope vocabulary is published by Peking University. The IAAA unified\n  authentication service exposes an OAuth authorization page (HTTP 200) but no\n  discovery document — /.well-known/openid-configuration was not served on any PKU\n  host probed on 2026-08-19 — and client registration is an internal, approval-gated\n  process. The federated surface uses SAML attribute release, not OAuth scopes;\n  the attribute authority is declared in the IdP metadata and its released attribute\n  set is negotiated per service provider through CARSI rather than published.\n  Nothing is asserted here that was not observed. This file records an absence.\nschemes: []\nscopes: []\nsaml_attribute_release:\n  documented_publicly: false\n  attribute_authority: https://idp.pku.edu.cn:8443/idp/profile/SAML2/SOAP/AttributeQuery\n  scope: pku.edu.cn\n  note: >-\n  \
  \  The IdP declares an AttributeAuthorityDescriptor and a shibmd:Scope of pku.edu.cn,\n    so attribute release exists and is machine-declared; the released attribute names\n    themselves are not published on a public surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/scopes/peking-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- China
- Public Research University
- C9 League
- Research Repository
- Identity Federation
- Research Data
- Open Data
- Research Computing
- OAI-PMH
token_urls: []
---
