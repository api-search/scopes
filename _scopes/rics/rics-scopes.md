---
api_specs:
- filename: rics-azurestorage-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Azure Storage API
  slug: rics-azurestorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-azurestorage-api-openapi.yml
- filename: rics-olamerchantpost-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Ola Merchant Post API
  slug: rics-olamerchantpost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-olamerchantpost-api-openapi.yml
- filename: rics-payment-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Payment API
  slug: rics-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-payment-api-openapi.yml
- filename: rics-profile-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Profile API
  slug: rics-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-profile-api-openapi.yml
- filename: rics-regulation-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Regulation API
  slug: rics-regulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-regulation-api-openapi.yml
- filename: rics-surveywriter-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Survey Writer API
  slug: rics-surveywriter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-surveywriter-api-openapi.yml
- filename: rics-token-api-openapi.yml
  format: yaml
  label: RICS (Royal Institution of Chartered Surveyors) Token API
  slug: rics-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/openapi/rics-token-api-openapi.yml
authorization_urls:
- https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Rics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RICS (Royal Institution of Chartered Surveyors) publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the RICS (Royal Institution of Chartered Surveyors) API on a user''s behalf.


  Tokens are issued from https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RICS (Royal Institution of Chartered Surveyors)
provider_slug: rics
schemes:
- end_session_endpoint: https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/oauth2/v2.0/logout
  flows:
  - authorizationUrl: https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/oauth2/v2.0/token
  issuer: https://b2clogin.rics.org/88b1d398-08db-4fc1-af82-65ba1595185c/v2.0/
  jwks_uri: https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/discovery/v2.0/keys
  name: Azure AD B2C - B2C_1A_RICS_signup_signin
  response_types_supported:
  - code
  - code id_token
  - code token
  - code id_token token
  - id_token
  - id_token token
  - token
  - token id_token
  source: openapi/rics-azure-ad-b2c-openid-configuration.json
  tenant: ricsb2clive.onmicrosoft.com
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
scope_count: 1
scope_names:
- openid
scopes:
- description: The only scope this authorization server advertises. Requests an ID token identifying the signed in RICS member; it grants no access to any RICS API resource.
  flows:
  - authorizationCode
  scope: openid
slug: rics-scopes
source_filename: rics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/B2C_1A_RICS_signup_signin/v2.0/.well-known/openid-configuration\n  (HTTP 200, fetched anonymously 2026-07-26)\nsummary: >-\n  RICS exposes exactly one OAuth/OIDC surface, and it is not the API. The Azure AD B2C tenant behind\n  RICS member sign-in publishes an OIDC discovery document whose scopes_supported list contains a\n  single value, \"openid\" - there is no resource scope, no API scope and no consent surface for\n  third-party applications. The DigitalCommunity API at api.rics.org has no scope model at all: it\n  authenticates with a RICS-issued username and password exchanged at POST /token for a bearer JWT,\n  and entitlement is decided server-side and surfaced only as 403 Forbidden.\napplies_to: RICS member sign-in (website and member portal), not api.rics.org\nschemes:\n- name: Azure AD B2C - B2C_1A_RICS_signup_signin\n  type: openIdConnect\n  source: openapi/rics-azure-ad-b2c-openid-configuration.json\n\
  \  issuer: https://b2clogin.rics.org/88b1d398-08db-4fc1-af82-65ba1595185c/v2.0/\n  tenant: ricsb2clive.onmicrosoft.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/oauth2/v2.0/authorize\n    tokenUrl: https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/oauth2/v2.0/token\n  response_types_supported: [code, code id_token, code token, code id_token token, id_token, id_token token, token, token id_token]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  end_session_endpoint: https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/oauth2/v2.0/logout\n  jwks_uri: https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/discovery/v2.0/keys\nscopes:\n- scope: openid\n  description: >-\n    The only scope this authorization server advertises. Requests an ID token identifying the signed\n \
  \   in RICS member; it grants no access to any RICS API resource.\n  flows: [authorizationCode]\n  sources: [openapi/rics-azure-ad-b2c-openid-configuration.json]\nclaims_supported:\n- contactNumber\n- sub\n- name\n- given_name\n- family_name\n- email\n- upn\n- oid\n- tid\n- uniqueId\n- iss\n- iat\n- exp\n- aud\n- acr\n- nonce\n- auth_time\nnotes:\n  api_scopes: >-\n    None. The DigitalCommunity API declares one securityScheme of type apiKey (Authorization header,\n    bearer JWT). No scope, permission or role is published, so an integrator cannot reason about\n    least privilege before receiving credentials from RICS.\n  contactNumber_claim: >-\n    The non-standard contactNumber claim is the RICS member/contact number, the same identifier the\n    DigitalCommunity API surfaces as contactNo on ProfileModel - the one visible join between the\n    member identity layer and the API data layer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rics/refs/heads/main/scopes/rics-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Real-Estate
- United Kingdom
- Industry Body
- Valuation
- Standards
- Surveying
- Property Measurement
- Regulations
- Construction
- PropTech
token_urls:
- https://b2clogin.rics.org/ricsb2clive.onmicrosoft.com/b2c_1a_rics_signup_signin/oauth2/v2.0/token
---
