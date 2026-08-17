---
api_specs:
- filename: zoho-campaigns-email-api-collection.json
  format: json
  label: Zoho Campaigns Email API
  slug: zoho-campaigns-email-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/zoho-campaigns/refs/heads/main/postman/zoho-campaigns-email-api-collection.json
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth
description: ''
docs: https://www.zoho.com/campaigns/help/developers/access-token.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Zoho Campaigns Scopes
name_suffix: OAuth Scopes
note: Transcribed verbatim from the Scope table on the Zoho Campaigns access-token developer guide. Zoho Campaigns publishes no OpenAPI, so these scopes could not be derived from a spec; every name below is printed on the docs page. An incorrectly specified scope returns an INVALID_SCOPE error.
overview: 'Zoho Campaigns publishes 15 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoho Campaigns API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoho Campaigns
provider_slug: zoho-campaigns
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: ZohoOAuth
  source: https://www.zoho.com/campaigns/help/developers/access-token.html
scope_count: 15
scope_names:
- ZohoCampaigns.campaign.CREATE
- ZohoCampaigns.campaign.READ
- ZohoCampaigns.campaign.UPDATE
- ZohoCampaigns.campaign.DELETE
- ZohoCampaigns.campaign.CREATE-UPDATE
- ZohoCampaigns.campaign.WRITE
- ZohoCampaigns.campaign.ALL
- ZohoCampaigns.contact.CREATE
- ZohoCampaigns.contact.READ
- ZohoCampaigns.contact.UPDATE
- ZohoCampaigns.contact.DELETE
- ZohoCampaigns.contact.CREATE-UPDATE
- ZohoCampaigns.contact.WRITE
- ZohoCampaigns.contact.ALL
- ZohoCampaigns.emailapi.ALL
scopes:
- description: To create campaigns and merge tags
  flows:
  - authorizationCode
  scope: ZohoCampaigns.campaign.CREATE
- description: To view a report or the details of a campaign
  flows:
  - authorizationCode
  scope: ZohoCampaigns.campaign.READ
- description: To update campaigns and coupons
  flows:
  - authorizationCode
  scope: ZohoCampaigns.campaign.UPDATE
- description: To delete a campaign
  flows:
  - authorizationCode
  scope: ZohoCampaigns.campaign.DELETE
- description: To create, clone, and edit a campaign (CREATE, UPDATE)
  flows:
  - authorizationCode
  scope: ZohoCampaigns.campaign.CREATE-UPDATE
- description: To create, modify, and delete campaigns (CREATE, UPDATE, DELETE)
  flows:
  - authorizationCode
  scope: ZohoCampaigns.campaign.WRITE
- description: To view, create, modify, and delete campaigns (READ, CREATE, UPDATE, DELETE)
  flows:
  - authorizationCode
  scope: ZohoCampaigns.campaign.ALL
- description: To create contacts or mailing lists
  flows:
  - authorizationCode
  scope: ZohoCampaigns.contact.CREATE
- description: To view details or a report of contacts or mailing lists
  flows:
  - authorizationCode
  scope: ZohoCampaigns.contact.READ
- description: To update contacts or mailing lists
  flows:
  - authorizationCode
  scope: ZohoCampaigns.contact.UPDATE
- description: To delete mailing lists
  flows:
  - authorizationCode
  scope: ZohoCampaigns.contact.DELETE
- description: To create and edit contacts or mailing lists (CREATE, UPDATE)
  flows:
  - authorizationCode
  scope: ZohoCampaigns.contact.CREATE-UPDATE
- description: To create, edit, and delete contacts or mailing lists (CREATE, UPDATE, DELETE)
  flows:
  - authorizationCode
  scope: ZohoCampaigns.contact.WRITE
- description: To create, edit, view, and delete contacts or mailing lists (READ, CREATE, UPDATE, DELETE)
  flows:
  - authorizationCode
  scope: ZohoCampaigns.contact.ALL
- description: The single scope selectable when creating a Zoho Campaigns Email API key (the Zoho-zapikey credential used by Email API v2).
  flows: []
  scope: ZohoCampaigns.emailapi.ALL
