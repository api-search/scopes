---
api_specs:
- filename: flowaccount-openapi-original.json
  format: json
  label: FlowAccount Open API
  slug: flowaccount-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-openapi-original.json
authorization_urls: []
description: 'FlowAccount Open API authorizes with OAuth 2.0 client credentials. Access is granted through a single coarse API scope, flowaccount-api, requested at the token endpoint; per-resource scopes are not published. Evidence: flowaccount/open-api apps/api/flowaccount-webhook/env.json (CLIENT_SCOPE=flowaccount-api).'
docs: https://developers.flowaccount.com/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Flowaccount Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FlowAccount publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the FlowAccount API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FlowAccount
provider_slug: flowaccount
schemes:
- flow: clientCredentials
  name: oauth2ClientCredentials
  source: https://github.com/flowaccount/open-api
  token_endpoint: '{base}/token'
scope_count: 1
scope_names:
- flowaccount-api
scopes:
- description: Full access to the FlowAccount Open API surface permitted for the registered integration (documents, contacts, products, payments). The API does not publish finer-grained per-resource scopes.
  flows:
  - clientCredentials
  scope: flowaccount-api
slug: flowaccount-scopes
source_filename: flowaccount-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/flowaccount/open-api\ndocs: https://developers.flowaccount.com/\ndescription: >-\n  FlowAccount Open API authorizes with OAuth 2.0 client credentials. Access is\n  granted through a single coarse API scope, flowaccount-api, requested at the\n  token endpoint; per-resource scopes are not published. Evidence:\n  flowaccount/open-api apps/api/flowaccount-webhook/env.json (CLIENT_SCOPE=flowaccount-api).\nschemes:\n  - name: oauth2ClientCredentials\n    flow: clientCredentials\n    token_endpoint: \"{base}/token\"\n    source: https://github.com/flowaccount/open-api\nscopes:\n  - scope: flowaccount-api\n    description: >-\n      Full access to the FlowAccount Open API surface permitted for the registered\n      integration (documents, contacts, products, payments). The API does not\n      publish finer-grained per-resource scopes.\n    flows: [clientCredentials]\n    sources: [https://github.com/flowaccount/open-api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/scopes/flowaccount-scopes.yml
summary_line: 1 scope
tags:
- Company
- Accounting
- Invoicing
- Payroll
- Point of Sale
- SME
- Finance
- Tax
- Thailand
- Bookkeeping
token_urls: []
---
