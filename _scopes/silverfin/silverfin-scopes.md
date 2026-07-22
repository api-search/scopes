---
authorization_urls:
- https://live.getsilverfin.com/f/{firm_id}/oauth/authorize
description: ''
docs: https://developer.silverfin.com/reference/oauth-application-scopes-syncapi
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Silverfin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Silverfin publishes 19 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Silverfin API on a user''s behalf.


  Tokens are issued from https://live.getsilverfin.com/f/{firm_id}/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Silverfin
provider_slug: silverfin
schemes:
- flows:
  - authorizationUrl: https://live.getsilverfin.com/f/{firm_id}/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://live.getsilverfin.com/f/{firm_id}/oauth/token
  name: OAuth2
scope_count: 19
scope_names:
- administration:read
- administration:write
- communication:read
- communication:write
- financials:read
- financials:write
- financials:transactions:read
- financials:transactions:write
- financials:transactions:sync
- links
- permanent_documents:read
- permanent_documents:write
- client_meetings:external_notes:write
- user:email
- user:firm
- user:profile
- webhooks
- workflows:read
- workflows:write
scopes:
- description: View administrative data (companies, accounts, users, groups, templates).
  flows:
  - authorizationCode
  scope: administration:read
- description: Modify administrative data (companies, accounts, users, groups, templates).
  flows:
  - authorizationCode
  scope: administration:write
- description: View communications (remarks, comments, periods).
  flows:
  - authorizationCode
  scope: communication:read
- description: Create communications (remarks, comments).
  flows:
  - authorizationCode
  scope: communication:write
- description: View financial records (balances, budgets, adjustments, reconciliations, reports, exports).
  flows:
  - authorizationCode
  scope: financials:read
- description: Modify financial records (adjustments, custom properties, export instances, periods).
  flows:
  - authorizationCode
  scope: financials:write
- description: View open transactions (payables and receivables).
  flows:
  - authorizationCode
  scope: financials:transactions:read
- description: Record bookkeeping transactions.
  flows:
  - authorizationCode
  scope: financials:transactions:write
- description: SyncAPI scope to submit/modify/delete bookkeeping transactions and manage sync settings.
  flows:
  - authorizationCode
  scope: financials:transactions:sync
- description: Register, list and destroy app links (AppLinks) in Silverfin menus.
  flows:
  - authorizationCode
  scope: links
- description: View permanent documents and folders.
  flows:
  - authorizationCode
  scope: permanent_documents:read
- description: Manage permanent documents, folders and mail.
  flows:
  - authorizationCode
  scope: permanent_documents:write
- description: Upload external notes and attachments to client meetings.
  flows:
  - authorizationCode
  scope: client_meetings:external_notes:write
- description: Access the current user's email address.
  flows:
  - authorizationCode
  scope: user:email
- description: Access firm information for the current user.
  flows:
  - authorizationCode
  scope: user:firm
- description: Access the current user's profile.
  flows:
  - authorizationCode
  scope: user:profile
- description: Register, list and destroy webhooks (including SyncAPI webhooks).
  flows:
  - authorizationCode
  scope: webhooks
- description: View workflows and workflow status.
  flows:
  - authorizationCode
  scope: workflows:read
- description: Add, archive and reactivate workflows.
  flows:
  - authorizationCode
  scope: workflows:write
slug: silverfin-scopes
source_filename: silverfin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.silverfin.com/reference/authentication\ndocs: https://developer.silverfin.com/reference/oauth-application-scopes-syncapi\nschemes:\n  - name: OAuth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://live.getsilverfin.com/f/{firm_id}/oauth/authorize\n        tokenUrl: https://live.getsilverfin.com/f/{firm_id}/oauth/token\nscopes:\n  - scope: administration:read\n    description: View administrative data (companies, accounts, users, groups, templates).\n    flows: [authorizationCode]\n  - scope: administration:write\n    description: Modify administrative data (companies, accounts, users, groups, templates).\n    flows: [authorizationCode]\n  - scope: communication:read\n    description: View communications (remarks, comments, periods).\n    flows: [authorizationCode]\n  - scope: communication:write\n    description: Create communications (remarks, comments).\n    flows: [authorizationCode]\n\
  \  - scope: financials:read\n    description: View financial records (balances, budgets, adjustments, reconciliations, reports, exports).\n    flows: [authorizationCode]\n  - scope: financials:write\n    description: Modify financial records (adjustments, custom properties, export instances, periods).\n    flows: [authorizationCode]\n  - scope: financials:transactions:read\n    description: View open transactions (payables and receivables).\n    flows: [authorizationCode]\n  - scope: financials:transactions:write\n    description: Record bookkeeping transactions.\n    flows: [authorizationCode]\n  - scope: financials:transactions:sync\n    description: SyncAPI scope to submit/modify/delete bookkeeping transactions and manage sync settings.\n    flows: [authorizationCode]\n  - scope: links\n    description: Register, list and destroy app links (AppLinks) in Silverfin menus.\n    flows: [authorizationCode]\n  - scope: permanent_documents:read\n    description: View permanent documents and\
  \ folders.\n    flows: [authorizationCode]\n  - scope: permanent_documents:write\n    description: Manage permanent documents, folders and mail.\n    flows: [authorizationCode]\n  - scope: client_meetings:external_notes:write\n    description: Upload external notes and attachments to client meetings.\n    flows: [authorizationCode]\n  - scope: user:email\n    description: Access the current user's email address.\n    flows: [authorizationCode]\n  - scope: user:firm\n    description: Access firm information for the current user.\n    flows: [authorizationCode]\n  - scope: user:profile\n    description: Access the current user's profile.\n    flows: [authorizationCode]\n  - scope: webhooks\n    description: Register, list and destroy webhooks (including SyncAPI webhooks).\n    flows: [authorizationCode]\n  - scope: workflows:read\n    description: View workflows and workflow status.\n    flows: [authorizationCode]\n  - scope: workflows:write\n    description: Add, archive and reactivate\
  \ workflows.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silverfin/refs/heads/main/scopes/silverfin-scopes.yml
summary_line: 19 scopes · authorizationCode
tags:
- Company
- Business Applications
- Accounting
- Financial Close
- Bookkeeping
- Reporting
- Compliance
- Fintech
- SaaS
- Belgium
token_urls:
- https://live.getsilverfin.com/f/{firm_id}/oauth/token
---
