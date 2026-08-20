---
api_specs:
- filename: lever-webhooks-asyncapi.yml
  format: yaml
  label: Lever Webhooks
  slug: lever-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-webhooks-asyncapi.yml
- filename: lever-co-applications-api-openapi.yml
  format: yaml
  label: Lever Applications API
  slug: lever-co-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-applications-api-openapi.yml
- filename: lever-co-archive-reasons-api-openapi.yml
  format: yaml
  label: Lever Archive Reasons API
  slug: lever-co-archive-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-archive-reasons-api-openapi.yml
- filename: lever-co-audit-events-api-openapi.yml
  format: yaml
  label: Lever Audit Events API
  slug: lever-co-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-audit-events-api-openapi.yml
- filename: lever-co-eeo-responses-api-openapi.yml
  format: yaml
  label: Lever EEO Responses API
  slug: lever-co-eeo-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-eeo-responses-api-openapi.yml
- filename: lever-co-feedback-api-openapi.yml
  format: yaml
  label: Lever Feedback API
  slug: lever-co-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-feedback-api-openapi.yml
- filename: lever-co-files-api-openapi.yml
  format: yaml
  label: Lever Files API
  slug: lever-co-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-files-api-openapi.yml
- filename: lever-co-interviews-api-openapi.yml
  format: yaml
  label: Lever Interviews API
  slug: lever-co-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-interviews-api-openapi.yml
- filename: lever-co-notes-api-openapi.yml
  format: yaml
  label: Lever Notes API
  slug: lever-co-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-notes-api-openapi.yml
- filename: lever-co-offers-api-openapi.yml
  format: yaml
  label: Lever Offers API
  slug: lever-co-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-offers-api-openapi.yml
- filename: lever-co-opportunities-api-openapi.yml
  format: yaml
  label: Lever Opportunities API
  slug: lever-co-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-opportunities-api-openapi.yml
- filename: lever-co-panels-api-openapi.yml
  format: yaml
  label: Lever Panels API
  slug: lever-co-panels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-panels-api-openapi.yml
- filename: lever-co-postings-api-openapi.yml
  format: yaml
  label: Lever Postings API
  slug: lever-co-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-postings-api-openapi.yml
- filename: lever-co-requisitions-api-openapi.yml
  format: yaml
  label: Lever Requisitions API
  slug: lever-co-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-requisitions-api-openapi.yml
- filename: lever-co-sources-api-openapi.yml
  format: yaml
  label: Lever Sources API
  slug: lever-co-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-sources-api-openapi.yml
- filename: lever-co-stages-api-openapi.yml
  format: yaml
  label: Lever Stages API
  slug: lever-co-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-stages-api-openapi.yml
- filename: lever-co-tags-api-openapi.yml
  format: yaml
  label: Lever Tags API
  slug: lever-co-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-tags-api-openapi.yml
- filename: lever-co-users-api-openapi.yml
  format: yaml
  label: Lever Users API
  slug: lever-co-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-users-api-openapi.yml
- filename: lever-co-webhooks-api-openapi.yml
  format: yaml
  label: Lever Webhooks API
  slug: lever-co-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-webhooks-api-openapi.yml
authorization_urls:
- https://auth.lever.co/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Lever Co Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lever publishes 22 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lever API on a user''s behalf.


  Tokens are issued from https://auth.lever.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lever
provider_slug: lever-co
schemes:
- flows:
  - authorizationUrl: https://auth.lever.co/authorize
    flow: authorizationCode
    tokenUrl: https://auth.lever.co/oauth/token
  name: OAuth2
  source: openapi/lever-data-api-openapi.yml
scope_count: 22
scope_names:
- audit_events:read:admin
- confidential:access:admin
- eeo_responses:read:admin
- eeo_responses_pii:read:admin
- feedback:read:admin
- feedback:write:admin
- files:read:admin
- files:write:admin
- interviews:read:admin
- interviews:write:admin
- offers:read:admin
- offline_access
- opportunities:read:admin
- opportunities:write:admin
- postings:read:admin
- postings:write:admin
- requisitions:read:admin
- requisitions:write:admin
- users:read:admin
- users:write:admin
- webhooks:read:admin
- webhooks:write:admin
scopes:
- description: Read audit log events.
  flows:
  - authorizationCode
  scope: audit_events:read:admin
