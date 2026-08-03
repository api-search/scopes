---
authorization_urls:
- https://guide.o9solutions.com/oauthserver/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: O9 Solutions Scopes
name_suffix: OAuth Scopes
note: o9 publishes no OpenAPI and no public scopes reference, so these are not derived from a spec or from a documented scope catalog. They are the scopes actually observed on live OAuth authorization requests issued by o9's own first-party clients against guide.o9solutions.com/oauthserver. They cover identity/profile only — no o9 Platform API resource scopes are publicly observable, and the API scope model (if any) sits behind the customer login.
overview: 'o9 Solutions publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the o9 Solutions API on a user''s behalf.


  Tokens are issued from not publicly documented.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: o9 Solutions
provider_slug: o9-solutions
schemes:
- flows:
  - authorizationUrl: https://guide.o9solutions.com/oauthserver/authorize
    flow: authorizationCode
    tokenUrl: not publicly documented
  name: o9 OAuth 2.0
  source: https://guide.o9solutions.com/oauthserver/authorize
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: OpenID Connect authentication — issues an ID token identifying the signed-in o9 user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the signed-in user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Access to the signed-in user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: o9-solutions-scopes
source_filename: o9-solutions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://guide.o9solutions.com/Resources/PlatformWiki\ndocs: null\nnote: >-\n  o9 publishes no OpenAPI and no public scopes reference, so these are not\n  derived from a spec or from a documented scope catalog. They are the scopes\n  actually observed on live OAuth authorization requests issued by o9's own\n  first-party clients against guide.o9solutions.com/oauthserver. They cover\n  identity/profile only — no o9 Platform API resource scopes are publicly\n  observable, and the API scope model (if any) sits behind the customer login.\nschemes:\n- name: o9 OAuth 2.0\n  source: https://guide.o9solutions.com/oauthserver/authorize\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://guide.o9solutions.com/oauthserver/authorize\n    tokenUrl: not publicly documented\nscopes:\n- scope: openid\n  description: OpenID Connect authentication — issues an ID token identifying the\n    signed-in o9 user.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - https://guide.o9solutions.com/Resources/PlatformWiki\n- scope: email\n  description: Access to the signed-in user's email address.\n  flows:\n  - authorizationCode\n  sources:\n  - https://guide.o9solutions.com/Resources/PlatformWiki\n- scope: profile\n  description: Access to the signed-in user's basic profile claims.\n  flows:\n  - authorizationCode\n  sources:\n  - https://guide.o9solutions.com/Resources/PlatformWiki\ncoverage:\n  scopes_observed: 3\n  resource_scopes_public: 0\n  scope_reference_page_published: false\nx-evidence:\n  fetched: '2026-07-31'\n  url: https://guide.o9solutions.com/Resources/PlatformWiki\n  http_status: 200\n  observed_query: client_id=c9fd4e6a-498d-43e9-aedc-3cf50d254308&scope=openid+email+profile&response_type=code\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/o9-solutions/refs/heads/main/scopes/o9-solutions-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Supply Chain
- Supply Chain Planning
- Integrated Business Planning
- Demand Planning
- Enterprise Software
- Artificial Intelligence
- Knowledge Graph
- Decision Intelligence
- Retail Planning
- Revenue Growth Management
- Enterprise Resource Planning
token_urls:
- not publicly documented
---
