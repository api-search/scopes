---
api_specs:
- filename: truora-openapi.yml
  format: yaml
  label: Truora Checks API
  slug: truora-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Validators API
  slug: truora-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Digital Identity API
  slug: truora-digital-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Account API
  slug: truora-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
authorization_urls:
- https://pass.truora.com/authorize
description: ''
docs: https://dev.truora.com/truora-pass/scopes_reference/
flows:
- authorizationCode
- ciba
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Truora Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Truora publishes 14 OAuth 2.0 scopes via the authorizationCode, ciba, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Truora API on a user''s behalf.


  Tokens are issued from https://api.pass.truora.com/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Truora
provider_slug: truora
schemes:
- flows:
  - authorizationUrl: https://pass.truora.com/authorize
    flow: authorizationCode
    tokenUrl: https://api.pass.truora.com/v1/oauth2/token
    userinfoUrl: https://api.pass.truora.com/v1/oauth2/userinfo
  - deviceAuthorizationUrl: https://api.pass.truora.com/v1/oauth2/bc-authorize
    flow: ciba
    tokenUrl: https://api.pass.truora.com/v1/oauth2/token
  - flow: refreshToken
    tokenUrl: https://api.pass.truora.com/v1/oauth2/token
  name: TruoraPassOAuth2
  source: https://dev.truora.com/truora-pass/getting_started/
  type: oauth2
scope_count: 14
scope_names:
- openid
- email
- phone
- profile
- identity
- documents
- age
- address
- background
- biometric
- verification
- contact
- nationality
- document:<COUNTRY>:<TYPE>
scopes:
- description: Enables OpenID Connect base functionality and the stable user identifier.
  flows:
  - authorizationCode
  - ciba
  scope: openid
- description: User's email address and verification state.
  flows:
  - authorizationCode
  - ciba
  scope: email
- description: User's phone number and verification state.
  flows:
  - authorizationCode
  - ciba
  scope: phone
- description: Basic profile — name, gender, birthdate, nationality.
  flows:
  - authorizationCode
  - ciba
  scope: profile
- description: Identity-verification status, document details, and verified name.
  flows:
  - authorizationCode
  - ciba
  scope: identity
- description: All verified documents from the user. Requires binding_message in CIBA.
  flows:
  - authorizationCode
  - ciba
  scope: documents
- description: Age range, verification status, and birthdate.
  flows:
  - authorizationCode
  - ciba
  scope: age
- description: User's address information.
  flows:
  - authorizationCode
  - ciba
  scope: address
- description: Background-check outcome and trust level. Requires binding_message in CIBA.
  flows:
  - authorizationCode
  - ciba
  scope: background
- description: Face-enrollment status, liveness verification, and confidence metrics.
  flows:
  - authorizationCode
  - ciba
  scope: biometric
- description: Overall verification status, methods used, and verification date.
  flows:
  - authorizationCode
  - ciba
  scope: verification
- description: Bundled contact info — email, phone, and communication preference.
  flows:
  - authorizationCode
  - ciba
  scope: contact
- description: User's nationality information.
  flows:
  - authorizationCode
  - ciba
  scope: nationality
- description: Granular scope filtering released documents by country and document type.
  flows:
  - authorizationCode
  - ciba
  scope: document:<COUNTRY>:<TYPE>
slug: truora-scopes
source_filename: truora-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://dev.truora.com/truora-pass/scopes_reference/\ndocs: https://dev.truora.com/truora-pass/scopes_reference/\nnotes: >-\n  OAuth scopes apply to Truora Pass — Truora's OAuth 2.0 / OpenID Connect Identity\n  Provider (developer/dev.truora.com/truora-pass/). Truora Pass lets applications\n  authenticate a user and consume that user's verified-identity data (document,\n  biometric, background, contact claims) via standard OIDC. This is distinct from\n  the core Checks/Validators/Digital-Identity/Account REST APIs, which authenticate\n  with the Truora-API-Key header and have no OAuth scope surface. The Authorization\n  Code, Embedded SDK (web_message), and CIBA (decoupled) flows all request these\n  scopes; the `documents` and `background` scopes require a `binding_message`\n  parameter in CIBA requests.\nschemes:\n  - name: TruoraPassOAuth2\n    type: oauth2\n    source: https://dev.truora.com/truora-pass/getting_started/\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://pass.truora.com/authorize\n        tokenUrl: https://api.pass.truora.com/v1/oauth2/token\n        userinfoUrl: https://api.pass.truora.com/v1/oauth2/userinfo\n      - flow: ciba\n        deviceAuthorizationUrl: https://api.pass.truora.com/v1/oauth2/bc-authorize\n        tokenUrl: https://api.pass.truora.com/v1/oauth2/token\n      - flow: refreshToken\n        tokenUrl: https://api.pass.truora.com/v1/oauth2/token\nscopes:\n  - scope: openid\n    description: Enables OpenID Connect base functionality and the stable user identifier.\n    flows: [authorizationCode, ciba]\n  - scope: email\n    description: User's email address and verification state.\n    flows: [authorizationCode, ciba]\n  - scope: phone\n    description: User's phone number and verification state.\n    flows: [authorizationCode, ciba]\n  - scope: profile\n    description: Basic profile — name, gender, birthdate, nationality.\n    flows: [authorizationCode,\
  \ ciba]\n  - scope: identity\n    description: Identity-verification status, document details, and verified name.\n    flows: [authorizationCode, ciba]\n  - scope: documents\n    description: All verified documents from the user. Requires binding_message in CIBA.\n    flows: [authorizationCode, ciba]\n  - scope: age\n    description: Age range, verification status, and birthdate.\n    flows: [authorizationCode, ciba]\n  - scope: address\n    description: User's address information.\n    flows: [authorizationCode, ciba]\n  - scope: background\n    description: Background-check outcome and trust level. Requires binding_message in CIBA.\n    flows: [authorizationCode, ciba]\n  - scope: biometric\n    description: Face-enrollment status, liveness verification, and confidence metrics.\n    flows: [authorizationCode, ciba]\n  - scope: verification\n    description: Overall verification status, methods used, and verification date.\n    flows: [authorizationCode, ciba]\n  - scope: contact\n  \
  \  description: Bundled contact info — email, phone, and communication preference.\n    flows: [authorizationCode, ciba]\n  - scope: nationality\n    description: User's nationality information.\n    flows: [authorizationCode, ciba]\n  - scope: \"document:<COUNTRY>:<TYPE>\"\n    description: Granular scope filtering released documents by country and document type.\n    flows: [authorizationCode, ciba]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/scopes/truora-scopes.yml
summary_line: 14 scopes · authorizationCode/ciba/refreshToken
tags:
- Identity Verification
- KYC
- Background Checks
- Fraud Prevention
- LatAm
- WhatsApp
token_urls:
- https://api.pass.truora.com/v1/oauth2/token
---
