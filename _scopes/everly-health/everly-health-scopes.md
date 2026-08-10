---
authorization_urls:
- https://secure.everlywell.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: searched
name: Everly Health Scopes
name_suffix: OAuth Scopes
note: Scopes were read from scopes_supported in the anonymously published OpenID Connect Discovery / RFC 8414 document. Everly Health publishes no scopes or permissions reference page, so descriptions below are the spec-defined meaning of the scope name only — nothing was invented on the provider's behalf.
overview: 'Everly Health publishes 2 OAuth 2.0 scopes via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Everly Health API on a user''s behalf.


  Tokens are issued from https://secure.everlywell.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Everly Health
provider_slug: everly-health
schemes:
- flows:
  - authorizationUrl: https://secure.everlywell.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://secure.everlywell.com/oauth2/token
  - flow: password
    tokenUrl: https://secure.everlywell.com/oauth2/token
  issuer: https://secure.everlywell.com
  name: oauth2
  source: well-known/everly-health-openid-configuration.json
scope_count: 2
scope_names:
- openid
- public
scopes:
- description: Required by OpenID Connect Core 1.0 to request an ID token and identify the authenticated Everlywell member.
  flows:
  - authorizationCode
  - password
  scope: openid
- description: Declared in scopes_supported by the authorization server. Everly Health publishes no definition for it; recorded verbatim without interpretation.
  flows:
  - authorizationCode
  - password
  scope: public
slug: everly-health-scopes
source_filename: everly-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://secure.everlywell.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Scopes were read from scopes_supported in the anonymously published OpenID Connect\n  Discovery / RFC 8414 document. Everly Health publishes no scopes or permissions\n  reference page, so descriptions below are the spec-defined meaning of the scope\n  name only — nothing was invented on the provider's behalf.\nschemes:\n- name: oauth2\n  source: well-known/everly-health-openid-configuration.json\n  issuer: https://secure.everlywell.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.everlywell.com/oauth2/authorize\n    tokenUrl: https://secure.everlywell.com/oauth2/token\n  - flow: password\n    tokenUrl: https://secure.everlywell.com/oauth2/token\nscopes:\n- scope: openid\n  description: >-\n    Required by OpenID Connect Core 1.0 to request an ID token and identify the\n    authenticated Everlywell member.\n\
  \  flows:\n  - authorizationCode\n  - password\n  sources:\n  - well-known/everly-health-openid-configuration.json\n- scope: public\n  description: >-\n    Declared in scopes_supported by the authorization server. Everly Health publishes\n    no definition for it; recorded verbatim without interpretation.\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - well-known/everly-health-openid-configuration.json\ncoverage:\n  scopes_declared: 2\n  granular_resource_scopes: 0\n  note: >-\n    Two scopes total. There is no resource-level scope surface — consent granularity\n    is effectively all-or-nothing for anything beyond OIDC identity.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://secure.everlywell.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everly-health/refs/heads/main/scopes/everly-health-scopes.yml
summary_line: 2 scopes · authorizationCode/password
tags:
- Company
- Health
- Healthcare
- Digital Health
- Diagnostics
- Lab Testing
- Telehealth
- Consumer Health
- Identity
token_urls:
- https://secure.everlywell.com/oauth2/token
---
