---
authorization_urls:
- https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Insurance Council Australia Scopes
name_suffix: OAuth Scopes
note: The only OAuth/OIDC surface on the Insurance Council of Australia estate is the Azure AD B2C tenant that fronts the member portal sign-in. Its discovery document advertises a single scope — openid — which is the bare OIDC authentication scope and carries no API authorization semantics. There is no scopes or permissions reference page on insurancecouncil.com.au, no delegated data scopes, and no client-credentials surface, so this artifact records the full (and minimal) real scope catalogue rather than a curated one.
overview: 'Insurance Council of Australia publishes 1 OAuth 2.0 scope via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Insurance Council of Australia API on a user''s behalf.


  Tokens are issued from https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Insurance Council of Australia
provider_slug: insurance-council-australia
schemes:
- flows:
  - authorizationUrl: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/token
  - authorizationUrl: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/authorize
    flow: implicit
    note: id_token / token response types are advertised in response_types_supported.
  name: azure-ad-b2c-signin
  source: well-known/insurance-council-australia-openid-configuration.json
  type: openIdConnect
scope_count: 1
scope_names:
- openid
scopes:
- description: Standard OpenID Connect authentication scope. Returns an id_token for a member portal user; grants no access to any ICA data API.
  flows:
  - authorizationCode
  - implicit
  scope: openid
slug: insurance-council-australia-scopes
source_filename: insurance-council-australia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/v2.0/.well-known/openid-configuration\nnote: |\n  The only OAuth/OIDC surface on the Insurance Council of Australia estate is the\n  Azure AD B2C tenant that fronts the member portal sign-in. Its discovery document\n  advertises a single scope — openid — which is the bare OIDC authentication scope\n  and carries no API authorization semantics. There is no scopes or permissions\n  reference page on insurancecouncil.com.au, no delegated data scopes, and no\n  client-credentials surface, so this artifact records the full (and minimal) real\n  scope catalogue rather than a curated one.\ndocs: null\nschemes:\n- name: azure-ad-b2c-signin\n  type: openIdConnect\n  source: well-known/insurance-council-australia-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/authorize\n\
  \    tokenUrl: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/token\n  - flow: implicit\n    authorizationUrl: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/authorize\n    note: id_token / token response types are advertised in response_types_supported.\nscopes:\n- scope: openid\n  description: |\n    Standard OpenID Connect authentication scope. Returns an id_token for a member\n    portal user; grants no access to any ICA data API.\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/insurance-council-australia-openid-configuration.json\ncoverage:\n  scope_count: 1\n  data_scopes: 0\n  client_credentials_scopes: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insurance-council-australia/refs/heads/main/scopes/insurance-council-australia-scopes.yml
summary_line: 1 scope · authorizationCode/implicit
tags:
- Insurance
- Australia
- General Insurance
- Industry Association
- Property and Casualty
- Claims
- Catastrophe
- Risk Data
- Code of Practice
token_urls:
- https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/token
---
