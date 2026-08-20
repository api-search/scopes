---
authorization_urls: []
description: ''
docs: https://help.keepface.com/brand/integrations/manage-with-claude-code/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Keepface Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'KeepFace publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the KeepFace API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: KeepFace
provider_slug: keepface
schemes: []
scope_count: 11
scope_names:
- discovery
- lists
- campaigns
- outreach
- reporting
- affiliate
- wallet
- crm
- brand
- analyze
- chat
scopes:
- description: Search the marketplace and read discovery profiles, autocomplete, curated rows and audience forecasts. Also carries the token-identity tools.
  flows: []
  scope: discovery
- description: Build and manage influencer lists, including submitting and recalling them and sending list email invites.
  flows: []
  scope: lists
- description: Create, update, submit and delete campaigns, and attach or detach influencers and lists.
  flows: []
  scope: campaigns
- description: Manage recruitment replies and the shortlist, and start outreach.
  flows: []
  scope: outreach
- description: Campaign performance, sales and barter overviews, account intelligence reports, payment events, escrow and subscription state.
  flows: []
  scope: reporting
- description: Affiliate program management — overview, stats, conversions, members, audit, settings and landing page; approve/reject/disable members and open disputes.
  flows: []
  scope: affiliate
- description: Balance, ledger, breakdown, transactions, FX quotes and rates, top-up packages.
  flows: []
  scope: wallet
- description: Creator contacts and the My Influencers roster — members, invites, roster records.
  flows: []
  scope: crm
- description: Company and brand profiles — list, create, update, set default, delete, and read the per-brand affiliate config.
  flows: []
  scope: brand
- description: Paid on-demand AI Intelligence reports plus the free pricing estimate.
  flows: []
  scope: analyze
- description: Read and send creator messages, including bulk sends across up to 200 threads.
  flows: []
  scope: chat
slug: keepface-scopes
source_filename: keepface-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.keepface.com/brand/integrations/claude-code-tools-reference/\ndocs: https://help.keepface.com/brand/integrations/manage-with-claude-code/\n\n# NOT OAuth. Keepface implements no OAuth 2.0 or OIDC anywhere (see\n# ../authentication/keepface-authentication.yml). These are the scopes attached to\n# the static bearer API token that authorises the MCP server, chosen as checkboxes\n# by a human at token-creation time. They are recorded here because they are a\n# real, published, enumerated permission surface — one checkbox per area of the\n# brand panel — and the token loads only the tools its scopes allow.\n\nscheme: bearer-api-token\noauth2: false\ngrant_flow: none (token minted in the panel, no authorization endpoint)\nselection: per-token checkbox at creation; least-privilege is the documented advice\n  (\"grant only the scopes you need. You can always create a second token with more\")\nenforcement: >-\n  The server\
  \ resolves scopes from the token and loads only the permitted tools.\n  A call outside the granted scopes returns HTTP 403.\nworkspace_binding: every token is pinned to one brand workspace and cannot act in\n  another\napplies_to: https://mcp.keepface.com/mcp\n\nscope_count: 11\n\nscopes:\n- scope: discovery\n  description: Search the marketplace and read discovery profiles, autocomplete,\n    curated rows and audience forecasts. Also carries the token-identity tools.\n  access: read-only\n  tools: 8\n- scope: lists\n  description: Build and manage influencer lists, including submitting and recalling\n    them and sending list email invites.\n  access: read+write\n  destructive_tools: [delete_list]\n  message_sending_tools: [create_list_email_invite]\n  tools: 11\n- scope: campaigns\n  description: Create, update, submit and delete campaigns, and attach or detach\n    influencers and lists.\n  access: read+write\n  destructive_tools: [delete_campaign]\n  tools: 11\n- scope: outreach\n\
  \  description: Manage recruitment replies and the shortlist, and start outreach.\n  access: read+write\n  wallet_charging_tools: [start_outreach]\n  message_sending_tools: [start_outreach]\n  tools: 6\n  note: start_outreach charges the wallet, locks escrow and notifies the creator\n- scope: reporting\n  description: Campaign performance, sales and barter overviews, account intelligence\n    reports, payment events, escrow and subscription state.\n  access: read-only\n  tools: 9\n- scope: affiliate\n  description: Affiliate program management — overview, stats, conversions, members,\n    audit, settings and landing page; approve/reject/disable members and open disputes.\n  access: read+write\n  tools: 15\n  excluded: >-\n    Changing commission, importing sales and rotating secrets are deliberately not\n    exposed to any token; they stay in the panel.\n- scope: wallet\n  description: Balance, ledger, breakdown, transactions, FX quotes and rates, top-up\n    packages.\n  access: read-only\n\
  \  tools: 7\n  note: read-only by design; no token can top up, convert, withdraw or pay out\n- scope: crm\n  description: Creator contacts and the My Influencers roster — members, invites,\n    roster records.\n  access: read+write\n  destructive_tools: [delete_crm_invite, remove_roster_member]\n  message_sending_tools: [invite_crm_email]\n  tools: 12\n- scope: brand\n  description: Company and brand profiles — list, create, update, set default, delete,\n    and read the per-brand affiliate config.\n  access: read+write\n  destructive_tools: [delete_brand]\n  tools: 6\n- scope: analyze\n  description: Paid on-demand AI Intelligence reports plus the free pricing estimate.\n  access: read+write\n  wallet_charging_tools: [start_analyze]\n  tools: 2\n- scope: chat\n  description: Read and send creator messages, including bulk sends across up to 200\n    threads.\n  access: read+write\n  message_sending_tools: [send_message, bulk_send]\n  tools: 6\n\nglobal_restrictions:\n# Enforced above the\
  \ scope layer — no combination of scopes unlocks these.\n- Top-up, currency conversion, withdrawal, influencer payouts and affiliate\n  commission settings are never available to any token.\n- Every write returns a preview and executes only after an explicit confirmation.\n- Account security settings cannot be changed by a token.\n\nerrors:\n- {status: 403, meaning: unauthorized, or the token lacks the scope for this tool}\n- {status: 402, meaning: insufficient wallet balance for a charging tool}\n\nx-evidence:\n- {url: 'https://help.keepface.com/brand/integrations/claude-code-tools-reference/',\n  http_status: 200, fetched: '2026-08-13'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keepface/refs/heads/main/scopes/keepface-scopes.yml
summary_line: 11 scopes
tags:
- Company
- Influencer Marketing
- Creator Economy
- Marketing
- Social-Media
- Affiliate Marketing
- Advocacy
- Campaign Management
- MCP
- AI Agents
- Attribution
- Webhook
token_urls: []
---
