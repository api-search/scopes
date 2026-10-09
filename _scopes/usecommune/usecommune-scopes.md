---
api_specs:
- filename: usecommune-articles-api-openapi.yml
  format: yaml
  label: Commune Articles API
  slug: usecommune-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-articles-api-openapi.yml
- filename: usecommune-engagement-api-openapi.yml
  format: yaml
  label: Commune Engagement API
  slug: usecommune-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-engagement-api-openapi.yml
- filename: usecommune-event-delivery-api-openapi.yml
  format: yaml
  label: Commune Event delivery API
  slug: usecommune-event-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-event-delivery-api-openapi.yml
- filename: usecommune-highlights-api-openapi.yml
  format: yaml
  label: Commune Highlights API
  slug: usecommune-highlights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-highlights-api-openapi.yml
- filename: usecommune-messages-api-openapi.yml
  format: yaml
  label: Commune Messages API
  slug: usecommune-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-messages-api-openapi.yml
- filename: usecommune-metrics-api-openapi.yml
  format: yaml
  label: Commune Metrics API
  slug: usecommune-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-metrics-api-openapi.yml
- filename: usecommune-newsletters-api-openapi.yml
  format: yaml
  label: Commune Newsletters API
  slug: usecommune-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-newsletters-api-openapi.yml
- filename: usecommune-platform-api-openapi.yml
  format: yaml
  label: Commune Platform API
  slug: usecommune-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-platform-api-openapi.yml
- filename: usecommune-search-api-openapi.yml
  format: yaml
  label: Commune Search API
  slug: usecommune-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-search-api-openapi.yml
- filename: usecommune-senders-api-openapi.yml
  format: yaml
  label: Commune Senders API
  slug: usecommune-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-senders-api-openapi.yml
- filename: usecommune-sends-api-openapi.yml
  format: yaml
  label: Commune Sends API
  slug: usecommune-sends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-sends-api-openapi.yml
- filename: usecommune-subscriber-tags-api-openapi.yml
  format: yaml
  label: Commune Subscriber tags API
  slug: usecommune-subscriber-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-subscriber-tags-api-openapi.yml
- filename: usecommune-subscribers-api-openapi.yml
  format: yaml
  label: Commune Subscribers API
  slug: usecommune-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-subscribers-api-openapi.yml
- filename: usecommune-team-api-openapi.yml
  format: yaml
  label: Commune Team API
  slug: usecommune-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-team-api-openapi.yml
- filename: usecommune-threads-api-openapi.yml
  format: yaml
  label: Commune Threads API
  slug: usecommune-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-threads-api-openapi.yml
- filename: usecommune-users-api-openapi.yml
  format: yaml
  label: Commune Users API
  slug: usecommune-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-users-api-openapi.yml
- filename: usecommune-webhooks-api-openapi.yml
  format: yaml
  label: Commune Webhooks API
  slug: usecommune-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-webhooks-api-openapi.yml
- filename: usecommune-website-domains-api-openapi.yml
  format: yaml
  label: Commune Website domains API
  slug: usecommune-website-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-website-domains-api-openapi.yml
authorization_urls:
- https://usecommune.com/api/oauth/authorize
description: ''
docs: https://usecommune.dev/use-cases/build-an-integration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Usecommune Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Commune publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Commune API on a user''s behalf.


  Tokens are issued from https://usecommune.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Commune
