---
authorization_urls:
- https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Elephas Biosciences Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Elephas Biosciences publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Elephas Biosciences API on a user''s behalf.


  Tokens are issued from https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elephas Biosciences
provider_slug: elephas-biosciences
schemes:
- flows:
  - authorizationUrl: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/token
  name: AzureAdB2C
  source: well-known/elephas-biosciences-openid-configuration.json
  type: openIdConnect
scope_count: 2
scope_names:
- openid
- https://elephasus.onmicrosoft.com/prod/api/User.Read
scopes:
- description: Standard OpenID Connect scope; the only value advertised in scopes_supported by the B2C discovery document.
  flows:
  - authorizationCode
  scope: openid
- description: Resource scope the Elephas Portal requests for the production backend API. The application id URI (elephasus.onmicrosoft.com/prod/api) names the Elephas Portal API resource; User.Read is the delegated permission the browser client asks for on the signed-in user's behalf.
  flows:
  - authorizationCode
  scope: https://elephasus.onmicrosoft.com/prod/api/User.Read
slug: elephas-biosciences-scopes
source_filename: elephas-biosciences-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: 'https://portal.elephas.com/assets/config/config.json (Scope value requested\n  by the Elephas Portal SPA) + well-known/elephas-biosciences-openid-configuration.json'\ndocs: null\ndocs_note: Elephas publishes no scopes or permissions reference. Both scopes below\n  were observed, not documented.\nschemes:\n- name: AzureAdB2C\n  type: openIdConnect\n  source: well-known/elephas-biosciences-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/authorize\n    tokenUrl: https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; the only value advertised in\n    scopes_supported by the B2C discovery document.\n  flows: [authorizationCode]\n  sources: [well-known/elephas-biosciences-openid-configuration.json]\n\
  - scope: https://elephasus.onmicrosoft.com/prod/api/User.Read\n  description: 'Resource scope the Elephas Portal requests for the production\n    backend API. The application id URI (elephasus.onmicrosoft.com/prod/api) names\n    the Elephas Portal API resource; User.Read is the delegated permission the\n    browser client asks for on the signed-in user''s behalf.'\n  resource: elephasus.onmicrosoft.com/prod/api\n  flows: [authorizationCode]\n  sources: [https://portal.elephas.com/assets/config/config.json]\nscope_count: 2\ncoverage_note: 'This is the complete OBSERVABLE scope surface, not necessarily the\n  complete one. Azure AD B2C does not advertise resource scopes in discovery, so any\n  additional delegated or application permissions the API defines are only visible\n  to an authenticated tenant administrator. A single User.Read-style delegated scope\n  fronting an entire clinical reporting API suggests authorization is enforced\n  server-side by role rather than by OAuth scope.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elephas-biosciences/refs/heads/main/scopes/elephas-biosciences-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Healthcare
- Life Sciences
- Biotechnology
- Precision Oncology
- Diagnostics
- Immunotherapy
- Clinical Research
- Laboratory
- Medical Devices
token_urls:
- https://na.login.elephas.com/bf865bf1-740f-49ec-922c-9b2c233faa13/b2c_1a_smart_hrd_susi/oauth2/v2.0/token
---
