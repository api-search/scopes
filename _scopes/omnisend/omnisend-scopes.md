---
api_specs:
- filename: omnisend-analytics-api-openapi.yml
  format: yaml
  label: Omnisend Analytics API
  slug: omnisend-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-analytics-api-openapi.yml
- filename: omnisend-batches-api-openapi.yml
  format: yaml
  label: Omnisend Batches API
  slug: omnisend-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-batches-api-openapi.yml
- filename: omnisend-brands-api-openapi.yml
  format: yaml
  label: Omnisend Brands API
  slug: omnisend-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-brands-api-openapi.yml
- filename: omnisend-campaigns-api-openapi.yml
  format: yaml
  label: Omnisend Campaigns API
  slug: omnisend-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-campaigns-api-openapi.yml
- filename: omnisend-contacts-api-openapi.yml
  format: yaml
  label: Omnisend Contacts API
  slug: omnisend-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-contacts-api-openapi.yml
- filename: omnisend-emailcontent-api-openapi.yml
  format: yaml
  label: Omnisend EmailContent API
  slug: omnisend-emailcontent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-emailcontent-api-openapi.yml
- filename: omnisend-emailtemplates-api-openapi.yml
  format: yaml
  label: Omnisend EmailTemplates API
  slug: omnisend-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-emailtemplates-api-openapi.yml
- filename: omnisend-emailuniversallayouts-api-openapi.yml
  format: yaml
  label: Omnisend EmailUniversalLayouts API
  slug: omnisend-emailuniversallayouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-emailuniversallayouts-api-openapi.yml
- filename: omnisend-events-api-openapi.yml
  format: yaml
  label: Omnisend Events API
  slug: omnisend-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-events-api-openapi.yml
- filename: omnisend-images-api-openapi.yml
  format: yaml
  label: Omnisend Images API
  slug: omnisend-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-images-api-openapi.yml
- filename: omnisend-productcategories-api-openapi.yml
  format: yaml
  label: Omnisend ProductCategories API
  slug: omnisend-productcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-productcategories-api-openapi.yml
- filename: omnisend-products-api-openapi.yml
  format: yaml
  label: Omnisend Products API
  slug: omnisend-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-products-api-openapi.yml
- filename: omnisend-segments-api-openapi.yml
  format: yaml
  label: Omnisend Segments API
  slug: omnisend-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-segments-api-openapi.yml
authorization_urls:
- https://app.omnisend.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Omnisend Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Omnisend publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Omnisend API on a user''s behalf.


  Tokens are issued from https://api.omnisend.com/v5/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Omnisend
provider_slug: omnisend
schemes:
- flows:
  - authorizationUrl: https://app.omnisend.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.omnisend.com/v5/oauth/token
  name: OAuth2
  source: openapi/omnisend-openapi.yml
scope_count: 5
scope_names:
- analytics.read
- campaigns.read
- campaigns.write
- contacts.read
- contacts.write
scopes:
- description: Read analytics
  flows:
  - authorizationCode
  scope: analytics.read
- description: Read campaigns
  flows:
  - authorizationCode
  scope: campaigns.read
- description: Manage campaigns
  flows:
  - authorizationCode
  scope: campaigns.write
- description: Read contacts
  flows:
  - authorizationCode
  scope: contacts.read
- description: Manage contacts
  flows:
  - authorizationCode
  scope: contacts.write
slug: omnisend-scopes
source_filename: omnisend-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/omnisend-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/omnisend-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.omnisend.com/oauth/authorize\n    tokenUrl: https://api.omnisend.com/v5/oauth/token\nscopes:\n- scope: analytics.read\n  description: Read analytics\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/omnisend-openapi.yml\n- scope: campaigns.read\n  description: Read campaigns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/omnisend-openapi.yml\n- scope: campaigns.write\n  description: Manage campaigns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/omnisend-openapi.yml\n- scope: contacts.read\n  description: Read contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/omnisend-openapi.yml\n- scope: contacts.write\n  description: Manage contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/omnisend-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/scopes/omnisend-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Email Marketing
- Marketing Automation
- Ecommerce
- SMS Marketing
- Customer Engagement
- Segmentation
- Campaigns
- Forms
- Popups
- Web Push
token_urls:
- https://api.omnisend.com/v5/oauth/token
---
