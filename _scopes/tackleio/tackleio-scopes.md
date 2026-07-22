---
api_specs:
- filename: tackleio-platform-openapi.json
  format: json
  label: Tackle Platform API
  slug: tackle-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-platform-openapi.json
- filename: tackleio-prospect-openapi.json
  format: json
  label: Tackle Prospect API
  slug: tackle-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-prospect-openapi.json
- filename: tackleio-cosell-aws-openapi.json
  format: json
  label: Tackle Co-Sell for AWS Partner Central
  slug: tackle-co-sell-for-aws-partner-central
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-cosell-aws-openapi.json
- filename: tackleio-cosell-gcp-openapi.json
  format: json
  label: Tackle Co-Sell for Google Cloud
  slug: tackle-co-sell-for-google-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-cosell-gcp-openapi.json
- filename: tackleio-cosell-msft-openapi.json
  format: json
  label: Tackle Co-Sell for Microsoft Partner Center
  slug: tackle-co-sell-for-microsoft-partner-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-cosell-msft-openapi.json
- filename: tackleio-offers-aws-openapi.json
  format: json
  label: Tackle Offers for AWS Marketplace
  slug: tackle-offers-for-aws-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-offers-aws-openapi.json
- filename: tackleio-offers-msft-openapi.json
  format: json
  label: Tackle Offers for Microsoft
  slug: tackle-offers-for-microsoft
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-offers-msft-openapi.json
- filename: tackleio-contracts-openapi.json
  format: json
  label: Tackle Public Contracts API
  slug: tackle-public-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-contracts-openapi.json
- filename: tackleio-scim-openapi.json
  format: json
  label: Tackle SCIM API
  slug: tackle-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-scim-openapi.json
authorization_urls: []
description: ''
docs: https://developers.tackle.io/docs/getting-an-access-token
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Tackleio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tackle.io uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tackle.io
provider_slug: tackleio
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: tackleio-scopes
source_filename: tackleio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.tackle.io/reference + https://auth.tackle.io/.well-known/openid-configuration\ndocs: https://developers.tackle.io/docs/getting-an-access-token\nmodel: OAuth 2.0 client-credentials issues a JWT whose fine-grained RBAC permissions gate each operation;\n  the OIDC provider (Auth0) also advertises standard OpenID scopes for interactive login.\noidc_scopes:\n- openid\n- profile\n- email\n- offline_access\n- name\n- given_name\n- family_name\n- nickname\n- email_verified\n- picture\n- phone\n- address\nrbac_permissions:\n- name: cosell:ListOpportunities\n  description: List co-sell opportunities.\n- name: cosell:CreateOpportunity\n  description: Create a co-sell opportunity.\n- name: cosell:GetOpportunity\n  description: Retrieve a co-sell opportunity.\n- name: cosell:UpdateOpportunity\n  description: Update a co-sell opportunity.\n- name: cosell:StartEngagement\n  description: Submit / start engagement on a co-sell\
  \ opportunity.\n- name: cosell:ListOpportunityEvents\n  description: List the event history for an opportunity.\n- name: cosell:GetPicklistOptions\n  description: Read acceptable picklist values for opportunity fields.\n- name: offers:ListOffers\n  description: List private offers.\n- name: offers:GetOffer\n  description: Retrieve a private offer.\n- name: offers:CreateDraftOffer\n  description: Create/update a draft private offer; also gates agreements, products, pricing, currencies\n    and partner lookups.\n- name: offers:UpdateOffer\n  description: Update/delete/archive/unarchive a private offer.\n- name: offers:CancelOffer\n  description: Cancel a private offer pushed to the marketplace.\n- name: offers:CreateOfferOnMarketplace\n  description: Push/submit a draft offer to the cloud marketplace.\n- name: offers:ListProducts\n  description: List marketplace product listings.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/scopes/tackleio-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cloud
- Cloud Marketplace
- Co-Sell
- AWS Marketplace
- Azure Marketplace
- Google Cloud Marketplace
- Private Offers
- Metering
- SCIM
- Webhooks
- B2B SaaS
token_urls: []
---
