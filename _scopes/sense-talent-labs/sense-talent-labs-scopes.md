---
api_specs:
- filename: sense-talent-labs-sense-api-openapi.json
  format: json
  label: Sense API
  slug: sense-talent-labs-sense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/openapi/sense-talent-labs-sense-api-openapi.json
authorization_urls: []
description: ''
docs: https://developer.sensehq.com/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Sense Talent Labs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sense Talent Labs publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sense Talent Labs API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sense Talent Labs
provider_slug: sense-talent-labs
schemes: []
scope_count: 1
scope_names:
- N/A
scopes:
- description: The Sense API does not require a scope to be provided.
  flows:
  - clientCredentials
  scope: N/A
slug: sense-talent-labs-scopes
source_filename: sense-talent-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://developer.sensehq.com/\ndocs: https://developer.sensehq.com/\nscheme: sense_authentication\nflow: clientCredentials\nscope_model: none\nscope_count: 0\nsummary: 'The Sense API declares an OAuth 2.0 clientCredentials securityScheme but publishes no\n  scope vocabulary. The single entry in the spec''s scopes map is the literal placeholder \"N/A\"\n  with the description \"The Sense API does not require a scope to be provided.\" Authorization is\n  therefore all-or-nothing per client credential: a credential is bound to one agency tenant\n  (your-agency-name.sensehq.com) and carries full read and write access to every entity type the\n  API exposes. There is no least-privilege or per-entity scoping surface available to an\n  integrator or an agent.'\nscopes:\n- scope: N/A\n  description: The Sense API does not require a scope to be provided.\n  verbatim: true\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sense-talent-labs-sense-api-openapi.json\n\
  tenancy:\n  model: one credential per agency tenant\n  source: https://developer.sensehq.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sense-talent-labs/refs/heads/main/scopes/sense-talent-labs-scopes.yml
summary_line: 1 scope
tags:
- Human Resources
- Recruiting
- Talent Acquisition
- Staffing
- Applicant Tracking
- Candidate Engagement
- Recruiting Automation
- Talent CRM
- Messaging
- Interview Scheduling
- Artificial Intelligence
- SaaS
token_urls: []
---
