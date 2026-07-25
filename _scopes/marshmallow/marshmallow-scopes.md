---
authorization_urls:
- https://auth.marshmallow.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- refreshToken
- tokenExchange
kind: oauth-scopes
layout: scope
method: searched
name: Marshmallow Scopes
name_suffix: OAuth Scopes
note: Marshmallow runs a real OAuth 2.0 / OpenID Connect authorization server but publishes only the `openid` scope in its discovery metadata. No product scopes are advertised anonymously and there is no public scopes or permissions reference page. Any partner-specific scopes are provisioned out of band with the client and are not recorded here — nothing is inferred.
overview: 'Marshmallow publishes 1 OAuth 2.0 scope via the authorizationCode, clientCredentials, refreshToken, and tokenExchange flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Marshmallow API on a user''s behalf.


  Tokens are issued from https://auth.marshmallow.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Marshmallow
provider_slug: marshmallow
schemes:
- flows:
  - authorizationUrl: https://auth.marshmallow.com/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://auth.marshmallow.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://auth.marshmallow.com/oauth2/token
  - flow: refreshToken
    tokenUrl: https://auth.marshmallow.com/oauth2/token
  - flow: tokenExchange
    grant: urn:ietf:params:oauth:grant-type:token-exchange
    tokenUrl: https://auth.marshmallow.com/oauth2/token
  issuer: https://auth.marshmallow.com
  name: MarshmallowOpenIDConnect
  source: well-known/marshmallow-openid-configuration.json
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect authentication scope — requests an ID token identifying the end user. The only scope Marshmallow advertises publicly.
  flows:
  - authorizationCode
  scope: openid
slug: marshmallow-scopes
source_filename: marshmallow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.marshmallow.com/.well-known/openid-configuration\nlocal_copy: well-known/marshmallow-openid-configuration.json\ndocs: null\nnote: >-\n  Marshmallow runs a real OAuth 2.0 / OpenID Connect authorization server but\n  publishes only the `openid` scope in its discovery metadata. No product\n  scopes are advertised anonymously and there is no public scopes or\n  permissions reference page. Any partner-specific scopes are provisioned out\n  of band with the client and are not recorded here — nothing is inferred.\nschemes:\n- name: MarshmallowOpenIDConnect\n  source: well-known/marshmallow-openid-configuration.json\n  issuer: https://auth.marshmallow.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.marshmallow.com/oauth2/authorize\n    tokenUrl: https://auth.marshmallow.com/oauth2/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://auth.marshmallow.com/oauth2/token\n\
  \  - flow: refreshToken\n    tokenUrl: https://auth.marshmallow.com/oauth2/token\n  - flow: tokenExchange\n    tokenUrl: https://auth.marshmallow.com/oauth2/token\n    grant: urn:ietf:params:oauth:grant-type:token-exchange\nscopes:\n- scope: openid\n  description: >-\n    OpenID Connect authentication scope — requests an ID token identifying the\n    end user. The only scope Marshmallow advertises publicly.\n  flows: [authorizationCode]\n  sources: [well-known/marshmallow-openid-configuration.json]\ncoverage:\n  scopes_published: 1\n  product_scopes_published: 0\n  dynamic_client_registration: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marshmallow/refs/heads/main/scopes/marshmallow-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials/refreshToken/tokenExchange
tags:
- Insurance
- United Kingdom
- Insurtech
- Property and Casualty
- Motor Insurance
- Home Insurance
- Telematics
- Underwriting
- Claims
- Direct to Consumer
- Partner Gated
- No Public API
token_urls:
- https://auth.marshmallow.com/oauth2/token
---
