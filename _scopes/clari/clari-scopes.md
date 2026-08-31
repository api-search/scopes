---
api_specs:
- filename: clari-activity-api-api-openapi.yml
  format: yaml
  label: Clari Activity API API
  slug: clari-activity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-activity-api-api-openapi.yml
- filename: clari-administrative-api-api-openapi.yml
  format: yaml
  label: Clari Administrative API API
  slug: clari-administrative-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-administrative-api-api-openapi.yml
- filename: clari-audit-api-api-openapi.yml
  format: yaml
  label: Clari Audit API API
  slug: clari-audit-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-audit-api-api-openapi.yml
- filename: clari-bulk-export-framework-api-openapi.yml
  format: yaml
  label: Clari Bulk Export Framework API
  slug: clari-bulk-export-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-export-framework-api-openapi.yml
- filename: clari-bulk-ingest-job-status-api-api-openapi.yml
  format: yaml
  label: Clari Bulk Ingest Job Status API API
  slug: clari-bulk-ingest-job-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-ingest-job-status-api-api-openapi.yml
- filename: clari-export-api-openapi.yml
  format: yaml
  label: Clari Export API
  slug: clari-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-export-api-openapi.yml
- filename: clari-forecast-api-api-openapi.yml
  format: yaml
  label: Clari Forecast API API
  slug: clari-forecast-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-forecast-api-api-openapi.yml
- filename: clari-ingestion-api-api-openapi.yml
  format: yaml
  label: Clari Ingestion API API
  slug: clari-ingestion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-ingestion-api-api-openapi.yml
- filename: clari-opportunity-api-api-openapi.yml
  format: yaml
  label: Clari Opportunity API API
  slug: clari-opportunity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-opportunity-api-api-openapi.yml
- filename: clari-account-api-openapi.yml
  format: yaml
  label: Clari Account API
  slug: clari-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-account-api-openapi.yml
- filename: clari-call-api-openapi.yml
  format: yaml
  label: Clari Call API
  slug: clari-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-call-api-openapi.yml
- filename: clari-contact-api-openapi.yml
  format: yaml
  label: Clari Contact API
  slug: clari-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-contact-api-openapi.yml
- filename: clari-deal-api-openapi.yml
  format: yaml
  label: Clari Deal API
  slug: clari-deal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-deal-api-openapi.yml
- filename: clari-scorecard-api-openapi.yml
  format: yaml
  label: Clari Scorecard API
  slug: clari-scorecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-scorecard-api-openapi.yml
- filename: clari-topics-api-openapi.yml
  format: yaml
  label: Clari Topics API
  slug: clari-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-topics-api-openapi.yml
- filename: clari-user-api-openapi.yml
  format: yaml
  label: Clari User API
  slug: clari-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-user-api-openapi.yml
