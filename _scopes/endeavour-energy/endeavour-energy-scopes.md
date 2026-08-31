---
api_specs:
- filename: endeavour-energy-catalog-api-openapi.yml
  format: yaml
  label: Endeavour Energy Catalog API
  slug: endeavour-energy-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavour-energy/refs/heads/main/openapi/endeavour-energy-catalog-api-openapi.yml
- filename: endeavour-energy-dataset-api-openapi.yml
  format: yaml
  label: Endeavour Energy Dataset API
  slug: endeavour-energy-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavour-energy/refs/heads/main/openapi/endeavour-energy-dataset-api-openapi.yml
authorization_urls:
- https://data.endeavourenergy.com.au/oauth2/authorize/
description: 'Endeavour Energy''s open data portal runs the Opendatasoft OAuth2 authorization-code flow, RFC 6749 compliant with RFC 6750 bearer tokens. The scope model is deliberately trivial: there is exactly ONE scope, `all`, and it is the only value the platform accepts. There is no read/write split, no per-dataset scope, and no least-privilege story — an authorized application gets whatever its authorizing user has. This is worth recording precisely because it is the opposite of a granular scope catalogue, and an agent planning consent needs to know that "all" is the only option.'
docs: https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html#section/Authentication/Using-OAuth2-authorization
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Endeavour Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Endeavour Energy publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Endeavour Energy API on a user''s behalf.


  Tokens are issued from https://data.endeavourenergy.com.au/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Endeavour Energy
provider_slug: endeavour-energy
schemes:
- client_types:
  - note: client secret kept server-side
    type: confidential
  - note: client secret embedded in a client-side app
    type: public
  discovery:
    note: No RFC 8414 metadata document. A client cannot discover these endpoints programmatically; they are only in the vendor documentation.
    well_known_oauth_authorization_server: 404
    well_known_openid_configuration: 404
  flows:
  - authorizationUrl: https://data.endeavourenergy.com.au/oauth2/authorize/
    authorization_code_ttl: 1 hour — the 30-character code must be exchanged before it expires
    authorize_params:
    - client_id
    - redirect_uri
    - response_type=code
    - scopes
    - state
    client_auth_at_token_endpoint: 'form parameters or HTTP Basic (Authorization: Basic base64(client_id:client_secret))'
    flow: authorizationCode
    refresh_supported: true
    state_recommended: true
    tokenUrl: https://data.endeavourenergy.com.au/oauth2/token/
    token_params:
    - client_id
    - client_secret
    - redirect_uri
    - grant_type=authorization_code
    - code
    - scopes
    - state
  name: oauth2
  registration:
    domain_bound: '"Currently, applications are registered on a specific domain and can only access data on this domain." An application registered here works only against data.endeavourenergy.com.au.'
    fields:
    - application name
    - type
    - redirection URL
    returns:
    - client_id
    - client_secret
    url: https://data.endeavourenergy.com.au/account/ -> "My applications" tab
  rfc:
  - RFC 6749
  - RFC 6750
  source: docs + live probe (not in openapi/)
  token_type: Bearer
  verified_live:
  - note: exists; redirects to the portal login
    status: 302
    url: https://data.endeavourenergy.com.au/oauth2/authorize/
  - note: exists; Method Not Allowed on GET, POST-only as documented
    status: 405
    url: https://data.endeavourenergy.com.au/oauth2/token/
scope_count: 1
scope_names:
- all
scopes:
- description: 'Full access to the data the authorizing user can see on this domain. The published wording is unambiguous: "a list of space-separated requested scopes. Currently, only `all` is supported."'
  flows:
  - authorizationCode
  scope: all