slug: zoho-campaigns-scopes
source_filename: zoho-campaigns-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.zoho.com/campaigns/help/developers/access-token.html\ndocs: https://www.zoho.com/campaigns/help/developers/access-token.html\nnote: >-\n  Transcribed verbatim from the Scope table on the Zoho Campaigns access-token\n  developer guide. Zoho Campaigns publishes no OpenAPI, so these scopes could\n  not be derived from a spec; every name below is printed on the docs page.\n  An incorrectly specified scope returns an INVALID_SCOPE error.\nschemes:\n  - name: ZohoOAuth\n    source: https://www.zoho.com/campaigns/help/developers/access-token.html\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n        tokenUrl: https://accounts.zoho.com/oauth/v2/token\nscopes:\n  - scope: ZohoCampaigns.campaign.CREATE\n    module: Campaigns\n    description: To create campaigns and merge tags\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.campaign.READ\n    module:\
  \ Campaigns\n    description: To view a report or the details of a campaign\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.campaign.UPDATE\n    module: Campaigns\n    description: To update campaigns and coupons\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.campaign.DELETE\n    module: Campaigns\n    description: To delete a campaign\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.campaign.CREATE-UPDATE\n    module: Campaigns\n    description: To create, clone, and edit a campaign (CREATE, UPDATE)\n    composite_of: [ZohoCampaigns.campaign.CREATE, ZohoCampaigns.campaign.UPDATE]\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.campaign.WRITE\n    module: Campaigns\n    description: To create, modify, and delete campaigns (CREATE, UPDATE, DELETE)\n    composite_of:\n      - ZohoCampaigns.campaign.CREATE\n      - ZohoCampaigns.campaign.UPDATE\n      - ZohoCampaigns.campaign.DELETE\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.campaign.ALL\n\
  \    module: Campaigns\n    description: To view, create, modify, and delete campaigns (READ, CREATE, UPDATE, DELETE)\n    composite_of:\n      - ZohoCampaigns.campaign.READ\n      - ZohoCampaigns.campaign.CREATE\n      - ZohoCampaigns.campaign.UPDATE\n      - ZohoCampaigns.campaign.DELETE\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.contact.CREATE\n    module: Contacts\n    description: To create contacts or mailing lists\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.contact.READ\n    module: Contacts\n    description: To view details or a report of contacts or mailing lists\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.contact.UPDATE\n    module: Contacts\n    description: To update contacts or mailing lists\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.contact.DELETE\n    module: Contacts\n    description: To delete mailing lists\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.contact.CREATE-UPDATE\n    module: Contacts\n  \
  \  description: To create and edit contacts or mailing lists (CREATE, UPDATE)\n    composite_of: [ZohoCampaigns.contact.CREATE, ZohoCampaigns.contact.UPDATE]\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.contact.WRITE\n    module: Contacts\n    description: To create, edit, and delete contacts or mailing lists (CREATE, UPDATE, DELETE)\n    composite_of:\n      - ZohoCampaigns.contact.CREATE\n      - ZohoCampaigns.contact.UPDATE\n      - ZohoCampaigns.contact.DELETE\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.contact.ALL\n    module: Contacts\n    description: To create, edit, view, and delete contacts or mailing lists (READ, CREATE, UPDATE, DELETE)\n    composite_of:\n      - ZohoCampaigns.contact.READ\n      - ZohoCampaigns.contact.CREATE\n      - ZohoCampaigns.contact.UPDATE\n      - ZohoCampaigns.contact.DELETE\n    flows: [authorizationCode]\n  - scope: ZohoCampaigns.emailapi.ALL\n    module: Email API\n    description: >-\n      The single scope selectable\
  \ when creating a Zoho Campaigns Email API key\n      (the Zoho-zapikey credential used by Email API v2).\n    source: https://www.zoho.com/campaigns/help/emailapi/authentication.html\n    flows: []\nidentity_scopes:\n  note: >-\n    The Zoho Accounts authorization server additionally advertises the standard\n    OIDC identity scopes in its discovery document.\n  source: well-known/zoho-campaigns-openid-configuration.json\n  scopes: [openid, email, profile, phone]\nsummary:\n  scope_count: 15\n  modules: [Campaigns, Contacts, Email API]\n  granularity: module + CRUD verb, with CREATE-UPDATE / WRITE / ALL composites\n  error_on_bad_scope: INVALID_SCOPE\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-campaigns/refs/heads/main/scopes/zoho-campaigns-scopes.yml
summary_line: 15 scopes · authorizationCode
tags:
- Email Marketing
- Campaigns
- Mailing Lists
- Subscribers
- Email Templates
- A/B Testing
- Campaign Analytics
- Marketing Automation
- Transactional Email
- Webhooks
token_urls:
- https://accounts.zoho.com/oauth/v2/token
---
