---
api_specs:
- filename: bluecore-openapi.yml
  format: yaml
  label: Bluecore API
  slug: bluecore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.bluecore.com/reference/authn_getaccesstoken
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bluecore Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bluecore publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bluecore API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bluecore
provider_slug: bluecore
schemes: []
scope_count: 7
scope_names:
- customers:read
- customers:write
- eligibility:read
- eligibility:write
- directsend:write
- direct_send:api
- transactional:api
scopes:
- description: Read access to Customer Profiles.
  flows: []
  scope: customers:read
- description: Create or update Customer Profiles (identifiers and attributes).
  flows: []
  scope: customers:write
- description: Read a customer's eligibility / subscription (consent) status.
  flows: []
  scope: eligibility:read
- description: Update a customer's eligibility / subscription (consent) status.
  flows: []
  scope: eligibility:write
- description: Create external direct-send campaigns in Bluecore. (API under construction.)
  flows: []
  scope: directsend:write
- description: Send a direct message via a previously created direct-send campaign. (API under construction.)
  flows: []
  scope: direct_send:api
- description: Send transactional (email/SMS/MMS) messages and retrieve their delivery status.
  flows: []
  scope: transactional:api
slug: bluecore-scopes
source_filename: bluecore-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.bluecore.com/reference/authn_getaccesstoken\ndocs: https://developers.bluecore.com/reference/authn_getaccesstoken\nnotes: >-\n  Bluecore access tokens carry space-delimited scopes in `resource:verb` form (e.g.\n  `customers:write` grants write access to the Customers API), returned in the token\n  response `scope` field. In the per-operation OpenAPI the same permissions appear as\n  dot-form scope strings on each operation's GlooAuth security requirement. Both forms\n  are recorded below.\nscheme:\n  name: GlooAuth\n  flow: clientCredentials\n  token_url: https://auth.bluecore.com/oauth/token\nscopes:\n- scope: customers:read\n  spec_form: customers.read\n  description: Read access to Customer Profiles.\n  operations: [Profile_Get]\n- scope: customers:write\n  spec_form: customers.write\n  description: Create or update Customer Profiles (identifiers and attributes).\n  operations: [Profile_CreateOrUpdate]\n\
  - scope: eligibility:read\n  spec_form: eligibility.read\n  description: Read a customer's eligibility / subscription (consent) status.\n  operations: [Eligibility_Get]\n- scope: eligibility:write\n  spec_form: eligibility.write\n  description: Update a customer's eligibility / subscription (consent) status.\n  operations: [Eligibility_Update]\n- scope: directsend:write\n  spec_form: directsend.write\n  description: Create external direct-send campaigns in Bluecore. (API under construction.)\n  operations: [CampaignsAPIPublic_CreateDirectSendCampaign]\n- scope: direct_send:api\n  spec_form: direct_send.api\n  description: Send a direct message via a previously created direct-send campaign. (API under construction.)\n  operations: [DirectSend_Send]\n- scope: transactional:api\n  spec_form: transactional.api\n  description: Send transactional (email/SMS/MMS) messages and retrieve their delivery status.\n  operations: [Transactional_Send, Transactional_Get]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/scopes/bluecore-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Retail
- Marketing
- Customer Data Platform
- Personalization
- Email
- SMS
- Messaging
- eCommerce
- Consent
token_urls: []
---
