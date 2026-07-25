---
api_specs:
- filename: hyperscience-audit-logs-api-openapi.yml
  format: yaml
  label: Hyperscience Audit Logs API
  slug: hyperscience-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-audit-logs-api-openapi.yml
- filename: hyperscience-cases-api-openapi.yml
  format: yaml
  label: Hyperscience Cases API
  slug: hyperscience-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-cases-api-openapi.yml
- filename: hyperscience-documents-api-openapi.yml
  format: yaml
  label: Hyperscience Documents API
  slug: hyperscience-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-documents-api-openapi.yml
- filename: hyperscience-flow-runs-api-openapi.yml
  format: yaml
  label: Hyperscience Flow Runs API
  slug: hyperscience-flow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-flow-runs-api-openapi.yml
- filename: hyperscience-flows-api-openapi.yml
  format: yaml
  label: Hyperscience Flows API
  slug: hyperscience-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-flows-api-openapi.yml
- filename: hyperscience-layouts-api-openapi.yml
  format: yaml
  label: Hyperscience Layouts API
  slug: hyperscience-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-layouts-api-openapi.yml
- filename: hyperscience-pages-api-openapi.yml
  format: yaml
  label: Hyperscience Pages API
  slug: hyperscience-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-pages-api-openapi.yml
- filename: hyperscience-submissions-api-openapi.yml
  format: yaml
  label: Hyperscience Submissions API
  slug: hyperscience-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-submissions-api-openapi.yml
- filename: hyperscience-version-api-openapi.yml
  format: yaml
  label: Hyperscience Version API
  slug: hyperscience-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-version-api-openapi.yml
authorization_urls: []
description: ''
docs: https://help.hyperscience.ai/deployment/docs/machine-to-machine-authentication-with-oauth-20
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Hyperscience Scopes
name_suffix: OAuth Scopes
note: Hyperscience's OAuth 2.0 M2M flow does not use published scopes; API access is governed by permission groups (e.g., the API Access permission) rather than OAuth scopes (https://help.hyperscience.ai/deployment/docs/machine-to-machine-authentication-with-oauth-20).
overview: 'Hyperscience uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{server}.{company}.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hyperscience
provider_slug: hyperscience
schemes:
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: hyperscience-scopes
source_filename: hyperscience-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hyperscience-openapi.yml\ndocs: https://help.hyperscience.ai/deployment/docs/machine-to-machine-authentication-with-oauth-20\nnote: Hyperscience's OAuth 2.0 M2M flow does not use published scopes; API access is\n  governed by permission groups (e.g., the API Access permission) rather than OAuth scopes\n  (https://help.hyperscience.ai/deployment/docs/machine-to-machine-authentication-with-oauth-20).\nschemes:\n- name: OAuth2\n  source: openapi/hyperscience-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/scopes/hyperscience-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI
- Document AI
- IDP
- Enterprise
- Automation
- GenAI
- FedRAMP
token_urls:
- https://{server}.{company}.com/oauth/token
---
