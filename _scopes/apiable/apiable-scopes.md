---
api_specs:
- filename: apiable-platform-api-openapi.json
  format: json
  label: Apiable Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-platform-api-openapi.json
authorization_urls: []
description: ''
docs: https://www.apiable.io/docs/automation/webhooks/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Apiable Scopes
name_suffix: OAuth Scopes
note: Two scopes appear in the spec's per-operation security requirements; the clientCredentials flow declares an EMPTY scopes map, so the spec alone does not enumerate them. The docs name a third, apiable/admin, which no operation in the published spec requires. Apiable's own scope docs at /docs/access-control/scopes/ describe scopes CUSTOMERS define for THEIR APIs (Resource Groups, Active/Optional/Restricted plan states, Keycloak and Auth0 as issuers) — that is a product feature, not the Platform API's own scope reference, and is recorded here only as context.
overview: 'Apiable publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apiable API on a user''s behalf.


  Tokens are issued from https://developer.apiable.io/api/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apiable
provider_slug: apiable
schemes:
- description: 'OAuth 2.0: Client Credentials'
  flows:
  - declared_scopes: 0
    flow: clientCredentials
    note: The flow's scopes map is empty in the published spec; scopes are only discoverable from each operation's security[] requirement.
    tokenUrl: https://developer.apiable.io/api/oauth2/token
  name: oauth-cc
  source: openapi/apiable-platform-api-openapi.json
scope_count: 3
scope_names:
- apiable/platform
- apiable/cicd
- apiable/admin
scopes:
- description: Full Platform API management. Required by all 66 published operations — products, plans, subscriptions, teams, users, companies, invitations, documentation, files and webhooks.
  flows:
  - clientCredentials
  scope: apiable/platform
- description: CI/CD scope. Accepted as an alternative on the 35 documentation, webhook, custom-property, file-upload and server-info operations — the set a pipeline needs to push an OpenAPI spec into a portal documentation entry.
  flows:
  - clientCredentials
  scope: apiable/cicd
- description: Named in the webhooks documentation as a third scope that authorizes webhook management. Not referenced by any operation in the published OpenAPI.
  flows:
  - clientCredentials
  scope: apiable/admin
slug: apiable-scopes
source_filename: apiable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: openapi/apiable-platform-api-openapi.json\ndocs: https://www.apiable.io/docs/automation/webhooks/\nnote: >-\n  Two scopes appear in the spec's per-operation security requirements; the clientCredentials flow\n  declares an EMPTY scopes map, so the spec alone does not enumerate them. The docs name a third,\n  apiable/admin, which no operation in the published spec requires. Apiable's own scope docs at\n  /docs/access-control/scopes/ describe scopes CUSTOMERS define for THEIR APIs (Resource Groups,\n  Active/Optional/Restricted plan states, Keycloak and Auth0 as issuers) — that is a product\n  feature, not the Platform API's own scope reference, and is recorded here only as context.\nschemes:\n  - name: oauth-cc\n    source: openapi/apiable-platform-api-openapi.json\n    description: 'OAuth 2.0: Client Credentials'\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://developer.apiable.io/api/oauth2/token\n \
  \       declared_scopes: 0\n        note: >-\n          The flow's scopes map is empty in the published spec; scopes are only discoverable from\n          each operation's security[] requirement.\nscopes:\n  - scope: apiable/platform\n    description: >-\n      Full Platform API management. Required by all 66 published operations — products, plans,\n      subscriptions, teams, users, companies, invitations, documentation, files and webhooks.\n    flows: [clientCredentials]\n    operations: 66\n    sources: [openapi/apiable-platform-api-openapi.json]\n  - scope: apiable/cicd\n    description: >-\n      CI/CD scope. Accepted as an alternative on the 35 documentation, webhook, custom-property,\n      file-upload and server-info operations — the set a pipeline needs to push an OpenAPI spec\n      into a portal documentation entry.\n    flows: [clientCredentials]\n    operations: 35\n    sources:\n      - openapi/apiable-platform-api-openapi.json\n      - https://www.apiable.io/docs/automation/ci-cd/\n\
  \  - scope: apiable/admin\n    description: >-\n      Named in the webhooks documentation as a third scope that authorizes webhook management.\n      Not referenced by any operation in the published OpenAPI.\n    flows: [clientCredentials]\n    operations: 0\n    sources: [https://www.apiable.io/docs/automation/webhooks/]\n    note: docs-only — absent from the published contract\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/scopes/apiable-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Amazon API Gateway
- API Gateway
- API Monetization
- API Portal
- Developer Experience
- Developer Portal
- Kong
- Platform
- Self-Service
token_urls:
- https://developer.apiable.io/api/oauth2/token
---
