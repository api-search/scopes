---
api_specs:
- filename: newforma-konekt-openapi-original.json
  format: json
  label: Newforma Konekt REST API
  slug: newforma-konekt-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newforma/refs/heads/main/openapi/newforma-konekt-openapi-original.json
authorization_urls:
- https://auth.bimtrackapp.co/connect/authorize
description: ''
docs: https://konekt.help.newforma.com/4408494681869-integrations-api/360008491831-api/360060182352-using-oauth-2-0/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Newforma Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Newforma publishes 14 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Newforma API on a user''s behalf.


  Tokens are issued from https://auth.bimtrackapp.co/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Newforma
provider_slug: newforma
schemes:
- flows:
  - authorizationUrl: https://auth.bimtrackapp.co/connect/authorize
    flow: authorizationCode
    tokenUrl: https://auth.bimtrackapp.co/connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.bimtrackapp.co/connect/token
  name: OAuth2
  source: https://auth.bimtrackapp.co/.well-known/openid-configuration
scope_count: 14
scope_names:
- openid
- profile
- email
- offline_access
- BIMTrack_Api
- BIMTrackEvent_Api
- BcfWebApi
- BIMTrackOrganizations_Api
- IdentityServerApi
- IdentityServer.HealthCheck
- BIMTrack_Website
- FileManagement_Api
- DocumentControl_Api
- PIMTrack_Api
scopes:
- description: OpenID Connect authentication (required for OIDC verification).
  flows: []
  scope: openid
- description: Access to the user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the user's email claim.
  flows: []
  scope: email
- description: Issue refresh tokens for long-lived access.
  flows: []
  scope: offline_access
- description: Access to the Newforma Konekt (BIM Track) REST API.
  flows: []
  scope: BIMTrack_Api
- description: Access to the Konekt events API surface.
  flows: []
  scope: BIMTrackEvent_Api
- description: Access to the BCF (BIM Collaboration Format) REST API.
  flows: []
  scope: BcfWebApi
- description: Access to organization-level Konekt resources.
  flows: []
  scope: BIMTrackOrganizations_Api
- description: Access to the IdentityServer administrative API.
  flows: []
  scope: IdentityServerApi
- description: IdentityServer health-check scope.
  flows: []
  scope: IdentityServer.HealthCheck
- description: Access to the Konekt web application surface.
  flows: []
  scope: BIMTrack_Website
- description: Access to the file-management API surface (documented in the OAuth 2.0 guide).
  flows: []
  scope: FileManagement_Api
- description: Access to the document-control API surface (documented in the OAuth 2.0 guide).
  flows: []
  scope: DocumentControl_Api
- description: Access to the PIM Track / project information management API surface (documented in the OAuth 2.0 guide).
  flows: []
  scope: PIMTrack_Api
slug: newforma-scopes
source_filename: newforma-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://auth.bimtrackapp.co/.well-known/openid-configuration\ndocs: https://konekt.help.newforma.com/4408494681869-integrations-api/360008491831-api/360060182352-using-oauth-2-0/\nschemes:\n- name: OAuth2\n  source: https://auth.bimtrackapp.co/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.bimtrackapp.co/connect/authorize\n    tokenUrl: https://auth.bimtrackapp.co/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.bimtrackapp.co/connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (required for OIDC verification).\n  sources: [oidc-discovery, docs]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  sources: [oidc-discovery]\n- scope: email\n  description: Access to the user's email claim.\n  sources: [oidc-discovery]\n- scope: offline_access\n  description: Issue refresh tokens for long-lived\
  \ access.\n  sources: [oidc-discovery, docs]\n- scope: BIMTrack_Api\n  description: Access to the Newforma Konekt (BIM Track) REST API.\n  sources: [oidc-discovery, docs]\n- scope: BIMTrackEvent_Api\n  description: Access to the Konekt events API surface.\n  sources: [oidc-discovery]\n- scope: BcfWebApi\n  description: Access to the BCF (BIM Collaboration Format) REST API.\n  sources: [oidc-discovery, docs]\n- scope: BIMTrackOrganizations_Api\n  description: Access to organization-level Konekt resources.\n  sources: [oidc-discovery]\n- scope: IdentityServerApi\n  description: Access to the IdentityServer administrative API.\n  sources: [oidc-discovery]\n- scope: IdentityServer.HealthCheck\n  description: IdentityServer health-check scope.\n  sources: [oidc-discovery]\n- scope: BIMTrack_Website\n  description: Access to the Konekt web application surface.\n  sources: [oidc-discovery]\n- scope: FileManagement_Api\n  description: Access to the file-management API surface (documented in the\
  \ OAuth 2.0 guide).\n  sources: [docs]\n- scope: DocumentControl_Api\n  description: Access to the document-control API surface (documented in the OAuth 2.0 guide).\n  sources: [docs]\n- scope: PIMTrack_Api\n  description: Access to the PIM Track / project information management API surface (documented in the OAuth 2.0 guide).\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newforma/refs/heads/main/scopes/newforma-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials
tags:
- Company
- AEC
- Construction
- Architecture
- Engineering
- BIM
- Building Information Modeling
- Project Management
- Issue Tracking
- Collaboration
token_urls:
- https://auth.bimtrackapp.co/connect/token
---
