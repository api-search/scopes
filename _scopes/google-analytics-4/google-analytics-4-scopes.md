---
api_specs:
- filename: google-analytics-4-data-v1beta-openapi.yml
  format: yaml
  label: Google Analytics Data API
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/openapi/google-analytics-4-data-v1beta-openapi.yml
- filename: google-analytics-4-admin-v1beta-openapi.yml
  format: yaml
  label: Google Analytics Admin API
  slug: google-analytics-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/openapi/google-analytics-4-admin-v1beta-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: https://developers.google.com/identity/protocols/oauth2/scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Analytics 4 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Analytics 4 publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Analytics 4 API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Analytics 4
provider_slug: google-analytics-4
schemes:
- description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope> identifier.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-analytics-4-admin-v1alpha-openapi.yml
- description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope> identifier.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-analytics-4-admin-v1beta-openapi.yml
- description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope> identifier.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-analytics-4-data-v1alpha-openapi.yml
- description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope> identifier.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-analytics-4-data-v1beta-openapi.yml
scope_count: 5
scope_names:
- analytics
- analytics.edit
- analytics.manage.users
- analytics.manage.users.readonly
- analytics.readonly
scopes:
- description: View and manage your Google Analytics data
  flows:
  - authorizationCode
  scope: analytics
- description: Edit Google Analytics management entities
  flows:
  - authorizationCode
  scope: analytics.edit
- description: Manage Google Analytics Account users by email address
  flows:
  - authorizationCode
  scope: analytics.manage.users
- description: View Google Analytics user permissions
  flows:
  - authorizationCode
  scope: analytics.manage.users.readonly
- description: See and download your Google Analytics data
  flows:
  - authorizationCode
  scope: analytics.readonly
slug: google-analytics-4-scopes
source_filename: google-analytics-4-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://developers.google.com/identity/protocols/oauth2/scopes\ndocs_note: >-\n  Google's canonical OAuth 2.0 scope reference lists the analyticsadmin and analyticsdata\n  scope sets. Every scope below is also declared in Google's own Discovery documents, so the\n  spec-derived set and the documented set agree exactly - no scope is documented that the\n  contract omits, and none is in the contract that the docs omit.\nscope_prefix: https://www.googleapis.com/auth/\nscope_prefix_note: >-\n  Scopes are recorded here in short form. The wire form an OAuth request must send is the\n  prefix above plus the short name, e.g.\n  https://www.googleapis.com/auth/analytics.readonly\nauthorization_server: https://accounts.google.com\noidc_discovery: well-known/google-analytics-4-openid-configuration.json\noauth_server_metadata: well-known/google-analytics-4-oauth-authorization-server.json\nsource: openapi/google-analytics-4-admin-v1alpha-openapi.yml,\
  \ openapi/google-analytics-4-admin-v1beta-openapi.yml,\n  openapi/google-analytics-4-data-v1alpha-openapi.yml, openapi/google-analytics-4-data-v1beta-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-analytics-4-admin-v1alpha-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope>\n    identifier.\n- name: OAuth2\n  source: openapi/google-analytics-4-admin-v1beta-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope>\n    identifier.\n- name: OAuth2\n  source: openapi/google-analytics-4-data-v1alpha-openapi.yml\n  flows:\n  - flow:\
  \ authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope>\n    identifier.\n- name: OAuth2\n  source: openapi/google-analytics-4-data-v1beta-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0. Scopes are the short form of the full https://www.googleapis.com/auth/<scope>\n    identifier.\nscopes:\n- scope: analytics\n  description: View and manage your Google Analytics data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-analytics-4-data-v1alpha-openapi.yml\n  - openapi/google-analytics-4-data-v1beta-openapi.yml\n- scope: analytics.edit\n  description: Edit Google Analytics management entities\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/google-analytics-4-admin-v1alpha-openapi.yml\n  - openapi/google-analytics-4-admin-v1beta-openapi.yml\n- scope: analytics.manage.users\n  description: Manage Google Analytics Account users by email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-analytics-4-admin-v1alpha-openapi.yml\n- scope: analytics.manage.users.readonly\n  description: View Google Analytics user permissions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-analytics-4-admin-v1alpha-openapi.yml\n- scope: analytics.readonly\n  description: See and download your Google Analytics data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-analytics-4-admin-v1alpha-openapi.yml\n  - openapi/google-analytics-4-admin-v1beta-openapi.yml\n  - openapi/google-analytics-4-data-v1alpha-openapi.yml\n  - openapi/google-analytics-4-data-v1beta-openapi.yml\ngrants:\n  supported:\n    - authorization_code\n    - refresh_token\n    - urn:ietf:params:oauth:grant-type:device_code\n\
  \    - urn:ietf:params:oauth:grant-type:jwt-bearer\n  source: well-known/google-analytics-4-oauth-authorization-server.json\n  note: >-\n    The jwt-bearer grant is how service accounts authenticate; it is the path Google's own\n    client libraries and the official MCP server take via Application Default Credentials.\n  client_credentials: false\n  client_credentials_note: >-\n    There is no client_credentials grant. Machine-to-machine access requires a service account\n    with a domain-delegated or property-granted identity, not a bare client id and secret.\nusage:\n  read_only: analytics.readonly\n  reporting_write: analytics\n  configuration_write: analytics.edit\n  user_management: analytics.manage.users\n  user_management_read: analytics.manage.users.readonly\n  mcp_server_requires:\n    - analytics.readonly\n    - cloud-platform\n  mcp_note: >-\n    The official analytics-mcp server additionally requests the broad\n    https://www.googleapis.com/auth/cloud-platform scope, which\
  \ is far wider than the GA4\n    surface it exposes. Worth flagging for anyone granting it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/scopes/google-analytics-4-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Analytics
- Data Collection
- Marketing
- Measurement
- Mobile Analytics
- Reporting
- Web Analytics
- Attribution
- Audiences
- Event Tracking
token_urls:
- https://oauth2.googleapis.com/token
---
