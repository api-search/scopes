---
authorization_urls:
- https://hydra.gridpoint.com:443/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Gridpoint Scopes
name_suffix: OAuth Scopes
note: GridPoint publishes no scopes or permissions reference page and no OpenAPI with oauth2 securitySchemes, so nothing could be derived from a contract. Every scope below is taken verbatim from scopes_supported in the anonymous OIDC discovery document GridPoint's own ORY Hydra authorization server serves. Unusually, GridPoint models authorization as ROLE_* scopes rather than resource verbs (read:sites / write:devices), so the list reveals the tenancy model — GridPoint staff, customer, partner, and machine roles — but not which API resources each role can reach. Descriptions below restate the role name and the audience it names; they are NOT quoted from GridPoint documentation, because none exists. No scope-to-operation mapping is publicly determinable.
overview: 'GridPoint publishes 16 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the GridPoint API on a user''s behalf.


  Tokens are issued from https://hydra.gridpoint.com:443/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GridPoint
provider_slug: gridpoint
schemes:
- flows:
  - authorizationUrl: https://hydra.gridpoint.com:443/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://hydra.gridpoint.com:443/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://hydra.gridpoint.com:443/oauth2/token
  - authorizationUrl: https://hydra.gridpoint.com:443/oauth2/auth
    flow: implicit
  issuer: https://hydra.gridpoint.com:443/
  name: gridpoint-oidc
  source: well-known/gridpoint-openid-configuration.json
scope_count: 16
scope_names:
- openid
- offline_access
- offline
- id_token
- ROLE_GP_ADMIN
- ROLE_GP_SUPPORT
- ROLE_GP_ANALYST
- ROLE_GP_SALES
- ROLE_CUSTOMER_ANALYST
- ROLE_CUSTOMER_SITE_MANAGER
- ROLE_PARTNER_COMMISSIONER
- ROLE_PARTNER_SUPPORT
- ROLE_PARTNER_SUPPORT_ADMIN
- ROLE_PROVISIONER
- ROLE_SYSTEM
- ROLE_OIDC_USER
scopes:
- description: Issue an OIDC ID token for the authenticated end user.
  flows: []
  scope: openid
- description: Issue a refresh token so the client can renew access without re-prompting.
  flows: []
  scope: offline_access
- description: ORY Hydra legacy alias for offline_access.
  flows: []
  scope: offline
- description: Request an ID token in the authorization response.
  flows: []
  scope: id_token
- description: GridPoint administrator role.
  flows: []
  scope: ROLE_GP_ADMIN
- description: GridPoint support role.
  flows: []
  scope: ROLE_GP_SUPPORT
- description: GridPoint analyst role.
  flows: []
  scope: ROLE_GP_ANALYST
- description: GridPoint sales role.
  flows: []
  scope: ROLE_GP_SALES
- description: Customer-side analyst role.
  flows: []
  scope: ROLE_CUSTOMER_ANALYST
- description: Customer-side site manager role.
  flows: []
  scope: ROLE_CUSTOMER_SITE_MANAGER
- description: Partner commissioning role (field installation / device commissioning).
  flows: []
  scope: ROLE_PARTNER_COMMISSIONER
- description: Partner support role.
  flows: []
  scope: ROLE_PARTNER_SUPPORT
- description: Partner support administrator role.
  flows: []
  scope: ROLE_PARTNER_SUPPORT_ADMIN
- description: Provisioning role.
  flows: []
  scope: ROLE_PROVISIONER
- description: System / service-to-service role.
  flows: []
  scope: ROLE_SYSTEM
- description: Baseline authenticated OIDC user role.
  flows: []
  scope: ROLE_OIDC_USER