- description: Access confidential records.
  flows:
  - authorizationCode
  scope: confidential:access:admin
- description: Read EEO survey responses.
  flows:
  - authorizationCode
  scope: eeo_responses:read:admin
- description: Read EEO survey responses with PII.
  flows:
  - authorizationCode
  scope: eeo_responses_pii:read:admin
- description: Read feedback.
  flows:
  - authorizationCode
  scope: feedback:read:admin
- description: Write feedback.
  flows:
  - authorizationCode
  scope: feedback:write:admin
- description: Read files.
  flows:
  - authorizationCode
  scope: files:read:admin
- description: Write files.
  flows:
  - authorizationCode
  scope: files:write:admin
- description: Read interviews.
  flows:
  - authorizationCode
  scope: interviews:read:admin
- description: Write interviews.
  flows:
  - authorizationCode
  scope: interviews:write:admin
- description: Read offers.
  flows:
  - authorizationCode
  scope: offers:read:admin
- description: Issue refresh tokens.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read opportunities.
  flows:
  - authorizationCode
  scope: opportunities:read:admin
- description: Write opportunities.
  flows:
  - authorizationCode
  scope: opportunities:write:admin
- description: Read postings.
  flows:
  - authorizationCode
  scope: postings:read:admin
- description: Write postings.
  flows:
  - authorizationCode
  scope: postings:write:admin
- description: Read requisitions.
  flows:
  - authorizationCode
  scope: requisitions:read:admin
- description: Write requisitions.
  flows:
  - authorizationCode
  scope: requisitions:write:admin
- description: Read users.
  flows:
  - authorizationCode
  scope: users:read:admin
- description: Write users.
  flows:
  - authorizationCode
  scope: users:write:admin
- description: Read webhook subscriptions.
  flows:
  - authorizationCode
  scope: webhooks:read:admin
- description: Write webhook subscriptions.
  flows:
  - authorizationCode
  scope: webhooks:write:admin
slug: lever-co-scopes
source_filename: lever-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lever-data-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/lever-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.lever.co/authorize\n    tokenUrl: https://auth.lever.co/oauth/token\nscopes:\n- scope: audit_events:read:admin\n  description: Read audit log events.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: confidential:access:admin\n  description: Access confidential records.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: eeo_responses:read:admin\n  description: Read EEO survey responses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: eeo_responses_pii:read:admin\n  description: Read EEO survey responses with PII.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: feedback:read:admin\n\
  \  description: Read feedback.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: feedback:write:admin\n  description: Write feedback.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: files:read:admin\n  description: Read files.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: files:write:admin\n  description: Write files.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: interviews:read:admin\n  description: Read interviews.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: interviews:write:admin\n  description: Write interviews.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: offers:read:admin\n  description: Read offers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope:\
  \ offline_access\n  description: Issue refresh tokens.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: opportunities:read:admin\n  description: Read opportunities.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: opportunities:write:admin\n  description: Write opportunities.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: postings:read:admin\n  description: Read postings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: postings:write:admin\n  description: Write postings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: requisitions:read:admin\n  description: Read requisitions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: requisitions:write:admin\n  description: Write requisitions.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: users:read:admin\n  description: Read users.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: users:write:admin\n  description: Write users.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: webhooks:read:admin\n  description: Read webhook subscriptions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- scope: webhooks:write:admin\n  description: Write webhook subscriptions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lever-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/scopes/lever-co-scopes.yml
summary_line: 22 scopes · authorizationCode
tags:
- Applicant Tracking
- ATS
- CRM
- Recruiting
- Hiring
- Talent Acquisition
- Human Resources
- HR Tech
- Postings
- Webhook
- Authentication
token_urls:
- https://auth.lever.co/oauth/token
---
