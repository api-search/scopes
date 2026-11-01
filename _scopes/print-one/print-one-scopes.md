---
api_specs:
- filename: print-one-address-api-openapi.yml
  format: yaml
  label: print-one Address API
  slug: print-one-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-address-api-openapi.yml
- filename: print-one-campaigns-api-openapi.yml
  format: yaml
  label: print-one Campaigns API
  slug: print-one-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-campaigns-api-openapi.yml
- filename: print-one-coupons-api-openapi.yml
  format: yaml
  label: print-one Coupons API
  slug: print-one-coupons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-coupons-api-openapi.yml
- filename: print-one-design-previews-api-openapi.yml
  format: yaml
  label: print-one Design Previews API
  slug: print-one-design-previews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-design-previews-api-openapi.yml
- filename: print-one-designs-api-openapi.yml
  format: yaml
  label: print-one Designs API
  slug: print-one-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-designs-api-openapi.yml
- filename: print-one-imports-api-openapi.yml
  format: yaml
  label: print-one Imports API
  slug: print-one-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-imports-api-openapi.yml
- filename: print-one-items-api-openapi.yml
  format: yaml
  label: print-one Items API
  slug: print-one-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-items-api-openapi.yml
- filename: print-one-mailings-api-openapi.yml
  format: yaml
  label: print-one Mailings API
  slug: print-one-mailings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-mailings-api-openapi.yml
- filename: print-one-webhooks-api-openapi.yml
  format: yaml
  label: print-one Webhooks API
  slug: print-one-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-webhooks-api-openapi.yml
- filename: print-one-webhook-events-api-openapi.yml
  format: yaml
  label: print-one Webhook Events API
  slug: print-one-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-webhook-events-api-openapi.yml
authorization_urls:
- https://api.print.one/v2/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Print One Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'print-one publishes 30 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the print-one API on a user''s behalf.


  Tokens are issued from https://api.print.one/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: print-one
provider_slug: print-one
schemes:
- flows:
  - authorizationUrl: https://api.print.one/v2/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.print.one/v2/oauth/token
  name: Oauth2
  source: openapi/print-one-openapi.json
scope_count: 30
scope_names:
- campaign.delete
- campaign.read
- campaign.write
- company.read
- coupons.read
- coupons.write
- customfile.read
- customfile.write
- draft.orders.read
- draft.orders.write
- integrations.read
- live.api.key
- live.batches.read
- live.batches.write
- live.orders.read
- live.orders.write
- shorten.urls.read
- shorten.urls.write
- template.read
- template.write
- tenant.admin
- test.api.key
- test.batches.read
- test.batches.write
- test.orders.read
- test.orders.write
- tracking.event.read
- tracking.event.write
- webhooks.read
- webhooks.write
scopes:
- description: campaign.delete
  flows:
  - authorizationCode
  scope: campaign.delete
- description: campaign.read
  flows:
  - authorizationCode
  scope: campaign.read
- description: campaign.write
  flows:
  - authorizationCode
  scope: campaign.write
- description: company.read
  flows:
  - authorizationCode
  scope: company.read
- description: coupons.read
  flows:
  - authorizationCode
  scope: coupons.read
- description: coupons.write
  flows:
  - authorizationCode
  scope: coupons.write
- description: customfile.read
  flows:
  - authorizationCode
  scope: customfile.read
- description: customfile.write
  flows:
  - authorizationCode
  scope: customfile.write
- description: draft.orders.read
  flows:
  - authorizationCode
  scope: draft.orders.read
- description: draft.orders.write
  flows:
  - authorizationCode
  scope: draft.orders.write
- description: integrations.read
  flows:
  - authorizationCode
  scope: integrations.read
- description: live.api.key
  flows:
  - authorizationCode
  scope: live.api.key
- description: live.batches.read
  flows:
  - authorizationCode
  scope: live.batches.read
- description: live.batches.write
  flows:
  - authorizationCode
  scope: live.batches.write
- description: live.orders.read
  flows:
  - authorizationCode
  scope: live.orders.read
- description: live.orders.write
  flows:
  - authorizationCode
  scope: live.orders.write
- description: shorten.urls.read
  flows:
  - authorizationCode
  scope: shorten.urls.read
- description: shorten.urls.write
  flows:
  - authorizationCode
  scope: shorten.urls.write
- description: template.read
  flows:
  - authorizationCode
  scope: template.read
- description: template.write
  flows:
  - authorizationCode
  scope: template.write
- description: tenant.admin
  flows:
  - authorizationCode
  scope: tenant.admin
- description: test.api.key
  flows:
  - authorizationCode
  scope: test.api.key
- description: test.batches.read
  flows:
  - authorizationCode
  scope: test.batches.read
- description: test.batches.write
  flows:
  - authorizationCode
  scope: test.batches.write
- description: test.orders.read
  flows:
  - authorizationCode
  scope: test.orders.read
- description: test.orders.write
  flows:
  - authorizationCode
  scope: test.orders.write
- description: tracking.event.read
  flows:
  - authorizationCode
  scope: tracking.event.read
- description: tracking.event.write
  flows:
  - authorizationCode
  scope: tracking.event.write
- description: webhooks.read
  flows:
  - authorizationCode
  scope: webhooks.read
- description: webhooks.write
  flows:
  - authorizationCode
  scope: webhooks.write
slug: print-one-scopes
source_filename: print-one-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/print-one-openapi.json\nschemes:\n- name: Oauth2\n  source: openapi/print-one-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.print.one/v2/oauth/authorize\n    tokenUrl: https://api.print.one/v2/oauth/token\nscopes:\n- scope: campaign.delete\n  description: campaign.delete\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: campaign.read\n  description: campaign.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: campaign.write\n  description: campaign.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: company.read\n  description: company.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: coupons.read\n  description: coupons.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n\
  - scope: coupons.write\n  description: coupons.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: customfile.read\n  description: customfile.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: customfile.write\n  description: customfile.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: draft.orders.read\n  description: draft.orders.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: draft.orders.write\n  description: draft.orders.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: integrations.read\n  description: integrations.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: live.api.key\n  description: live.api.key\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: live.batches.read\n\
  \  description: live.batches.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: live.batches.write\n  description: live.batches.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: live.orders.read\n  description: live.orders.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: live.orders.write\n  description: live.orders.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: shorten.urls.read\n  description: shorten.urls.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: shorten.urls.write\n  description: shorten.urls.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: template.read\n  description: template.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: template.write\n  description:\
  \ template.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: tenant.admin\n  description: tenant.admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: test.api.key\n  description: test.api.key\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: test.batches.read\n  description: test.batches.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: test.batches.write\n  description: test.batches.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: test.orders.read\n  description: test.orders.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: test.orders.write\n  description: test.orders.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: tracking.event.read\n  description: tracking.event.read\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: tracking.event.write\n  description: tracking.event.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: webhooks.read\n  description: webhooks.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n- scope: webhooks.write\n  description: webhooks.write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/print-one-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/print-one/scopes/print-one-scopes.yml
summary_line: 30 scopes · authorizationCode
tags:
- Postcards
- API
- Direct Mail
- Marketing
- Automation
token_bound: false
token_urls:
- https://api.print.one/v2/oauth/token
---
