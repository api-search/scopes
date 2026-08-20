---
authorization_urls:
- https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/authorize
description: 'Trestle''s OAuth2 scope surface is deliberately tiny: the scope selects a transport/product surface, not a permission set. Row-level authorization is not expressed in scopes at all — it comes from the per-MLS licence contracts attached to the credential (which MLSs, which feed type, IDX vs IDX Plus). There is no published scope-to-permission matrix because there are no fine-grained scopes.'
docs: https://trestle-documentation.corelogic.com/webapi.html
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Trestle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Trestle publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Trestle API on a user''s behalf.


  Tokens are issued from https://api.cotality.com/trestle/oidc/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Trestle
provider_slug: trestle
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.cotality.com/trestle/oidc/connect/token
  - authorizationUrl: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/authorize
    flow: authorizationCode
    note: Advertised by discovery (grant_types_supported includes authorization_code, implicit, refresh_token and device_code) but the documented developer flow is client_credentials only.
    tokenUrl: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/token
  name: TrestleIdentityServer
  source: well-known/trestle-openid-configuration.json
  type: oauth2
scope_count: 3
scope_names:
- api
- rets
- offline_access
scopes:
- description: RESO Web API (OData 4.0) access, and Participant Reporting for Web API feeds. The documentation states this "should always be api for WebAPI".
  flows:
  - clientCredentials
  scope: api
- description: RETS 1.8 access, and Participant Reporting for RETS feeds. Requesting scope=api with RETS credentials is documented to fail with a 400.
  flows:
  - clientCredentials
  scope: rets
- description: Standard OIDC refresh-token scope, advertised in scopes_supported. Not referenced anywhere in the Trestle developer documentation; the documented client_credentials flow simply re-requests an 8-hour token.
  flows:
  - authorizationCode
  scope: offline_access
slug: trestle-scopes
source_filename: trestle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://api.cotality.com/trestle/oidc/.well-known/openid-configuration\n  (scopes_supported, fetched anonymously, HTTP 200 — saved verbatim at\n  well-known/trestle-openid-configuration.json) cross-checked against the\n  documented scope values in\n  https://trestle-documentation.corelogic.com/webapi.html,\n  https://trestle-documentation.corelogic.com/rets.html and\n  https://trestle-documentation.corelogic.com/participant-reporting-api.html\ndocs: https://trestle-documentation.corelogic.com/webapi.html\ndescription: >-\n  Trestle's OAuth2 scope surface is deliberately tiny: the scope selects a\n  transport/product surface, not a permission set. Row-level authorization is\n  not expressed in scopes at all — it comes from the per-MLS licence contracts\n  attached to the credential (which MLSs, which feed type, IDX vs IDX Plus).\n  There is no published scope-to-permission matrix because there are no\n  fine-grained scopes.\n\
  \nschemes:\n  - name: TrestleIdentityServer\n    type: oauth2\n    source: well-known/trestle-openid-configuration.json\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.cotality.com/trestle/oidc/connect/token\n      - flow: authorizationCode\n        authorizationUrl: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/authorize\n        tokenUrl: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/token\n        note: >-\n          Advertised by discovery (grant_types_supported includes\n          authorization_code, implicit, refresh_token and device_code) but the\n          documented developer flow is client_credentials only.\n\nscopes:\n  - scope: api\n    description: >-\n      RESO Web API (OData 4.0) access, and Participant Reporting for Web API\n      feeds. The documentation states this \"should always be api for WebAPI\".\n    flows: [clientCredentials]\n    sources:\n      - well-known/trestle-openid-configuration.json\n\
  \      - https://trestle-documentation.corelogic.com/webapi.html\n  - scope: rets\n    description: >-\n      RETS 1.8 access, and Participant Reporting for RETS feeds. Requesting\n      scope=api with RETS credentials is documented to fail with a 400.\n    flows: [clientCredentials]\n    sources:\n      - well-known/trestle-openid-configuration.json\n      - https://trestle-documentation.corelogic.com/rets.html\n  - scope: offline_access\n    description: >-\n      Standard OIDC refresh-token scope, advertised in scopes_supported. Not\n      referenced anywhere in the Trestle developer documentation; the documented\n      client_credentials flow simply re-requests an 8-hour token.\n    flows: [authorizationCode]\n    sources: [well-known/trestle-openid-configuration.json]\n\nauthorization_beyond_scopes:\n  model: contract-scoped credentials\n  detail: >-\n    Each credential is issued per product / feed-type pair and carries the set\n    of multiple listing organizations that pair is\
  \ licensed for. An observed\n    example JWT published in Trestle's own Postman collection carries\n    client_mlo_id_list, client_business_conn_id_list, client_product_id,\n    client_product_datafeed_transport and client_role claims — i.e. entitlement\n    is expressed as claims on the token, not as OAuth scopes.\n  evidence: postman/trestle-webapi.postman_collection.json\n  feed_types_documented: [IDX, IDX Plus]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trestle/refs/heads/main/scopes/trestle-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Real-Estate
- United States
- MLS
- RESO
- Property Listings
- IDX
- PropTech
- Data Distribution
- OData
- RETS
- Listing Syndication
token_urls:
- https://api.cotality.com/trestle/oidc/connect/token
- https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/token
---
