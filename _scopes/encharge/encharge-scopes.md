---
api_specs:
- filename: encharge-openapi.yml
  format: yaml
  label: Encharge REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/_original/encharge-openapi.yml
- filename: TVRj5o3E
  format: yaml
  label: Encharge Transactional Email API
  slug: transactional-email-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/460427/TVRj5o3E
- filename: SVfNwVFU
  format: yaml
  label: Encharge Ingest API
  slug: ingest-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/460427/SVfNwVFU
- filename: encharge-account-api-openapi.yml
  format: yaml
  label: Encharge Account API
  slug: encharge-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-account-api-openapi.yml
- filename: encharge-broadcasts-api-openapi.yml
  format: yaml
  label: Encharge Broadcasts API
  slug: encharge-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-broadcasts-api-openapi.yml
- filename: encharge-customobjects-api-openapi.yml
  format: yaml
  label: Encharge Custom Objects API
  slug: encharge-customobjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-customobjects-api-openapi.yml
- filename: encharge-customobjectsschema-api-openapi.yml
  format: yaml
  label: Encharge Custom Objects Schema API
  slug: encharge-customobjectsschema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-customobjectsschema-api-openapi.yml
- filename: encharge-emailtemplates-api-openapi.yml
  format: yaml
  label: Encharge Email Templates API
  slug: encharge-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-emailtemplates-api-openapi.yml
- filename: encharge-folders-api-openapi.yml
  format: yaml
  label: Encharge Folders API
  slug: encharge-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-folders-api-openapi.yml
- filename: encharge-people-api-openapi.yml
  format: yaml
  label: Encharge People API
  slug: encharge-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-people-api-openapi.yml
- filename: encharge-personfields-api-openapi.yml
  format: yaml
  label: Encharge Person Fields API
  slug: encharge-personfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-personfields-api-openapi.yml
- filename: encharge-segments-api-openapi.yml
  format: yaml
  label: Encharge Segments API
  slug: encharge-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-segments-api-openapi.yml
- filename: encharge-settings-api-openapi.yml
  format: yaml
  label: Encharge Email Domain Settings API
  slug: encharge-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-settings-api-openapi.yml
- filename: encharge-tags-api-openapi.yml
  format: yaml
  label: Encharge Tags API
  slug: encharge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-tags-api-openapi.yml
- filename: encharge-tags-management-api-openapi.yml
  format: yaml
  label: Encharge Tags Management API
  slug: encharge-tags-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-tags-management-api-openapi.yml
- filename: encharge-webhooks-api-openapi.yml
  format: yaml
  label: Encharge Webhooks API
  slug: encharge-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-webhooks-api-openapi.yml
authorization_urls:
- https://api.encharge.io/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Encharge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Encharge publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Encharge API on a user''s behalf.


  Tokens are issued from https://api.encharge.io/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Encharge
provider_slug: encharge
schemes:
- description: "The Encharge API uses OAuth 2 with the authorization code flow. \n\nGet for your OAuth credentials (Client ID and Client Secret) by filling out [this form](https://research.typeform.com/to/I680YtLA)."
  flows:
  - authorizationUrl: https://api.encharge.io/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.encharge.io/v1/oauth/token
  name: oauth2
  source: openapi/_original/encharge-openapi.yml (13 refined specs carry the same scheme)
scope_count: 8
scope_names:
- account:write
- broadcasts:write
- emailSettings:write
- emails:read
- emails:write
- people:read
- people:write
- personFields:write
scopes:
- description: Account-level writes — webhook/event subscriptions, custom object data and account tag management.
  flows: []
  scope: account:write
- description: Confirm and send broadcasts.
  flows: []
  scope: broadcasts:write
- description: Manage sending email domains and their DNS verification.
  flows: []
  scope: emailSettings:write
- description: Read email templates and their version history.
  flows: []
  scope: emails:read
- description: Create, modify, delete and restore versions of email templates.
  flows: []
  scope: emails:write
