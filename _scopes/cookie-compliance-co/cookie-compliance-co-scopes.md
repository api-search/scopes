---
authorization_urls: []
description: ''
docs: https://manual.hu-manity.co/connect/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cookie Compliance Scopes
name_suffix: OAuth Scopes
note: Scopes and descriptions are copied from the signIn.scopes block of the MCP server's landing metadata (saved as examples/cookie-compliance-co-mcp-landing-metadata.json). They apply to https://mcp.cookie-compliance.co/mcp/account.
overview: 'Cookie Compliance publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cookie Compliance API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cookie Compliance
provider_slug: cookie-compliance-co
schemes: []
scope_count: 3
scope_names:
- banner:read
- banner:write
- offline_access
scopes:
- description: See your registered websites, how their cookie banner is set up, and daily totals of the consent choices visitors made (never individual visitors' details)
  flows: []
  scope: banner:read
- description: Change your cookie banner — its design, wording, and its consent and blocking settings
  flows: []
  scope: banner:write
- description: 'Accepted for clients that ask for it. Grants nothing extra: a signed-in connection already renews itself.'
  flows: []
  scope: offline_access
slug: cookie-compliance-co-scopes
source_filename: cookie-compliance-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://mcp.cookie-compliance.co/\ndocs: https://manual.hu-manity.co/connect/\nname: Cookie Compliance OAuth scopes\nnote: Scopes and descriptions are copied from the signIn.scopes block of the MCP server's landing metadata (saved as examples/cookie-compliance-co-mcp-landing-metadata.json). They apply to https://mcp.cookie-compliance.co/mcp/account.\nscopes:\n- name: banner:read\n  description: See your registered websites, how their cookie banner is set up, and daily totals of the consent choices visitors made (never individual visitors' details)\n- name: banner:write\n  description: Change your cookie banner — its design, wording, and its consent and blocking settings\n- name: offline_access\n  description: 'Accepted for clients that ask for it. Grants nothing extra: a signed-in connection already renews itself.'\n"
source_yaml_url: https://artifacts.apis.io/cookie-compliance-co/scopes/cookie-compliance-co-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Cookie Consent
- Consent Management
- Privacy
- GDPR
- CCPA
- Compliance
- MCP
token_bound: false
token_urls: []
---