slug: gridpoint-scopes
source_filename: gridpoint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://hydra.gridpoint.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  GridPoint publishes no scopes or permissions reference page and no OpenAPI\n  with oauth2 securitySchemes, so nothing could be derived from a contract.\n  Every scope below is taken verbatim from scopes_supported in the anonymous\n  OIDC discovery document GridPoint's own ORY Hydra authorization server serves.\n  Unusually, GridPoint models authorization as ROLE_* scopes rather than\n  resource verbs (read:sites / write:devices), so the list reveals the tenancy\n  model — GridPoint staff, customer, partner, and machine roles — but not which\n  API resources each role can reach. Descriptions below restate the role name\n  and the audience it names; they are NOT quoted from GridPoint documentation,\n  because none exists. No scope-to-operation mapping is publicly determinable.\nschemes:\n  - name: gridpoint-oidc\n    source: well-known/gridpoint-openid-configuration.json\n\
  \    issuer: https://hydra.gridpoint.com:443/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://hydra.gridpoint.com:443/oauth2/auth\n        tokenUrl: https://hydra.gridpoint.com:443/oauth2/token\n      - flow: clientCredentials\n        tokenUrl: https://hydra.gridpoint.com:443/oauth2/token\n      - flow: implicit\n        authorizationUrl: https://hydra.gridpoint.com:443/oauth2/auth\nscope_count: 16\nscopes:\n  - scope: openid\n    kind: oidc-standard\n    description: Issue an OIDC ID token for the authenticated end user.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: offline_access\n    kind: oidc-standard\n    description: Issue a refresh token so the client can renew access without re-prompting.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: offline\n    kind: oidc-standard\n    description: ORY Hydra legacy alias for offline_access.\n    sources: [well-known/gridpoint-openid-configuration.json]\n\
  \  - scope: id_token\n    kind: oidc-standard\n    description: Request an ID token in the authorization response.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_GP_ADMIN\n    kind: gridpoint-role\n    audience: gridpoint-staff\n    description: GridPoint administrator role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_GP_SUPPORT\n    kind: gridpoint-role\n    audience: gridpoint-staff\n    description: GridPoint support role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_GP_ANALYST\n    kind: gridpoint-role\n    audience: gridpoint-staff\n    description: GridPoint analyst role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_GP_SALES\n    kind: gridpoint-role\n    audience: gridpoint-staff\n    description: GridPoint sales role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_CUSTOMER_ANALYST\n    kind: gridpoint-role\n\
  \    audience: customer\n    description: Customer-side analyst role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_CUSTOMER_SITE_MANAGER\n    kind: gridpoint-role\n    audience: customer\n    description: Customer-side site manager role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_PARTNER_COMMISSIONER\n    kind: gridpoint-role\n    audience: partner\n    description: Partner commissioning role (field installation / device commissioning).\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_PARTNER_SUPPORT\n    kind: gridpoint-role\n    audience: partner\n    description: Partner support role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_PARTNER_SUPPORT_ADMIN\n    kind: gridpoint-role\n    audience: partner\n    description: Partner support administrator role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_PROVISIONER\n   \
  \ kind: gridpoint-role\n    audience: machine\n    description: Provisioning role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_SYSTEM\n    kind: gridpoint-role\n    audience: machine\n    description: System / service-to-service role.\n    sources: [well-known/gridpoint-openid-configuration.json]\n  - scope: ROLE_OIDC_USER\n    kind: gridpoint-role\n    audience: end-user\n    description: Baseline authenticated OIDC user role.\n    sources: [well-known/gridpoint-openid-configuration.json]\ngaps:\n  - No published scope reference; no scope is bound to a documented operation.\n  - Scopes are coarse roles, not resource permissions, so least-privilege delegation\n    to an agent or an integrator is not expressible with the published vocabulary.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridpoint/refs/heads/main/scopes/gridpoint-scopes.yml
summary_line: 16 scopes · authorizationCode/clientCredentials/implicit
tags:
- Company
- Energy
- Energy Management
- Buildings
- Building Automation
- Sustainability
- Internet of Things
- Demand Response
- Facilities
- Analytics
token_urls:
- https://hydra.gridpoint.com:443/oauth2/token
---