provider_slug: usecommune
schemes:
- description: 'An OAuth access token, sent as `Authorization: Bearer <token>`. The

    walkthrough of the whole flow is at

    [usecommune.dev/use-cases/build-an-integration](https://usecommune.dev/use-cases/build-an-integration):

    discovery, registration, PKCE, the consent screen, the exchange, refresh

    and revocation.


    Ask for a family scope and the person picks which newsletter

    the token reaches; ask for `account:read` alone and it reaches no

    newsletter and reads only the account it belongs to.


    Each operation lists the scopes a token must carry to call it. An

    operation that lists none takes any token.


    Discover the URLs under `flows` at runtime from

    `GET /.well-known/oauth-authorization-server` rather than hardcoding

    them.'
  flows:
  - authorizationUrl: https://usecommune.com/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://usecommune.com/api/oauth/token
  name: oauth2
  source: openapi/usecommune-openapi.yml
scope_count: 14
scope_names:
- account:read
- audience:read
- audience:write
- content:read
- content:write
- insights:read
- insights:write
- sending:read
- sending:write
- settings:read
- settings:write
- webhooks:read
- webhooks:write
- offline_access
scopes:
- description: Read the person the credential belongs to, and nothing about any newsletter.
  flows:
  - authorizationCode
  scope: account:read
- description: Read subscribers, tags and segments, including email addresses.
  flows:
  - authorizationCode
  scope: audience:read
- description: Add, tag and remove subscribers.
  flows:
  - authorizationCode
  scope: audience:write
- description: Read articles, threads and the rest of what a newsletter publishes.
  flows:
  - authorizationCode
  scope: content:read
- description: Create, edit and delete that content.
  flows:
  - authorizationCode
  scope: content:write
- description: Read engagement, delivery and growth figures.
  flows:
  - authorizationCode
  scope: insights:read
- description: Write back an insight the newsletter owns.
  flows:
  - authorizationCode
  scope: insights:write
- description: Read sends, schedules and delivery outcomes.
  flows:
  - authorizationCode
  scope: sending:read
- description: Send an article, schedule one, and cancel a schedule.
  flows:
  - authorizationCode
  scope: sending:write
- description: Read a newsletter's configuration, senders and domains.
  flows:
  - authorizationCode
  scope: settings:read
- description: Change that configuration.
  flows:
  - authorizationCode
  scope: settings:write
- description: Read event destinations and their delivery history.
  flows:
  - authorizationCode
  scope: webhooks:read
- description: Create and remove event destinations.
  flows:
  - authorizationCode
  scope: webhooks:write
- description: Issues a refresh token (grant_types_supported includes refresh_token). Listed in the authorization server metadata scopes_supported but not in the OpenAPI securityScheme.
  flows: []
  scope: offline_access
slug: usecommune-scopes
source_filename: usecommune-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: openapi/usecommune-openapi.yml; https://usecommune.com/.well-known/oauth-authorization-server; https://api.usecommune.com/.well-known/oauth-protected-resource\nschemes:\n- name: oauth2\n  source: openapi/usecommune-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://usecommune.com/api/oauth/authorize\n    tokenUrl: https://usecommune.com/api/oauth/token\n  description: 'An OAuth access token, sent as `Authorization: Bearer <token>`. The\n\n    walkthrough of the whole flow is at\n\n    [usecommune.dev/use-cases/build-an-integration](https://usecommune.dev/use-cases/build-an-integration):\n\n    discovery, registration, PKCE, the consent screen, the exchange, refresh\n\n    and revocation.\n\n\n    Ask for a family scope and the person picks which newsletter\n\n    the token reaches; ask for `account:read` alone and it reaches no\n\n    newsletter and reads only the account it belongs to.\n\n\n\
  \    Each operation lists the scopes a token must carry to call it. An\n\n    operation that lists none takes any token.\n\n\n    Discover the URLs under `flows` at runtime from\n\n    `GET /.well-known/oauth-authorization-server` rather than hardcoding\n\n    them.'\nscopes:\n- scope: account:read\n  description: Read the person the credential belongs to, and nothing about any newsletter.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: audience:read\n  description: Read subscribers, tags and segments, including email addresses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: audience:write\n  description: Add, tag and remove subscribers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: content:read\n  description: Read articles, threads and the rest of what a newsletter publishes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n\
  - scope: content:write\n  description: Create, edit and delete that content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: insights:read\n  description: Read engagement, delivery and growth figures.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: insights:write\n  description: Write back an insight the newsletter owns.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: sending:read\n  description: Read sends, schedules and delivery outcomes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: sending:write\n  description: Send an article, schedule one, and cancel a schedule.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: settings:read\n  description: Read a newsletter's configuration, senders and domains.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n\
  - scope: settings:write\n  description: Change that configuration.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: webhooks:read\n  description: Read event destinations and their delivery history.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: webhooks:write\n  description: Create and remove event destinations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/usecommune-openapi.yml\n- scope: offline_access\n  description: Issues a refresh token (grant_types_supported includes refresh_token). Listed in the authorization\n    server metadata scopes_supported but not in the OpenAPI securityScheme.\n  source: https://usecommune.com/.well-known/oauth-authorization-server\ndocs: https://usecommune.dev/use-cases/build-an-integration\nmodel:\n  families:\n  - content\n  - audience\n  - sending\n  - insights\n  - settings\n  - webhooks\n  levels:\n  - none\n  - read\n  - write\n  rules:\n  - write implies\
  \ read within its own family and nowhere else\n  - permissions are granted per newsletter and bounded live by what the holder can do there\n  - account:read is a separate axis, implied by no family and implying none\n  - an authorization asking only for account:read is granted no newsletter\n  docs: https://api.usecommune.com/openapi.json (info.description, Authentication)\nauthorization_server:\n  issuer: https://usecommune.com\n  authorization_endpoint: https://usecommune.com/api/oauth/authorize\n  token_endpoint: https://usecommune.com/api/oauth/token\n  registration_endpoint: https://usecommune.com/api/oauth/register\n  revocation_endpoint: https://usecommune.com/api/oauth/revoke\n  userinfo_endpoint: https://usecommune.com/api/oauth/userinfo\n  code_challenge_methods_supported:\n  - S256\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  resource_indicators_supported:\
  \ true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/scopes/usecommune-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Newsletters
- Email
- Community
- Publishing
- Creator Economy
- Subscribers
- Webhooks
- MCP
- Analytics
- Content
token_bound: false
token_urls:
- https://usecommune.com/api/oauth/token
---
