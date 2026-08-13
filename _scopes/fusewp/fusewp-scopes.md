---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Fusewp Scopes
name_suffix: OAuth Scopes
note: 'READ THIS BEFORE USING THE ROWS BELOW. FuseWP does not issue OAuth scopes of its own — it has no OAuth-protected product API for third parties to call. The one exception is the single `mcp` scope its WordPress MCP server advertises, recorded separately at the bottom. Everything in delegated_scopes[] is the reverse direction: the scope set FuseWP REQUESTS FROM each partner platform when a site administrator connects an account. Each row was read verbatim from the Location header of a live 302 issued by https://auth.fusewp.com/{integration_id} on 2026-08-12 — this is the access FuseWP actually asks for over your CRM, observed rather than documented. The provider publishes no scopes reference page; nothing here comes from prose. Partner client_id values are omitted deliberately: they are public but secret-shaped, and they are not the finding.'
overview: 'FuseWP uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FuseWP
provider_slug: fusewp
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: fusewp-scopes
source_filename: fusewp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://auth.fusewp.com/\ndirection: outbound-delegated\nnote: >-\n  READ THIS BEFORE USING THE ROWS BELOW. FuseWP does not issue OAuth scopes of\n  its own — it has no OAuth-protected product API for third parties to call. The\n  one exception is the single `mcp` scope its WordPress MCP server advertises,\n  recorded separately at the bottom. Everything in delegated_scopes[] is the\n  reverse direction: the scope set FuseWP REQUESTS FROM each partner platform\n  when a site administrator connects an account. Each row was read verbatim from\n  the Location header of a live 302 issued by\n  https://auth.fusewp.com/{integration_id} on 2026-08-12 — this is the access\n  FuseWP actually asks for over your CRM, observed rather than documented. The\n  provider publishes no scopes reference page; nothing here comes from prose.\n  Partner client_id values are omitted deliberately: they are public but\n  secret-shaped, and they are not\
  \ the finding.\nissued_scopes:\n- scope: mcp\n  description: >-\n    The only scope FuseWP itself issues. Advertised in both\n    /.well-known/oauth-authorization-server and\n    /.well-known/oauth-protected-resource; gates the MCP endpoint at\n    https://fusewp.com/wp-json/mcp/mcp-oauth-server.\n  flows: [authorizationCode]\n  pkce: S256\n  sources: [well-known/fusewp-oauth-authorization-server.json]\ndelegated_scopes:\n- integration_id: aweber\n  partner: AWeber\n  authorize_host: auth.aweber.com\n  scopes: [account.read, list.read, list.write, subscriber.read, subscriber.write, email.write]\n  status: 302\n- integration_id: birdsend\n  partner: BirdSend\n  authorize_host: app.birdsend.co\n  scopes: [read, write]\n  status: 302\n- integration_id: campaignmonitor\n  partner: Campaign Monitor\n  authorize_host: api.createsend.com\n  scopes: [ManageLists, ImportSubscribers, CreateCampaigns, SendCampaigns]\n  status: 302\n  note: State parameter present; scope delimiter is a comma on this\
  \ partner.\n- integration_id: constantcontact\n  partner: Constant Contact\n  authorize_host: authz.constantcontact.com\n  scopes: [contact_data, campaign_data, offline_access]\n  status: 302\n- integration_id: copper\n  partner: Copper CRM\n  authorize_host: app.copper.com\n  scopes: ['developer/v1/all']\n  status: 302\n  note: >-\n    Copper exposes no granular scopes — the only value available is full\n    developer API access.\n- integration_id: gohl\n  partner: GoHighLevel\n  authorize_host: marketplace.gohighlevel.com\n  scopes: [contacts.write, contacts.readonly, workflows.readonly, 'locations/tags.write',\n    'locations/tags.readonly', 'locations/customFields.readonly', 'locations/customFields.write']\n  status: 302\n- integration_id: hubspot\n  partner: HubSpot\n  authorize_host: app.hubspot.com\n  scopes: [oauth, crm.objects.owners.read, crm.objects.contacts.write, crm.lists.write,\n    crm.lists.read, crm.schemas.contacts.read, crm.objects.contacts.read]\n  status: 302\n- integration_id:\
  \ keap\n  partner: Keap / Infusionsoft\n  authorize_host: accounts.infusionsoft.com\n  scopes: [full]\n  status: 302\n  note: >-\n    Keap publishes only a single `full` scope, so connecting FuseWP grants\n    complete account access. A least-privilege limitation of the partner, not of\n    FuseWP.\n- integration_id: mailchimp\n  partner: Mailchimp\n  authorize_host: login.mailchimp.com\n  scopes: []\n  status: 302\n  note: >-\n    Empty scope parameter — Mailchimp's OAuth2 grants full account access to the\n    authorizing user and defines no scope vocabulary.\n- integration_id: zohocrm\n  partner: Zoho CRM\n  authorize_host: accounts.zoho.com\n  scopes: [ZohoCRM.modules.READ, ZohoCRM.modules.CREATE, ZohoCRM.modules.UPDATE,\n    ZohoCRM.users.READ, ZohoCRM.users.CREATE, ZohoCRM.users.UPDATE, ZohoCRM.settings.all]\n  status: 302\n  note: Requests access_type=offline and prompt=consent.\n- integration_id: zohocampaigns\n  partner: Zoho Campaigns\n  authorize_host: accounts.zoho.com\n  scopes:\
  \ [ZohoCampaigns.contact.CREATE, ZohoCampaigns.contact.READ, ZohoCampaigns.contact.UPDATE,\n    ZohoCampaigns.campaign.READ, ZohoCampaigns.campaign.CREATE, ZohoCampaigns.campaign.UPDATE]\n  status: 302\n  note: >-\n    The redirect_uri returned for this integration is\n    https://auth.fusewp.com/zohocrm rather than /zohocampaigns — the two Zoho\n    integrations share one registered OAuth application. Recorded as observed.\nunresolved:\n- integration_id: google_sheet\n  partner: Google Sheets\n  status: 500\n- integration_id: salesforce\n  partner: Salesforce\n  status: 500\nsummary:\n  issued_scope_count: 1\n  delegated_integrations_probed: 13\n  delegated_integrations_resolved: 11\n  write_capable_integrations: 10\n  full_access_integrations: [keap, mailchimp, copper]\nx-evidence:\n  fetched: '2026-08-12'\n  method: 'GET https://auth.fusewp.com/{integration_id}, Location header read without following'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusewp/refs/heads/main/scopes/fusewp-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- WordPress
- Email Marketing
- Marketing Automation
- CRM
- Integration
- Data Synchronization
- OAuth
- Plugins
- No Code
token_urls: []
---
