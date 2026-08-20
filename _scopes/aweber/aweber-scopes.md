---
api_specs:
- filename: aweber-accounts-api-openapi.yml
  format: yaml
  label: AWeber Accounts API
  slug: aweber-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-accounts-api-openapi.yml
- filename: aweber-broadcasts-api-openapi.yml
  format: yaml
  label: AWeber Broadcasts API
  slug: aweber-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-broadcasts-api-openapi.yml
- filename: aweber-campaigns-api-openapi.yml
  format: yaml
  label: AWeber Campaigns API
  slug: aweber-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-campaigns-api-openapi.yml
- filename: aweber-custom-fields-api-openapi.yml
  format: yaml
  label: AWeber Custom Fields API
  slug: aweber-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-custom-fields-api-openapi.yml
- filename: aweber-landing-pages-api-openapi.yml
  format: yaml
  label: AWeber Landing Pages API
  slug: aweber-landing-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-landing-pages-api-openapi.yml
- filename: aweber-lists-api-openapi.yml
  format: yaml
  label: AWeber Lists API
  slug: aweber-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-lists-api-openapi.yml
- filename: aweber-segments-api-openapi.yml
  format: yaml
  label: AWeber Segments API
  slug: aweber-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-segments-api-openapi.yml
- filename: aweber-subscribers-api-openapi.yml
  format: yaml
  label: AWeber Subscribers API
  slug: aweber-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-subscribers-api-openapi.yml
- filename: aweber-web-forms-api-openapi.yml
  format: yaml
  label: AWeber Web Forms API
  slug: aweber-web-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-web-forms-api-openapi.yml
- filename: aweber-integrations-api-openapi.yml
  format: yaml
  label: AWeber Integrations API
  slug: aweber-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-integrations-api-openapi.yml
- filename: aweber-authentication-api-openapi.yml
  format: yaml
  label: AWeber Authentication API
  slug: aweber-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-authentication-api-openapi.yml
- filename: aweber-beta-api-openapi.yml
  format: yaml
  label: AWeber Beta API
  slug: aweber-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/openapi/aweber-beta-api-openapi.yml
authorization_urls:
- https://auth.aweber.com/oauth2/authorize
description: ''
docs: https://api.aweber.com/#tag/OAuth-2.0-Overview
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Aweber Scopes
name_suffix: OAuth Scopes
note: 'Nine scopes, all declared in the provider''s own OpenAPI securitySchemes and all documented with the exact endpoints each one unlocks — an unusually complete scope reference. Descriptions below are AWeber''s, with the inline HTML stripped and the endpoint lists split out as `required_for` so they are readable as data. Scopes are space-separated and URL-encoded on the authorize URL. Note the deprecation: subscriber.read-extended has been equivalent to subscriber.read since API 1.1.0 (2021-06-16) and should not be requested in new code.'
overview: 'AWeber publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AWeber API on a user''s behalf.


  Tokens are issued from https://auth.aweber.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AWeber
provider_slug: aweber
schemes:
- flows:
  - authorizationUrl: https://auth.aweber.com/oauth2/authorize
    flow: authorizationCode
    pkce: required-for-public-clients
    refreshUrl: https://auth.aweber.com/oauth2/token
    revokeUrl: https://auth.aweber.com/oauth2/revoke
    tokenUrl: https://auth.aweber.com/oauth2/token
  name: OAuth 2.0
  source: openapi/_original/aweber-api-openapi.yml
  type: oauth2
scope_count: 9
scope_names:
- account.read
- list.read
- list.write
- subscriber.read
- subscriber.write
- subscriber.read-extended
- email.read
- email.write
- landing-page.read
scopes:
- description: Access account information and associated integrations.
  flows:
  - authorizationCode
  scope: account.read
- description: Retrieve lists, custom fields, tags, and sign up forms.
  flows:
  - authorizationCode
  scope: list.read
- description: Create, edit, and delete custom fields.
  flows:
  - authorizationCode
  scope: list.write
- description: Retrieve subscribers and their activity.
  flows:
  - authorizationCode
  scope: subscriber.read
- description: Create, edit, delete, retrieve, search for, and move subscribers.
  flows:
  - authorizationCode
  scope: subscriber.write
- description: Previously required to retrieve subscriber PII such as name, email and IP address. That functionality moved to the subscriber.read scope.
  flows:
  - authorizationCode
  scope: subscriber.read-extended
- description: Retrieve email activity related to broadcasts and follow-ups.
  flows:
  - authorizationCode
  scope: email.read
