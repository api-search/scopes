---
api_specs:
- filename: microsoft-azure-networking-openapi.yml
  format: yaml
  label: Azure Virtual Networks API
  slug: azure-virtual-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/openapi/microsoft-azure-networking-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Networking Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Networking publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Networking API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Networking
provider_slug: microsoft-azure-networking
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: OAuth2Auth
  source: openapi/azure-networking-load-balancer-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: OAuth2Auth
  source: openapi/azure-networking-virtual-networks-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-networking-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Access Azure Load Balancer API
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-networking-scopes
source_filename: microsoft-azure-networking-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-networking-load-balancer-openapi.yml, openapi/azure-networking-virtual-networks-openapi.yml,\n  openapi/microsoft-azure-networking-openapi.yml\nschemes:\n- name: OAuth2Auth\n  source: openapi/azure-networking-load-balancer-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: OAuth2Auth\n  source: openapi/azure-networking-virtual-networks-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-networking-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n\
  \  description: Access Azure Load Balancer API\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-networking-load-balancer-openapi.yml\n  - openapi/azure-networking-virtual-networks-openapi.yml\n  - openapi/microsoft-azure-networking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/scopes/microsoft-azure-networking-scopes.yml
summary_line: 1 scope · implicit
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
token_urls: []
---
