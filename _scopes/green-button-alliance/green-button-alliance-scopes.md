---
api_specs:
- filename: green-button-alliance-applicationinformation-api-openapi.yml
  format: yaml
  label: Green Button Alliance Application Information API
  slug: green-button-alliance-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-applicationinformation-api-openapi.yml
- filename: green-button-alliance-authorization-api-openapi.yml
  format: yaml
  label: Green Button Alliance Authorization API
  slug: green-button-alliance-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-authorization-api-openapi.yml
- filename: green-button-alliance-batch-api-openapi.yml
  format: yaml
  label: Green Button Alliance Batch API
  slug: green-button-alliance-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-batch-api-openapi.yml
- filename: green-button-alliance-datacustodian-integration-api-openapi.yml
  format: yaml
  label: Green Button Alliance DataCustodian Integration API
  slug: green-button-alliance-datacustodian-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-datacustodian-integration-api-openapi.yml
- filename: green-button-alliance-oauth2-client-management-api-openapi.yml
  format: yaml
  label: Green Button Alliance OAuth2 Client Management API
  slug: green-button-alliance-oauth2-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-oauth2-client-management-api-openapi.yml
- filename: green-button-alliance-oauth2-standard-api-openapi.yml
  format: yaml
  label: Green Button Alliance OAuth2 Standard API
  slug: green-button-alliance-oauth2-standard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-oauth2-standard-api-openapi.yml
- filename: green-button-alliance-oidc-api-openapi.yml
  format: yaml
  label: Green Button Alliance OIDC API
  slug: green-button-alliance-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-oidc-api-openapi.yml
- filename: green-button-alliance-usagepoint-api-openapi.yml
  format: yaml
  label: Green Button Alliance Usage Point API
  slug: green-button-alliance-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-usagepoint-api-openapi.yml
authorization_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
description: Green Button does not use conventional string scopes such as "read:usage". The NAESB REQ.21 ESPI profile encodes the entire authorization request into a single structured OAuth 2.0 scope value built from Function Block ids plus data-shape parameters. GBA's own words on /function-blocks - "The NAESB REQ.21 ESPI standard uses Function Blocks to define the type of data a Utility can provide a Third Party service provider and the type of data a Third Party service provider requests from the Utility during the OAuth 2.0 access-token request process. The list of available Function Blocks a Utility supports is shown in the <scope> element field of the <ApplicationInformation> resource - and the resource may contain multiple <scope> entries." The harvested OpenAPI declares oauth2 with an EMPTY scopes map for both flows, so the scope vocabulary below comes from GBA's published Function Block catalog and from GBA's own wire-contract fixtures - not from the spec, and not invented.
docs: https://www.greenbuttonalliance.org/function-blocks
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Green Button Alliance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Green Button Alliance uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox.greenbuttonalliance.org:8443/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Green Button Alliance
provider_slug: green-button-alliance
schemes:
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    declared_scopes_in_spec: 0
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - declared_scopes_in_spec: 0
    flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/green-button-alliance-green-button-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: green-button-alliance-scopes
