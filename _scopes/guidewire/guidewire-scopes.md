---
api_specs:
- filename: guidewire-integration-gateway-asyncapi.yml
  format: yaml
  label: Guidewire Integration Gateway API
  slug: guidewire-integration-gateway-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/asyncapi/guidewire-integration-gateway-asyncapi.yml
- filename: guidewire-accounts-api-openapi.yml
  format: yaml
  label: Guidewire Accounts API
  slug: guidewire-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-accounts-api-openapi.yml
- filename: guidewire-claims-api-openapi.yml
  format: yaml
  label: Guidewire Claims API
  slug: guidewire-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-claims-api-openapi.yml
- filename: guidewire-exposures-api-openapi.yml
  format: yaml
  label: Guidewire Exposures API
  slug: guidewire-exposures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-exposures-api-openapi.yml
- filename: guidewire-fnol-api-openapi.yml
  format: yaml
  label: Guidewire FNOL API
  slug: guidewire-fnol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-fnol-api-openapi.yml
- filename: guidewire-payments-api-openapi.yml
  format: yaml
  label: Guidewire Payments API
  slug: guidewire-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-payments-api-openapi.yml
- filename: guidewire-policies-api-openapi.yml
  format: yaml
  label: Guidewire Policies API
  slug: guidewire-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-policies-api-openapi.yml
- filename: guidewire-quotes-api-openapi.yml
  format: yaml
  label: Guidewire Quotes API
  slug: guidewire-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-quotes-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthImplement/endpoint-access/c_API-role-files.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Guidewire Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Guidewire uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Guidewire
provider_slug: guidewire
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: guidewire-scopes
source_filename: guidewire-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  Guidewire InsuranceSuite Cloud API Configuration & Authentication Guide on docs.guidewire.com.\ndocs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthImplement/endpoint-access/c_API-role-files.html\nprovider: guidewire\nproviderId: guidewire\nscope_count: 0\noauth2: false\nsupersedes: >-\n  A derived scope list written from openapi/*.yml on 2026-09-12 that reported three OAuth scopes\n  (cc.claims.read, cc.claims.write, cc.payments.write) under an authorizationCode flow at\n  https://login.guidewire.com/oauth/authorize. That authorization-server host does NOT RESOLVE\n  (NXDOMAIN, checked 2026-09-12), the scope strings appear nowhere in Guidewire's documentation, and\n  the values came from the documentation-shaped scaffold specs in openapi/ rather than from Guidewire.\n  They are removed here rather than carried forward.\nfinding: >-\n  Guidewire's InsuranceSuite Cloud API has NO OAuth 2.0 scope surface.\
  \ Guidewire does not run an\n  authorization server for it, publishes no scope catalog, and expresses authorization a different way\n  entirely: named API roles, defined in role.yaml files and assigned to callers, which enumerate the\n  endpoints, operations and fields a caller may reach. Bearer JWTs carry authorization as token claims\n  interpreted against those roles.\nscopes: []\nequivalent_mechanism:\n  name: Cloud API roles\n  artifact: role.yaml files shipped and configured per deployment\n  granularity: [endpoint, operation, field]\n  additional_access_types:\n    - endpoint access\n    - resource access\n    - proxy-user access\n  reserved_roles_docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthImplement/endpoint-access/c_reserved-roles.html\n  assignment_docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthImplement/endpoint-access/c_assigning-API-roles-to-callers.html\n  note: >-\n    Role names are defined per customer deployment,\
  \ so there is no catalog-wide list to publish. This\n    is why no OAuthScopes pointer is wired in apis.yml — a scope surface that does not exist should not\n    be asserted on Guidewire's behalf.\nother_oauth_surfaces:\n  - host: community.guidewire.com\n    note: >-\n      Salesforce Experience Cloud OIDC for the Guidewire Community portal, with a Salesforce-standard\n      scopes_supported list (openid, profile, email, api, offline_access, …). It governs portal\n      sign-in, NOT Cloud API access, and its scopes are Salesforce's, not Guidewire's.\n    document: well-known/guidewire-community-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/scopes/guidewire-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Policy
- Claims
- Billing
- P&C
token_urls: []
---
