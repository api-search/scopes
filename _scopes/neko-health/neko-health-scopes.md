---
authorization_urls:
- https://account.nekohealth.com/connect/authorize
description: ''
docs: https://account.nekohealth.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Neko Health Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by the Neko patient-app OIDC provider (Duende IdentityServer). These are consumer/patient authentication scopes, not a third-party API permission surface. Descriptions are standard OIDC meanings; api.backend is Neko's own backend resource scope.
overview: 'Neko Health publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Neko Health API on a user''s behalf.


  Tokens are issued from https://account.nekohealth.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Neko Health
provider_slug: neko-health
schemes:
- flows:
  - authorizationUrl: https://account.nekohealth.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://account.nekohealth.com/connect/token
  name: NekoOIDC
  source: https://account.nekohealth.com/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- profile
- api.backend
- offline_access
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the subject.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the end-user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to Neko's backend resource API used by the patient application.
  flows:
  - authorizationCode
  scope: api.backend
- description: Requests a refresh token for long-lived offline access.
  flows:
  - authorizationCode
  scope: offline_access
slug: neko-health-scopes
source_filename: neko-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://account.nekohealth.com/.well-known/openid-configuration\ndocs: https://account.nekohealth.com/.well-known/oauth-authorization-server\nnote: >-\n  Scopes advertised by the Neko patient-app OIDC provider (Duende IdentityServer).\n  These are consumer/patient authentication scopes, not a third-party API\n  permission surface. Descriptions are standard OIDC meanings; api.backend is\n  Neko's own backend resource scope.\nschemes:\n- name: NekoOIDC\n  source: https://account.nekohealth.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.nekohealth.com/connect/authorize\n    tokenUrl: https://account.nekohealth.com/connect/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token for the subject.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the end-user's basic profile claims.\n  flows: [authorizationCode]\n\
  - scope: api.backend\n  description: Access to Neko's backend resource API used by the patient application.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Requests a refresh token for long-lived offline access.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neko-health/refs/heads/main/scopes/neko-health-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Health
- Healthcare
- Preventive Health
- Medical
- Body Scan
- Diagnostics
- Consumer Health
- OpenID Connect
token_urls:
- https://account.nekohealth.com/connect/token
---