source_filename: green-button-alliance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/green-button-alliance-green-button-api-openapi.yml\ndocs: https://www.greenbuttonalliance.org/function-blocks\nadditional_docs:\n- https://www.greenbuttonalliance.org/cmd-function-blocks\n- https://www.greenbuttonalliance.org/access-tokens\n- https://www.greenbuttonalliance.org/oauth-20-access-and-refresh-token-duration\n- https://github.com/GreenButtonAlliance/OpenESPI-GreenButton-Java/tree/main/contracts\ndescription: >-\n  Green Button does not use conventional string scopes such as \"read:usage\". The\n  NAESB REQ.21 ESPI profile encodes the entire authorization request into a single\n  structured OAuth 2.0 scope value built from Function Block ids plus data-shape\n  parameters. GBA's own words on /function-blocks - \"The NAESB REQ.21 ESPI\n  standard uses Function Blocks to define the type of data a Utility can provide a\n  Third Party service provider and the type of data a Third Party service provider\n  requests\
  \ from the Utility during the OAuth 2.0 access-token request process. The\n  list of available Function Blocks a Utility supports is shown in the <scope>\n  element field of the <ApplicationInformation> resource - and the resource may\n  contain multiple <scope> entries.\"\n  The harvested OpenAPI declares oauth2 with an EMPTY scopes map for both flows,\n  so the scope vocabulary below comes from GBA's published Function Block catalog\n  and from GBA's own wire-contract fixtures - not from the spec, and not invented.\nscope_model: espi-function-block-grammar\nschemes:\n- name: oauth2\n  source: openapi/green-button-alliance-green-button-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    declared_scopes_in_spec: 0\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    declared_scopes_in_spec:\
  \ 0\ngrammar:\n  shape: FB=<fb_ids>;<parameter>=<value>;...\n  separator: ';'\n  fb_id_separator: '_'\n  parameters:\n  - name: FB\n    required: true\n    description: >-\n      Underscore-joined list of NAESB ESPI Function Block ids being requested,\n      without the FB_ prefix and without leading zeros (e.g. FB=1_3_4_5_13_31_37_39\n      means FB_01, FB_03, FB_04, FB_05, FB_13, FB_31, FB_37, FB_39). The catalog of\n      valid ids is vocabulary/green-button-alliance-function-blocks.yml.\n  - name: IntervalDuration\n    required: false\n    description: Interval length in seconds for interval data (observed published values 900, 3600).\n  - name: BlockDuration\n    required: false\n    description: Aggregation block for the data (observed published values monthly, daily).\n  - name: HistoryLength\n    required: false\n    description: How much history is being authorized (observed published value 13).\n  - name: BR\n    required: false\n    description: >-\n      Observed in GBA's client-credentials\
  \ Bulk fixture (BR=1). The normative\n      definition lives in the paywalled NAESB REQ.21 ESPI standard and is not\n      reproduced here.\n  published_examples:\n  - value: FB=1_3_4_5_13_31_37_39;IntervalDuration=900;BlockDuration=monthly;HistoryLength=13\n    source: openapi/green-button-alliance-application-information-openapi.yml (ApplicationInformation.scope example)\n  - value: FB=1_3_4_10_13_15_31_37_39;IntervalDuration=3600;BlockDuration=monthly;HistoryLength=13\n    source: openapi/green-button-alliance-application-information-openapi.yml (ApplicationInformation.scope example)\n  - value: FB=1_3_4_11_13_31_37_39;IntervalDuration=900;BlockDuration=monthly;HistoryLength=13\n    source: openapi/green-button-alliance-application-information-openapi.yml (ApplicationInformation.scope example)\n  - value: FB=4_5_15;IntervalDuration=3600;BlockDuration=monthly;HistoryLength=13\n    source: examples/green-button-alliance-token-response-subscription.json (authorization_code grant)\n  -\
  \ value: FB=1_3_4_5_10_11_35;BlockDuration=daily;BR=1\n    source: examples/green-button-alliance-token-response-bulk.json (client_credentials / Bulk grant)\n  - value: FB=44\n    source: >-\n      openapi/green-button-alliance-application-information-openapi.yml -\n      registration_access_token is \"generated in response to a Third Party OAuth 2.0\n      Client Credentials Request with FB=44 in the Scope parameter\" (FB_44 Manage\n      Authorization Resource).\nscopes: []\nscopes_note: >-\n  Deliberately empty. There is no flat scope-string list to enumerate: a Green\n  Button scope is composed at request time from the Function Block catalog plus the\n  parameters above. Enumerating a synthetic list of \"scopes\" here would fabricate a\n  vocabulary GBA does not publish. Use vocabulary/green-button-alliance-function-blocks.yml\n  as the scope vocabulary and the grammar block above as the composition rule.\ntoken_types:\n  source: https://www.greenbuttonalliance.org/access-tokens\n\
  \  types:\n  - name: access_token\n    description: >-\n      Allocated by the Data Custodian for individual account authorizations. The\n      normal access token used for accessing individual subscriptions.\n    obtained: During the Customer authorization process.\n  - name: refresh_token\n    description: >-\n      Allocated at the time of an authorization and used to renew an access_token\n      once it expires.\n    obtained: During the Customer authorization process.\n  - name: datacustodian_access_token\n    description: Access token used by trusted administrative accounts, allocated by administrative action by the Data Custodian.\n  - name: client_access_token\n    description: >-\n      Used by Third-Party applications to access bulk or multiple authorization\n      subscriptions; allocated at Third Party registration when the Data Custodian\n      provides Bulk data transfers. Obtained via the OAuth client_credentials flow.\n  - name: upload_access_token\n    description: >-\n\
  \      Used by Meter Data Management (backend) systems to upload/import data into a\n      Data Custodian; allocated by administrative action.\n  - name: registration_access_token\n    description: >-\n      Used by the Third Party to manage its ApplicationInformation (RFC 7592\n      registration management). Assigned during registration or minted via a\n      client_credentials request with FB=44.\nmember_sso_scopes:\n  note: >-\n    Separate and unrelated to energy data - these are the scopes of GBA's own\n    member single sign-on (association management), harvested from\n    well-known/green-button-alliance-openid-configuration.json.\n  source: https://www.greenbuttonalliance.org/.well-known/openid-configuration\n  scopes: [openid, email, profile]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/scopes/green-button-alliance-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- Water
- Smart Metering
- Green Button
- ESPI
- Standards Body
- Certification
- Consumer Energy Data
token_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/token
---
