---
api_specs:
- filename: oracle-integration-developer-api.yaml
  format: yaml
  label: Oracle Integration Developer API
  slug: oracle-integration-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/openapi/oracle-integration-developer-api.yaml
- filename: oracle-integration-process-automation-api.yaml
  format: yaml
  label: Oracle Integration Process Automation API
  slug: oracle-integration-process-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/openapi/oracle-integration-process-automation-api.yaml
authorization_urls:
- https://{idcs-url}/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Oracle Integration Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Oracle Integration publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Oracle Integration API on a user''s behalf.


  Tokens are issued from https://{idcs-url}/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oracle Integration
provider_slug: oracle-integration
schemes:
- description: OAuth 2.0 authentication via Oracle Identity Cloud Service (IDCS).
  flows:
  - authorizationUrl: https://{idcs-url}/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://{idcs-url}/oauth2/v1/token
  name: oauth2
  source: openapi/oracle-integration-developer-api.yaml
- description: OAuth 2.0 authentication via Oracle Identity Cloud Service.
  flows:
  - authorizationUrl: https://{idcs-url}/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://{idcs-url}/oauth2/v1/token
  name: oauth2
  source: openapi/oracle-integration-process-automation-api.yaml
scope_count: 1
scope_names:
- urn:opc:resource:consumer::all
scopes:
- description: Full access to Oracle Integration APIs
  flows:
  - authorizationCode
  scope: urn:opc:resource:consumer::all
slug: oracle-integration-scopes
source_filename: oracle-integration-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-integration-developer-api.yaml, openapi/oracle-integration-process-automation-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/oracle-integration-developer-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{idcs-url}/oauth2/v1/authorize\n    tokenUrl: https://{idcs-url}/oauth2/v1/token\n  description: OAuth 2.0 authentication via Oracle Identity Cloud Service (IDCS).\n- name: oauth2\n  source: openapi/oracle-integration-process-automation-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{idcs-url}/oauth2/v1/authorize\n    tokenUrl: https://{idcs-url}/oauth2/v1/token\n  description: OAuth 2.0 authentication via Oracle Identity Cloud Service.\nscopes:\n- scope: urn:opc:resource:consumer::all\n  description: Full access to Oracle Integration APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oracle-integration-developer-api.yaml\n  - openapi/oracle-integration-process-automation-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/scopes/oracle-integration-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- API Management
- Automation
- B2B Integration
- Cloud Integration
- Enterprise Integration
- Integration
- iPaaS
- Process Automation
token_urls:
- https://{idcs-url}/oauth2/v1/token
---
