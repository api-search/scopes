---
authorization_urls: []
description: ''
docs: https://docs.clutchcall.dev/platform/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: ClutchCall Scopes
name_suffix: OAuth Scopes
note: Scope form is mcp:<domain>:<action>; "There is no scope that permits everything." List is scopes_supported from the live Protected Resource Metadata (HTTP 200, 2026-11-04). Control-plane API-key capability scopes are not enumerated in the docs.
overview: 'ClutchCall publishes 41 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClutchCall API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClutchCall
provider_slug: clutchcall-dev
schemes: []
scope_count: 41
scope_names:
- mcp:catalog:read
- mcp:telephony:read
- mcp:telephony:write
- mcp:telephony:delete
- mcp:cdr:read
- mcp:cdr:write
- mcp:cdr:delete
- mcp:reports:read
- mcp:reports:write
- mcp:reports:delete
- mcp:agents:read
- mcp:agents:write
- mcp:agents:delete
- mcp:ai:read
- mcp:ai:write
- mcp:ai:delete
- mcp:billing:read
- mcp:billing:write
- mcp:billing:delete
- mcp:media:read
- mcp:media:write
- mcp:media:delete
- mcp:robotics:read
- mcp:robotics:write
- mcp:robotics:delete
- mcp:infra:read
- mcp:infra:write
- mcp:infra:delete
- mcp:compute:read
- mcp:compute:write
- mcp:compute:delete
- mcp:sms:read
- mcp:sms:write
- mcp:sms:delete
- mcp:tags:read
- mcp:tags:write
- mcp:tags:delete
- mcp:security:read
- mcp:security:admin
- mcp:keys:read
- mcp:keys:admin
scopes:
- description: 'Queries. A `read` scope can never change data. (domain: catalog)'
  flows: []
  scope: mcp:catalog:read
- description: 'Queries. A `read` scope can never change data. (domain: telephony)'
  flows: []
  scope: mcp:telephony:read
- description: 'Mutations that create or update. (domain: telephony)'
  flows: []
  scope: mcp:telephony:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: telephony)'
  flows: []
  scope: mcp:telephony:delete
- description: 'Queries. A `read` scope can never change data. (domain: cdr)'
  flows: []
  scope: mcp:cdr:read
- description: 'Mutations that create or update. (domain: cdr)'
  flows: []
  scope: mcp:cdr:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: cdr)'
  flows: []
  scope: mcp:cdr:delete
- description: 'Queries. A `read` scope can never change data. (domain: reports)'
  flows: []
  scope: mcp:reports:read
- description: 'Mutations that create or update. (domain: reports)'
  flows: []
  scope: mcp:reports:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: reports)'
  flows: []
  scope: mcp:reports:delete
- description: 'Queries. A `read` scope can never change data. (domain: agents)'
  flows: []
  scope: mcp:agents:read
- description: 'Mutations that create or update. (domain: agents)'
  flows: []
  scope: mcp:agents:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: agents)'
  flows: []
  scope: mcp:agents:delete
- description: 'Queries. A `read` scope can never change data. (domain: ai)'
  flows: []
  scope: mcp:ai:read
- description: 'Mutations that create or update. (domain: ai)'
  flows: []
  scope: mcp:ai:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: ai)'
  flows: []
  scope: mcp:ai:delete
- description: 'Queries. A `read` scope can never change data. (domain: billing)'
  flows: []
  scope: mcp:billing:read
- description: 'Mutations that create or update. (domain: billing)'
  flows: []
  scope: mcp:billing:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: billing)'
  flows: []
  scope: mcp:billing:delete
- description: 'Queries. A `read` scope can never change data. (domain: media)'
  flows: []
  scope: mcp:media:read
- description: 'Mutations that create or update. (domain: media)'
  flows: []
  scope: mcp:media:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: media)'
  flows: []
  scope: mcp:media:delete
- description: 'Queries. A `read` scope can never change data. (domain: robotics)'
  flows: []
  scope: mcp:robotics:read
- description: 'Mutations that create or update. (domain: robotics)'
  flows: []
  scope: mcp:robotics:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: robotics)'
  flows: []
  scope: mcp:robotics:delete
- description: 'Queries. A `read` scope can never change data. (domain: infra)'
  flows: []
  scope: mcp:infra:read
- description: 'Mutations that create or update. (domain: infra)'
  flows: []
  scope: mcp:infra:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: infra)'
  flows: []
  scope: mcp:infra:delete
- description: 'Queries. A `read` scope can never change data. (domain: compute)'
  flows: []
  scope: mcp:compute:read
- description: 'Mutations that create or update. (domain: compute)'
  flows: []
  scope: mcp:compute:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: compute)'
  flows: []
  scope: mcp:compute:delete
- description: 'Queries. A `read` scope can never change data. (domain: sms)'
  flows: []
  scope: mcp:sms:read
- description: 'Mutations that create or update. (domain: sms)'
  flows: []
  scope: mcp:sms:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: sms)'
  flows: []
  scope: mcp:sms:delete
- description: 'Queries. A `read` scope can never change data. (domain: tags)'
  flows: []
  scope: mcp:tags:read
