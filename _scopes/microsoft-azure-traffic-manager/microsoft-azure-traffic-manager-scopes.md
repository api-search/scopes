---
api_specs:
- filename: microsoft-azure-traffic-manager-endpoints-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Endpoints API
  slug: microsoft-azure-traffic-manager-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-endpoints-api-openapi.yml
- filename: microsoft-azure-traffic-manager-geographichierarchies-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager GeographicHierarchies API
  slug: microsoft-azure-traffic-manager-geographichierarchies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-geographichierarchies-api-openapi.yml
- filename: microsoft-azure-traffic-manager-heatmap-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager HeatMap API
  slug: microsoft-azure-traffic-manager-heatmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-heatmap-api-openapi.yml
- filename: microsoft-azure-traffic-manager-profiles-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Profiles API
  slug: microsoft-azure-traffic-manager-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-profiles-api-openapi.yml
- filename: microsoft-azure-traffic-manager-usermetrics-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager UserMetrics API
  slug: microsoft-azure-traffic-manager-usermetrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/openapi/microsoft-azure-traffic-manager-usermetrics-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Traffic Manager Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Traffic Manager publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Traffic Manager API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Traffic Manager
provider_slug: microsoft-azure-traffic-manager
schemes:
- description: Azure Active Directory OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-traffic-manager-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-traffic-manager-scopes
source_filename: microsoft-azure-traffic-manager-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-traffic-manager-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-traffic-manager-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth 2.0\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-traffic-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-traffic-manager/refs/heads/main/scopes/microsoft-azure-traffic-manager-scopes.yml
summary_line: 1 scope · implicit
tags:
- DNS Load Balancing
- Failover
- Global Routing
- Networking
- Traffic Distribution
- Traffic Manager
token_urls: []
---
