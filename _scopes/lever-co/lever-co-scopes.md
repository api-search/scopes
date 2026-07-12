---
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
- Webhooks
- OAuth
token_urls:
- https://auth.lever.co/oauth/token
---
