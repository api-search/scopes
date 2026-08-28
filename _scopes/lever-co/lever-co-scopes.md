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
description: OAuth 2.0 scopes an application can request against the Lever Data API. Scopes follow a resource:access:role convention where role is always `admin` (Lever grants integrations admin-level access to a resource, not a per-user subset). `offline_access` is requested at the /authorize step to receive a refresh token. Basic Auth API keys do NOT use scopes — key permissions are configured per key in the Lever account Integrations and API settings, including a separate grant for confidential data that can only be given at key-creation time.
docs: https://hire.lever.co/developer/documentation
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lever Co Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lever publishes 52 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lever API on a user''s behalf.


  Tokens are issued from https://auth.lever.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lever
provider_slug: lever-co
schemes:
- flows:
  - audience: https://api.lever.co/v1/
    authorizationUrl: https://auth.lever.co/authorize
    flow: authorizationCode
    refresh_tokens: Request the offline_access scope to receive a refresh_token.
    sandbox_authorizationUrl: https://sandbox-lever.auth0.com/authorize
    tokenUrl: https://auth.lever.co/oauth/token
    token_lifetime_seconds: 3600
  name: OAuth2
  sources:
  - https://hire.lever.co/developer/documentation
  - https://hire.lever.co/developer/oauth
  type: oauth2
scope_count: 52
scope_names:
- offline_access
- applications:read:admin
- archive_reasons:read:admin
- audit_events:read:admin
- confidential:access:admin
- contact:read:admin
- contact:write:admin
- diversity_surveys:read:admin
- eeo_responses:read:admin
- eeo_responses_pii:read:admin
- feedback:read:admin
- feedback:write:admin
- feedback_templates:read:admin
- feedback_templates:write:admin
- files:read:admin
- files:write:admin
- forms:read:admin
- forms:write:admin
- form_templates:read:admin
- form_templates:write:admin
- groups:read:admin
- groups:write:admin
- interviews:read:admin
- interviews:write:admin
- notes:read:admin
- notes:write:admin
- offers:read:admin
- opportunities:read:admin
- opportunities:write:admin
- panels:read:admin
- panels:write:admin
- permissions:read:admin
- permissions:write:admin
- postings:read:admin
- postings:write:admin
- referrals:read:admin
- requisitions:read:admin
- requisitions:write:admin
- requisition_fields:read:admin
- requisition_fields:write:admin
- resumes:read:admin
- roles:read:admin
- roles:write:admin
- sources:read:admin
- stages:read:admin
- tags:read:admin
- tasks:read:admin
- uploads:write:admin
- users:read:admin
- users:write:admin
- webhooks:read:admin
- webhooks:write:admin
scopes:
- description: Include this scope in the authorize call in order to get a refresh token during the token exchange.
  flows:
  - authorizationCode
  scope: offline_access
- description: View all opportunity applications.
  flows:
  - authorizationCode
  scope: applications:read:admin
- description: View all archived reasons.
  flows:
  - authorizationCode
  scope: archive_reasons:read:admin
- description: View all audit events.
  flows:
  - authorizationCode
  scope: audit_events:read:admin
- description: Access all confidential data.
  flows:
  - authorizationCode
  scope: confidential:access:admin
- description: View an opportunity's contact.
  flows:
  - authorizationCode
  scope: contact:read:admin
- description: View and manage an opportunity's contact.
  flows:
  - authorizationCode
  scope: contact:write:admin
- description: View all diversity surveys.
  flows:
  - authorizationCode
  scope: diversity_surveys:read:admin
- description: View all EEO responses without personally identifiable information.
  flows:
  - authorizationCode
  scope: eeo_responses:read:admin
- description: View all EEO responses with or without personally identifiable information.
  flows:
  - authorizationCode
  scope: eeo_responses_pii:read:admin
- description: View all of an opportunity's feedback.
  flows:
  - authorizationCode
  scope: feedback:read:admin
- description: View and manage all of an opportunity's feedback.
  flows:
  - authorizationCode
  scope: feedback:write:admin
