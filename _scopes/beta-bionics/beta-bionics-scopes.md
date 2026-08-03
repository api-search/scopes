---
authorization_urls:
- https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Beta Bionics Scopes
name_suffix: OAuth Scopes
note: Beta Bionics publishes no scope or permission reference — there is no developer program. The only scopes observable are the four standard OIDC scopes advertised by the Amazon Cognito user pool that fronts the Bionic Portal and the iLet / Bionic Circle mobile apps. No custom resource-server scopes are advertised anonymously; any that exist would require authenticated introspection of the Cognito user pool, which is not public.
overview: 'Beta Bionics publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beta Bionics API on a user''s behalf.


  Tokens are issued from https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beta Bionics
provider_slug: beta-bionics
schemes:
- flows:
  - authorizationUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/token
  name: CognitoHostedUI
  source: well-known/beta-bionics-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- phone
- profile
scopes:
- description: OpenID Connect authentication; issues an ID token identifying the user.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Access to the user's email address and email_verified claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Access to the user's phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  - implicit
  scope: profile
slug: beta-bionics-scopes
source_filename: beta-bionics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_HNbbVuwO8/.well-known/openid-configuration\nnote: >-\n  Beta Bionics publishes no scope or permission reference — there is no developer\n  program. The only scopes observable are the four standard OIDC scopes advertised\n  by the Amazon Cognito user pool that fronts the Bionic Portal and the iLet /\n  Bionic Circle mobile apps. No custom resource-server scopes are advertised\n  anonymously; any that exist would require authenticated introspection of the\n  Cognito user pool, which is not public.\nschemes:\n- name: CognitoHostedUI\n  source: well-known/beta-bionics-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication;\
  \ issues an ID token identifying the user.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/beta-bionics-openid-configuration.json]\n- scope: email\n  description: Access to the user's email address and email_verified claim.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/beta-bionics-openid-configuration.json]\n- scope: phone\n  description: Access to the user's phone_number and phone_number_verified claims.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/beta-bionics-openid-configuration.json]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/beta-bionics-openid-configuration.json]\ncustom_scopes: []\ndocs: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beta-bionics/refs/heads/main/scopes/beta-bionics-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Health
- Healthcare
- Medical Devices
- Diabetes
- Automated Insulin Delivery
- Digital Health
- Remote Patient Monitoring
- HIPAA
- Connected Devices
token_urls:
- https://us-east-2hnbbvuwo8.auth.us-east-2.amazoncognito.com/oauth2/token
---