- description: Read people and the people in a segment.
  flows: []
  scope: people:read
- description: Create, update, archive, unsubscribe and tag people; create and modify segments.
  flows: []
  scope: people:write
- description: Create, modify and delete person fields and custom-object fields.
  flows: []
  scope: personFields:write
slug: encharge-scopes
source_filename: encharge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/encharge-account-api-openapi.yml, openapi/encharge-broadcasts-api-openapi.yml, openapi/encharge-customobjects-api-openapi.yml,\n  openapi/encharge-customobjectsschema-api-openapi.yml, openapi/encharge-emailtemplates-api-openapi.yml,\n  openapi/encharge-folders-api-openapi.yml, openapi/encharge-people-api-openapi.yml, openapi/encharge-personfields-api-openapi.yml,\n  openapi/encharge-segments-api-openapi.yml, openapi/encharge-settings-api-openapi.yml, openapi/encharge-tags-api-openapi.yml,\n  openapi/encharge-tags-management-api-openapi.yml, openapi/encharge-webhooks-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/_original/encharge-openapi.yml (13 refined specs carry the same scheme)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.encharge.io/v1/oauth/authorize\n    tokenUrl: https://api.encharge.io/v1/oauth/token\n  description: \"The Encharge API uses OAuth 2 with the authorization\
  \ code flow. \\n\\nGet for your OAuth\\\n    \\ credentials (Client ID and Client Secret) by filling out [this form](https://research.typeform.com/to/I680YtLA).\"\nscopes:\n- scope: account:write\n  sources:\n  - openapi/encharge-customobjects-api-openapi.yml\n  - openapi/encharge-customobjectsschema-api-openapi.yml\n  - openapi/encharge-tags-management-api-openapi.yml\n  - openapi/encharge-webhooks-api-openapi.yml\n  description: Account-level writes — webhook/event subscriptions, custom object data and account tag\n    management.\n- scope: broadcasts:write\n  sources:\n  - openapi/encharge-broadcasts-api-openapi.yml\n  description: Confirm and send broadcasts.\n- scope: emailSettings:write\n  sources:\n  - openapi/encharge-settings-api-openapi.yml\n  description: Manage sending email domains and their DNS verification.\n- scope: emails:read\n  sources:\n  - openapi/encharge-emailtemplates-api-openapi.yml\n  description: Read email templates and their version history.\n- scope: emails:write\n\
  \  sources:\n  - openapi/encharge-emailtemplates-api-openapi.yml\n  description: Create, modify, delete and restore versions of email templates.\n- scope: people:read\n  sources:\n  - openapi/encharge-people-api-openapi.yml\n  - openapi/encharge-segments-api-openapi.yml\n  description: Read people and the people in a segment.\n- scope: people:write\n  sources:\n  - openapi/encharge-people-api-openapi.yml\n  - openapi/encharge-segments-api-openapi.yml\n  - openapi/encharge-tags-api-openapi.yml\n  description: Create, update, archive, unsubscribe and tag people; create and modify segments.\n- scope: personFields:write\n  sources:\n  - openapi/encharge-customobjectsschema-api-openapi.yml\n  - openapi/encharge-personfields-api-openapi.yml\n  description: Create, modify and delete person fields and custom-object fields.\ndocs: null\ndocs_note: Encharge publishes NO OAuth scope reference page, and the oauth2 flow in the published OpenAPI\n  declares an EMPTY scopes map. Every scope below was\
  \ read out of the operation-level security[] requirements\n  in the spec, which is the only place they appear. Descriptions are derived from the operations each\n  scope guards, not from provider copy.\noauth_credentials: Client id/secret are issued manually via a request form linked from the spec's oauth2\n  description; there is no self-serve app registration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/scopes/encharge-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Email Marketing
- Marketing Automation
- Transactional Email
- Software-as-a-Service
- Behavioral Email
- Customer Engagement
- Customer Data
- Webhook
token_urls:
- https://api.encharge.io/v1/oauth/token
---
