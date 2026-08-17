---
api_specs:
- filename: factiva-apis
  format: yaml
  label: Factiva Snapshots API
  slug: factiva-snapshots-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Streams API
  slug: factiva-streams-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Extractions API
  slug: factiva-extractions-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Analytics API
  slug: factiva-analytics-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva DJID Taxonomy API
  slug: factiva-djid-taxonomy-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Code API
  slug: factiva-code-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-content-api-swagger.json
  format: json
  label: Factiva Content API
  slug: factiva-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-content-api-swagger.json
- filename: factiva-newsletters-api-openapi.json
  format: json
  label: DJ Factiva Newsletters API
  slug: dj-factiva-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-newsletters-api-openapi.json
- filename: factiva-company-news-radar-api-openapi.json
  format: json
  label: Factiva Company News Radar API
  slug: factiva-company-news-radar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-company-news-radar-api-openapi.json
authorization_urls:
- https://sso.accounts.dowjones.com/authorize
description: The Factiva APIs do not carry per-resource OAuth scopes. Scope on the Dow Jones identity service selects WHICH TOKENS the exchange returns (and whether a refresh token is issued), not which Factiva resources the caller may touch — entitlement to Factiva content is granted on the account/service-account by contract, outside the token. Recorded here because the scope strings are load-bearing for anyone implementing the flow, not because they are a permission model. None of the three harvested OpenAPI documents declares an oauth2 securityScheme, so the mechanical derive pass produced nothing.
docs: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication
flows:
- password
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Factiva Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Factiva publishes 8 OAuth 2.0 scopes via the password, authorizationCode, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Factiva API on a user''s behalf.


  Tokens are issued from https://accounts.dowjones.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Factiva
provider_slug: factiva
schemes:
- flows:
  - flow: password
    note: The flow the Factiva Integration docs prescribe (connection=service-account).
    tokenUrl: https://accounts.dowjones.com/oauth2/v1/token
  - authorizationUrl: https://sso.accounts.dowjones.com/authorize
    flow: authorizationCode
    tokenUrl: https://sso.accounts.dowjones.com/oauth/token
  - authorizationUrl: https://sso.accounts.dowjones.com/authorize
    flow: implicit
  issuer: https://sso.accounts.dowjones.com/
  local_copy: well-known/factiva-openid-configuration.json
  name: DowJonesIdentityService
  source: https://accounts.dowjones.com/.well-known/openid-configuration
scope_count: 8
scope_names:
- openid
- service_account_id
- offline_access
- profile
- email
- email_verified
- given_name
- family_name
scopes:
- description: Required. Requests an OpenID Connect id_token from the identity service.
  flows:
  - password
  - authorizationCode
  - implicit
  scope: openid
- description: Documented by Factiva for the service-account exchange. Combined with `openid`, it tells the token endpoint to return the two AuthN tokens (id_token and access_token).
  flows:
  - password
  scope: service_account_id
- description: Adds a refresh token to the response. When requested, the `device` parameter becomes mandatory and acts as the identifier under which the refresh token can later be revoked.
  flows:
  - password
  - authorizationCode
  scope: offline_access
- description: Standard OIDC profile claims.
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Standard OIDC email claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Email verification claim.
  flows:
  - authorizationCode
  - implicit
  scope: email_verified
- description: Standard OIDC given-name claim.
  flows:
  - authorizationCode
  - implicit
  scope: given_name
- description: Standard OIDC family-name claim.
  flows:
  - authorizationCode
  - implicit
  scope: family_name
slug: factiva-scopes
source_filename: factiva-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://accounts.dowjones.com/.well-known/openid-configuration\ndocs: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication\ndescription: >-\n  The Factiva APIs do not carry per-resource OAuth scopes. Scope on the Dow Jones identity\n  service selects WHICH TOKENS the exchange returns (and whether a refresh token is issued),\n  not which Factiva resources the caller may touch — entitlement to Factiva content is granted\n  on the account/service-account by contract, outside the token. Recorded here because the\n  scope strings are load-bearing for anyone implementing the flow, not because they are a\n  permission model. None of the three harvested OpenAPI documents declares an oauth2\n  securityScheme, so the mechanical derive pass produced nothing.\nschemes:\n  - name: DowJonesIdentityService\n    source: https://accounts.dowjones.com/.well-known/openid-configuration\n    local_copy: well-known/factiva-openid-configuration.json\n\
  \    issuer: https://sso.accounts.dowjones.com/\n    flows:\n      - flow: password\n        tokenUrl: https://accounts.dowjones.com/oauth2/v1/token\n        note: The flow the Factiva Integration docs prescribe (connection=service-account).\n      - flow: authorizationCode\n        authorizationUrl: https://sso.accounts.dowjones.com/authorize\n        tokenUrl: https://sso.accounts.dowjones.com/oauth/token\n      - flow: implicit\n        authorizationUrl: https://sso.accounts.dowjones.com/authorize\nscopes:\n  - scope: openid\n    description: Required. Requests an OpenID Connect id_token from the identity service.\n    flows: [password, authorizationCode, implicit]\n    sources: [https://accounts.dowjones.com/.well-known/openid-configuration]\n  - scope: service_account_id\n    description: >-\n      Documented by Factiva for the service-account exchange. Combined with `openid`, it tells\n      the token endpoint to return the two AuthN tokens (id_token and access_token).\n    flows:\
  \ [password]\n    sources: [https://developer.dowjones.com/documents/factiva_integration-essentials-authentication]\n    note: >-\n      Documented by Factiva but not listed in the identity service's scopes_supported array.\n  - scope: offline_access\n    description: >-\n      Adds a refresh token to the response. When requested, the `device` parameter becomes\n      mandatory and acts as the identifier under which the refresh token can later be revoked.\n    flows: [password, authorizationCode]\n    sources:\n      - https://accounts.dowjones.com/.well-known/openid-configuration\n      - https://developer.dowjones.com/documents/factiva_integration-essentials-authentication\n  - scope: profile\n    description: Standard OIDC profile claims.\n    flows: [authorizationCode, implicit]\n    sources: [https://accounts.dowjones.com/.well-known/openid-configuration]\n  - scope: email\n    description: Standard OIDC email claim.\n    flows: [authorizationCode, implicit]\n    sources: [https://accounts.dowjones.com/.well-known/openid-configuration]\n\
  \  - scope: email_verified\n    description: Email verification claim.\n    flows: [authorizationCode, implicit]\n    sources: [https://accounts.dowjones.com/.well-known/openid-configuration]\n  - scope: given_name\n    description: Standard OIDC given-name claim.\n    flows: [authorizationCode, implicit]\n    sources: [https://accounts.dowjones.com/.well-known/openid-configuration]\n  - scope: family_name\n    description: Standard OIDC family-name claim.\n    flows: [authorizationCode, implicit]\n    sources: [https://accounts.dowjones.com/.well-known/openid-configuration]\nsummary:\n  scope_count: 8\n  resource_scopes: 0\n  authorization_model: >-\n    Contract/entitlement-based. Access to Factiva content sets is provisioned against the\n    account by Dow Jones; the token conveys identity, not per-resource permission.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/scopes/factiva-scopes.yml
summary_line: 8 scopes · password/authorizationCode/implicit
tags:
- AI
- Business Intelligence
- Content Aggregation
- Enterprise Data
- GenAI
- Market Data
- Media Monitoring
- News
- News API
- Research
- Taxonomy
token_urls:
- https://accounts.dowjones.com/oauth2/v1/token
- https://sso.accounts.dowjones.com/oauth/token
---
