---
authorization_urls: []
description: ''
docs: https://help.enboarder.com/en/articles/4151199-enboarder-api-docs-authentication-overview
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Enboarder Scopes
name_suffix: OAuth Scopes
note: Enboarder publishes no OpenAPI, so these scopes were not derived from a spec — they are the exact scope string the Authentication & Overview article instructs clients to request on the OAuth 2.0 client-credentials token call. Enboarder does not publish a dedicated scopes/permissions reference page, so descriptions below are mapped from the URI families each scope gates in the documentation, not from provider-written text.
overview: 'Enboarder publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Enboarder API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Enboarder
provider_slug: enboarder
schemes:
- flows:
  - flow: clientCredentials
    tokenUrls:
    - https://auth.syd.e1.enboarder.com/oauth2/token
    - https://auth.fra.e1.enboarder.com/oauth2/token
    - https://auth.ore.e1.enboarder.com/oauth2/token
  name: oauth2-client-credentials
scope_count: 3
scope_names:
- api/workflow.basic
- api/workflow.advance
- api/settings.all
scopes:
- description: Launch and manage single-manager (basic) Enboarder workflows.
  flows:
  - clientCredentials
  scope: api/workflow.basic
- description: Launch and manage multi-manager (advanced) Enboarder workflows, including bulk advanced launches.
  flows:
  - clientCredentials
  scope: api/workflow.advance
- description: Read and sync account settings surfaces — Categories, Custom Fields, Locations and Brands — against a core system.
  flows:
  - clientCredentials
  scope: api/settings.all
slug: enboarder-scopes
source_filename: enboarder-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://help.enboarder.com/en/articles/4151199-enboarder-api-docs-authentication-overview\ndocs: https://help.enboarder.com/en/articles/4151199-enboarder-api-docs-authentication-overview\nnote: >-\n  Enboarder publishes no OpenAPI, so these scopes were not derived from a spec — they\n  are the exact scope string the Authentication & Overview article instructs clients to\n  request on the OAuth 2.0 client-credentials token call. Enboarder does not publish a\n  dedicated scopes/permissions reference page, so descriptions below are mapped from the\n  URI families each scope gates in the documentation, not from provider-written text.\nschemes:\n- name: oauth2-client-credentials\n  flows:\n  - flow: clientCredentials\n    tokenUrls:\n    - https://auth.syd.e1.enboarder.com/oauth2/token\n    - https://auth.fra.e1.enboarder.com/oauth2/token\n    - https://auth.ore.e1.enboarder.com/oauth2/token\nscope_string_published: api/workflow.basic\
  \ api/workflow.advance api/settings.all\nscopes:\n- scope: api/workflow.basic\n  description: Launch and manage single-manager (basic) Enboarder workflows.\n  flows:\n  - clientCredentials\n  sources:\n  - https://help.enboarder.com/en/articles/4151224-enboarder-api-docs-launch-a-basic-workflow\n- scope: api/workflow.advance\n  description: Launch and manage multi-manager (advanced) Enboarder workflows, including bulk advanced launches.\n  flows:\n  - clientCredentials\n  sources:\n  - https://help.enboarder.com/en/articles/4151298-enboarder-api-docs-launch-an-advanced-workflow\n- scope: api/settings.all\n  description: >-\n    Read and sync account settings surfaces — Categories, Custom Fields, Locations and\n    Brands — against a core system.\n  flows:\n  - clientCredentials\n  sources:\n  - https://help.enboarder.com/en/collections/2404029-enboarder-api-docs\ngaps:\n- No published scope reference page; the scope list is embedded in the authentication article only.\n- No scope is documented\
  \ for the /scim/v2 surface, which uses bearer or basic auth rather than the scoped OAuth grant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enboarder/refs/heads/main/scopes/enboarder-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Company
- Human Resources
- Employee Onboarding
- Employee Experience
- HR Technology
- Workflow Automation
- SCIM
- Identity Provisioning
- Webhooks
- Offboarding
token_urls: []
---
