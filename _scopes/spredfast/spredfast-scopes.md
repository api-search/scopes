---
api_specs:
- filename: spredfast-conversations-api-openapi.yml
  format: yaml
  label: Spredfast Conversations API (v2)
  slug: spredfast-conversations-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-conversations-api-openapi.yml
- filename: spredfast-conversations-api-v1-openapi.yml
  format: yaml
  label: Spredfast Conversations API (v1)
  slug: spredfast-conversations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-conversations-api-v1-openapi.yml
- filename: spredfast-analytics-api-openapi.yml
  format: yaml
  label: Spredfast Analytics Reporting API
  slug: spredfast-analytics-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-analytics-api-openapi.yml
- filename: spredfast-notification-api-openapi.yml
  format: yaml
  label: Spredfast Notifications (Events) API
  slug: spredfast-notifications-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-notification-api-openapi.yml
- filename: spredfast-experiences-stream-api-openapi.yml
  format: yaml
  label: Spredfast Experiences Stream API
  slug: spredfast-experiences-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-experiences-stream-api-openapi.yml
- filename: spredfast-crm-api-openapi.yml
  format: yaml
  label: Spredfast CRM Registration API
  slug: spredfast-crm-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-crm-api-openapi.yml
- filename: spredfast-custom-crm-callback-api-openapi.yml
  format: yaml
  label: Spredfast Custom CRM Callback Contract
  slug: spredfast-custom-crm-callback-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-custom-crm-callback-api-openapi.yml
- filename: spredfast-labelsets-api-openapi.yml
  format: yaml
  label: Spredfast Label Sets API
  slug: spredfast-label-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-labelsets-api-openapi.yml
- filename: spredfast-introspection-api-openapi.yml
  format: yaml
  label: Spredfast Introspection API
  slug: spredfast-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-introspection-api-openapi.yml
authorization_urls:
- https://login.spredfast.com/v3/oauth/authorize
description: ''
docs: https://developer.khoros.com/khorosmarketingdevdocs
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Spredfast Scopes
name_suffix: OAuth Scopes
note: 'Spredfast / Khoros Marketing publishes exactly ONE OAuth scope: `all`, granting read/write across every endpoint. There is no scopes or permissions reference page on the developer center — searched, none exists — and no per-resource or read-only scope is defined anywhere in the nine harvested contracts. That is the finding: an integration that only needs to read analytics must be issued the same credential that can publish to every connected social account and delete users. There is no least-privilege path available to a customer. Coarse authorization is instead done OUTSIDE OAuth, at the platform layer: a client id is allow-listed per company, and the acting user''s effective permissions are readable at GET /conversations/privilege (`retrieve-permissions-for-current-user`), with roles listed at GET /conversations/roles. Those are runtime permission checks, not token scopes — an issued token does not narrow to them.'
overview: 'Spredfast publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spredfast API on a user''s behalf.


  Tokens are issued from https://login.spredfast.com/v3/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spredfast
provider_slug: spredfast
schemes:
- authoritative: true
  flows:
  - authorizationUrl: https://login.spredfast.com/v3/oauth/authorize
    flow: authorizationCode
    scopes:
      all: Read/write access for all endpoints.
    tokenUrl: https://login.spredfast.com/v3/oauth/token
  name: oauth2
  source: openapi/spredfast-conversations-api-v1-openapi.yml
- authoritative: false
  defect: placeholder-token-url
  name: sec0
  note: Declared in eight of the nine published contracts with tokenUrl https://example.com/oauth2/token and an EMPTY scopes object. example.com is the IANA reserved domain — this is a docs-platform default, not a Spredfast endpoint, and its empty scopes map must not be read as "no scopes required". See authentication/spredfast-authentication.yml.
  sources:
  - openapi/spredfast-conversations-api-openapi.yml
  - openapi/spredfast-analytics-api-openapi.yml
  - openapi/spredfast-crm-api-openapi.yml
  - openapi/spredfast-notification-api-openapi.yml
  - openapi/spredfast-labelsets-api-openapi.yml
  - openapi/spredfast-introspection-api-openapi.yml
  - openapi/spredfast-experiences-stream-api-openapi.yml
