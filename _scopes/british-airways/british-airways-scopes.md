---
authorization_urls:
- https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/authorize
description: The only OAuth 2.0 / OpenID Connect scope surface British Airways exposes publicly. These scopes belong to the Microsoft Entra External ID (CIAM) tenant that authenticates developers and partners into the NDC Communication Hub at ndc.ba.com — they govern who can read the NDC documentation and use the in-browser sandbox screens, not what an integration may do against the NDC message API. British Airways publishes no scope model for the NDC API itself; API authorisation is carried by a certification-gated client-key and a signed Live API Contract, not by scopes. See authentication/british-airways-authentication.yml.
docs: ''
flows:
- authorizationCode
- implicit
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: British Airways Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'British Airways publishes 4 OAuth 2.0 scopes via the authorizationCode, implicit, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the British Airways API on a user''s behalf.


  Tokens are issued from https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: British Airways
provider_slug: british-airways
schemes:
- flows:
  - authorizationUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token
  - authorizationUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/authorize
    flow: implicit
    note: id_token and id_token token response types are advertised as supported
  - deviceAuthorizationUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/devicecode
    flow: deviceCode
    tokenUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token
  issuer: https://45c0456f-2aef-40f6-847e-d3d957348527.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/v2.0
  name: EntraExternalID
  provider: Microsoft Entra External ID (CIAM)
  source: well-known/british-airways-openid-configuration.json
  tenant_id: 45c0456f-2aef-40f6-847e-d3d957348527
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Request an ID token — authenticate the developer/partner user against the British Airways Entra External ID tenant.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  scope: openid
- description: Release basic profile claims (name, preferred_username) into the ID token.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  scope: profile
- description: Release the email claim into the ID token.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  scope: email
- description: Issue a refresh token so the hub session can be renewed without re-prompting.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: british-airways-scopes
source_filename: british-airways-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/v2.0/.well-known/openid-configuration\n  (fetched 2026-07-28, HTTP 200)\ndescription: >-\n  The only OAuth 2.0 / OpenID Connect scope surface British Airways exposes publicly. These\n  scopes belong to the Microsoft Entra External ID (CIAM) tenant that authenticates developers\n  and partners into the NDC Communication Hub at ndc.ba.com — they govern who can read the NDC\n  documentation and use the in-browser sandbox screens, not what an integration may do against\n  the NDC message API. British Airways publishes no scope model for the NDC API itself; API\n  authorisation is carried by a certification-gated client-key and a signed Live API Contract,\n  not by scopes. See authentication/british-airways-authentication.yml.\nscope_of_this_document: developer-portal-login\ncovers_api_authorization: false\nschemes:\n  - name: EntraExternalID\n    type:\
  \ openIdConnect\n    provider: Microsoft Entra External ID (CIAM)\n    tenant_id: 45c0456f-2aef-40f6-847e-d3d957348527\n    issuer: https://45c0456f-2aef-40f6-847e-d3d957348527.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/v2.0\n    source: well-known/british-airways-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/authorize\n        tokenUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token\n      - flow: implicit\n        authorizationUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/authorize\n        note: id_token and id_token token response types are advertised as supported\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/devicecode\n        tokenUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token\n\
  scopes:\n  - scope: openid\n    description: >-\n      Request an ID token — authenticate the developer/partner user against the British Airways\n      Entra External ID tenant.\n    flows: [authorizationCode, implicit, deviceCode]\n    sources: [well-known/british-airways-openid-configuration.json]\n  - scope: profile\n    description: Release basic profile claims (name, preferred_username) into the ID token.\n    flows: [authorizationCode, implicit, deviceCode]\n    sources: [well-known/british-airways-openid-configuration.json]\n  - scope: email\n    description: Release the email claim into the ID token.\n    flows: [authorizationCode, implicit, deviceCode]\n    sources: [well-known/british-airways-openid-configuration.json]\n  - scope: offline_access\n    description: Issue a refresh token so the hub session can be renewed without re-prompting.\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/british-airways-openid-configuration.json]\nclaims_supported:\n  - sub\n\
  \  - iss\n  - aud\n  - exp\n  - iat\n  - auth_time\n  - acr\n  - nonce\n  - preferred_username\n  - name\n  - email\n  - tid\n  - ver\n  - at_hash\n  - c_hash\nnotes:\n  - >-\n    scopes_supported contains only the four standard OIDC scopes. No British Airways\n    application-specific scope (no api://... resource scope, no NDC-specific permission) is\n    advertised anonymously; any such scope would live on a protected resource registration\n    that is not publicly discoverable.\n  - >-\n    tls_client_certificate_bound_access_tokens is true and an mTLS token endpoint alias is\n    published (mtlsauth.microsoft.com), so certificate-bound tokens (RFC 8705) are available\n    on this tenant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/british-airways/refs/heads/main/scopes/british-airways-scopes.yml
summary_line: 4 scopes · authorizationCode/implicit/deviceCode
tags:
- Travel
- United Kingdom
- Aviation
- Airline
- Distribution
- NDC
- Booking
- Corporate Travel
- Airports
token_urls:
- https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token
---
