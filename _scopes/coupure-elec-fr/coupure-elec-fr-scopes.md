---
authorization_urls: []
description: ''
docs: https://www.coupure-elec.fr/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Coupure-Elec.fr Scopes
name_suffix: OAuth Scopes
note: These are partner-key scopes, not OAuth scopes. "Toutes les clés ont le scope read . Le scope report est activé au cas par cas."
overview: 'Coupure-Elec.fr publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coupure-Elec.fr API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coupure-Elec.fr
provider_slug: coupure-elec-fr
schemes: []
scope_count: 2
scope_names:
- read
- report
scopes:
- description: Granted to every key. Covers get_city_outage_status, list_recent_outages, get_global_stats and get_network_quality.
  flows: []
  scope: read
- description: Enabled case by case. Covers report_outage, which reports an outage at a given position or reinforces a nearby active outage.
  flows: []
  scope: report
slug: coupure-elec-fr-scopes
source_filename: coupure-elec-fr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.coupure-elec.fr/mcp\ndocs: https://www.coupure-elec.fr/mcp\nnote: These are partner-key scopes, not OAuth scopes. \"Toutes les clés ont le scope read . Le scope report est activé au cas par cas.\"\nscopes:\n- name: read\n  description: Granted to every key. Covers get_city_outage_status, list_recent_outages, get_global_stats and get_network_quality.\n  default: true\n  tools: [get_city_outage_status, list_recent_outages, get_global_stats, get_network_quality]\n- name: report\n  description: Enabled case by case. Covers report_outage, which reports an outage at a given position or reinforces a nearby active outage.\n  default: false\n  tools: [report_outage]\n"
source_yaml_url: https://artifacts.apis.io/coupure-elec-fr/scopes/coupure-elec-fr-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Electricity
- Power Outages
- Energy
- France
- MCP
- Crowdsourcing
- Open Data
token_bound: false
token_urls: []
---
