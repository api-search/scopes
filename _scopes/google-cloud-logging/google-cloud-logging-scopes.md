---
api_specs:
- filename: google-cloud-logging-bucket-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Bucket API
  slug: google-cloud-logging-bucket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-bucket-api-openapi.yml
- filename: google-cloud-logging-buckets-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Buckets API
  slug: google-cloud-logging-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-buckets-api-openapi.yml
- filename: google-cloud-logging-entries-copy-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:copy API
  slug: google-cloud-logging-entries-copy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-copy-api-openapi.yml
- filename: google-cloud-logging-entries-list-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:list API
  slug: google-cloud-logging-entries-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-list-api-openapi.yml
- filename: google-cloud-logging-entries-tail-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:tail API
  slug: google-cloud-logging-entries-tail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-tail-api-openapi.yml
- filename: google-cloud-logging-entries-write-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:write API
  slug: google-cloud-logging-entries-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-write-api-openapi.yml
- filename: google-cloud-logging-exclusions-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Exclusions API
  slug: google-cloud-logging-exclusions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-exclusions-api-openapi.yml
- filename: google-cloud-logging-google-cloud-logging-api-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Google Cloud Logging API
  slug: google-cloud-logging-google-cloud-logging-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-google-cloud-logging-api-api-openapi.yml
- filename: google-cloud-logging-sinks-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Sinks API
  slug: google-cloud-logging-sinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-sinks-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: https://docs.cloud.google.com/logging/docs/access-control
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Cloud Logging Scopes
name_suffix: OAuth Scopes
note: Upgraded from the 2026-07-11 derived pass, which read the four scopes in the local OpenAPI and used short names. The names below are the full scope URIs exactly as Google publishes them in the Discovery document's auth.oauth2.scopes block (revision 20260818), with Google's own descriptions verbatim. cloud-platform.read-only was missing from the derived file.
overview: 'Google Cloud Logging publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Logging API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Logging
provider_slug: google-cloud-logging
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: discovery/google-cloud-logging-discovery-v2.json
scope_count: 5
scope_names:
- https://www.googleapis.com/auth/logging.read
- https://www.googleapis.com/auth/logging.write
- https://www.googleapis.com/auth/logging.admin
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/cloud-platform.read-only
scopes:
- description: View log data for your projects
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/logging.read
- description: Submit log data for your projects
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/logging.write
- description: Administrate log data for your projects
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/logging.admin
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View your data across Google Cloud services and see the email address of your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform.read-only
slug: google-cloud-logging-scopes
source_filename: google-cloud-logging-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: discovery/google-cloud-logging-discovery-v2.json\ndocs: https://docs.cloud.google.com/logging/docs/access-control\nnote: >-\n  Upgraded from the 2026-07-11 derived pass, which read the four scopes in the local OpenAPI\n  and used short names. The names below are the full scope URIs exactly as Google publishes\n  them in the Discovery document's auth.oauth2.scopes block (revision 20260818), with Google's\n  own descriptions verbatim. cloud-platform.read-only was missing from the derived file.\nschemes:\n  - name: OAuth2\n    source: discovery/google-cloud-logging-discovery-v2.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n  - scope: https://www.googleapis.com/auth/logging.read\n    short: logging.read\n    description: View log data for your projects\n    flows: [authorizationCode]\n   \
  \ sources: [discovery/google-cloud-logging-discovery-v2.json, openapi/google-cloud-logging-openapi.yml]\n  - scope: https://www.googleapis.com/auth/logging.write\n    short: logging.write\n    description: Submit log data for your projects\n    flows: [authorizationCode]\n    sources: [discovery/google-cloud-logging-discovery-v2.json, openapi/google-cloud-logging-openapi.yml]\n  - scope: https://www.googleapis.com/auth/logging.admin\n    short: logging.admin\n    description: Administrate log data for your projects\n    flows: [authorizationCode]\n    sources: [discovery/google-cloud-logging-discovery-v2.json, openapi/google-cloud-logging-openapi.yml]\n  - scope: https://www.googleapis.com/auth/cloud-platform\n    short: cloud-platform\n    description: >-\n      See, edit, configure, and delete your Google Cloud data and see the email address for\n      your Google Account.\n    flows: [authorizationCode]\n    sources: [discovery/google-cloud-logging-discovery-v2.json, openapi/google-cloud-logging-openapi.yml]\n\
  \  - scope: https://www.googleapis.com/auth/cloud-platform.read-only\n    short: cloud-platform.read-only\n    description: >-\n      View your data across Google Cloud services and see the email address of your Google\n      Account\n    flows: [authorizationCode]\n    sources: [discovery/google-cloud-logging-discovery-v2.json]\nmcp_scopes:\n  note: >-\n    The Cloud Logging remote MCP server accepts the same scopes; its setup page names\n    logging.admin and logging.write specifically, alongside the roles/mcp.toolUser IAM role.\n  url: https://docs.cloud.google.com/logging/docs/use-logging-mcp\nauthorization_note: >-\n  A scope is necessary but not sufficient — Google Cloud IAM roles decide the actual\n  permission. See authentication/google-cloud-logging-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/scopes/google-cloud-logging-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Cloud
- Logging
- Monitoring
- Observability
- Telemetry
- Log Management
- SRE
- DevOps
- OpenTelemetry
- Google Cloud
token_urls:
- https://oauth2.googleapis.com/token
---
