---
api_specs:
- filename: thumbtack-demand-openapi.yml
  format: yaml
  label: Thumbtack Demand API
  slug: thumbtack-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-demand-openapi.yml
- filename: thumbtack-pro-openapi.yml
  format: yaml
  label: Thumbtack Pro API
  slug: thumbtack-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/openapi/thumbtack-pro-openapi.yml
authorization_urls:
- https://www.thumbtack.com/services/partner-connect/
description: ''
docs: https://developers.thumbtack.com/docs/getting-started/authentication
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Thumbtack Scopes
name_suffix: OAuth Scopes
note: 'Clients are provisioned either purely demand:: or purely supply:: prefixed scopes, never a mix; per-route required scopes are listed in the API Reference (https://developers.thumbtack.com/docs/getting-started/authentication).'
overview: 'Thumbtack publishes 21 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Thumbtack API on a user''s behalf.


  Tokens are issued from https://api.thumbtack.com/v4/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Thumbtack
provider_slug: thumbtack
schemes:
- description: Used by v4 routes. Authorization Code and Client Credentials flows.
  flows:
  - authorizationUrl: https://www.thumbtack.com/services/partner-connect/
    flow: authorizationCode
    tokenUrl: https://api.thumbtack.com/v4/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.thumbtack.com/v4/oauth/token
  name: oauth2
  source: openapi/thumbtack-demand-openapi.yml
- description: Bearer token obtained via the partner-connect authorization code flow.
  flows:
  - authorizationUrl: https://www.thumbtack.com/services/partner-connect/
    flow: authorizationCode
    tokenUrl: https://pro-api.thumbtack.com/v2/tokens/access
  name: oauth2
  source: openapi/thumbtack-pro-openapi.yml
scope_count: 21
scope_names:
- demand::messages.read
- demand::messages.write
- demand::negotiations.read
- demand::users.read
- demand::users.disconnect
- demand::webhooks.read
- demand::webhooks.write
- demand::orders.read
- demand::orders.write
- demand::orders/availability.read
- demand::categories.read
- demand::keywords.read
- messages
- availability
- bookings
- targeting
- openid
- profile
- email
- phone
- offline_access
scopes:
- description: Read access to messages (Demand API v4, authorization code flow).
  flows: []
  scope: demand::messages.read
- description: Write access to messages (Demand API v4, authorization code flow).
  flows: []
  scope: demand::messages.write
- description: Read access to negotiations (Demand API v4, authorization code flow).
  flows: []
  scope: demand::negotiations.read
- description: Read access to user information (Demand API v4, authorization code flow).
  flows: []
  scope: demand::users.read
- description: Disconnect access to user and revoke tokens (Demand API v4, authorization code flow).
  flows: []
  scope: demand::users.disconnect
- description: Read access to user webhooks (Demand API v4, authorization code flow).
  flows: []
  scope: demand::webhooks.read
- description: Write access to user webhooks (Demand API v4, authorization code flow).
  flows: []
  scope: demand::webhooks.write
- description: Read access to on-demand orders (Demand API v4, client credentials flow).
  flows: []
  scope: demand::orders.read
- description: Write access to on-demand orders (Demand API v4, client credentials flow).
  flows: []
  scope: demand::orders.write
- description: Read access to supply availability for on-demand orders (Demand API v4, client credentials flow).
  flows: []
  scope: demand::orders/availability.read
- description: Read access to categories (Demand API v4, client credentials flow).
  flows: []
  scope: demand::categories.read
- description: Read access to keywords (Demand API v4, client credentials flow).
  flows: []
  scope: demand::keywords.read
- description: Pro API scope allowing partners to send messages on behalf of pros to customers for given leads via the Messages endpoints.
  flows: []
  scope: messages
- description: Pro API scope for accessing pro availability functionality.
  flows: []
  scope: availability
- description: Pro API scope for accessing bookings functionality.
  flows: []
  scope: bookings
- description: Pro API scope for managing a pro's targeting preferences for services and categories (service-based and category-based targeting endpoints).
  flows: []
  scope: targeting
- description: Required OpenID Connect scope; always returns sub (user ID) plus standard claims (iss, aud, exp, iat, at_hash).
  flows: []
  scope: openid
- description: Optional OpenID Connect scope returning the user's name, given_name, family_name, picture, and zoneinfo.
  flows: []
  scope: profile
- description: Optional OpenID Connect scope returning the user's email and email_verified status.
  flows: []
  scope: email
- description: Optional OpenID Connect scope returning the user's phone_number.
  flows: []
  scope: phone
