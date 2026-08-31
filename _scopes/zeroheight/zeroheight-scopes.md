---
api_specs:
- filename: zeroheight-open-api-v2.yml
  format: yaml
  label: Zeroheight API
  slug: zeroheight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeroheight/refs/heads/main/openapi/zeroheight-open-api-v2.yml
authorization_urls: []
description: 'zeroheight''s REST API is key-authenticated, not OAuth, so there is no OAuth scope registry to derive. What zeroheight does publish is a token-scoping model: every token is created against a pre-defined "use case" that fixes its scope set, with an access level of Read or Read and write, and Enterprise customers can additionally pick granular CLI scopes. The named use cases below are the closest thing zeroheight publishes to a scope reference; the individual granular scope strings are only shown inside the Enterprise token-creation UI and are not published, so they are recorded as unknown rather than guessed.'
docs: https://help.zeroheight.com/hc/en-us/articles/35887043412251-Zeroheight-API-Authentication-token-creation
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Zeroheight Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zeroheight uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zeroheight
provider_slug: zeroheight
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: zeroheight-scopes
source_filename: zeroheight-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons Scopes\nspecificationVersion: '0.1'\nprovider: Zeroheight\nproviderId: zeroheight\ngenerated: '2026-08-28'\nmethod: searched\nsource: https://help.zeroheight.com/hc/en-us/articles/35887043412251-Zeroheight-API-Authentication-token-creation\ndocs: https://help.zeroheight.com/hc/en-us/articles/35887043412251-Zeroheight-API-Authentication-token-creation\ndescription: >-\n  zeroheight's REST API is key-authenticated, not OAuth, so there is no OAuth scope registry to\n  derive. What zeroheight does publish is a token-scoping model: every token is created against a\n  pre-defined \"use case\" that fixes its scope set, with an access level of Read or Read and write,\n  and Enterprise customers can additionally pick granular CLI scopes. The named use cases below are\n  the closest thing zeroheight publishes to a scope reference; the individual granular scope strings\n  are only shown inside the Enterprise token-creation UI and are not published, so they are\
  \ recorded\n  as unknown rather than guessed.\nmodel: use-case-scoped API keys (no OAuth scopes on the REST surface)\naccess_levels:\n  - id: read\n    description: Read-only access to the resources covered by the token's use case.\n  - id: read-write\n    description: Required for any action that changes content in zeroheight, e.g. Zapier \"Update Page Status\".\nscopes:\n  - id: measure-adoption\n    name: Measure Adoption\n    type: use-case\n    description: Authenticates @zeroheight/adoption-cli to monitor package versions and track component usage.\n    docs: https://help.zeroheight.com/hc/en-us/articles/35887094424347-Using-the-Adoption-CLI-as-part-a-CI-pipeline\n  - id: zapier\n    name: Zapier\n    type: use-case\n    description: Authenticates Zapier to run automation workflows against page statuses and styleguide releases.\n    docs: https://help.zeroheight.com/hc/en-us/articles/35887062307355-Automate-zeroheight-with-Zapier\n  - id: style-dictionary-exports\n    name: Style\
  \ Dictionary Exports\n    type: use-case\n    description: Authenticates requests to private design-token export URLs.\n    docs: https://help.zeroheight.com/hc/en-us/articles/35887016596123-Exporting-and-integrating-design-tokens-into-developer-pipelines\ngranular_scopes:\n  available: true\n  plans: Enterprise only\n  description: Specific CLI scopes selectable at token creation for precise control over access levels.\n  enumerated: false\n  note: The scope identifiers are not published anywhere zeroheight makes public; they are shown only in the Enterprise token-creation form. Not guessed here.\nmcp_scopes:\n  model: role-derived, not scope-string based\n  note: >-\n    Over MCP, capability follows the signed-in user's zeroheight role rather than a scope claim.\n    Admins/editors connected via MCP via login get the closed-beta write tools; SSO viewers, MCP via\n    link and local MCP connections are read-only.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeroheight/refs/heads/main/scopes/zeroheight-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Design Systems
- Design Tokens
- Documentation
- Model Context Protocol
- Agent Readiness
- Developer Tools
- Design
- Figma
- Storybook
- Design Operations
token_urls: []
---