- description: 'Mutations that create or update. (domain: tags)'
  flows: []
  scope: mcp:tags:write
- description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: tags)'
  flows: []
  scope: mcp:tags:delete
- description: 'Queries. A `read` scope can never change data. (domain: security)'
  flows: []
  scope: mcp:security:read
- description: 'Every mutation in the `security` and `keys` domains. (domain: security)'
  flows: []
  scope: mcp:security:admin
- description: 'Queries. A `read` scope can never change data. (domain: keys)'
  flows: []
  scope: mcp:keys:read
- description: 'Every mutation in the `security` and `keys` domains. (domain: keys)'
  flows: []
  scope: mcp:keys:admin
slug: clutchcall-dev-scopes
source_filename: clutchcall-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://portal.clutchcall.dev/.well-known/oauth-protected-resource\ndocs: https://docs.clutchcall.dev/platform/mcp\nnote: Scope form is mcp:<domain>:<action>; \"There is no scope that permits everything.\" List is scopes_supported from the live Protected Resource Metadata (HTTP 200, 2026-11-04). Control-plane API-key capability\n  scopes are not enumerated in the docs.\nscopes:\n- name: mcp:catalog:read\n  description: 'Queries. A `read` scope can never change data. (domain: catalog)'\n- name: mcp:telephony:read\n  description: 'Queries. A `read` scope can never change data. (domain: telephony)'\n- name: mcp:telephony:write\n  description: 'Mutations that create or update. (domain: telephony)'\n- name: mcp:telephony:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: telephony)'\n- name: mcp:cdr:read\n  description: 'Queries. A `read` scope can never change data. (domain:\
  \ cdr)'\n- name: mcp:cdr:write\n  description: 'Mutations that create or update. (domain: cdr)'\n- name: mcp:cdr:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: cdr)'\n- name: mcp:reports:read\n  description: 'Queries. A `read` scope can never change data. (domain: reports)'\n- name: mcp:reports:write\n  description: 'Mutations that create or update. (domain: reports)'\n- name: mcp:reports:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: reports)'\n- name: mcp:agents:read\n  description: 'Queries. A `read` scope can never change data. (domain: agents)'\n- name: mcp:agents:write\n  description: 'Mutations that create or update. (domain: agents)'\n- name: mcp:agents:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: agents)'\n- name: mcp:ai:read\n  description: 'Queries. A `read` scope can never change data. (domain: ai)'\n\
  - name: mcp:ai:write\n  description: 'Mutations that create or update. (domain: ai)'\n- name: mcp:ai:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: ai)'\n- name: mcp:billing:read\n  description: 'Queries. A `read` scope can never change data. (domain: billing)'\n- name: mcp:billing:write\n  description: 'Mutations that create or update. (domain: billing)'\n- name: mcp:billing:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: billing)'\n- name: mcp:media:read\n  description: 'Queries. A `read` scope can never change data. (domain: media)'\n- name: mcp:media:write\n  description: 'Mutations that create or update. (domain: media)'\n- name: mcp:media:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: media)'\n- name: mcp:robotics:read\n  description: 'Queries. A `read` scope can never change data. (domain: robotics)'\n- name:\
  \ mcp:robotics:write\n  description: 'Mutations that create or update. (domain: robotics)'\n- name: mcp:robotics:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: robotics)'\n- name: mcp:infra:read\n  description: 'Queries. A `read` scope can never change data. (domain: infra)'\n- name: mcp:infra:write\n  description: 'Mutations that create or update. (domain: infra)'\n- name: mcp:infra:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: infra)'\n- name: mcp:compute:read\n  description: 'Queries. A `read` scope can never change data. (domain: compute)'\n- name: mcp:compute:write\n  description: 'Mutations that create or update. (domain: compute)'\n- name: mcp:compute:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: compute)'\n- name: mcp:sms:read\n  description: 'Queries. A `read` scope can never change data. (domain: sms)'\n\
  - name: mcp:sms:write\n  description: 'Mutations that create or update. (domain: sms)'\n- name: mcp:sms:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: sms)'\n- name: mcp:tags:read\n  description: 'Queries. A `read` scope can never change data. (domain: tags)'\n- name: mcp:tags:write\n  description: 'Mutations that create or update. (domain: tags)'\n- name: mcp:tags:delete\n  description: 'Mutations that destroy or revoke. A `write` scope does not permit these. (domain: tags)'\n- name: mcp:security:read\n  description: 'Queries. A `read` scope can never change data. (domain: security)'\n- name: mcp:security:admin\n  description: 'Every mutation in the `security` and `keys` domains. (domain: security)'\n- name: mcp:keys:read\n  description: 'Queries. A `read` scope can never change data. (domain: keys)'\n- name: mcp:keys:admin\n  description: 'Every mutation in the `security` and `keys` domains. (domain: keys)'\n"
source_yaml_url: https://artifacts.apis.io/clutchcall-dev/scopes/clutchcall-dev-scopes.yml
summary_line: 41 scopes
tags:
- Company
- Voice AI
- Real-Time Communication
- QUIC
- Telephony
- SIP
- Live Streaming
- Robotics
- Inference
- WebTransport
token_bound: false
token_urls: []
---
