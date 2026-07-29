---
api_specs:
- filename: ercot-public-data-api-openapi.json
  format: json
  label: ERCOT Public Data API
  slug: ercot-public-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ercot/refs/heads/main/openapi/ercot-public-data-api-openapi.json
authorization_urls:
- https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/b2c_1_pubapi-ropc-flow/oauth2/v2.0/authorize
description: 'The ERCOT Public Data API has no authorization-scope surface in the usual sense — there is no scopes/permissions reference page and no per-resource scope. The OpenAPI declares only apiKey security schemes. What ERCOT does operate is an Azure AD B2C ROPC user flow whose token request carries a fixed scope string; the B2C OIDC discovery document advertises exactly one supported scope (openid). Authorization is effectively all-or-nothing: any registered developer with a valid subscription key and ID token sees the same public EMIL data products. Access differentiation happens at the API Management product/subscription layer, not through scopes.'
docs: https://developer.ercot.com/applications/pubapi/user-guide/registration-and-authentication/
flows:
- password
kind: oauth-scopes
layout: scope
method: searched
name: Ercot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ERCOT publishes 3 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ERCOT API on a user''s behalf.


  Tokens are issued from https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/B2C_1_PUBAPI-ROPC-FLOW/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ERCOT
provider_slug: ercot
schemes:
- flows:
  - authorizationUrl: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/b2c_1_pubapi-ropc-flow/oauth2/v2.0/authorize
    flow: password
    tokenUrl: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/B2C_1_PUBAPI-ROPC-FLOW/oauth2/v2.0/token
  name: ercotB2C
  source: well-known/ercot-openid-configuration.json
  type: oauth2
scope_count: 3
scope_names:
- openid
- fec253ea-0d06-4272-a5e6-b478baeecd70
- offline_access
scopes:
- description: Standard OIDC scope; the only value in scopes_supported on the ERCOT B2C discovery document. Yields the id_token the Public Data API consumes.
  flows:
  - password
  scope: openid
- description: The Public Data API B2C application (client) id, used as a resource scope in the documented token request so the issued token is audienced to the Public Data API.
  flows:
  - password
  scope: fec253ea-0d06-4272-a5e6-b478baeecd70
- description: Requests a refresh_token alongside the id_token. Note the developer docs state ID tokens cannot be refreshed and a new POST is required each hour.
  flows:
  - password
  scope: offline_access
slug: ercot-scopes
source_filename: ercot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: well-known/ercot-openid-configuration.json\ndocs: https://developer.ercot.com/applications/pubapi/user-guide/registration-and-authentication/\ndescription: >-\n  The ERCOT Public Data API has no authorization-scope surface in the usual sense — there is no\n  scopes/permissions reference page and no per-resource scope. The OpenAPI declares only apiKey\n  security schemes. What ERCOT does operate is an Azure AD B2C ROPC user flow whose token request\n  carries a fixed scope string; the B2C OIDC discovery document advertises exactly one supported\n  scope (openid). Authorization is effectively all-or-nothing: any registered developer with a\n  valid subscription key and ID token sees the same public EMIL data products. Access\n  differentiation happens at the API Management product/subscription layer, not through scopes.\nschemes:\n- name: ercotB2C\n  type: oauth2\n  source: well-known/ercot-openid-configuration.json\n  flows:\n\
  \  - flow: password\n    tokenUrl: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/B2C_1_PUBAPI-ROPC-FLOW/oauth2/v2.0/token\n    authorizationUrl: https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/b2c_1_pubapi-ropc-flow/oauth2/v2.0/authorize\nscopes:\n- scope: openid\n  description: >-\n    Standard OIDC scope; the only value in scopes_supported on the ERCOT B2C discovery document.\n    Yields the id_token the Public Data API consumes.\n  flows: [password]\n  sources: [well-known/ercot-openid-configuration.json]\n- scope: fec253ea-0d06-4272-a5e6-b478baeecd70\n  description: >-\n    The Public Data API B2C application (client) id, used as a resource scope in the documented\n    token request so the issued token is audienced to the Public Data API.\n  flows: [password]\n  sources: [https://developer.ercot.com/applications/pubapi/user-guide/registration-and-authentication/]\n- scope: offline_access\n  description: >-\n    Requests a refresh_token alongside the id_token. Note the\
  \ developer docs state ID tokens\n    cannot be refreshed and a new POST is required each hour.\n  flows: [password]\n  sources: [https://developer.ercot.com/applications/pubapi/user-guide/registration-and-authentication/]\ndocumented_scope_string: openid+fec253ea-0d06-4272-a5e6-b478baeecd70+offline_access\nper_operation_scopes: false\nnotes: >-\n  The SOAP market-participant estate (EWS, MarkeTrak, Retail) authorizes by ERCOT digital\n  certificate ROLE (certificateRole appears on EMIL product metadata), not by OAuth scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ercot/refs/heads/main/scopes/ercot-scopes.yml
summary_line: 3 scopes · password
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- System Operator
- Texas
- Renewables
- Demand Response
- Open Data
token_urls:
- https://ercotb2c.b2clogin.com/ercotb2c.onmicrosoft.com/B2C_1_PUBAPI-ROPC-FLOW/oauth2/v2.0/token
---
