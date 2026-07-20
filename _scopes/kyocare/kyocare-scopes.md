---
authorization_urls:
- https://api.attain.kyocare.com/oauth/authorize
description: ''
docs: https://api.attain.kyocare.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Kyocare Scopes
name_suffix: OAuth Scopes
note: Scopes read verbatim from the published `scopes_supported` of the Attain platform API discovery document. Kyo publishes no scope/permission reference page, so this is the complete advertised scope surface — standard OIDC identity scopes only, with no resource-level scopes exposed publicly.
overview: 'Kyo publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kyo API on a user''s behalf.


  Tokens are issued from https://api.attain.kyocare.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kyo
provider_slug: kyocare
schemes:
- flows:
  - authorizationUrl: https://api.attain.kyocare.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.attain.kyocare.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.attain.kyocare.com/oauth/token
  name: oauth2
  source: well-known/kyocare-openid-configuration.json
scope_count: 2
scope_names:
- openid
- email
scopes:
- description: Standard OpenID Connect scope; requests an ID token asserting the end user's identity.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the end user's email address and email_verified claim to the client.
  flows:
  - authorizationCode
  scope: email
slug: kyocare-scopes
source_filename: kyocare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.attain.kyocare.com/.well-known/openid-configuration\ndocs: https://api.attain.kyocare.com/.well-known/oauth-authorization-server\nnote: Scopes read verbatim from the published `scopes_supported` of the Attain platform\n  API discovery document. Kyo publishes no scope/permission reference page, so this is\n  the complete advertised scope surface — standard OIDC identity scopes only, with no\n  resource-level scopes exposed publicly.\nschemes:\n- name: oauth2\n  source: well-known/kyocare-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.attain.kyocare.com/oauth/authorize\n    tokenUrl: https://api.attain.kyocare.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.attain.kyocare.com/oauth/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token asserting the end\n    user's identity.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - well-known/kyocare-openid-configuration.json\n- scope: email\n  description: Releases the end user's email address and email_verified claim to the\n    client.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/kyocare-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyocare/refs/heads/main/scopes/kyocare-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Company
- Healthcare
- Autism
- ABA Therapy
- Behavioral Health
- Patient Engagement
- Digital Health
- Scheduling
- Private API
token_urls:
- https://api.attain.kyocare.com/oauth/token
---