slug: endeavour-energy-scopes
source_filename: endeavour-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html#section/Authentication/Using-OAuth2-authorization\n  plus live probes of the OAuth2 endpoints on Endeavour Energy's own portal host\n  on 2026-07-27. The mechanical derive pass\n  (0-working/derive-oauth-scopes.py) found ZERO oauth2 schemes because the\n  harvested OpenAPI declares only an apiKey — this file exists because the\n  OAuth2 surface is real but undeclared.\ndocs: 'https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html#section/Authentication/Using-OAuth2-authorization'\ndescription: >-\n  Endeavour Energy's open data portal runs the Opendatasoft OAuth2\n  authorization-code flow, RFC 6749 compliant with RFC 6750 bearer tokens. The\n  scope model is deliberately trivial: there is exactly ONE scope, `all`, and\n  it is the only value the platform accepts. There is no read/write split, no\n  per-dataset scope, and no least-privilege\
  \ story — an authorized application\n  gets whatever its authorizing user has. This is worth recording precisely\n  because it is the opposite of a granular scope catalogue, and an agent\n  planning consent needs to know that \"all\" is the only option.\n\ndeclared_in_openapi: false\nderive_pass_result: 'no oauth2 securityScheme in any harvested spec'\n\nschemes:\n  - name: oauth2\n    source: 'docs + live probe (not in openapi/)'\n    rfc: [RFC 6749, RFC 6750]\n    token_type: Bearer\n    client_types:\n      - {type: confidential, note: 'client secret kept server-side'}\n      - {type: public, note: 'client secret embedded in a client-side app'}\n    registration:\n      url: 'https://data.endeavourenergy.com.au/account/ -> \"My applications\" tab'\n      fields: [application name, type, redirection URL]\n      returns: [client_id, client_secret]\n      domain_bound: >-\n        \"Currently, applications are registered on a specific domain and can\n        only access data on this domain.\"\
  \ An application registered here works\n        only against data.endeavourenergy.com.au.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://data.endeavourenergy.com.au/oauth2/authorize/\n        tokenUrl: https://data.endeavourenergy.com.au/oauth2/token/\n        refresh_supported: true\n        authorize_params: [client_id, redirect_uri, 'response_type=code', scopes, state]\n        token_params: [client_id, client_secret, redirect_uri, 'grant_type=authorization_code', code, scopes, state]\n        client_auth_at_token_endpoint: 'form parameters or HTTP Basic (Authorization: Basic base64(client_id:client_secret))'\n        authorization_code_ttl: '1 hour — the 30-character code must be exchanged before it expires'\n        state_recommended: true\n    verified_live:\n      - {url: 'https://data.endeavourenergy.com.au/oauth2/authorize/', status: 302, note: 'exists; redirects to the portal login'}\n      - {url: 'https://data.endeavourenergy.com.au/oauth2/token/',\
  \ status: 405, note: 'exists; Method Not Allowed on GET, POST-only as documented'}\n    discovery:\n      well_known_oauth_authorization_server: 404\n      well_known_openid_configuration: 404\n      note: >-\n        No RFC 8414 metadata document. A client cannot discover these endpoints\n        programmatically; they are only in the vendor documentation.\n\nscopes:\n  - scope: all\n    description: >-\n      Full access to the data the authorizing user can see on this domain.\n      The published wording is unambiguous: \"a list of space-separated\n      requested scopes. Currently, only `all` is supported.\"\n    flows: [authorizationCode]\n    optional: true\n    sources: ['https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html#section/Authentication/Using-OAuth2-authorization']\n\ngranularity:\n  scope_count: 1\n  read_write_split: false\n  per_dataset_scopes: false\n  least_privilege_possible: false\n  assessment: >-\n    On this domain the practical consequence is\
  \ small — all eight datasets are\n    public and readable anonymously, and the API is GET-only, so an `all` token\n    grants nothing an unauthenticated caller does not already have. The scope\n    model would matter on a portal with restricted datasets; here it is\n    effectively decorative.\n\nalternative_credentials:\n  note: >-\n    API keys carry the same problem in a sharper form: \"every API key\n    authenticates requests as coming from your user, which means they grant the\n    same rights (yours) to any person using them.\" Key permissions can only be\n    narrowed through the separate Automation API, whose surface on this host\n    (/api/management/v2/swagger.json) returns 401.\n\nrelated:\n  - authentication/endeavour-energy-authentication.yml\n  - well-known/endeavour-energy-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endeavour-energy/refs/heads/main/scopes/endeavour-energy-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Open Data
- Energy Networks
- Distribution
- Outages
- Consumer Data Right
- Smart Metering
- DER
- Solar
- Renewables
token_urls:
- https://data.endeavourenergy.com.au/oauth2/token/
---