- description: View all feedback templates.
  flows:
  - authorizationCode
  scope: feedback_templates:read:admin
- description: View and manage all feedback templates.
  flows:
  - authorizationCode
  scope: feedback_templates:write:admin
- description: View all of an opportunity's files.
  flows:
  - authorizationCode
  scope: files:read:admin
- description: View and manage all of an opportunity's files.
  flows:
  - authorizationCode
  scope: files:write:admin
- description: View all of an opportunity's forms.
  flows:
  - authorizationCode
  scope: forms:read:admin
- description: View and manage all of an opportunity's forms.
  flows:
  - authorizationCode
  scope: forms:write:admin
- description: View all form templates.
  flows:
  - authorizationCode
  scope: form_templates:read:admin
- description: View and manage all form templates.
  flows:
  - authorizationCode
  scope: form_templates:write:admin
- description: View all user groups.
  flows:
  - authorizationCode
  scope: groups:read:admin
- description: View and manage all user groups.
  flows:
  - authorizationCode
  scope: groups:write:admin
- description: View all of an opportunity's interviews.
  flows:
  - authorizationCode
  scope: interviews:read:admin
- description: View and manage all of an opportunity's interviews.
  flows:
  - authorizationCode
  scope: interviews:write:admin
- description: View all of an opportunity's notes.
  flows:
  - authorizationCode
  scope: notes:read:admin
- description: View and manage all of an opportunity's notes.
  flows:
  - authorizationCode
  scope: notes:write:admin
- description: View all of an opportunity's offers.
  flows:
  - authorizationCode
  scope: offers:read:admin
- description: View all opportunities.
  flows:
  - authorizationCode
  scope: opportunities:read:admin
- description: View and manage all opportunities.
  flows:
  - authorizationCode
  scope: opportunities:write:admin
- description: View all of an opportunity's panels.
  flows:
  - authorizationCode
  scope: panels:read:admin
- description: View and manage all of an opportunity's panels.
  flows:
  - authorizationCode
  scope: panels:write:admin
- description: View all user or role permissions.
  flows:
  - authorizationCode
  scope: permissions:read:admin
- description: View and manage all user or role permissions.
  flows:
  - authorizationCode
  scope: permissions:write:admin
- description: View all postings.
  flows:
  - authorizationCode
  scope: postings:read:admin
- description: View and manage all postings.
  flows:
  - authorizationCode
  scope: postings:write:admin
- description: View all of an opportunity's referrals.
  flows:
  - authorizationCode
  scope: referrals:read:admin
- description: View all requisitions.
  flows:
  - authorizationCode
  scope: requisitions:read:admin
- description: View and manage all requisitions.
  flows:
  - authorizationCode
  scope: requisitions:write:admin
- description: View all requisition fields.
  flows:
  - authorizationCode
  scope: requisition_fields:read:admin
- description: View and manage all requisition fields.
  flows:
  - authorizationCode
  scope: requisition_fields:write:admin
- description: View all of an opportunity's resumes.
  flows:
  - authorizationCode
  scope: resumes:read:admin
- description: View all roles.
  flows:
  - authorizationCode
  scope: roles:read:admin
- description: View and manage all roles.
  flows:
  - authorizationCode
  scope: roles:write:admin
- description: View all sources.
  flows:
  - authorizationCode
  scope: sources:read:admin
- description: View all stages.
  flows:
  - authorizationCode
  scope: stages:read:admin
- description: View all tags.
  flows:
  - authorizationCode
  scope: tags:read:admin
- description: View all tasks.
  flows:
  - authorizationCode
  scope: tasks:read:admin
- description: Manage all file uploads.
  flows:
  - authorizationCode
  scope: uploads:write:admin
- description: View all users.
  flows:
  - authorizationCode
  scope: users:read:admin
- description: View and manage all users.
  flows:
  - authorizationCode
  scope: users:write:admin
- description: View all webhooks.
  flows:
  - authorizationCode
  scope: webhooks:read:admin
- description: Manage all webhooks.
  flows:
  - authorizationCode
  scope: webhooks:write:admin
