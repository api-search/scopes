---
authorization_urls: []
description: ''
docs: https://developers.pismo.io/pismo-docs/docs/authentication-with-oauth2
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Pismo Scopes
name_suffix: OAuth Scopes
note: Pismo uses OAuth 2.0 client-credentials tokens with permission-group scopes of the form pismo-v1:<resource>:<access>; only three example scopes are publicly documented, and the complete list of API permission groups is only viewable by customers inside Control Center per https://developers.pismo.io/pismo-docs/docs/cc-api-permission-groups.
overview: 'Pismo publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pismo API on a user''s behalf.


  Tokens are issued from https://api.pismo.io/passport/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pismo
provider_slug: pismo
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.pismo.io/passport/v2/oauth/token
  name: oauth2
  source: openapi/pismo-openapi.yml
scope_count: 3
scope_names:
- pismo-v1:accounts:rw
- pismo-v1:cards:rw
- pismo-v1:bankaccounts:rw
scopes:
- description: Read-write access to the accounts group of endpoints; documented as an example permission-group scope in the OAuth2 authentication guide.
  flows: []
  scope: pismo-v1:accounts:rw
- description: Read-write access to the cards group of endpoints; documented as an example permission-group scope in the OAuth2 authentication guide.
  flows: []
  scope: pismo-v1:cards:rw
- description: Read-write access to the bank accounts group of endpoints; documented as an example permission-group scope in the OAuth2 authentication guide.
  flows: []
  scope: pismo-v1:bankaccounts:rw
slug: pismo-scopes
source_filename: pismo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/pismo-openapi.yml\ndocs: https://developers.pismo.io/pismo-docs/docs/authentication-with-oauth2\nnote: Pismo uses OAuth 2.0 client-credentials tokens with permission-group scopes\n  of the form pismo-v1:<resource>:<access>; only three example scopes are publicly\n  documented, and the complete list of API permission groups is only viewable by\n  customers inside Control Center per\n  https://developers.pismo.io/pismo-docs/docs/cc-api-permission-groups.\nschemes:\n- name: oauth2\n  source: openapi/pismo-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.pismo.io/passport/v2/oauth/token\nscopes:\n- scope: pismo-v1:accounts:rw\n  description: Read-write access to the accounts group of endpoints; documented as\n    an example permission-group scope in the OAuth2 authentication guide.\n  sources:\n  - https://developers.pismo.io/pismo-docs/docs/authentication-with-oauth2\n- scope: pismo-v1:cards:rw\n\
  \  description: Read-write access to the cards group of endpoints; documented as an\n    example permission-group scope in the OAuth2 authentication guide.\n  sources:\n  - https://developers.pismo.io/pismo-docs/docs/authentication-with-oauth2\n- scope: pismo-v1:bankaccounts:rw\n  description: Read-write access to the bank accounts group of endpoints; documented\n    as an example permission-group scope in the OAuth2 authentication guide.\n  sources:\n  - https://developers.pismo.io/pismo-docs/docs/authentication-with-oauth2\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/scopes/pismo-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Banking
- Card Issuing
- Payments
- Fintech
- Core Banking
- Cloud Native
token_urls:
- https://api.pismo.io/passport/v2/oauth/token
---