- description: Create and send email broadcasts.
  flows:
  - authorizationCode
  scope: email.write
- description: Retrieve landing pages.
  flows:
  - authorizationCode
  scope: landing-page.read
slug: aweber-scopes
source_filename: aweber-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/aweber-api-openapi.yml\ndocs: https://api.aweber.com/#tag/OAuth-2.0-Overview\ndocs_alt: https://help.aweber.com/hc/en-us/articles/360021487653\nnote: >-\n  Nine scopes, all declared in the provider's own OpenAPI securitySchemes and all documented with\n  the exact endpoints each one unlocks — an unusually complete scope reference. Descriptions\n  below are AWeber's, with the inline HTML stripped and the endpoint lists split out as\n  `required_for` so they are readable as data. Scopes are space-separated and URL-encoded on the\n  authorize URL. Note the deprecation: subscriber.read-extended has been equivalent to\n  subscriber.read since API 1.1.0 (2021-06-16) and should not be requested in new code.\nschemes:\n  - name: OAuth 2.0\n    type: oauth2\n    source: openapi/_original/aweber-api-openapi.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.aweber.com/oauth2/authorize\n\
  \        tokenUrl: https://auth.aweber.com/oauth2/token\n        refreshUrl: https://auth.aweber.com/oauth2/token\n        revokeUrl: https://auth.aweber.com/oauth2/revoke\n        pkce: required-for-public-clients\nscope_count: 9\nscopes:\n  - scope: account.read\n    description: Access account information and associated integrations.\n    flows: [authorizationCode]\n    required_for: [get accounts, get account, get integrations, get integration]\n  - scope: list.read\n    description: Retrieve lists, custom fields, tags, and sign up forms.\n    flows: [authorizationCode]\n    required_for: [get list, get lists, find lists, get tags for list, get custom fields,\n                   get custom field, get webforms for list, get split tests for list,\n                   get split test components, get split test component, get webforms for account,\n                   get split tests for account]\n  - scope: list.write\n    description: Create, edit, and delete custom fields.\n    flows:\
  \ [authorizationCode]\n    required_for: [add custom field, update custom field, delete custom field]\n  - scope: subscriber.read\n    description: Retrieve subscribers and their activity.\n    flows: [authorizationCode]\n    required_for: [get subscribers, get subscriber, get subscriber activity,\n                   get subscribers for message, find subscribers for account,\n                   find subscribers for list]\n    note: Also required (with account.read) to authorize a webhooks-enabled integration.\n  - scope: subscriber.write\n    description: Create, edit, delete, retrieve, search for, and move subscribers.\n    flows: [authorizationCode]\n    required_for: [add subscriber, move subscriber, update subscriber, delete subscriber]\n  - scope: subscriber.read-extended\n    description: >-\n      Previously required to retrieve subscriber PII such as name, email and IP address. That\n      functionality moved to the subscriber.read scope.\n    flows: [authorizationCode]\n    status:\
  \ deprecated\n    superseded_by: subscriber.read\n    deprecated_since: '2021-06-16'\n    note: >-\n      Still accepted, but equivalent to subscriber.read. Tokens that already held it were\n      implicitly granted subscriber.read.\n  - scope: email.read\n    description: Retrieve email activity related to broadcasts and follow-ups.\n    flows: [authorizationCode]\n    required_for: [get messages, get message, get broadcasts, get broadcast, get message opens,\n                   get message open, get message tracked events, get message tracked event,\n                   get total broadcasts, get campaigns, get campaign, find campaigns,\n                   get broadcast statistics, get broadcast statistic]\n  - scope: email.write\n    description: Create and send email broadcasts.\n    flows: [authorizationCode]\n    required_for: [create broadcast, update broadcast, delete broadcast, cancel broadcast,\n                   schedule broadcast]\n    note: >-\n      The AWeber customer must\
  \ additionally grant the \"Manage All Email Communications\"\n      permission; without it these calls return 403 \"Application not authorized to manage email.\"\n  - scope: landing-page.read\n    description: Retrieve landing pages.\n    flows: [authorizationCode]\n    required_for: [get landing pages, get landing page]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aweber/refs/heads/main/scopes/aweber-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Email Marketing
- Marketing Automation
- Email
- Newsletters
- Subscribers
- Campaigns
- Landing Pages
- Web Forms
- Segments
- Webhook
- Authentication
- Small Business
token_urls:
- https://auth.aweber.com/oauth2/token
---