- description: When included in the scope list for the authorization code flow, Thumbtack's authorization server issues a refresh_token alongside the access_token.
  flows: []
  scope: offline_access
slug: thumbtack-scopes
source_filename: thumbtack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/thumbtack-demand-openapi.yml, openapi/thumbtack-pro-openapi.yml\ndocs: https://developers.thumbtack.com/docs/getting-started/authentication\nschemes:\n- name: oauth2\n  source: openapi/thumbtack-demand-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.thumbtack.com/services/partner-connect/\n    tokenUrl: https://api.thumbtack.com/v4/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.thumbtack.com/v4/oauth/token\n  description: Used by v4 routes. Authorization Code and Client Credentials flows.\n- name: oauth2\n  source: openapi/thumbtack-pro-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.thumbtack.com/services/partner-connect/\n    tokenUrl: https://pro-api.thumbtack.com/v2/tokens/access\n  description: Bearer token obtained via the partner-connect authorization code flow.\nscopes:\n- scope: demand::messages.read\n  description:\
  \ Read access to messages (Demand API v4, authorization code flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::messages.write\n  description: Write access to messages (Demand API v4, authorization code flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::negotiations.read\n  description: Read access to negotiations (Demand API v4, authorization code flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::users.read\n  description: Read access to user information (Demand API v4, authorization code\n    flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::users.disconnect\n  description: Disconnect access to user and revoke tokens (Demand API v4, authorization\n    code flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::webhooks.read\n  description: Read access to user webhooks (Demand API v4, authorization code\
  \ flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::webhooks.write\n  description: Write access to user webhooks (Demand API v4, authorization code flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::orders.read\n  description: Read access to on-demand orders (Demand API v4, client credentials\n    flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::orders.write\n  description: Write access to on-demand orders (Demand API v4, client credentials\n    flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::orders/availability.read\n  description: Read access to supply availability for on-demand orders (Demand API\n    v4, client credentials flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: demand::categories.read\n  description: Read access to categories (Demand API v4, client credentials flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n\
  - scope: demand::keywords.read\n  description: Read access to keywords (Demand API v4, client credentials flow).\n  sources:\n  - https://api.thumbtack.com/docs/demand_api.html\n- scope: messages\n  description: Pro API scope allowing partners to send messages on behalf of pros\n    to customers for given leads via the Messages endpoints.\n  sources:\n  - https://pro-api.thumbtack.com/docs/\n- scope: availability\n  description: Pro API scope for accessing pro availability functionality.\n  sources:\n  - https://pro-api.thumbtack.com/docs/\n- scope: bookings\n  description: Pro API scope for accessing bookings functionality.\n  sources:\n  - https://pro-api.thumbtack.com/docs/\n- scope: targeting\n  description: Pro API scope for managing a pro's targeting preferences for services\n    and categories (service-based and category-based targeting endpoints).\n  sources:\n  - https://pro-api.thumbtack.com/docs/\n- scope: openid\n  description: Required OpenID Connect scope; always returns\
  \ sub (user ID) plus standard\n    claims (iss, aud, exp, iat, at_hash).\n  sources:\n  - https://developers.thumbtack.com/docs/getting-started/authentication\n- scope: profile\n  description: Optional OpenID Connect scope returning the user's name, given_name,\n    family_name, picture, and zoneinfo.\n  sources:\n  - https://developers.thumbtack.com/docs/getting-started/authentication\n- scope: email\n  description: Optional OpenID Connect scope returning the user's email and email_verified\n    status.\n  sources:\n  - https://developers.thumbtack.com/docs/getting-started/authentication\n- scope: phone\n  description: Optional OpenID Connect scope returning the user's phone_number.\n  sources:\n  - https://developers.thumbtack.com/docs/getting-started/authentication\n- scope: offline_access\n  description: When included in the scope list for the authorization code flow, Thumbtack's\n    authorization server issues a refresh_token alongside the access_token.\n  sources:\n  - https://developers.thumbtack.com/docs/getting-started/authentication\n\
  note: \"Clients are provisioned either purely demand:: or purely supply:: prefixed\n  scopes, never a mix; per-route required scopes are listed in the API Reference\n  (https://developers.thumbtack.com/docs/getting-started/authentication).\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thumbtack/refs/heads/main/scopes/thumbtack-scopes.yml
summary_line: 21 scopes · authorizationCode/clientCredentials
tags:
- Local Services
- Marketplace
- Home Services
- Leads
- Partner API
token_urls:
- https://api.thumbtack.com/v4/oauth/token
- https://pro-api.thumbtack.com/v2/tokens/access
---
