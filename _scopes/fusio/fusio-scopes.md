---
api_specs:
- filename: fusio-backend.json
  format: json
  label: Fusio Backend API
  slug: fusio-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-backend.json
- filename: fusio-consumer.json
  format: json
  label: Fusio Consumer API
  slug: fusio-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-consumer.json
- filename: fusio-system.json
  format: json
  label: Fusio System API
  slug: fusio-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-system.json
- filename: fusio-authorization.json
  format: json
  label: Fusio Authorization API
  slug: fusio-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-authorization.json
authorization_urls:
- https://demo.fusio-project.org/authorization/authorize
description: 'Fusio''s scope model is namespaced by category and then by resource: ''backend'' grants the whole backend surface, ''backend.operation'' grants only the operation resource within it, and the same shape repeats for ''consumer''. Scopes are instance data, not product constants - an operator creates their own alongside these through backend.scope.create - so this list is the 58 scopes Fusio''s own reference instance defines for its management surface. Personal access tokens can be issued against any subset.'
docs: https://docs.fusio-project.org/docs/security/authorization
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Fusio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fusio publishes 58 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fusio API on a user''s behalf.


  Tokens are issued from https://demo.fusio-project.org/authorization/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fusio
provider_slug: fusio
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://demo.fusio-project.org/authorization/token
  - authorizationUrl: https://demo.fusio-project.org/authorization/authorize
    flow: authorizationCode
    tokenUrl: https://demo.fusio-project.org/authorization/token
  name: app
  source: openapi/fusio-authorization.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://demo.fusio-project.org/authorization/token
  - authorizationUrl: https://demo.fusio-project.org/authorization/authorize
    flow: authorizationCode
    tokenUrl: https://demo.fusio-project.org/authorization/token
  name: app
  source: openapi/fusio-backend.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://demo.fusio-project.org/authorization/token
  - authorizationUrl: https://demo.fusio-project.org/authorization/authorize
    flow: authorizationCode
    tokenUrl: https://demo.fusio-project.org/authorization/token
  name: app
  source: openapi/fusio-consumer.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://demo.fusio-project.org/authorization/token
  - authorizationUrl: https://demo.fusio-project.org/authorization/authorize
    flow: authorizationCode
    tokenUrl: https://demo.fusio-project.org/authorization/token
  name: app
  source: openapi/fusio-system.json
