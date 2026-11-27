---
api_specs:
- filename: buymeacoffee-webhooks-openapi.json
  format: json
  label: Buy Me a Coffee Webhooks
  slug: buymeacoffee-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buymeacoffee/openapi/buymeacoffee-webhooks-openapi.json
- filename: buymeacoffee.postman_collection.json
  format: json
  label: Buy Me a Coffee Extras API
  slug: buymeacoffee-extras-api
  spec_type: Postman
  url: https://artifacts.apis.io/buymeacoffee/collections/buymeacoffee.postman_collection.json
- filename: buymeacoffee.postman_collection.json
  format: json
  label: Buy Me a Coffee Subscriptions API
  slug: buymeacoffee-subscriptions-api
  spec_type: Postman
  url: https://artifacts.apis.io/buymeacoffee/collections/buymeacoffee.postman_collection.json
- filename: buymeacoffee.postman_collection.json
  format: json
  label: Buy Me a Coffee Supporters API
  slug: buymeacoffee-supporters-api
  spec_type: Postman
  url: https://artifacts.apis.io/buymeacoffee/collections/buymeacoffee.postman_collection.json
authorization_urls: []
description: ''
docs: https://developers.buymeacoffee.com/#/?id=scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Buy Me a Coffee Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Buy Me a Coffee publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Buy Me a Coffee API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Buy Me a Coffee
provider_slug: buymeacoffee
schemes: []
scope_count: 1
scope_names:
- read-only
scopes:
- description: '"read-only access to the user''s public information and products." This is the only scope the developer portal currently offers. The docs add: "Scopes with write permissions will be launched soon stay tuned to our creator community for more information."'
  flows: []
  scope: read-only
slug: buymeacoffee-scopes
source_filename: buymeacoffee-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: searched\nsource: https://developers.buymeacoffee.com/#/?id=scopes\ndocs: https://developers.buymeacoffee.com/#/?id=scopes\nscopes:\n- name: read-only\n  description: >-\n    \"read-only access to the user's public information and products.\" This\n    is the only scope the developer portal currently offers. The docs add:\n    \"Scopes with write permissions will be launched soon stay tuned to our\n    creator community for more information.\"\n  source: https://developers.buymeacoffee.com/#/?id=scopes\nnotes: >-\n  Buy Me a Coffee's developer portal describes OAuth-style scopes but the\n  actual access flow is personal-access-token (Bearer). Every token created\n  in the dashboard is implicitly bound to the `read-only` scope. The portal\n  flags write scopes as \"coming soon\" but no date is published.\n"
source_yaml_url: https://artifacts.apis.io/buymeacoffee/scopes/buymeacoffee-scopes.yml
summary_line: 1 scope
tags:
- Creator Economy
- Membership
- Subscription
- Tips
- Payments
- Donations
token_bound: false
token_urls: []
---