authorization_urls: []
description: Clari's OAuth surface exists ONLY on the MCP server. Neither published OpenAPI declares an oauth2 securityScheme — the Revenue API uses an `apikey` header and the Copilot API uses `X-Api-Key` + `X-Api-Password`. The scopes below are read verbatim from the RFC 9728 / RFC 8414 metadata the Clari MCP gateway serves anonymously. They are standard OpenID Connect scopes; Clari publishes NO product-specific authorization scopes (nothing like forecast:read or calls:read), so a granted MCP token is not scoped by Clari data domain at the protocol level. Access is instead gated by tenant admin toggles and the user's own Clari permissions.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Clari Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Clari uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clari
provider_slug: clari
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: clari-scopes
source_filename: clari-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://mcp.clari.com/.well-known/oauth-protected-resource/mcp and\n  https://mcp.clari.com/.well-known/oauth-authorization-server/mcp (both HTTP 200,\n  fetched anonymously 2026-08-13)\nname: Clari OAuth scopes\ndescription: >-\n  Clari's OAuth surface exists ONLY on the MCP server. Neither published OpenAPI\n  declares an oauth2 securityScheme — the Revenue API uses an `apikey` header and the\n  Copilot API uses `X-Api-Key` + `X-Api-Password`. The scopes below are read verbatim\n  from the RFC 9728 / RFC 8414 metadata the Clari MCP gateway serves anonymously.\n  They are standard OpenID Connect scopes; Clari publishes NO product-specific\n  authorization scopes (nothing like forecast:read or calls:read), so a granted MCP\n  token is not scoped by Clari data domain at the protocol level. Access is instead\n  gated by tenant admin toggles and the user's own Clari permissions.\napplies_to: mcp\ndocs: null\ndocs_note: >-\n\
  \  No scopes or permissions reference page is published on developer.clari.com,\n  api-doc.copilot.clari.com or clari.com. Only the machine-readable metadata exists.\n\nauthorization_server:\n  issuer: https://clariciam.okta.com/oauth2/aus13shznanP7WOkp698\n  authorization_endpoint: https://app.clari.com/authorize\n  token_endpoint: https://clariciam.okta.com/oauth2/aus13shznanP7WOkp698/v1/token\n  registration_endpoint: https://mcp.clari.com/okta/clients\n  jwks_uri: https://clariciam.okta.com/oauth2/aus13shznanP7WOkp698/v1/keys\n  introspection_endpoint: https://clariciam.okta.com/oauth2/aus13shznanP7WOkp698/v1/introspect\n  revocation_endpoint: https://clariciam.okta.com/oauth2/aus13shznanP7WOkp698/v1/revoke\n  end_session_endpoint: https://clariciam.okta.com/oauth2/aus13shznanP7WOkp698/v1/logout\n  device_authorization_endpoint: https://clariciam.okta.com/oauth2/aus13shznanP7WOkp698/v1/device/authorize\n  code_challenge_methods_supported: [S256]\n  dpop_signing_alg_values_supported:\
  \ [RS256, RS384, RS512, ES256, ES384, ES512]\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n\nprotected_resource:\n  resource: https://mcp.clari.com/mcp\n  resource_name: Clari MCP Server\n  bearer_methods_supported: [header]\n\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token. Required by the MCP resource.\n  required: true\n  source: protected-resource metadata (scopes_supported)\n  standard: openid-connect-core\n- name: profile\n  description: Standard OIDC scope granting basic profile claims about the authenticating Clari user.\n  required: true\n  source: protected-resource metadata (scopes_supported)\n  standard: openid-connect-core\n- name: email\n  description: Standard OIDC scope granting the user's email claim. Advertised by the authorization server; not required by the MCP resource.\n  required: false\n  source: authorization-server\
  \ metadata (scopes_supported)\n  standard: openid-connect-core\n- name: address\n  description: Standard OIDC address claim scope. Advertised by the authorization server only.\n  required: false\n  source: authorization-server metadata (scopes_supported)\n  standard: openid-connect-core\n- name: phone\n  description: Standard OIDC phone claim scope. Advertised by the authorization server only.\n  required: false\n  source: authorization-server metadata (scopes_supported)\n  standard: openid-connect-core\n- name: offline_access\n  description: Requests a refresh token so an agent can maintain a long-lived MCP session.\n  required: false\n  source: authorization-server metadata (scopes_supported)\n  standard: openid-connect-core\n- name: device_sso\n  description: Okta device single-sign-on scope, used with the device authorization grant.\n  required: false\n  source: authorization-server metadata (scopes_supported)\n  standard: okta-extension\n\ntoken_claims_supported:\n- ver\n- jti\n-\
  \ iss\n- aud\n- iat\n- exp\n- cid\n- uid\n- scp\n- sub\n\nfindings:\n- Product-scoped authorization is absent. Nothing in the published metadata lets a client request read-only access to, say, calls but not deals.\n- Consent granularity is therefore all-or-nothing at the protocol layer; least-privilege has to be enforced by the Clari admin toggles and the user's own role.\n- The authorization server advertises `implicit` and `password` grants, both discouraged by OAuth 2.1. An MCP client should use authorization_code + PKCE (S256), which is supported.\n- Dynamic client registration is open at https://mcp.clari.com/okta/clients, which is what allows Claude and ChatGPT to connect without a pre-provisioned client id.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/scopes/clari-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Revenue Operations
- Forecasting
- Pipeline Management
- Sales Intelligence
- Activity Intelligence
- Deal Insights
- CRM
- Conversation Intelligence
- B2B
- Enterprise
- MCP
- Agents
- Sales Engagement
- Bulk Export
- Data Ingestion
token_urls: []
---
