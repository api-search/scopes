---
api_specs:
- filename: leo-prospects-api-openapi.yml
  format: yaml
  label: LeO Public API
  slug: leo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/openapi/leo-prospects-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.meetleo.com/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Leo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LeO uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LeO
provider_slug: leo
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: leo-scopes
source_filename: leo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.meetleo.com/.well-known/oauth-protected-resource\ndocs: https://www.meetleo.com/mcp\nnotes: >-\n  LeO's OpenAPI declares only an HTTP bearer (JWT) scheme with no oauth2 flows,\n  so no scopes can be derived from the spec. The scopes below are read verbatim\n  from the two anonymous discovery documents the LeO MCP Connector publishes:\n  the RFC 9728 protected-resource metadata at\n  https://mcp.meetleo.com/.well-known/oauth-protected-resource and the RFC 8414\n  authorization-server metadata at\n  https://mcp.meetleo.com/.well-known/oauth-authorization-server. They are\n  resource-URI-namespaced scopes issued by an AWS Cognito user pool\n  (us-east-1_RnOkUWIRc) fronted by https://insights-app-auth.meetleo.com. LeO\n  publishes no prose scope/permission reference page; the descriptions below are\n  derived from the matching REST operations in openapi/ and are marked as such.\nauthorization_server:\n  issuer: https://mcp.meetleo.com\n\
  \  authorization_endpoint: https://insights-app-auth.meetleo.com/oauth2/authorize\n  token_endpoint: https://insights-app-auth.meetleo.com/oauth2/token\n  revocation_endpoint: https://insights-app-auth.meetleo.com/oauth2/revoke\n  userinfo_endpoint: https://insights-app-auth.meetleo.com/oauth2/userInfo\n  end_session_endpoint: https://insights-app-auth.meetleo.com/logout\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_RnOkUWIRc/.well-known/jwks.json\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  dynamic_client_registration: false\n  dcr_probe:\n    url: https://mcp.meetleo.com/register\n    status: 404\n    note: >-\n      No RFC 7591 registration endpoint is advertised or served, so MCP clients\n      cannot self-register; a client_id must be issued by LeO out of band.\nresource:\n  resource: https://mcp.meetleo.com\n  bearer_methods_supported:\n\
  \  - header\nscope_count: 7\nscopes:\n- name: https://mcp.meetleo.com/prospects:read\n  resource_scope: true\n  description: >-\n    Read access to the LeO prospect graph -- firmographics, NAICS/NTEE class,\n    renewal dates, workers' comp, OSHA, DOT/FMCSA, Form 5500 and IRS 990 data.\n  method: derived\n  maps_to:\n  - ProspectsController_search\n  - ProspectsController_getById\n  source: openapi/leo-prospects-api-openapi.yml\n- name: https://mcp.meetleo.com/prospects:enrich\n  resource_scope: true\n  description: >-\n    Permission to queue a contact-enrichment job that resolves decision-maker\n    emails and titles and consumes credits.\n  method: derived\n  maps_to:\n  - ProspectsController_enrich\n  - JobsController_getJob\n  source: openapi/leo-prospects-api-openapi.yml, openapi/leo-jobs-api-openapi.yml\n- name: https://mcp.meetleo.com/account:read\n  resource_scope: true\n  description: >-\n    Read the authenticated identity, tenant, plan entitlements\n    (hasApiAccess / hasMcpAccess)\
  \ and credit balance.\n  method: derived\n  maps_to:\n  - AccountController_getAccount\n  - CreditsController_getCreditBalance\n  source: openapi/leo-account-api-openapi.yml, openapi/leo-credits-api-openapi.yml\n- name: openid\n  resource_scope: false\n  description: Standard OpenID Connect scope; requests an ID token.\n  method: probed\n- name: email\n  resource_scope: false\n  description: Standard OIDC claim scope. Advertised by the authorization server only.\n  method: probed\n- name: profile\n  resource_scope: false\n  description: Standard OIDC claim scope. Advertised by the authorization server only.\n  method: probed\n- name: aws.cognito.signin.user.admin\n  resource_scope: false\n  description: >-\n    AWS Cognito built-in scope granting the token holder self-service management\n    of its own user attributes. Not a LeO product scope.\n  method: probed\nobservations:\n- >-\n  The three LeO product scopes map one-to-one onto the three REST tag groups that\n  require authentication\
  \ (prospects, jobs+enrich, account+credits). Nothing in the\n  scope set corresponds to email sending, CRM writes or reporting, which supports\n  reading the compose_email / log_to_crm / daily_report steps in LeO's published\n  workflow illustration as client-side or third-party tools rather than LeO tools.\n- >-\n  Scope names are absolute resource URIs, the AWS Cognito resource-server\n  convention, so a client must request the full URI string, not a bare\n  \"prospects:read\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/scopes/leo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Insurance
- Commercial Insurance
- Property and Casualty
- Employee Benefits
- Insurtech
- Artificial Intelligence
- Sales
- Lead Generation
- Prospecting
- Data Enrichment
- Sales Intelligence
- Non-Profit
- Trucking
- MCP
- agent-native
token_urls: []
---
