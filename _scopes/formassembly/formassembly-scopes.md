---
authorization_urls:
- https://app.formassembly.com/oauth/login
description: ''
docs: https://github.com/FormAssembly/formassembly-api
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Formassembly Scopes
name_suffix: OAuth Scopes
note: FormAssembly's OAuth2 API documents an authorization-code flow whose token response includes a scope field, but publishes no named scopes; access tokens are user-based with permissions tied to the authorizing user's account (https://github.com/FormAssembly/formassembly-api).
overview: 'FormAssembly uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://app.formassembly.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FormAssembly
provider_slug: formassembly
schemes:
- flows:
  - authorizationUrl: https://app.formassembly.com/oauth/login
    flow: authorizationCode
    tokenUrl: https://app.formassembly.com/oauth/access_token
  name: oauth2
  source: openapi/formassembly-formassembly-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: formassembly-scopes
source_filename: formassembly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formassembly-formassembly-api-openapi.yml\ndocs: https://github.com/FormAssembly/formassembly-api\nnote: FormAssembly's OAuth2 API documents an authorization-code flow whose token response includes a scope field, but publishes no named scopes; access tokens are user-based with permissions tied to the authorizing user's account (https://github.com/FormAssembly/formassembly-api).\nschemes:\n- name: oauth2\n  source: openapi/formassembly-formassembly-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.formassembly.com/oauth/login\n    tokenUrl: https://app.formassembly.com/oauth/access_token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/scopes/formassembly-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Forms
- Data Collection
- Salesforce
- Enterprise
- HIPAA
- Compliance
- Government
- FedRAMP
- Workflows
- E-Signatures
token_urls:
- https://app.formassembly.com/oauth/access_token
---
