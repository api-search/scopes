---
api_specs:
- filename: harvard-dataverse-openapi.yml
  format: yaml
  label: Harvard Dataverse API
  slug: dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harvard/refs/heads/main/openapi/harvard-dataverse-openapi.yml
- filename: harvard-lil-legal-ed-skills-hub-openapi.yml
  format: yaml
  label: Legal Ed Skills Hub (Harvard Law School Library Innovation Lab)
  slug: lil-lawskills
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harvard/refs/heads/main/openapi/harvard-lil-legal-ed-skills-hub-openapi.yml
authorization_urls: []
description: Harvard publishes NO OAuth scope vocabulary on any surface an outside developer can reach. This artifact records that absence with evidence rather than leaving the slot empty, because an absent scopes file and a verified-empty scopes file are different findings. The one place scopes plausibly exist - the HUIT API Portal's OAuth application registration - is behind HarvardKey, so the vocabulary could not be read.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Harvard Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Harvard University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Harvard University
provider_slug: harvard
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: harvard-scopes
source_filename: harvard-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons Scopes\nspecificationVersion: '0.1'\nprovider: Harvard University\nproviderId: harvard\ngenerated: '2026-08-19'\nmethod: probed\nsource: >-\n  Probes of every institution-operated surface listed in apis.yml, 2026-08-19, checking for\n  OAuth scope declarations, securitySchemes with scope maps, and discovery documents.\nx-operator: institution\ndescription: >-\n  Harvard publishes NO OAuth scope vocabulary on any surface an outside developer can reach.\n  This artifact records that absence with evidence rather than leaving the slot empty, because\n  an absent scopes file and a verified-empty scopes file are different findings. The one place\n  scopes plausibly exist - the HUIT API Portal's OAuth application registration - is behind\n  HarvardKey, so the vocabulary could not be read.\nscopes: []\nfindings:\n  - surface: Harvard Dataverse native REST API\n    result: no_scopes\n    evidence:\n      - url: https://dataverse.harvard.edu/openapi\n     \
  \   status: 200\n        note: >-\n          The 450-path, 574-operation contract Harvard Dataverse serves declares no\n          components.securitySchemes block at all and no top-level security requirement.\n          Authorization is a bearer-style API token with no scope dimension.\n  - surface: Harvard Art Museums API\n    result: no_scopes\n    evidence:\n      - url: https://api.harvardartmuseums.org/object?size=1\n        status: 401\n        note: Single flat API key. No scope, tier or grant vocabulary documented.\n  - surface: Harvard API Portal (HUIT)\n    result: unreadable\n    evidence:\n      - url: https://portal.apis.huit.harvard.edu/apis\n        status: 200\n        note: >-\n          Apigee developer portal. OAuth app registration and any per-product scope\n          vocabulary sit behind HarvardKey; the anonymous response is an Angular shell.\n  - surface: Harvard DASH / LibraryCloud / OAI-PMH\n    result: not_applicable\n    evidence:\n      - url: https://api.lib.harvard.edu/v2/items.json?title=chess&limit=1\n\
  \        status: 200\n        note: Fully open read surfaces with no authorization layer to scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harvard/refs/heads/main/scopes/harvard-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United States
- Ivy League
- Private Research University
- Research Data
- Research Repository
- Open Metadata
- OAI-PMH
- Identity Federation
- Libraries
- Museums
- Course Catalog
- Research Computing
token_urls: []
---
