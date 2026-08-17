---
api_specs:
- filename: adobe-analytics-livestream-asyncapi.yml
  format: yaml
  label: Adobe Analytics Livestream API
  slug: adobe-analytics-livestream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/asyncapi/adobe-analytics-livestream-asyncapi.yml
- filename: adobe-analytics-annotations-api-openapi.yml
  format: yaml
  label: Adobe Analytics Annotations API
  slug: adobe-analytics-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-annotations-api-openapi.yml
- filename: adobe-analytics-calculated-metrics-api-openapi.yml
  format: yaml
  label: Adobe Analytics Calculated Metrics API
  slug: adobe-analytics-calculated-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-calculated-metrics-api-openapi.yml
- filename: adobe-analytics-date-ranges-api-openapi.yml
  format: yaml
  label: Adobe Analytics Date Ranges API
  slug: adobe-analytics-date-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-date-ranges-api-openapi.yml
- filename: adobe-analytics-dimensions-api-openapi.yml
  format: yaml
  label: Adobe Analytics Dimensions API
  slug: adobe-analytics-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-dimensions-api-openapi.yml
- filename: adobe-analytics-events-api-openapi.yml
  format: yaml
  label: Adobe Analytics Events API
  slug: adobe-analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-events-api-openapi.yml
- filename: adobe-analytics-jobs-api-openapi.yml
  format: yaml
  label: Adobe Analytics Jobs API
  slug: adobe-analytics-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-jobs-api-openapi.yml
- filename: adobe-analytics-metrics-api-openapi.yml
  format: yaml
  label: Adobe Analytics Metrics API
  slug: adobe-analytics-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-metrics-api-openapi.yml
- filename: adobe-analytics-report-suites-api-openapi.yml
  format: yaml
  label: Adobe Analytics Report Suites API
  slug: adobe-analytics-report-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-report-suites-api-openapi.yml
- filename: adobe-analytics-reports-api-openapi.yml
  format: yaml
  label: Adobe Analytics Reports API
  slug: adobe-analytics-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-reports-api-openapi.yml
- filename: adobe-analytics-segments-api-openapi.yml
  format: yaml
  label: Adobe Analytics Segments API
  slug: adobe-analytics-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-segments-api-openapi.yml
- filename: adobe-analytics-server-call-estimate-api-openapi.yml
  format: yaml
  label: Adobe Analytics Server Call Estimate API
  slug: adobe-analytics-server-call-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-server-call-estimate-api-openapi.yml
- filename: adobe-analytics-classification-api-openapi.json
  format: json
  label: Adobe Analytics Classification API
  slug: adobe-analytics-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/_original/adobe-analytics-classification-api-openapi.json
- filename: adobe-analytics-data-feeds-api-openapi.json
  format: json
  label: Adobe Analytics Data Feed API
  slug: adobe-analytics-data-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/_original/adobe-analytics-data-feeds-api-openapi.json
- filename: adobe-analytics-data-warehouse-api-openapi.json
  format: json
  label: Adobe Analytics Data Warehouse API
  slug: adobe-analytics-data-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/_original/adobe-analytics-data-warehouse-api-openapi.json
- filename: adobe-analytics-data-sources-api-openapi.json
  format: json
  label: Adobe Analytics Data Sources API
  slug: adobe-analytics-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/_original/adobe-analytics-data-sources-api-openapi.json
- filename: adobe-analytics-marketing-channels-api-openapi.json
  format: json
  label: Adobe Analytics Marketing Channels API
  slug: adobe-analytics-marketing-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/_original/adobe-analytics-marketing-channels-api-openapi.json
- filename: adobe-analytics-cloud-locations-api-openapi.json
  format: json
  label: Adobe Analytics Cloud Locations API
  slug: adobe-analytics-cloud-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/_original/adobe-analytics-cloud-locations-api-openapi.json
- filename: adobe-analytics-report-suites-admin-api-openapi.json
  format: json
  label: Adobe Analytics Report Suites Admin API
  slug: adobe-analytics-report-suites-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/_original/adobe-analytics-report-suites-admin-api-openapi.json
- filename: adobe-analytics-component-migration-api-openapi.json
  format: json
  label: Adobe Analytics Component Migration API
  slug: adobe-analytics-component-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/_original/adobe-analytics-component-migration-api-openapi.json
