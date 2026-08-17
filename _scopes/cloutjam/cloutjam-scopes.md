---
authorization_urls: []
description: ''
docs: https://www.cloutdesk.com/agent-platform
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cloutjam Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CloutJam publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CloutJam API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CloutJam
provider_slug: cloutjam
schemes:
- flows:
  - detail: OAuth 2.1 + PKCE, stated for Claude Managed Agents one-click install
    flow: authorizationCode
    pkce: true
  name: oauth2
  source: https://www.cloutdesk.com/agent-platform
- detail: Scoped PAT (cd_pat_) minted from the Cloutdesk dashboard; the repo calls these "required scopes on the integrator's Cloutdesk PAT", so the same scope names gate PATs and OAuth grants.
  name: personalAccessToken
  source: https://github.com/cloutdesk/agents/blob/main/README.md
scope_count: 4
scope_names:
- collaborations:read
- creators:read
- events:emit
- transactions:read
scopes:
- description: Read collaborations — deliverable state, locked commercial terms, payment schedule, commission split, and metrics.
  flows: []
  scope: collaborations:read
- description: Read creator/talent profiles — audience demographics, brand-fit signals, historical performance baseline.
  flows: []
  scope: creators:read
- description: Append events to a collaboration timeline / audit trail.
  flows: []
  scope: events:emit
- description: Read financial state — AR aging, invoice state, payout queue and Stripe Connect account context.
  flows: []
  scope: transactions:read
slug: cloutjam-scopes
source_filename: cloutjam-scopes.yml
source_heading: OAuth Scopes
source_url: https://github.com/cloutdesk/agents
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://github.com/cloutdesk/agents\nsources:\n- https://github.com/cloutdesk/agents\n- https://www.cloutdesk.com/agent-platform\ndocs: https://www.cloutdesk.com/agent-platform\nstatus: beta\nnotes: >-\n  UPGRADE over the 2026-07-18 round, which had only the three scope names shown in the\n  Agent Platform page's `npx @cloutdesk/mcp oauth login` example. Cloutdesk's public\n  agents repo (MIT) declares scopes formally — in the `scopes:` frontmatter array of each\n  of the four agent templates and in a \"## Required scopes\" section of each of the 16\n  SKILL.md files — giving four verified `<resource>:<verb>` scopes. TWO NAMING SYSTEMS ARE\n  IN PLAY and they do not reconcile: the repo uses `collaborations:read` / `creators:read` /\n  `events:emit` / `transactions:read`, while the marketing page's login example uses bare\n  `campaigns` and `collaborations` plus `agreements:write`. Both sets are recorded below\n  under their\
  \ own source. No scope reference or permissions page is published, so the full\n  catalog is still unknown and neither set can be treated as complete.\nscope_count: 4\nscheme_note: '<resource>:<verb> in the repo; bare resource names in the marketing example'\nschemes:\n- name: oauth2\n  source: https://www.cloutdesk.com/agent-platform\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    detail: OAuth 2.1 + PKCE, stated for Claude Managed Agents one-click install\n- name: personalAccessToken\n  source: https://github.com/cloutdesk/agents/blob/main/README.md\n  detail: Scoped PAT (cd_pat_) minted from the Cloutdesk dashboard; the repo calls these\n    \"required scopes on the integrator's Cloutdesk PAT\", so the same scope names gate PATs\n    and OAuth grants.\nscopes:\n- scope: collaborations:read\n  description: Read collaborations — deliverable state, locked commercial terms, payment schedule,\n    commission split, and metrics.\n  access: read\n  tools: [list_collabs, get_collab,\
  \ comment_on_deliverable]\n  used_by_templates: [rep-assistant, agreement-reviewer, finance-coordinator, talent-dev]\n  occurrences: 24\n  sources: ['https://github.com/cloutdesk/agents']\n- scope: creators:read\n  description: Read creator/talent profiles — audience demographics, brand-fit signals, historical\n    performance baseline.\n  access: read\n  tools: [get_talent_profile]\n  used_by_templates: [rep-assistant, talent-dev]\n  occurrences: 10\n  sources: ['https://github.com/cloutdesk/agents']\n- scope: events:emit\n  description: Append events to a collaboration timeline / audit trail.\n  access: write\n  tools: [emit_event, comment_on_deliverable]\n  used_by_templates: [rep-assistant, agreement-reviewer]\n  occurrences: 9\n  sources: ['https://github.com/cloutdesk/agents']\n- scope: transactions:read\n  description: Read financial state — AR aging, invoice state, payout queue and Stripe Connect\n    account context.\n  access: read\n  tools: [get_revenue_summary]\n  used_by_templates:\
  \ [finance-coordinator]\n  occurrences: 4\n  sources: ['https://github.com/cloutdesk/agents']\nscopes_marketing_example:\n  note: >-\n    Named on the Agent Platform page in the MCP OAuth login example\n    (`# scopes: campaigns, collaborations, agreements:write`). These do not match the repo's\n    naming scheme and no reconciliation is published; recorded separately rather than merged.\n  source: https://www.cloutdesk.com/agent-platform\n  scopes:\n  - {scope: campaigns, description: Access to campaigns}\n  - {scope: collaborations, description: Access to collaborations}\n  - {scope: 'agreements:write', description: Write access to agreements, access: write}\nconsent_model:\n  granular: true\n  detail: >-\n    'Every action declares the scopes it requires; user consent is granular, not\n    all-or-nothing.' Sensitive actions — e-signature, email send, and creator ingest — are\n    separately consented and explicitly NOT folded into a generic write scope.\n  source: https://www.cloutdesk.com/agent-platform\n\
  gaps:\n- No scopes are published for campaigns, agreements, messaging, or content-approval writes, even\n  though the Agent Platform page lists all four as agent capabilities.\n- No scope reference / permissions page exists; the catalog below is a floor, not a ceiling.\n- The repo scheme and the marketing scheme use different names for the same resources.\ncross_links:\n  authentication: authentication/cloutjam-authentication.yml\n  mcp: mcp/cloutjam-mcp.yml\n  skills: skills/_index.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloutjam/refs/heads/main/scopes/cloutjam-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Influencer Marketing
- Creator Management
- Creator Economy
- Marketing
- Agentic AI
- Agents
- MCP
- Agent Skills
- Talent Management
- Influencer Marketing Platform
token_urls: []
---
