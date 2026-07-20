---
authorization_urls: []
description: ''
docs: https://developer.fourth.com/en-gb/docs/authenticating-oauth
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Fourth Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fourth publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fourth API on a user''s behalf.


  Tokens are issued from [ROOT]/oauth/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fourth
provider_slug: fourth
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: '[ROOT]/oauth/connect/token'
  name: OAuth2
scope_count: 1
scope_names:
- NotificationService
scopes:
- description: Access to the Fourth Notifications API.
  flows:
  - clientCredentials
  scope: NotificationService
slug: fourth-scopes
source_filename: fourth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.fourth.com/en-gb/docs/authenticating-oauth\ndocs: https://developer.fourth.com/en-gb/docs/authenticating-oauth\nschemes:\n- name: OAuth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: '[ROOT]/oauth/connect/token'\nscopes:\n- scope: NotificationService\n  description: Access to the Fourth Notifications API.\n  flows: [clientCredentials]\n  api: Notifications API\nnotes: >-\n  Fourth documents OAuth scopes per-API on each reference page under the\n  Authentication heading; only NotificationService is given as a published\n  example in the OAuth guide. Additional per-API scopes exist on the individual\n  reference pages but production hosts/specs are not publicly disclosed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fourth/refs/heads/main/scopes/fourth-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Workforce Management
- Restaurants
- Hospitality
- Inventory Management
- Payroll
- Scheduling
- Human Capital Management
- Point of Sale
- Food and Beverage
token_urls:
- '[ROOT]/oauth/connect/token'
---
