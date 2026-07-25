---
api_specs:
- filename: google-cloud-platform-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Folders API
  slug: google-cloud-platform-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-folders-api-openapi.yml
- filename: google-cloud-platform-operations-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Operations API
  slug: google-cloud-platform-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-operations-api-openapi.yml
- filename: google-cloud-platform-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Organizations API
  slug: google-cloud-platform-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-organizations-api-openapi.yml
- filename: google-cloud-platform-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Projects API
  slug: google-cloud-platform-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-projects-api-openapi.yml
- filename: google-cloud-platform-tagbindings-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagBindings API
  slug: google-cloud-platform-tagbindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagbindings-api-openapi.yml
- filename: google-cloud-platform-tagkeys-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagKeys API
  slug: google-cloud-platform-tagkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagkeys-api-openapi.yml
- filename: google-cloud-platform-tagvalues-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagValues API
  slug: google-cloud-platform-tagvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagvalues-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: https://developers.google.com/identity/protocols/oauth2/scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Cloud Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Platform publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Platform API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schemes:
- description: OAuth 2.0 authentication using Google Cloud service accounts or user credentials. Supports both service-to-service and end-user authentication flows.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/cloud-resource-manager-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/cloud-platform.read-only
scopes:
- description: Full access to view and manage Google Cloud resources.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: Read-only access to view Google Cloud resources.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform.read-only
slug: google-cloud-platform-scopes
source_filename: google-cloud-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/cloud-resource-manager-openapi.yml\ndocs: https://developers.google.com/identity/protocols/oauth2/scopes\nnotes: >-\n  Google publishes the full OAuth 2.0 scope reference across all APIs at the\n  docs URL above. Cloud Resource Manager uses the two platform-wide scopes\n  below; most GCP services also accept the broad cloud-platform scope in\n  addition to any service-specific scopes.\nschemes:\n- name: oauth2\n  source: openapi/cloud-resource-manager-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication using Google Cloud service accounts or user credentials.\n    Supports both service-to-service and end-user authentication flows.\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to view and manage Google Cloud resources.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-resource-manager-openapi.yml\n- scope: https://www.googleapis.com/auth/cloud-platform.read-only\n  description: Read-only access to view Google Cloud resources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloud-resource-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/scopes/google-cloud-platform-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
token_urls:
- https://oauth2.googleapis.com/token
---
