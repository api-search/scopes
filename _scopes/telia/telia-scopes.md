---
api_specs:
- filename: telia-listgeographicsite-api-openapi.yml
  format: yaml
  label: Telia Company List Geographic Site API
  slug: telia-listgeographicsite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telia/refs/heads/main/openapi/telia-listgeographicsite-api-openapi.yml
- filename: telia-retrievegeographicsite-api-openapi.yml
  format: yaml
  label: Telia Company Retrieve Geographic Site API
  slug: telia-retrievegeographicsite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telia/refs/heads/main/openapi/telia-retrievegeographicsite-api-openapi.yml
authorization_urls:
- https://tunnistus.telia.fi/uas/oauth2/authorization
description: ''
docs: https://tunnistus.telia.fi/.well-known/openid-configuration
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Telia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Telia Company publishes 2 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Telia Company API on a user''s behalf.


  Tokens are issued from https://api-garden.teliacompany.com/v4/oauth/client_credential/accesstoken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Telia Company
provider_slug: telia
schemes:
- description: Token endpoint for the production environment
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-garden.teliacompany.com/v4/oauth/client_credential/accesstoken
  name: prodBearerAuth
  scopes_declared: 0
  source: openapi/telia-lso-sonata-site-management.yml
- description: Token endpoint for all test environments
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-garden-test.teliacompany.com/v4/oauth/client_credential/accesstoken
  name: testBearerAuth
  scopes_declared: 0
  source: openapi/telia-lso-sonata-site-management.yml
- description: Telia Tunnistus identification broker (Telia Finland strong electronic identification)
  flows:
  - authorizationUrl: https://tunnistus.telia.fi/uas/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://tunnistus.telia.fi/uas/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://tunnistus.telia.fi/uas/oauth2/token
  local_copy: well-known/telia-openid-configuration.json
  name: tunnistusOidc
  scopes_declared: 2
  source: https://tunnistus.telia.fi/.well-known/openid-configuration
scope_count: 2
scope_names:
- openid
- userinfo
scopes:
- description: Standard OpenID Connect scope; requests an ID token from the Telia Tunnistus identification broker.
  flows:
  - authorizationCode
  scope: openid
- description: Grants access to the Tunnistus userinfo endpoint (https://tunnistus.telia.fi/uas/oauth2/userinfo) for the identified subject.
  flows:
  - authorizationCode
  scope: userinfo
slug: telia-scopes
source_filename: telia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/telia-lso-sonata-site-management.yml\ndocs: https://tunnistus.telia.fi/.well-known/openid-configuration\nnotes: >-\n  Telia publishes almost no scope vocabulary. The LSO Sonata specification\n  declares two oauth2 clientCredentials schemes with EMPTY scopes maps, so\n  authorization on that surface is a function of the commercial entitlement\n  attached to the client id rather than of any scope the caller can request. The\n  only scopes published anywhere on Telia's estate are the two advertised by the\n  Telia Tunnistus identification broker's OIDC discovery document. No scopes or\n  permissions reference page was found on developer.teliacompany.io,\n  lso.teliacompany.com, camara.teliacompany.com or developer.telia.fi.\nschemes:\n- name: prodBearerAuth\n  source: openapi/telia-lso-sonata-site-management.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-garden.teliacompany.com/v4/oauth/client_credential/accesstoken\n\
  \  description: Token endpoint for the production environment\n  scopes_declared: 0\n- name: testBearerAuth\n  source: openapi/telia-lso-sonata-site-management.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-garden-test.teliacompany.com/v4/oauth/client_credential/accesstoken\n  description: Token endpoint for all test environments\n  scopes_declared: 0\n- name: tunnistusOidc\n  source: https://tunnistus.telia.fi/.well-known/openid-configuration\n  local_copy: well-known/telia-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://tunnistus.telia.fi/uas/oauth2/authorization\n    tokenUrl: https://tunnistus.telia.fi/uas/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://tunnistus.telia.fi/uas/oauth2/token\n  description: Telia Tunnistus identification broker (Telia Finland strong\n    electronic identification)\n  scopes_declared: 2\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests\
  \ an ID token from the Telia\n    Tunnistus identification broker.\n  flows:\n  - authorizationCode\n  sources:\n  - https://tunnistus.telia.fi/.well-known/openid-configuration\n- scope: userinfo\n  description: Grants access to the Tunnistus userinfo endpoint\n    (https://tunnistus.telia.fi/uas/oauth2/userinfo) for the identified subject.\n  flows:\n  - authorizationCode\n  sources:\n  - https://tunnistus.telia.fi/.well-known/openid-configuration\ngaps:\n- No CAMARA scope vocabulary is published; CAMARA APIs normally define\n  purpose-bound scopes such as qod or device-location, and none is discoverable\n  on Telia's CAMARA portal.\n- The LSO Sonata oauth2 schemes declare no scopes at all.\n- The Bulk Messaging APIs use HTTP Basic and have no scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telia/refs/heads/main/scopes/telia-scopes.yml
summary_line: 2 scopes · clientCredentials/authorizationCode
tags:
- Telecommunications
- Sweden
- Nordics
- Baltics
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- Messaging
- SMS
- SMPP
- IoT
- 5G
- Broadband
- Identity Verification
- BSS
- OSS
- TM Forum
- MEF
- Standards
token_urls:
- https://api-garden.teliacompany.com/v4/oauth/client_credential/accesstoken
- https://api-garden-test.teliacompany.com/v4/oauth/client_credential/accesstoken
- https://tunnistus.telia.fi/uas/oauth2/token
---