scope_count: 58
scope_names:
- authorization
- backend
- backend.account
- backend.action
- backend.agent
- backend.app
- backend.audit
- backend.backup
- backend.bundle
- backend.category
- backend.config
- backend.connection
- backend.cronjob
- backend.dashboard
- backend.event
- backend.firewall
- backend.form
- backend.generator
- backend.identity
- backend.log
- backend.marketplace
- backend.operation
- backend.page
- backend.plan
- backend.rate
- backend.role
- backend.schema
- backend.scope
- backend.sdk
- backend.specification
- backend.statistic
- backend.taxonomy
- backend.tenant
- backend.test
- backend.token
- backend.transaction
- backend.trash
- backend.trigger
- backend.user
- backend.webhook
- consumer
- consumer.account
- consumer.agent
- consumer.app
- consumer.event
- consumer.form
- consumer.grant
- consumer.identity
- consumer.log
- consumer.page
- consumer.payment
- consumer.plan
- consumer.scope
- consumer.token
- consumer.transaction
- consumer.webhook
- openid
- system
scopes:
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: authorization
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.account
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.action
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.agent
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.app
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.audit
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.backup
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.bundle
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.category
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.config
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.connection
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.cronjob
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.dashboard
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.event
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.firewall
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.form
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.generator
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.identity
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.log
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.marketplace
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.operation
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.page
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.plan
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.rate
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.role
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.schema
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.scope
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.sdk
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.specification
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.statistic
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.taxonomy
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.tenant
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.test
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.token
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.transaction
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.trash
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.trigger
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.user
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: backend.webhook
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.account
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.agent
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.app
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.event
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.form
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.grant
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.identity
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.log
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.page
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.payment
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.plan
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.scope
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.token
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.transaction
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: consumer.webhook
- description: OpenID scope
  flows:
  - authorizationCode
  - clientCredentials
  scope: openid
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: system
slug: fusio-scopes
source_filename: fusio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: openapi/fusio-authorization.json, openapi/fusio-backend.json, openapi/fusio-consumer.json, openapi/fusio-system.json;\n  scope semantics from https://docs.fusio-project.org/docs/security/authorization, https://docs.fusio-project.org/docs/security/personal_access_token\n  and https://docs.fusio-project.org/docs/backend/system/role\nschemes:\n- name: app\n  source: openapi/fusio-authorization.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://demo.fusio-project.org/authorization/token\n  - flow: authorizationCode\n    authorizationUrl: https://demo.fusio-project.org/authorization/authorize\n    tokenUrl: https://demo.fusio-project.org/authorization/token\n- name: app\n  source: openapi/fusio-backend.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://demo.fusio-project.org/authorization/token\n  - flow: authorizationCode\n    authorizationUrl: https://demo.fusio-project.org/authorization/authorize\n\
  \    tokenUrl: https://demo.fusio-project.org/authorization/token\n- name: app\n  source: openapi/fusio-consumer.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://demo.fusio-project.org/authorization/token\n  - flow: authorizationCode\n    authorizationUrl: https://demo.fusio-project.org/authorization/authorize\n    tokenUrl: https://demo.fusio-project.org/authorization/token\n- name: app\n  source: openapi/fusio-system.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://demo.fusio-project.org/authorization/token\n  - flow: authorizationCode\n    authorizationUrl: https://demo.fusio-project.org/authorization/authorize\n    tokenUrl: https://demo.fusio-project.org/authorization/token\nscopes:\n- scope: authorization\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-authorization.json\n- scope: backend\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.account\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.action\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.agent\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.app\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.audit\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.backup\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.bundle\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.category\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.config\n \
  \ flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.connection\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.cronjob\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.dashboard\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.event\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.firewall\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.form\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.generator\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.identity\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.log\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.marketplace\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.operation\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.page\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.plan\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.rate\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.role\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.schema\n \
  \ flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.scope\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.sdk\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.specification\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.statistic\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.taxonomy\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.tenant\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.test\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.token\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.transaction\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.trash\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.trigger\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.user\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: backend.webhook\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-backend.json\n- scope: consumer\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.account\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.agent\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.app\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.event\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.form\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.grant\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.identity\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.log\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.page\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.payment\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.plan\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.scope\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.token\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.transaction\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: consumer.webhook\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-consumer.json\n- scope: openid\n  description: OpenID scope\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-authorization.json\n- scope: system\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fusio-system.json\n\
  provider: Fusio\nproviderId: fusio\ndocs: https://docs.fusio-project.org/docs/security/authorization\ndescription: 'Fusio''s scope model is namespaced by category and then by resource: ''backend'' grants\n  the whole backend surface, ''backend.operation'' grants only the operation resource within it, and the\n  same shape repeats for ''consumer''. Scopes are instance data, not product constants - an operator creates\n  their own alongside these through backend.scope.create - so this list is the 58 scopes Fusio''s own\n  reference instance defines for its management surface. Personal access tokens can be issued against\n  any subset.'\nnamespaces:\n- prefix: backend\n  grants: the entire backend management surface\n  narrower: backend.<resource>\n- prefix: consumer\n  grants: the entire developer-portal surface\n  narrower: consumer.<resource>\n- prefix: system\n  grants: meta, health, route table and spec generation\n- prefix: authorization\n  grants: token introspection and revocation\n\
  - prefix: openid\n  grants: OIDC claims when Fusio acts as an identity provider\n- prefix: default\n  grants: the scope every app receives; the only one advertised anonymously\nroles_note: Scopes are granted to a user through a ROLE (backend.role.*), and a role belongs to a category.\n  An operator assigns scopes to roles rather than to users directly.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/scopes/fusio-scopes.yml
summary_line: 58 scopes · clientCredentials/authorizationCode
tags:
- API Management
- Open-Source
- REST API
- API Gateway
- Developer Portal
- OpenAPI
- Self-Hosted
- MCP
token_urls:
- https://demo.fusio-project.org/authorization/token
---
