---
api_specs:
- filename: pax8-authentication-openapi.json
  format: json
  label: Pax8 Authentication API
  slug: pax8-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-authentication-openapi.json
- filename: pax8-partner-endpoints-openapi.json
  format: json
  label: Pax8 Partner Endpoints
  slug: pax8-partner-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-partner-endpoints-openapi.json
- filename: pax8-quoting-endpoints-openapi.json
  format: json
  label: Pax8 Quoting Endpoints
  slug: pax8-quoting-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-quoting-endpoints-openapi.json
- filename: pax8-vendor-provisioning-endpoints-openapi.json
  format: json
  label: Pax8 Vendor Provisioning Endpoints
  slug: pax8-vendor-provisioning-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-vendor-provisioning-endpoints-openapi.json
- filename: pax8-vendor-usage-endpoints-openapi.json
  format: json
  label: Pax8 Vendor Usage Endpoints
  slug: pax8-vendor-usage-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-vendor-usage-endpoints-openapi.json
- filename: pax8-webhooks-api-openapi.json
  format: json
  label: Pax8 Webhooks API
  slug: pax8-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-webhooks-api-openapi.json
authorization_urls: []
description: ''
docs: https://devx.pax8.com/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Pax8 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pax8 publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pax8 API on a user''s behalf.


  Tokens are issued from https://token-manager.pax8.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pax8
provider_slug: pax8
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://token-manager.pax8.com/oauth/token
  name: OAuth2
  source: openapi/pax8-authentication-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://token-manager.pax8.com/oauth/token
  name: OAuth2
  source: openapi/pax8-partner-endpoints-openapi.json
- description: 'Requires ''audience'' parameter in token request: `api://provisioning`.


    Simulation credentials will return `vendorSimulation:provisioning` scope.

    Production credentials will return `vendor:provisioning` scope.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.pax8.com/v1/token
  name: OAuth2
  source: openapi/pax8-vendor-provisioning-endpoints-openapi.json
- description: 'Requires ''audience'' parameter in token request: `api://usage`.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.pax8.com/v1/token
  name: OAuth2
  source: openapi/pax8-vendor-usage-endpoints-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://token-manager.pax8.com/oauth/token
  name: OAuth2
  source: openapi/pax8-webhooks-api-openapi.json
scope_count: 4
scope_names:
- read:usageLine
- vendor:provisioning
- vendorSimulation:provisioning
- write:usageLine
scopes:
- description: Grants read access for usage
  flows:
  - clientCredentials
  scope: read:usageLine
- description: Access to production provisioning endpoints
  flows:
  - clientCredentials
  scope: vendor:provisioning
- description: Access to simulation provisioning endpoints
  flows:
  - clientCredentials
  scope: vendorSimulation:provisioning
- description: Grants write access for usage
  flows:
  - clientCredentials
  scope: write:usageLine
slug: pax8-scopes
source_filename: pax8-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/pax8-authentication-openapi.json, openapi/pax8-partner-endpoints-openapi.json,\n  openapi/pax8-vendor-provisioning-endpoints-openapi.json, openapi/pax8-vendor-usage-endpoints-openapi.json,\n  openapi/pax8-webhooks-api-openapi.json\ndocs: https://devx.pax8.com/docs/authentication\nnotes: |-\n  Pax8 uses OAuth2 client-credentials. The `audience` parameter in the token request selects the\n  surface and the returned scope: `https://api.pax8.com` (partner/quoting/webhooks), `api://provisioning`\n  (vendor provisioning), `api://usage` (vendor usage). Simulation vs production credentials return\n  `vendorSimulation:provisioning` vs `vendor:provisioning`.\nschemes:\n- name: OAuth2\n  source: openapi/pax8-authentication-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://token-manager.pax8.com/oauth/token\n- name: OAuth2\n  source: openapi/pax8-partner-endpoints-openapi.json\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://token-manager.pax8.com/oauth/token\n- name: OAuth2\n  source: openapi/pax8-vendor-provisioning-endpoints-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.pax8.com/v1/token\n  description: |-\n    Requires 'audience' parameter in token request: `api://provisioning`.\n\n    Simulation credentials will return `vendorSimulation:provisioning` scope.\n    Production credentials will return `vendor:provisioning` scope.\n- name: OAuth2\n  source: openapi/pax8-vendor-usage-endpoints-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.pax8.com/v1/token\n  description: 'Requires ''audience'' parameter in token request: `api://usage`.'\n- name: OAuth2\n  source: openapi/pax8-webhooks-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://token-manager.pax8.com/oauth/token\nscopes:\n- scope: read:usageLine\n  description: Grants read access for usage\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/pax8-vendor-usage-endpoints-openapi.json\n- scope: vendor:provisioning\n  description: Access to production provisioning endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pax8-vendor-provisioning-endpoints-openapi.json\n- scope: vendorSimulation:provisioning\n  description: Access to simulation provisioning endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pax8-vendor-provisioning-endpoints-openapi.json\n- scope: write:usageLine\n  description: Grants write access for usage\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pax8-vendor-usage-endpoints-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/scopes/pax8-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Company
- Enterprise
- Cloud Marketplace
- MSP
- Distribution
- Provisioning
- Billing
- Quoting
- Subscriptions
- Webhooks
token_urls:
- https://token-manager.pax8.com/oauth/token
- https://api.pax8.com/v1/token
---