scope_count: 1
scope_names:
- all
scopes:
- description: Read/write access for all endpoints.
  flows:
  - authorizationCode
  scope: all
slug: spredfast-scopes
source_filename: spredfast-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api\ndocs: https://developer.khoros.com/khorosmarketingdevdocs\nderived_from:\n- openapi/spredfast-conversations-api-v1-openapi.yml\n- openapi/spredfast-conversations-api-openapi.yml\n- openapi/spredfast-analytics-api-openapi.yml\n- openapi/spredfast-crm-api-openapi.yml\n- openapi/spredfast-notification-api-openapi.yml\n- openapi/spredfast-labelsets-api-openapi.yml\n- openapi/spredfast-introspection-api-openapi.yml\n- openapi/spredfast-experiences-stream-api-openapi.yml\nscope_count: 1\nnote: >-\n  Spredfast / Khoros Marketing publishes exactly ONE OAuth scope: `all`, granting\n  read/write across every endpoint. There is no scopes or permissions reference\n  page on the developer center — searched, none exists — and no per-resource or\n  read-only scope is defined anywhere in the nine harvested contracts. That is\n  the finding:\
  \ an integration that only needs to read analytics must be issued\n  the same credential that can publish to every connected social account and\n  delete users. There is no least-privilege path available to a customer.\n  Coarse authorization is instead done OUTSIDE OAuth, at the platform layer:\n  a client id is allow-listed per company, and the acting user's effective\n  permissions are readable at GET /conversations/privilege\n  (`retrieve-permissions-for-current-user`), with roles listed at\n  GET /conversations/roles. Those are runtime permission checks, not token\n  scopes — an issued token does not narrow to them.\nscopes:\n- scope: all\n  description: Read/write access for all endpoints.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spredfast-conversations-api-v1-openapi.yml\nschemes:\n- name: oauth2\n  authoritative: true\n  source: openapi/spredfast-conversations-api-v1-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.spredfast.com/v3/oauth/authorize\n\
  \    tokenUrl: https://login.spredfast.com/v3/oauth/token\n    scopes:\n      all: Read/write access for all endpoints.\n- name: sec0\n  authoritative: false\n  defect: placeholder-token-url\n  note: >-\n    Declared in eight of the nine published contracts with tokenUrl\n    https://example.com/oauth2/token and an EMPTY scopes object. example.com is\n    the IANA reserved domain — this is a docs-platform default, not a Spredfast\n    endpoint, and its empty scopes map must not be read as \"no scopes required\".\n    See authentication/spredfast-authentication.yml.\n  sources:\n  - openapi/spredfast-conversations-api-openapi.yml\n  - openapi/spredfast-analytics-api-openapi.yml\n  - openapi/spredfast-crm-api-openapi.yml\n  - openapi/spredfast-notification-api-openapi.yml\n  - openapi/spredfast-labelsets-api-openapi.yml\n  - openapi/spredfast-introspection-api-openapi.yml\n  - openapi/spredfast-experiences-stream-api-openapi.yml\nplatform_permissions:\n  note: >-\n    Not OAuth scopes, but\
  \ the only authorization granularity that exists.\n  operations:\n  - operationId: retrieve-permissions-for-current-user\n    path: GET /conversations/privilege\n    description: The acting user's effective privilege set.\n  - operationId: list-roles-for-the-company\n    path: GET /conversations/roles\n    description: Named permission bundles assigned to users.\n  - operationId: list-conversations-publishers\n    path: GET /conversations/users/initiative/{initiativeId}/publishers\n    description: The subset of users permitted to publish to an initiative.\n  spec: openapi/spredfast-conversations-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/scopes/spredfast-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Social-Media
- Social Media Management
- Marketing
- Social Marketing
- Publishing
- Analytics
- Engagement
- Content Management
- Webhook
- Event
- Enterprise
token_urls:
- https://login.spredfast.com/v3/oauth/token
---
