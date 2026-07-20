---
api_specs:
- filename: hopae-inc-hconnect-openapi-original.json
  format: json
  label: Hopae hConnect API
  slug: hopae-inc-hconnect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopae-inc/refs/heads/main/openapi/hopae-inc-hconnect-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.hopae.com/api-reference/oidc/well-known
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Hopae Inc Scopes
name_suffix: OAuth Scopes
note: The hConnect REST OpenAPI declares only HTTP basic + bearer security schemes (no oauth2 block), but the OIDC OP surface (connect.hopae.com) publishes an OpenID Connect discovery document that declares scopes_supported. These are the OIDC request scopes used in the Authorization Code flow for browser-based sign-in.
overview: 'Hopae, Inc. publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hopae, Inc. API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hopae, Inc.
provider_slug: hopae-inc
schemes:
- authorization_endpoint: https://connect.hopae.com/auth
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  issuer: https://connect.hopae.com
  jwks_uri: https://connect.hopae.com/jwks
  name: OpenID Connect (Hopae Connect OP)
  token_endpoint: https://connect.hopae.com/token
  type: openIdConnect
  userinfo_endpoint: https://connect.hopae.com/userinfo
scope_count: 7
scope_names:
- openid
- hopae
- idv
- profile
- email
- phone
- address
scopes:
- description: Required OIDC scope; requests an ID token for the authenticated subject.
  flows:
  - authorizationCode
  scope: openid
- description: Hopae-specific scope granting access to Hopae Connect verification claims and provenance.
  flows:
  - authorizationCode
  scope: hopae
- description: Identity verification scope; grants the normalized eID verification result and level of assurance.
  flows:
  - authorizationCode
  scope: idv
- description: Standard OIDC profile claims (name, given_name, family_name, birthdate, gender, locale, etc.).
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC email + email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Standard OIDC phone_number + phone_number_verified claims.
  flows:
  - authorizationCode
  scope: phone
- description: Standard OIDC address claim.
  flows:
  - authorizationCode
  scope: address
slug: hopae-inc-scopes
source_filename: hopae-inc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://connect.hopae.com/.well-known/openid-configuration\ndocs: https://docs.hopae.com/api-reference/oidc/well-known\nnote: >-\n  The hConnect REST OpenAPI declares only HTTP basic + bearer security schemes (no\n  oauth2 block), but the OIDC OP surface (connect.hopae.com) publishes an OpenID\n  Connect discovery document that declares scopes_supported. These are the OIDC\n  request scopes used in the Authorization Code flow for browser-based sign-in.\nschemes:\n  - name: OpenID Connect (Hopae Connect OP)\n    type: openIdConnect\n    issuer: https://connect.hopae.com\n    authorization_endpoint: https://connect.hopae.com/auth\n    token_endpoint: https://connect.hopae.com/token\n    userinfo_endpoint: https://connect.hopae.com/userinfo\n    jwks_uri: https://connect.hopae.com/jwks\n    grant_types: [authorization_code, implicit, refresh_token]\nscopes:\n  - scope: openid\n    description: Required OIDC scope; requests an\
  \ ID token for the authenticated subject.\n    flows: [authorizationCode]\n  - scope: hopae\n    description: Hopae-specific scope granting access to Hopae Connect verification claims and provenance.\n    flows: [authorizationCode]\n  - scope: idv\n    description: Identity verification scope; grants the normalized eID verification result and level of assurance.\n    flows: [authorizationCode]\n  - scope: profile\n    description: Standard OIDC profile claims (name, given_name, family_name, birthdate, gender, locale, etc.).\n    flows: [authorizationCode]\n  - scope: email\n    description: Standard OIDC email + email_verified claims.\n    flows: [authorizationCode]\n  - scope: phone\n    description: Standard OIDC phone_number + phone_number_verified claims.\n    flows: [authorizationCode]\n  - scope: address\n    description: Standard OIDC address claim.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopae-inc/refs/heads/main/scopes/hopae-inc-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Identity
- Identity Verification
- Digital Identity
- eID
- Verifiable Credentials
- Authentication
- OpenID Connect
- eIDAS
- KYC
token_urls: []
---
