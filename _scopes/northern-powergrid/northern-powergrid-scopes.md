---
api_specs:
- filename: northern-powergrid-open-data-explore-api-v2-1-openapi.json
  format: json
  label: Northern Powergrid Open Data Explore API
  slug: northern-powergrid-open-data-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northern-powergrid/refs/heads/main/openapi/northern-powergrid-open-data-explore-api-v2-1-openapi.json
- filename: northern-powergrid-open-data-explore-api-v2-0-openapi.json
  format: json
  label: Northern Powergrid Open Data Explore API v2.0
  slug: northern-powergrid-open-data-explore-api-v2-0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northern-powergrid/refs/heads/main/openapi/northern-powergrid-open-data-explore-api-v2-0-openapi.json
authorization_urls:
- https://northernpowergrid.opendatasoft.com/oauth2/authorize/
description: ''
docs: https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Using-OAuth2-authorization
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Northern Powergrid Scopes
name_suffix: OAuth Scopes
note: The OpenAPI for this API declares no oauth2 security scheme — it only carries the apikey query parameter — so the mechanical derivation returned nothing. The platform documentation does document a full OAuth 2.0 authorization-code flow for this API, and it publishes exactly one scope. That single scope is recorded here verbatim; no scope taxonomy was invented. Both endpoints were confirmed live on this portal host on 2026-07-27 (/oauth2/authorize/ -> 302, /oauth2/token/ -> 405 to a GET, i.e. POST-only).
overview: 'Northern Powergrid publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Northern Powergrid API on a user''s behalf.


  Tokens are issued from https://northernpowergrid.opendatasoft.com/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Northern Powergrid
provider_slug: northern-powergrid
schemes:
- flows:
  - authorizationUrl: https://northernpowergrid.opendatasoft.com/oauth2/authorize/
    delimiter: space
    flow: authorizationCode
    parameter_name: scopes
    refresh_supported: true
    tokenUrl: https://northernpowergrid.opendatasoft.com/oauth2/token/
  name: oauth2
  source: https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Using-OAuth2-authorization
  standards:
  - RFC 6749
  - RFC 6750
scope_count: 1
scope_names:
- all
scopes:
- description: Full access to the data the granting user can see on this domain. The platform documents this as the only supported scope value; there is no finer-grained read/write split, and applications are registered per domain so a grant never spans portals.
  flows:
  - authorizationCode
  scope: all
slug: northern-powergrid-scopes
source_filename: northern-powergrid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Using-OAuth2-authorization\ndocs: https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Using-OAuth2-authorization\nnote: >-\n  The OpenAPI for this API declares no oauth2 security scheme — it only carries the apikey query\n  parameter — so the mechanical derivation returned nothing. The platform documentation does\n  document a full OAuth 2.0 authorization-code flow for this API, and it publishes exactly one\n  scope. That single scope is recorded here verbatim; no scope taxonomy was invented. Both endpoints\n  were confirmed live on this portal host on 2026-07-27 (/oauth2/authorize/ -> 302,\n  /oauth2/token/ -> 405 to a GET, i.e. POST-only).\nschemes:\n- name: oauth2\n  source: https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Using-OAuth2-authorization\n  standards: [RFC 6749, RFC 6750]\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://northernpowergrid.opendatasoft.com/oauth2/authorize/\n    tokenUrl: https://northernpowergrid.opendatasoft.com/oauth2/token/\n    refresh_supported: true\n    parameter_name: scopes\n    delimiter: space\nscopes:\n- scope: all\n  description: >-\n    Full access to the data the granting user can see on this domain. The platform documents this as\n    the only supported scope value; there is no finer-grained read/write split, and applications are\n    registered per domain so a grant never spans portals.\n  flows: [authorizationCode]\n  sources:\n  - https://help.huwise.com/apis/ods-explore-v2/#section/Authentication/Using-OAuth2-authorization\ncoverage:\n  scopes_published: 1\n  granularity: coarse\n  note: >-\n    A one-scope model on a read-only, GET-only API. Least-privilege delegation is not expressible\n    here; an agent granted \"all\" inherits everything its granting user can read on this portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northern-powergrid/refs/heads/main/scopes/northern-powergrid-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Open Data
- Distribution Network Operator
- Smart Metering
- Network Capacity
- Flexibility
- DER
- Renewables
token_urls:
- https://northernpowergrid.opendatasoft.com/oauth2/token/
---
