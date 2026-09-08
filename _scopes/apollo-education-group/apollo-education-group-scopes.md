---
authorization_urls:
- https://login.phoenix.edu:443/am/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Apollo Education Group Scopes
name_suffix: OAuth Scopes
note: 'Apollo Education Group / University of Phoenix publishes no scopes or permissions reference page — there is no developer program to publish one for. This catalogue is taken verbatim from the `scopes_supported` array of the University of Phoenix single sign-on OIDC discovery document (ForgeRock Access Management, realm /alpha), fetched anonymously HTTP 200 on 2026-09-04. These scopes govern institutional sign-on to MyPhoenix / eCampus. They are not scopes a third-party integrator can request: no public client registration path is documented.'
overview: 'Apollo Education Group publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apollo Education Group API on a user''s behalf.


  Tokens are issued from https://login.phoenix.edu:443/am/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apollo Education Group
provider_slug: apollo-education-group
schemes:
- flows:
  - authorizationUrl: https://login.phoenix.edu:443/am/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.phoenix.edu:443/am/oauth2/access_token
  issuer: https://login.phoenix.edu:443/am/oauth2
  name: PhoenixSSO
  source: well-known/apollo-education-group-openid-configuration.json
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- fr:idm:*
- am-introspect-all-tokens
scopes:
- description: Standard OpenID Connect scope — requests an ID token for the signed-in University of Phoenix user.
  flows: []
  scope: openid
- description: Standard OIDC claim set — name and profile claims for the signed-in user.
  flows: []
  scope: profile
- description: Standard OIDC email claim.
  flows: []
  scope: email
- description: Standard OIDC address claim.
  flows: []
  scope: address
- description: Standard OIDC phone-number claim.
  flows: []
  scope: phone
- description: ForgeRock Identity Management product scope — grants access to the IDM REST surface behind the platform. Vendor-defined, not an OIDC standard scope.
  flows: []
  scope: fr:idm:*
- description: ForgeRock Access Management product scope — allows a client to introspect tokens issued to other clients in the realm. Vendor-defined, administrative.
  flows: []
  scope: am-introspect-all-tokens
slug: apollo-education-group-scopes
source_filename: apollo-education-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://login.phoenix.edu/.well-known/openid-configuration\ndocs: null\nnote: |\n  Apollo Education Group / University of Phoenix publishes no scopes or permissions reference\n  page — there is no developer program to publish one for. This catalogue is taken verbatim from\n  the `scopes_supported` array of the University of Phoenix single sign-on OIDC discovery\n  document (ForgeRock Access Management, realm /alpha), fetched anonymously HTTP 200 on\n  2026-09-04.\n\n  These scopes govern institutional sign-on to MyPhoenix / eCampus. They are not scopes a\n  third-party integrator can request: no public client registration path is documented.\nschemes:\n  - name: PhoenixSSO\n    source: well-known/apollo-education-group-openid-configuration.json\n    issuer: https://login.phoenix.edu:443/am/oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.phoenix.edu:443/am/oauth2/authorize\n       \
  \ tokenUrl: https://login.phoenix.edu:443/am/oauth2/access_token\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope — requests an ID token for the signed-in\n      University of Phoenix user.\n    standard: OIDC Core 1.0\n    sources: [well-known/apollo-education-group-openid-configuration.json]\n  - scope: profile\n    description: Standard OIDC claim set — name and profile claims for the signed-in user.\n    standard: OIDC Core 1.0\n    sources: [well-known/apollo-education-group-openid-configuration.json]\n  - scope: email\n    description: Standard OIDC email claim.\n    standard: OIDC Core 1.0\n    sources: [well-known/apollo-education-group-openid-configuration.json]\n  - scope: address\n    description: Standard OIDC address claim.\n    standard: OIDC Core 1.0\n    sources: [well-known/apollo-education-group-openid-configuration.json]\n  - scope: phone\n    description: Standard OIDC phone-number claim.\n    standard: OIDC Core 1.0\n    sources: [well-known/apollo-education-group-openid-configuration.json]\n\
  \  - scope: fr:idm:*\n    description: ForgeRock Identity Management product scope — grants access to the IDM REST\n      surface behind the platform. Vendor-defined, not an OIDC standard scope.\n    standard: null\n    vendor: ForgeRock (Ping Identity)\n    sources: [well-known/apollo-education-group-openid-configuration.json]\n  - scope: am-introspect-all-tokens\n    description: ForgeRock Access Management product scope — allows a client to introspect\n      tokens issued to other clients in the realm. Vendor-defined, administrative.\n    standard: null\n    vendor: ForgeRock (Ping Identity)\n    sources: [well-known/apollo-education-group-openid-configuration.json]\ncoverage:\n  scope_count: 7\n  standard_oidc: 5\n  vendor_defined: 2\n  note: >-\n    The two vendor scopes are ForgeRock platform defaults, present on every AM deployment. They\n    are recorded because they are what the server advertises, not because University of Phoenix\n    documents them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-education-group/refs/heads/main/scopes/apollo-education-group-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Education
- Higher Education
- Online Education
- Private Education
- University
token_urls:
- https://login.phoenix.edu:443/am/oauth2/access_token
---
