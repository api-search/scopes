---
authorization_urls: []
description: ''
docs: https://congressmcp.com/docs
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: CongressMCP Scopes
name_suffix: OAuth Scopes
note: Scope table copied from the docs "Scope / What it allows / Availability" table. Default connection permissions are legislative.read, personal.read, personal.write, workspace.read, workspace.write and browser.drive; automation.run stays opt-in. The legacy `read` scope is an alias of legislative.read.
overview: 'CongressMCP publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CongressMCP API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CongressMCP
provider_slug: congressmcp-com
schemes: []
scope_count: 7
scope_names:
- legislative.read
- personal.read
- personal.write
- workspace.read
- workspace.write
- automation.run
- browser.drive
scopes:
- description: Federal and state legislative research tools (bills, members, votes, committees, sessions, datasets). The legacy read scope is an alias.
  flows: []
  scope: legislative.read
- description: Read your own personal settings, representatives, watchlist and alert preferences.
  flows: []
  scope: personal.read
- description: Save personal settings and follow or unfollow bills in your own personal workspaces. Explorer allows 10 active follows and one daily in-app digest for enabled alerts.
  flows: []
  scope: personal.write
- description: Read your tenant's contacts, organizations, issues, tracked bills, news, briefings, and other workspace records.
  flows: []
  scope: workspace.read
- description: 'Create and update workspace records: notes, tasks, tracked bills, CRM entries, monitors, webhooks, review queues, comments.'
  flows: []
  scope: workspace.write
- description: Run scheduled and bulk workflows (monitors, cascades, playbooks) on the workspace's behalf.
  flows: []
  scope: automation.run
- description: 'Watch Mode: navigate, highlight, and refresh an open CongressMCP browser tab while the AI works.'
  flows: []
  scope: browser.drive
slug: congressmcp-com-scopes
source_filename: congressmcp-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://congressmcp.com/docs\ndocs: https://congressmcp.com/docs\nnote: Scope table copied from the docs \"Scope / What it allows / Availability\" table. Default connection permissions are legislative.read, personal.read, personal.write, workspace.read, workspace.write and browser.drive; automation.run stays opt-in. The legacy `read` scope is an alias of legislative.read.\nscopes:\n- name: legislative.read\n  description: Federal and state legislative research tools (bills, members, votes, committees, sessions, datasets). The legacy read scope is an alias.\n  availability: All plans. Free covers federal Congress.gov records; state data and calculated intelligence need a paid plan.\n- name: personal.read\n  description: Read your own personal settings, representatives, watchlist and alert preferences.\n  availability: Paid plans (Explorer and above)\n- name: personal.write\n  description: Save personal settings and follow or\
  \ unfollow bills in your own personal workspaces. Explorer allows 10 active follows and one daily in-app digest for enabled alerts.\n  availability: Paid plans (Explorer and above), within plan limits\n- name: workspace.read\n  description: Read your tenant's contacts, organizations, issues, tracked bills, news, briefings, and other workspace records.\n  availability: Briefcase, Indie, Pro, Platform & Teams\n- name: workspace.write\n  description: 'Create and update workspace records: notes, tasks, tracked bills, CRM entries, monitors, webhooks, review queues, comments.'\n  availability: Briefcase, Indie, Pro, Platform & Teams\n- name: automation.run\n  description: Run scheduled and bulk workflows (monitors, cascades, playbooks) on the workspace's behalf.\n  availability: Briefcase, Indie, Pro, Platform & Teams · opt-in\n- name: browser.drive\n  description: 'Watch Mode: navigate, highlight, and refresh an open CongressMCP browser tab while the AI works.'\n  availability: Briefcase, Indie,\
  \ Pro, Platform & Teams · on by default\n"
source_yaml_url: https://artifacts.apis.io/congressmcp-com/scopes/congressmcp-com-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Legislation
- Government
- Congress
- State Legislatures
- Bill Tracking
- MCP
- Artificial Intelligence
- Policy Research
token_bound: false
token_urls: []
---
