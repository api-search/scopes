---
api_specs:
- filename: outsystems-user-access-management-api-v1-openapi.json
  format: json
  label: OutSystems ODC User and Access Management API
  slug: user-access-management-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-user-access-management-api-v1-openapi.json
- filename: outsystems-portfolio-api-v2-openapi.json
  format: json
  label: OutSystems ODC Portfolio API
  slug: portfolio-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-portfolio-api-v2-openapi.json
- filename: outsystems-portfolio-api-v1-openapi.json
  format: json
  label: OutSystems ODC Portfolio API (v1)
  slug: portfolio-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-portfolio-api-v1-openapi.json
- filename: outsystems-asset-repository-api-v1-openapi.json
  format: json
  label: OutSystems ODC Asset Repository API
  slug: asset-repository-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-asset-repository-api-v1-openapi.json
- filename: outsystems-asset-configurations-api-v1-openapi.json
  format: json
  label: OutSystems ODC Asset Configurations API
  slug: asset-configurations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-asset-configurations-api-v1-openapi.json
- filename: outsystems-environment-configurations-api-v1-openapi.json
  format: json
  label: OutSystems ODC Environment Configurations API
  slug: environment-configurations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-environment-configurations-api-v1-openapi.json
- filename: outsystems-build-operations-api-v1-openapi.json
  format: json
  label: OutSystems ODC Build Operations API
  slug: build-operations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-build-operations-api-v1-openapi.json
- filename: outsystems-deployments-api-v1-openapi.json
  format: json
  label: OutSystems ODC Deployments API
  slug: deployments-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-deployments-api-v1-openapi.json
- filename: outsystems-dependency-management-api-v1-openapi.json
  format: json
  label: OutSystems ODC Dependency Management API
  slug: dependency-management-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-dependency-management-api-v1-openapi.json
- filename: outsystems-code-quality-api-v1-openapi.json
  format: json
  label: OutSystems ODC Code Quality API
  slug: code-quality-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-code-quality-api-v1-openapi.json
- filename: outsystems-native-application-orchestration-service-api-v1-openapi.json
  format: json
  label: OutSystems ODC Native Mobile Build API
  slug: native-mobile-build-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-native-application-orchestration-service-api-v1-openapi.json
- filename: outsystems-external-library-generation-api-v1-openapi.json
  format: json
  label: OutSystems ODC External Library Generation API
  slug: external-library-generation-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-external-library-generation-api-v1-openapi.json
- filename: outsystems-subscription-api-v1-openapi.json
  format: json
  label: OutSystems ODC Subscription API
  slug: subscription-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-subscription-api-v1-openapi.json
authorization_urls: []
description: ''
docs: https://success.outsystems.com/documentation/outsystems_developer_cloud/odc_rest_apis/authentication/create_api_client/
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Outsystems Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OutSystems uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OutSystems
provider_slug: outsystems
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources: openapi/*.json (all 13 specs)
  type: http
scope_count: 0
scope_names: []
scopes: []
slug: outsystems-scopes
source_filename: outsystems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/*.json (operation descriptions) + ODC REST API authentication docs\ndocs: https://success.outsystems.com/documentation/outsystems_developer_cloud/odc_rest_apis/authentication/create_api_client/\nmodel: portal-assigned-permissions\nmodel_note: >-\n  The ODC REST APIs use OAuth 2.0 client-credentials, but they do NOT use requested\n  OAuth scopes. The token request carries only grant_type, client_id and client_secret\n  — no `scope` parameter — and the OpenAPI specs declare a plain `bearerAuth` HTTP\n  bearer scheme with no oauth2 flows and no scopes map. Authorization is instead\n  attached to the API Client in the ODC Portal: permissions are granted per ODC stage,\n  and the issued access token inherits them. Each operation's description names the\n  permission it requires. The catalog below is therefore a PERMISSION model derived\n  from those descriptions, not a scope list lifted from a securityScheme.\noauth2:\n \
  \ grant_type: client_credentials\n  scope_parameter_used: false\n  discovery: https://{odc-portal-domain}/identity/.well-known/openid-configuration\n  token_lifetime_seconds: 43200\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources: openapi/*.json (all 13 specs)\npermission_groups:\n- group: User management\n  permissions:\n  - name: User management > View end users\n    operations_referencing: 3\n  - name: User management > View members\n    operations_referencing: 1\n  - name: User management > Manage users\n    operations_referencing: 7\n  - name: User management > Manage end-user groups\n    operations_referencing: 11\n  - name: User management > Manage end-user access\n    operations_referencing: 2\n  - name: User management > Manage member access\n    operations_referencing: 2\n  - name: User management > Manage organization roles\n    operations_referencing: 3\n- group: Configuration management\n  permissions:\n  - name: Configuration management\
  \ > View configurations\n    operations_referencing: 14\n  - name: Configuration management > Edit configurations\n    operations_referencing: 3\n  - name: Configuration management > Edit asset configurations\n    operations_referencing: 3\n  - name: Configuration management > Manage custom domains\n    operations_referencing: 4\n  - name: Configuration management > Manage IP filters\n    operations_referencing: 3\n  - name: Configuration management > Manage private gateways\n    operations_referencing: 3\n  - name: Configuration management > Manage Email SMTP configuration\n    operations_referencing: 1\n- group: Stage\n  permissions:\n  - name: Stage > View stage\n    operations_referencing: 12\n- group: Asset management\n  permissions:\n  - name: Asset management > Open\n    operations_referencing: 8\n  - name: Asset management > Create\n    operations_referencing: 1\n  - name: Asset management > Change\n    operations_referencing: 2\n  - name: Asset management > Delete\n    operations_referencing:\
  \ 2\n- group: Release management\n  permissions:\n  - name: Release management > Deploy assets\n    operations_referencing: 3\n  - name: Release management > Release\n    operations_referencing: 1\n- group: Analyze\n  permissions:\n  - name: Analyze > View Code Quality findings\n    operations_referencing: 9\n  - name: Analyze > Manage code quality findings\n    operations_referencing: 1\n- group: Subscriptions\n  permissions:\n  - name: Subscriptions > View subscription\n    operations_referencing: 4\n  - name: Subscriptions > Manage subscription\n    operations_referencing: 1\ncomposite_requirements:\n- operations_requiring: Stage > View stage AND Subscriptions > View subscription\n  count: 2\n- operations_requiring: User management > View members OR User management > Manage users\n  count: 1\n- operations_requiring: Asset management > Change OR Release management > Release\n  count: 1\n- operations_requiring: at least one permission (unspecified) to fetch entitlements\n  count: 1\n\
  enforcement:\n  insufficient_permission_status: 403\n  invalid_or_expired_token_status: 401\n  note: >-\n    An API Client created without any permissions is placed in a \"Needs attention\"\n    state in the ODC Portal until permissions are assigned.\nderivation:\n  method: >-\n    Regex extraction of \"API Client needs the <X> permission\" phrasing from the\n    description/summary of all 150 operations across the 13 OpenAPI specs, then\n    deduplicated and grouped by the \"<Group> > <Action>\" naming the platform uses.\n  caveat: >-\n    Counts are operations that reference each permission in prose; they are not a\n    machine-declared security requirement, because the specs apply only the bearerAuth\n    scheme uniformly. No published permissions-reference page was found to upgrade this\n    to method: searched.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/scopes/outsystems-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Low-Code
- Application Development
- Platform as a Service
- DevOps
- Deployment
- Identity and Access Management
- Artificial Intelligence
- Enterprise Software
- Mobile Development
token_urls: []
---
