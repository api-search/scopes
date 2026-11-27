---
api_specs:
- filename: microsoft-azure-arc-machines-api-openapi.yml
  format: yaml
  label: Azure Arc Machines API
  slug: microsoft-azure-arc-machines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machines-api-openapi.yml
- filename: microsoft-azure-arc-connectedclusters-api-openapi.yml
  format: yaml
  label: Azure Arc Connected Clusters API
  slug: microsoft-azure-arc-connectedclusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-connectedclusters-api-openapi.yml
- filename: microsoft-azure-arc-extensions-api-openapi.yml
  format: yaml
  label: Azure Arc Extensions API
  slug: microsoft-azure-arc-extensions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-extensions-api-openapi.yml
- filename: microsoft-azure-arc-gateways-api-openapi.yml
  format: yaml
  label: Azure Arc Gateways API
  slug: microsoft-azure-arc-gateways-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-gateways-api-openapi.yml
- filename: microsoft-azure-arc-licenseprofiles-api-openapi.yml
  format: yaml
  label: Azure Arc License Profiles API
  slug: microsoft-azure-arc-licenseprofiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-licenseprofiles-api-openapi.yml
- filename: microsoft-azure-arc-licenses-api-openapi.yml
  format: yaml
  label: Azure Arc Licenses API
  slug: microsoft-azure-arc-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-licenses-api-openapi.yml
- filename: microsoft-azure-arc-machineextensions-api-openapi.yml
  format: yaml
  label: Azure Arc Machine Extensions API
  slug: microsoft-azure-arc-machineextensions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machineextensions-api-openapi.yml
- filename: microsoft-azure-arc-machineextensions-setup-api-openapi.yml
  format: yaml
  label: Azure Arc MachineExtensions Setup API
  slug: microsoft-azure-arc-machineextensions-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machineextensions-setup-api-openapi.yml
- filename: microsoft-azure-arc-machineextensions-upgrade-api-openapi.yml
  format: yaml
  label: Azure Arc MachineExtensions Upgrade API
  slug: microsoft-azure-arc-machineextensions-upgrade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machineextensions-upgrade-api-openapi.yml
- filename: microsoft-azure-arc-machinenetworkprofile-api-openapi.yml
  format: yaml
  label: Azure Arc Machine Network Profile API
  slug: microsoft-azure-arc-machinenetworkprofile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machinenetworkprofile-api-openapi.yml
- filename: microsoft-azure-arc-machineruncommands-api-openapi.yml
  format: yaml
  label: Azure Arc Machine Run Commands API
  slug: microsoft-azure-arc-machineruncommands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machineruncommands-api-openapi.yml
- filename: microsoft-azure-arc-networksecurityperimeterconfiguration-api-openapi.yml
  format: yaml
  label: Azure Arc Network Security Perimeter Configuration API
  slug: microsoft-azure-arc-networksecurityperimeterconfiguration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-networksecurityperimeterconfiguration-api-openapi.yml
- filename: microsoft-azure-arc-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Arc Private Link Resources API
  slug: microsoft-azure-arc-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-privatelinkresources-api-openapi.yml
- filename: microsoft-azure-arc-settings-api-openapi.yml
  format: yaml
  label: Azure Arc Settings API
  slug: microsoft-azure-arc-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-settings-api-openapi.yml
- filename: microsoft-azure-arc-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Arc Subscriptions API
  slug: microsoft-azure-arc-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-subscriptions-api-openapi.yml
- filename: microsoft-azure-arc-vmapplications-api-openapi.yml
  format: yaml
  label: Azure Arc Vm Applications API
  slug: microsoft-azure-arc-vmapplications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-vmapplications-api-openapi.yml
- filename: microsoft-azure-arc-operations-api-openapi.yml
  format: yaml
  label: Azure Arc Operations API
  slug: microsoft-azure-arc-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-operations-api-openapi.yml
- filename: microsoft-azure-arc-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Arc Private Endpoint Connections API
  slug: microsoft-azure-arc-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-private-endpoint-connections-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Arc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Arc publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Arc API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Arc
provider_slug: microsoft-azure-arc
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-arc-hybridcompute-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-arc-openapi.yml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-arc-scopes
source_filename: microsoft-azure-arc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/microsoft-azure-arc-hybridcompute-openapi.yml, openapi/microsoft-azure-arc-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-arc-hybridcompute-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\n- name: azure_auth\n  source: openapi/microsoft-azure-arc-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-arc-hybridcompute-openapi.yml\n  - openapi/microsoft-azure-arc-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-arc/scopes/microsoft-azure-arc-scopes.yml
summary_line: 1 scope · implicit
tags:
- Arc
- Hybrid Cloud
- Kubernetes
- Multi-Cloud
- Server Management
token_bound: false
token_urls: []
---