slug: lever-co-scopes
source_filename: lever-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://hire.lever.co/developer/documentation#scopes — the complete OAuth scope reference published on the\n  Lever Data API documentation page (fetched 2026-08-26, HTTP 200). Baseline derived from openapi/*.yml securitySchemes\n  with 0-working/derive-oauth-scopes.py, then upgraded with the full published list.\ndocs: https://hire.lever.co/developer/documentation\ndescription: OAuth 2.0 scopes an application can request against the Lever Data API. Scopes follow a resource:access:role\n  convention where role is always `admin` (Lever grants integrations admin-level access to a resource, not a per-user\n  subset). `offline_access` is requested at the /authorize step to receive a refresh token. Basic Auth API keys\n  do NOT use scopes — key permissions are configured per key in the Lever account Integrations and API settings,\n  including a separate grant for confidential data that can only be given at key-creation time.\nschemes:\n\
  - name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.lever.co/authorize\n    tokenUrl: https://auth.lever.co/oauth/token\n    audience: https://api.lever.co/v1/\n    sandbox_authorizationUrl: https://sandbox-lever.auth0.com/authorize\n    token_lifetime_seconds: 3600\n    refresh_tokens: Request the offline_access scope to receive a refresh_token.\n  sources:\n  - https://hire.lever.co/developer/documentation\n  - https://hire.lever.co/developer/oauth\nscope_count: 52\nscopes:\n- scope: offline_access\n  description: Include this scope in the authorize call in order to get a refresh token during the token exchange.\n  flows:\n  - authorizationCode\n- scope: applications:read:admin\n  description: View all opportunity applications.\n  flows:\n  - authorizationCode\n- scope: archive_reasons:read:admin\n  description: View all archived reasons.\n  flows:\n  - authorizationCode\n- scope: audit_events:read:admin\n  description: View all audit\
  \ events.\n  flows:\n  - authorizationCode\n- scope: confidential:access:admin\n  description: Access all confidential data.\n  flows:\n  - authorizationCode\n- scope: contact:read:admin\n  description: View an opportunity's contact.\n  flows:\n  - authorizationCode\n- scope: contact:write:admin\n  description: View and manage an opportunity's contact.\n  flows:\n  - authorizationCode\n- scope: diversity_surveys:read:admin\n  description: View all diversity surveys.\n  flows:\n  - authorizationCode\n- scope: eeo_responses:read:admin\n  description: View all EEO responses without personally identifiable information.\n  flows:\n  - authorizationCode\n- scope: eeo_responses_pii:read:admin\n  description: View all EEO responses with or without personally identifiable information.\n  flows:\n  - authorizationCode\n- scope: feedback:read:admin\n  description: View all of an opportunity's feedback.\n  flows:\n  - authorizationCode\n- scope: feedback:write:admin\n  description: View and manage\
  \ all of an opportunity's feedback.\n  flows:\n  - authorizationCode\n- scope: feedback_templates:read:admin\n  description: View all feedback templates.\n  flows:\n  - authorizationCode\n- scope: feedback_templates:write:admin\n  description: View and manage all feedback templates.\n  flows:\n  - authorizationCode\n- scope: files:read:admin\n  description: View all of an opportunity's files.\n  flows:\n  - authorizationCode\n- scope: files:write:admin\n  description: View and manage all of an opportunity's files.\n  flows:\n  - authorizationCode\n- scope: forms:read:admin\n  description: View all of an opportunity's forms.\n  flows:\n  - authorizationCode\n- scope: forms:write:admin\n  description: View and manage all of an opportunity's forms.\n  flows:\n  - authorizationCode\n- scope: form_templates:read:admin\n  description: View all form templates.\n  flows:\n  - authorizationCode\n- scope: form_templates:write:admin\n  description: View and manage all form templates.\n  flows:\n\
  \  - authorizationCode\n- scope: groups:read:admin\n  description: View all user groups.\n  flows:\n  - authorizationCode\n- scope: groups:write:admin\n  description: View and manage all user groups.\n  flows:\n  - authorizationCode\n- scope: interviews:read:admin\n  description: View all of an opportunity's interviews.\n  flows:\n  - authorizationCode\n- scope: interviews:write:admin\n  description: View and manage all of an opportunity's interviews.\n  flows:\n  - authorizationCode\n- scope: notes:read:admin\n  description: View all of an opportunity's notes.\n  flows:\n  - authorizationCode\n- scope: notes:write:admin\n  description: View and manage all of an opportunity's notes.\n  flows:\n  - authorizationCode\n- scope: offers:read:admin\n  description: View all of an opportunity's offers.\n  flows:\n  - authorizationCode\n- scope: opportunities:read:admin\n  description: View all opportunities.\n  flows:\n  - authorizationCode\n- scope: opportunities:write:admin\n  description: View\
  \ and manage all opportunities.\n  flows:\n  - authorizationCode\n- scope: panels:read:admin\n  description: View all of an opportunity's panels.\n  flows:\n  - authorizationCode\n- scope: panels:write:admin\n  description: View and manage all of an opportunity's panels.\n  flows:\n  - authorizationCode\n- scope: permissions:read:admin\n  description: View all user or role permissions.\n  flows:\n  - authorizationCode\n- scope: permissions:write:admin\n  description: View and manage all user or role permissions.\n  flows:\n  - authorizationCode\n- scope: postings:read:admin\n  description: View all postings.\n  flows:\n  - authorizationCode\n- scope: postings:write:admin\n  description: View and manage all postings.\n  flows:\n  - authorizationCode\n- scope: referrals:read:admin\n  description: View all of an opportunity's referrals.\n  flows:\n  - authorizationCode\n- scope: requisitions:read:admin\n  description: View all requisitions.\n  flows:\n  - authorizationCode\n- scope: requisitions:write:admin\n\
  \  description: View and manage all requisitions.\n  flows:\n  - authorizationCode\n- scope: requisition_fields:read:admin\n  description: View all requisition fields.\n  flows:\n  - authorizationCode\n- scope: requisition_fields:write:admin\n  description: View and manage all requisition fields.\n  flows:\n  - authorizationCode\n- scope: resumes:read:admin\n  description: View all of an opportunity's resumes.\n  flows:\n  - authorizationCode\n- scope: roles:read:admin\n  description: View all roles.\n  flows:\n  - authorizationCode\n- scope: roles:write:admin\n  description: View and manage all roles.\n  flows:\n  - authorizationCode\n- scope: sources:read:admin\n  description: View all sources.\n  flows:\n  - authorizationCode\n- scope: stages:read:admin\n  description: View all stages.\n  flows:\n  - authorizationCode\n- scope: tags:read:admin\n  description: View all tags.\n  flows:\n  - authorizationCode\n- scope: tasks:read:admin\n  description: View all tasks.\n  flows:\n  - authorizationCode\n\
  - scope: uploads:write:admin\n  description: Manage all file uploads.\n  flows:\n  - authorizationCode\n- scope: users:read:admin\n  description: View all users.\n  flows:\n  - authorizationCode\n- scope: users:write:admin\n  description: View and manage all users.\n  flows:\n  - authorizationCode\n- scope: webhooks:read:admin\n  description: View all webhooks.\n  flows:\n  - authorizationCode\n- scope: webhooks:write:admin\n  description: Manage all webhooks.\n  flows:\n  - authorizationCode\nnotes:\n- 'OAuth registration is gated: apps must be approved through the Lever partner program before Lever issues a client_id/secret\n  (https://hire.lever.co/developer/partner).'\n- The `audience` query parameter (https://api.lever.co/v1/) is REQUIRED on the /authorize call; omitting it is the\n  most common integration failure and the published Postman collection omits it, so its auth tab only works against\n  sandbox.\n- confidential:access:admin only returns confidential postings/opportunities/requisitions\
  \ when the underlying credential\n  was also granted confidential access.\n- Requisitions endpoints (requisitions:*, requisition_fields:*) require the customer to hold the Lever TRM Enterprise\n  package or the Advanced HR feature.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/scopes/lever-co-scopes.yml
summary_line: 52 scopes · authorizationCode
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
