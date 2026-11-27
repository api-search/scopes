---
authorization_urls: []
description: ''
docs: https://crawlraven.com/docs/mcp-full-access
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: CrawlRaven Scopes
name_suffix: OAuth Scopes
note: Scopes for the OAuth-protected MCP server. "A paid connection can approve up to 11 scopes. Existing grants keep their approved scopes. Reconnect to add a newly available scope such as technical_seo:read or a write scope; CrawlRaven never widens a connection silently."
overview: 'CrawlRaven publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CrawlRaven API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CrawlRaven
provider_slug: crawlraven-com
schemes: []
scope_count: 11
scope_names:
- websites:read
- search_performance:read
- opportunities:read
- targets:read
- annotations:read
- analytics:read
- technical_seo:read
- opportunities:write
- targets:write
- notes:write
- annotations:write
scopes:
- description: List websites available to the connection.
  flows: []
  scope: websites:read
- description: Read Search Console overview, series, Query, and Page reports, plus paid imported Generative AI snapshots.
  flows: []
  scope: search_performance:read
- description: Read active CrawlRaven opportunity records and the prioritized SEO plan.
  flows: []
  scope: opportunities:read
- description: Read the durable Target Keywords plan and target-to-page alignment.
  flows: []
  scope: targets:read
- description: Read active website timeline annotations.
  flows: []
  scope: annotations:read
- description: Read bounded reports from an already linked GA4 property.
  flows: []
  scope: analytics:read
- description: Read stored Technical SEO audits, findings, and comparisons. Cannot start audits.
  flows: []
  scope: technical_seo:read
- description: Directly resolve, ignore, snooze, or reopen individual opportunities without further approval.
  flows: []
  scope: opportunities:write
- description: Directly add target keywords, assign intended pages, and change priority without further approval.
  flows: []
  scope: targets:write
- description: Directly create, edit, archive, and restore manual notes without further approval. Cannot change automatic events or permanently delete notes.
  flows: []
  scope: notes:write
- description: Propose manual annotation changes that require same-user approval in CrawlRaven before execution.
  flows: []
  scope: annotations:write
slug: crawlraven-com-scopes
source_filename: crawlraven-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'generated: ''2026-11-04''

  method: searched

  source: https://crawlraven.com/docs/mcp

  docs: https://crawlraven.com/docs/mcp-full-access

  note: Scopes for the OAuth-protected MCP server. "A paid connection can approve up to 11 scopes. Existing grants keep their approved scopes. Reconnect to add a newly available scope such as technical_seo:read or a write scope; CrawlRaven never widens a connection silently."

  scopes:

  - {name: ''websites:read'', description: List websites available to the connection., access: read}

  - {name: ''search_performance:read'', description: ''Read Search Console overview, series, Query, and Page reports, plus paid imported Generative AI snapshots.'', access: read}

  - {name: ''opportunities:read'', description: Read active CrawlRaven opportunity records and the prioritized SEO plan., access: read}

  - {name: ''targets:read'', description: Read the durable Target Keywords plan and target-to-page alignment., access: read}

  - {name: ''annotations:read'', description: Read active website timeline annotations., access: read}

  - {name: ''analytics:read'', description: Read bounded reports from an already linked GA4 property., access: read, plan: paid}

  - {name: ''technical_seo:read'', description: ''Read stored Technical SEO audits, findings, and comparisons. Cannot start audits.'', access: read, plan: paid}

  - {name: ''opportunities:write'', description: ''Directly resolve, ignore, snooze, or reopen individual opportunities without further approval.'', access: write, plan: paid}

  - {name: ''targets:write'', description: ''Directly add target keywords, assign intended pages, and change priority without further approval.'', access: write, plan: paid}

  - {name: ''notes:write'', description: ''Directly create, edit, archive, and restore manual notes without further approval. Cannot change automatic events or permanently delete notes.'', access: write, plan: paid}

  - {name: ''annotations:write'', description: Propose manual annotation changes that require same-user approval in CrawlRaven before execution., access: write, plan: paid}

  '
source_yaml_url: https://artifacts.apis.io/crawlraven-com/scopes/crawlraven-com-scopes.yml
summary_line: 11 scopes
tags:
- Company
- SEO
- Search Console
- Google Analytics
- Technical SEO Audit
- Analytics
- MCP
- Marketing
token_bound: false
token_urls: []
---
