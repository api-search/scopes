---
api_specs:
- filename: nimble-activities-api-openapi.yml
  format: yaml
  label: Nimble Activities API
  slug: nimble-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-activities-api-openapi.yml
- filename: nimble-contacts-api-openapi.yml
  format: yaml
  label: Nimble Contacts API
  slug: nimble-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-contacts-api-openapi.yml
- filename: nimble-contacts-fields-api-openapi.yml
  format: yaml
  label: Nimble Contacts Fields API
  slug: nimble-contacts-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-contacts-fields-api-openapi.yml
- filename: nimble-contacts-pipelines-api-openapi.yml
  format: yaml
  label: Nimble Contacts Pipelines API
  slug: nimble-contacts-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-contacts-pipelines-api-openapi.yml
- filename: nimble-deals-api-openapi.yml
  format: yaml
  label: Nimble Deals API
  slug: nimble-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-api-openapi.yml
- filename: nimble-deals-fields-api-openapi.yml
  format: yaml
  label: Nimble Deals Fields API
  slug: nimble-deals-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-fields-api-openapi.yml
- filename: nimble-deals-pipelines-api-openapi.yml
  format: yaml
  label: Nimble Deals Pipelines API
  slug: nimble-deals-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-pipelines-api-openapi.yml
- filename: nimble-deals-pipelines-fields-api-openapi.yml
  format: yaml
  label: Nimble Deals Pipelines Fields API
  slug: nimble-deals-pipelines-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-pipelines-fields-api-openapi.yml
- filename: nimble-leads-api-openapi.yml
  format: yaml
  label: Nimble Leads API
  slug: nimble-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-leads-api-openapi.yml
- filename: nimble-messages-api-openapi.yml
  format: yaml
  label: Nimble Messages API
  slug: nimble-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-messages-api-openapi.yml
- filename: nimble-tasks-api-openapi.yml
  format: yaml
  label: Nimble Tasks API
  slug: nimble-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-tasks-api-openapi.yml
- filename: nimble-users-api-openapi.yml
  format: yaml
  label: Nimble Users API
  slug: nimble-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-users-api-openapi.yml
authorization_urls:
- https://app.nimble.com/oauth/authorize
description: ''
docs: https://www.nimble.com/developers/docs/#tag/Authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nimble Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nimble publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nimble API on a user''s behalf.


  Tokens are issued from https://app.nimble.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nimble
provider_slug: nimble
schemes:
- declared_in_spec: false
  flows:
  - authorizationUrl: https://app.nimble.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.nimble.com/api/oauth/token
    tokenUrl: https://app.nimble.com/api/oauth/token
  name: OAuth2
  source: https://www.nimble.com/developers/docs/#tag/Authentication
scope_count: 3
scope_names:
- basic
- contacts
- deals
scopes:
- description: User and Company info.
  flows:
  - authorizationCode
  scope: basic
- description: Contacts access — contact records, contact custom fields, field groups and tabs, notes, tags, activities, tasks and contact pipelines.
  flows:
  - authorizationCode
  scope: contacts
- description: Deals access — deals, deal pipelines, deal stages, deal pipeline custom fields, deal tags, files, notes and lead transitions.
  flows:
  - authorizationCode
  scope: deals
slug: nimble-scopes
source_filename: nimble-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.nimble.com/developers/docs/#tag/Authentication\ndocs: https://www.nimble.com/developers/docs/#tag/Authentication\nnotes: >-\n  Nimble's OAuth scope model is coarse — three product-level scopes with no\n  read/write split and no per-resource granularity. An agent granted\n  `contacts` can create, update and delete contacts; there is no read-only\n  variant. Scopes are documented in prose in the Authentication reference;\n  they are NOT declared in the OpenAPI securitySchemes block, which carries\n  only the X-Nimble-Token apiKey scheme with no scopes map.\nschemes:\n  - name: OAuth2\n    source: https://www.nimble.com/developers/docs/#tag/Authentication\n    declared_in_spec: false\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.nimble.com/oauth/authorize\n        tokenUrl: https://app.nimble.com/api/oauth/token\n        refreshUrl: https://app.nimble.com/api/oauth/token\nscope_delimiter:\
  \ >-\n  Comma or plus sign — send as \"basic,contacts,deals\" or\n  \"basic+contacts+deals\" on the authorize request.\nscope_count: 3\nscopes:\n  - scope: basic\n    description: User and Company info.\n    grants:\n      - openapi/nimble-users-api-openapi.yml#get-myself\n    read_write: read\n    flows: [authorizationCode]\n    sources:\n      - https://www.nimble.com/developers/docs/#tag/Authentication\n  - scope: contacts\n    description: >-\n      Contacts access — contact records, contact custom fields, field groups\n      and tabs, notes, tags, activities, tasks and contact pipelines.\n    grants:\n      - openapi/nimble-contacts-api-openapi.yml\n      - openapi/nimble-contacts-fields-api-openapi.yml\n      - openapi/nimble-contacts-pipelines-api-openapi.yml\n    read_write: read-write\n    flows: [authorizationCode]\n    sources:\n      - https://www.nimble.com/developers/docs/#tag/Authentication\n  - scope: deals\n    description: >-\n      Deals access — deals, deal pipelines,\
  \ deal stages, deal pipeline custom\n      fields, deal tags, files, notes and lead transitions.\n    grants:\n      - openapi/nimble-deals-api-openapi.yml\n      - openapi/nimble-deals-fields-api-openapi.yml\n      - openapi/nimble-deals-pipelines-api-openapi.yml\n      - openapi/nimble-deals-pipelines-fields-api-openapi.yml\n      - openapi/nimble-leads-api-openapi.yml\n    read_write: read-write\n    flows: [authorizationCode]\n    sources:\n      - https://www.nimble.com/developers/docs/#tag/Authentication\nunscoped_surfaces:\n  - openapi/nimble-messages-api-openapi.yml\n  - note: >-\n      The Messages (draft) operations are not attributed to any of the three\n      published scopes in the Authentication reference. Mapping above is by\n      the scope names Nimble publishes; where the docs are silent it is\n      recorded as unmapped rather than guessed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/scopes/nimble-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- CRM
- Sales
- Contact Management
- Relationship Management
- Marketing Automation
- Pipeline Management
- Small Business
- Email Marketing
- Sales Automation
- Lead Management
token_urls:
- https://app.nimble.com/api/oauth/token
---