authorization_urls: []
description: Adobe Analytics access tokens are issued by Adobe IMS (Identity Management System). The Adobe Analytics 2.0 REST OpenAPI declares its credential as an HTTP bearer scheme plus an x-api-key header and does NOT declare an inline oauth2 flow with a scope map, so the scopes below are not derivable from the spec. They are taken from the two RFC 8414 / RFC 9728 discovery documents the Adobe Analytics MCP server publishes anonymously — those are the authoritative machine-readable statement of what the Analytics OAuth surface accepts. Saved copies live in well-known/.
docs: https://developer.adobe.com/analytics-apis/docs/2.0/guides/authentication/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Adobe Analytics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adobe Analytics uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: adobe-analytics-scopes
source_filename: adobe-analytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://aa-mcp.adobe.io/.well-known/oauth-protected-resource (HTTP 200),\n  https://aa-mcp.adobe.io/.well-known/oauth-authorization-server (HTTP 200),\n  https://ims-na1.adobelogin.com/.well-known/openid-configuration\ndocs: https://developer.adobe.com/analytics-apis/docs/2.0/guides/authentication/\ndescription: >-\n  Adobe Analytics access tokens are issued by Adobe IMS (Identity Management System).\n  The Adobe Analytics 2.0 REST OpenAPI declares its credential as an HTTP bearer scheme\n  plus an x-api-key header and does NOT declare an inline oauth2 flow with a scope map,\n  so the scopes below are not derivable from the spec. They are taken from the two RFC\n  8414 / RFC 9728 discovery documents the Adobe Analytics MCP server publishes\n  anonymously — those are the authoritative machine-readable statement of what the\n  Analytics OAuth surface accepts. Saved copies live in well-known/.\nauthorization_server:\n  issuer:\
  \ https://aa-mcp.adobe.io\n  authorization_endpoint: https://ims-na1.adobelogin.com/ims/authorize/v2\n  token_endpoint: https://ims-na1.adobelogin.com/ims/token/v3\n  revocation_endpoint: https://ims-na1.adobelogin.com/ims/revoke\n  registration_endpoint: https://aa-mcp.adobe.io/register\n  grant_types_supported: [authorization_code]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  files:\n    - well-known/adobe-analytics-aa-mcp-oauth-authorization-server.json\n    - well-known/adobe-analytics-aa-mcp-oauth-protected-resource.json\n    - well-known/adobe-analytics-ims-openid-configuration.json\n    - well-known/adobe-analytics-ims-oauth-authorization-server.json\nprotected_resource:\n  resource: https://aa-mcp.adobe.io/mcp\n  bearer_methods_supported: [header]\nscopes:\n  - name: openid\n    description: >-\n      Standard OpenID Connect scope; requests an ID token identifying the Adobe user.\n    standard:\
  \ true\n  - name: AdobeID\n    description: >-\n      Adobe IMS scope granting a token bound to the user's Adobe ID. Required on every\n      Adobe Analytics OAuth authorization.\n    standard: false\n  - name: additional_info.projectedProductContext\n    description: >-\n      Adobe IMS scope that projects the user's product entitlements (product profiles and\n      permission items) into the token. This is what carries the Adobe Analytics company\n      access and, for the MCP server, the \"MCP Access\" permission item.\n    standard: false\nauthorization:\n  model: >-\n    Scopes are coarse. Actual authorization is enforced downstream by Adobe Analytics\n    product profiles and permission items (report suite access, component access,\n    admin rights) attached to the authenticated user, not by fine-grained OAuth scopes.\n    There is no per-endpoint or per-resource scope on the Analytics 2.0 REST API.\n  credential_types:\n    - OAuth Server-to-Server (client credentials, Adobe Developer\
  \ Console)\n    - OAuth User Authentication (authorization code + PKCE, used by the MCP server)\nnotes: >-\n  No scopes/permissions reference page enumerating per-operation scopes is published for\n  the Adobe Analytics 2.0 API — the docs describe credential setup, not a scope catalog.\n  Recording that absence honestly rather than inventing per-operation scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/scopes/adobe-analytics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
token_urls: []
---
