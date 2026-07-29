---
api_specs:
- filename: electricity-north-west-explore-api-v2-1-openapi.json
  format: json
  label: SP Electricity North West Open Data Explore API v2.1
  slug: explore-api-v2-1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricity-north-west/refs/heads/main/openapi/electricity-north-west-explore-api-v2-1-openapi.json
- filename: electricity-north-west-explore-api-v2-0-openapi.json
  format: json
  label: SP Electricity North West Open Data Explore API v2.0
  slug: explore-api-v2-0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electricity-north-west/refs/heads/main/openapi/electricity-north-west-explore-api-v2-0-openapi.json
authorization_urls:
- https://electricitynorthwest.opendatasoft.com/oauth2/authorize/
description: 'Neither OpenAPI document declares an oauth2 securityScheme — both declare only the `apikey` query parameter — so the mechanical derivation from the specs yields nothing. The vendor documentation, however, does document a full OAuth2 authorization-code flow against this domain, with a deliberately minimal scope model: exactly one scope, `all`. That is the entire scope surface. It is recorded here so the absence of granular scopes is on the record as a finding rather than as a gap in our harvesting.'
docs: https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Electricity North West Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Electricity North West publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Electricity North West API on a user''s behalf.


  Tokens are issued from https://electricitynorthwest.opendatasoft.com/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Electricity North West
provider_slug: electricity-north-west
schemes:
- flows:
  - authorizationUrl: https://electricitynorthwest.opendatasoft.com/oauth2/authorize/
    delimiter: space
    flow: authorizationCode
    parameter_name: scopes
    refresh: supported via refresh_token grant
    tokenUrl: https://electricitynorthwest.opendatasoft.com/oauth2/token/
  name: OAuth2
  source: https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication
  standards:
  - RFC 6749
  - RFC 6750
scope_count: 1
scope_names:
- all
scopes:
- description: 'Full access to the data the authorizing user can see on this domain. The documentation states plainly: "a list of space-separated requested scopes. Currently, only `all` is supported."'
  flows:
  - authorizationCode
  scope: all
slug: electricity-north-west-scopes
source_filename: electricity-north-west-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication —\n  the \"Using OAuth2 authorization\" section of the Opendatasoft (Huwise) Explore\n  API reference that governs the SP Electricity North West domain.\ndocs: https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication\ndescription: >-\n  Neither OpenAPI document declares an oauth2 securityScheme — both declare only\n  the `apikey` query parameter — so the mechanical derivation from the specs\n  yields nothing. The vendor documentation, however, does document a full OAuth2\n  authorization-code flow against this domain, with a deliberately minimal scope\n  model: exactly one scope, `all`. That is the entire scope surface. It is\n  recorded here so the absence of granular scopes is on the record as a finding\n  rather than as a gap in our harvesting.\nspec_declared: false\nschemes:\n- name: OAuth2\n  source: https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication\n\
  \  standards: [RFC 6749, RFC 6750]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://electricitynorthwest.opendatasoft.com/oauth2/authorize/\n    tokenUrl: https://electricitynorthwest.opendatasoft.com/oauth2/token/\n    refresh: supported via refresh_token grant\n    parameter_name: scopes\n    delimiter: space\nscopes:\n- scope: all\n  description: >-\n    Full access to the data the authorizing user can see on this domain. The\n    documentation states plainly: \"a list of space-separated requested scopes.\n    Currently, only `all` is supported.\"\n  flows: [authorizationCode]\n  sources: [https://help.opendatasoft.com/apis/ods-explore-v2/#section/Authentication]\nnotes:\n- >-\n  There is no read/write split, no per-dataset scope and no per-resource scope.\n  Consent is all-or-nothing at the domain level, and an application registered\n  on one domain cannot reach another domain's data.\n- >-\n  API keys are the other authorization surface and they are not scoped\
  \ by\n  default either — a key inherits the creating user's full rights. Per-key\n  permissions can only be narrowed through the separate Automation API.\n- >-\n  Because every Explore operation is a read (GET only), the coarse scope model\n  is less consequential than it would be on a write-capable API — but it still\n  means an OAuth2 client cannot be least-privileged.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electricity-north-west/refs/heads/main/scopes/electricity-north-west-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- DER
- Renewables
- Energy Markets
- Smart Metering
token_urls:
- https://electricitynorthwest.opendatasoft.com/oauth2/token/
---
