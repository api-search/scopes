---
api_specs:
- filename: backstage-events-backend-openapi.yaml
  format: yaml
  label: Backstage Events System
  slug: events-system
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-events-backend-openapi.yaml
- filename: backstage-actions-api-openapi.yml
  format: yaml
  label: Backstage Actions API
  slug: backstage-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-actions-api-openapi.yml
- filename: backstage-auth-backend-openapi.yaml
  format: yaml
  label: Backstage Authentication API
  slug: backstage-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-auth-backend-openapi.yaml
- filename: backstage-authorization-api-openapi.yml
  format: yaml
  label: Backstage Authorization API
  slug: backstage-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-authorization-api-openapi.yml
- filename: backstage-documentation-api-openapi.yml
  format: yaml
  label: Backstage Documentation API
  slug: backstage-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-documentation-api-openapi.yml
- filename: backstage-catalog-backend-openapi.yaml
  format: yaml
  label: Backstage Entities API
  slug: backstage-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-catalog-backend-openapi.yaml
- filename: backstage-locations-api-openapi.yml
  format: yaml
  label: Backstage Locations API
  slug: backstage-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-locations-api-openapi.yml
- filename: backstage-metadata-api-openapi.yml
  format: yaml
  label: Backstage Metadata API
  slug: backstage-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-metadata-api-openapi.yml
- filename: backstage-search-backend-openapi.yaml
  format: yaml
  label: Backstage Search API
  slug: backstage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-search-backend-openapi.yaml
- filename: backstage-sync-api-openapi.yml
  format: yaml
  label: Backstage Sync API
  slug: backstage-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-sync-api-openapi.yml
- filename: backstage-scaffolder-backend-openapi.yaml
  format: yaml
  label: Backstage Tasks API
  slug: backstage-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-scaffolder-backend-openapi.yaml
- filename: backstage-templates-api-openapi.yml
  format: yaml
  label: Backstage Templates API
  slug: backstage-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-templates-api-openapi.yml
- filename: backstage-token-verification-api-openapi.yml
  format: yaml
  label: Backstage Token Verification API
  slug: backstage-token-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-token-verification-api-openapi.yml
- filename: backstage-notifications-backend-openapi.yaml
  format: yaml
  label: Backstage Notifications API
  slug: backstage-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-notifications-backend-openapi.yaml
- filename: backstage-dynamic-features-openapi.yaml
  format: yaml
  label: Backstage Dynamic Feature Service API
  slug: backstage-dynamic-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-dynamic-features-openapi.yaml
authorization_urls: []
description: 'Backstage''s first-party plugin OpenAPIs declare a bearer `JWT` scheme with no oauth2 flows and no scopes, so there is no scope surface on the REST APIs. A real OAuth scope surface does exist on the MCP Actions endpoint: the protected-resource and authorization-server metadata documents served by a running Backstage backend advertise a single scope. Authorization inside Backstage is not scope-based — it is the Permissions framework, which evaluates named permissions (e.g. catalog.entity.read) through a policy, and that is a different mechanism from OAuth scopes.'
docs: https://backstage.io/docs/ai/mcp-actions
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Backstage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Backstage uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Backstage
provider_slug: backstage
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: backstage-scopes
source_filename: backstage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://demo.backstage.io/.well-known/oauth-authorization-server and\n  https://demo.backstage.io/.well-known/oauth-protected-resource/api/mcp-actions/v1 (both HTTP 200),\n  plus https://backstage.io/docs/ai/mcp-actions\nprovider: Backstage\nproviderId: backstage\ndocs: https://backstage.io/docs/ai/mcp-actions\ndescription: >-\n  Backstage's first-party plugin OpenAPIs declare a bearer `JWT` scheme with no oauth2 flows and no\n  scopes, so there is no scope surface on the REST APIs. A real OAuth scope surface does exist on\n  the MCP Actions endpoint: the protected-resource and authorization-server metadata documents\n  served by a running Backstage backend advertise a single scope. Authorization inside Backstage is\n  not scope-based — it is the Permissions framework, which evaluates named permissions\n  (e.g. catalog.entity.read) through a policy, and that is a different mechanism from OAuth scopes.\nauthorization_server:\n\
  \  issuer: https://demo.backstage.io/api/auth\n  observed_on: demo.backstage.io\n  grant_types_supported: [authorization_code]\n  code_challenge_methods_supported: [S256, plain]\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  revocation_endpoint: https://demo.backstage.io/api/auth/v1/revoke\nscopes:\n  - name: openid\n    description: >-\n      The only scope advertised in scopes_supported by both the authorization server metadata and\n      the MCP Actions protected-resource metadata. It carries OIDC identity, not per-resource\n      permission.\n    source: /.well-known/oauth-authorization-server\nscope_count: 1\nauthorization_model_note: >-\n  Fine-grained access is enforced by the Backstage Permissions framework rather than OAuth scopes.\n  See https://backstage.io/docs/permissions/overview — permissions are named\n  (<plugin>.<resource>.<action>) and resolved by a policy that can attach conditional rules.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/scopes/backstage-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open-Source
- Platform Engineering
- Software Templates
- CNCF
token_urls: []
---
