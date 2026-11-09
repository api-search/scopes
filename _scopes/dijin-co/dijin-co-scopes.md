---
authorization_urls: []
description: ''
docs: https://dijin.co/en/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Dijin Co Scopes
name_suffix: OAuth Scopes
note: 'Dijin documents two scope vocabularies: the "8 canonical scopes" on the MCP reference / developers page (memory.summary ...), and the connector guide catalogue with a .read suffix (memory.summary.read ...). Recorded both verbatim; llms-full.txt states "external AI clients are read-only — memory.write stays internal".'
overview: 'Dijin publishes 13 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dijin API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dijin
provider_slug: dijin-co
schemes: []
scope_count: 13
scope_names:
- memory.summary
- memory.decisions
- memory.entities
- memory.evidence
- memory.conflicts
- memory.audit
- memory.raw_source.read
- memory.write
- memory.summary.read
- memory.evidence.read
- memory.entities.read
- memory.audit.read
- memory.conflicts.read
scopes:
- description: Read high-level summaries only.
  flows: []
  scope: memory.summary
- description: Read confirmed decisions and their rationale.
  flows: []
  scope: memory.decisions
- description: Read people, projects, and things in your memory graph.
  flows: []
  scope: memory.entities
- description: Read the evidence pack behind an answer.
  flows: []
  scope: memory.evidence
- description: Read where claims disagree or were superseded.
  flows: []
  scope: memory.conflicts
- description: Read the tamper-evident access log.
  flows: []
  scope: memory.audit
- description: Read raw source text. Highest-trust scope. Pro-gated, device-confirmed, and never granted by default.
  flows: []
  scope: memory.raw_source.read
- description: memory.write proposes memory, corrections, or links. It never silently mutates the graph; proposals pass through the worker, policy checks, and review gates.
  flows: []
  scope: memory.write
- description: Daily/weekly summaries, action items, decisions extracted from the user’s memory.
  flows: []
  scope: memory.summary.read
- description: Short quoted passages tied to specific insights and decisions.
  flows: []
  scope: memory.evidence.read
- description: People, organisations, places, concepts extracted across sessions.
  flows: []
  scope: memory.entities.read
- description: The user’s connector access ledger — every OAuth grant, scope-denied event, rate-limit hit, tool call.
  flows: []
  scope: memory.audit.read
- description: Flagged contradictions across the user’s memory (same subject + same predicate but different facts).
  flows: []
  scope: memory.conflicts.read
slug: dijin-co-scopes
source_filename: dijin-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dijin.co/en/mcp ; https://dijin.co/docs/connector\ndocs: https://dijin.co/en/mcp\nscopes:\n- name: memory.summary\n  description: Read high-level summaries only.\n  source: https://dijin.co/en/mcp\n- name: memory.decisions\n  description: Read confirmed decisions and their rationale.\n  source: https://dijin.co/en/mcp\n- name: memory.entities\n  description: Read people, projects, and things in your memory graph.\n  source: https://dijin.co/en/mcp\n- name: memory.evidence\n  description: Read the evidence pack behind an answer.\n  source: https://dijin.co/en/mcp\n- name: memory.conflicts\n  description: Read where claims disagree or were superseded.\n  source: https://dijin.co/en/mcp\n- name: memory.audit\n  description: Read the tamper-evident access log.\n  source: https://dijin.co/en/mcp\n- name: memory.raw_source.read\n  description: Read raw source text. Highest-trust scope. Pro-gated, device-confirmed, and never\
  \ granted\n    by default.\n  source: https://dijin.co/en/mcp\n  gated: Pro\n- name: memory.write\n  description: memory.write proposes memory, corrections, or links. It never silently mutates the graph;\n    proposals pass through the worker, policy checks, and review gates.\n  source: https://dijin.co/en/mcp\n  gated: Pro\n- name: memory.summary.read\n  description: Daily/weekly summaries, action items, decisions extracted from the user’s memory.\n  source: https://dijin.co/docs/connector\n- name: memory.evidence.read\n  description: Short quoted passages tied to specific insights and decisions.\n  source: https://dijin.co/docs/connector\n- name: memory.entities.read\n  description: People, organisations, places, concepts extracted across sessions.\n  source: https://dijin.co/docs/connector\n- name: memory.audit.read\n  description: The user’s connector access ledger — every OAuth grant, scope-denied event, rate-limit\n    hit, tool call.\n  source: https://dijin.co/docs/connector\n\
  - name: memory.conflicts.read\n  description: Flagged contradictions across the user’s memory (same subject + same predicate but different\n    facts).\n  source: https://dijin.co/docs/connector\nnote: 'Dijin documents two scope vocabularies: the \"8 canonical scopes\" on the MCP reference / developers\n  page (memory.summary ...), and the connector guide catalogue with a .read suffix (memory.summary.read\n  ...). Recorded both verbatim; llms-full.txt states \"external AI clients are read-only — memory.write\n  stays internal\".'\n"
source_yaml_url: https://artifacts.apis.io/dijin-co/scopes/dijin-co-scopes.yml
summary_line: 13 scopes
tags:
- Company
- AI Agents
- Memory
- MCP
- Personal Data
- Privacy
- OAuth
token_bound: false
token_urls: []
---
