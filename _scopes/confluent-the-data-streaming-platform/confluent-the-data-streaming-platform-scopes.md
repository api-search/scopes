---
api_specs:
- filename: confluent-the-data-streaming-platform-cloud-apis-openapi.yml
  format: yaml
  label: Confluent Cloud REST API
  slug: cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml
- filename: confluent-the-data-streaming-platform-api-keys-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform API Keys API
  slug: confluent-the-data-streaming-platform-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-api-keys-api-openapi.yml
- filename: confluent-the-data-streaming-platform-clusters-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform Clusters API
  slug: confluent-the-data-streaming-platform-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-clusters-api-openapi.yml
- filename: confluent-the-data-streaming-platform-environments-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform Environments API
  slug: confluent-the-data-streaming-platform-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-environments-api-openapi.yml
- filename: confluent-the-data-streaming-platform-organizations-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform Organizations API
  slug: confluent-the-data-streaming-platform-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-organizations-api-openapi.yml
- filename: confluent-the-data-streaming-platform-service-accounts-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform Service Accounts API
  slug: confluent-the-data-streaming-platform-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-service-accounts-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.confluent.io/cloud/current/security/access-control/rbac/predefined-rbac-roles.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Confluent The Data Streaming Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Confluent | the Data Streaming Platform publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Confluent | the Data Streaming Platform API on a user''s behalf.


  Tokens are issued from https://api.confluent.cloud/sts/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Confluent | the Data Streaming Platform
provider_slug: confluent-the-data-streaming-platform
schemes:
- description: Authenticate with Confluent API using this credentials (JSON Web Tokens) following OAuth 2.0.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.confluent.cloud/sts/v1/oauth2/token
  name: confluent-sts-access-token
  source: openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml
- description: Authenticate with Confluent API using this credentials (JSON Web Tokens) following OAuth 2.0.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.confluent.cloud/sts/v1/oauth2/token
  name: external-access-token
  source: openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml
- description: Authenticate with OAuth 2.0. Currently this is only supported for partner APIs.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: oauth
  source: openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml
scope_count: 5
scope_names:
- marketplace::describe
- partner:alter
- partner:create
- partner:delete
- partner:describe
scopes:
- description: ''
  flows: []
  scope: marketplace::describe
- description: enables partners to alter entitlements
  flows:
  - clientCredentials
  scope: partner:alter
- description: enables partners to create entitlements and signup on behalf of customers
  flows:
  - clientCredentials
  scope: partner:create
- description: enables partners to delete entitlements and organizations
  flows:
  - clientCredentials
  scope: partner:delete
- description: enables partners to read and list entitlements and organizations
  flows:
  - clientCredentials
  scope: partner:describe
slug: confluent-the-data-streaming-platform-scopes
source_filename: confluent-the-data-streaming-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\nschemes:\n- name: confluent-sts-access-token\n  source: openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.confluent.cloud/sts/v1/oauth2/token\n  description: Authenticate with Confluent API using this credentials (JSON Web Tokens) following OAuth\n    2.0.\n- name: external-access-token\n  source: openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.confluent.cloud/sts/v1/oauth2/token\n  description: Authenticate with Confluent API using this credentials (JSON Web Tokens) following OAuth\n    2.0.\n- name: oauth\n  source: openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n  description: Authenticate with\
  \ OAuth 2.0. Currently this is only supported for partner APIs.\nscopes:\n- scope: marketplace::describe\n  sources:\n  - openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\n- scope: partner:alter\n  description: enables partners to alter entitlements\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\n- scope: partner:create\n  description: enables partners to create entitlements and signup on behalf of customers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\n- scope: partner:delete\n  description: enables partners to delete entitlements and organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\n- scope: partner:describe\n  description: enables partners to read and list entitlements and organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\n\
  docs: https://docs.confluent.io/cloud/current/security/access-control/rbac/predefined-rbac-roles.html\ndocs_note: 'Confluent publishes no OAuth SCOPES reference page, because scopes are not how this API authorizes.\n  Only the partner OAuth scheme declares any (partner:describe / create / alter / delete, plus marketplace::describe),\n  and those cover a partner-entitlement surface most callers never touch. Every other request is authorized\n  by RBAC ROLE BINDINGS attached to the calling user, service account or identity pool — the predefined\n  role list at the docs URL above is the real permission reference for this provider, and it is what an\n  integrator should read where they would normally read a scope table. Searched 2026-09-05 and confirmed:\n  there is no scope catalogue to add.'\nauthorization_model: rbac-role-bindings\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/scopes/confluent-the-data-streaming-platform-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Apache Flink
- Apache Kafka
- Confluent Cloud
- Connectors
- Data Streaming
- Event Streaming
- Kafka Connect
- ksqlDB
- Real-Time Data
- REST
- Schema Registry
- Stream Processing
token_urls:
- https://api.confluent.cloud/sts/v1/oauth2/token
- /oauth2/token
---
