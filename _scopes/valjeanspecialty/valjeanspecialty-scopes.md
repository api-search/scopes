---
api_specs:
- filename: valjeanspecialty-account-api-openapi.yml
  format: yaml
  label: Valjean Specialty Account API
  slug: valjeanspecialty-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-account-api-openapi.yml
- filename: valjeanspecialty-answers-api-openapi.yml
  format: yaml
  label: Valjean Specialty Answers API
  slug: valjeanspecialty-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-answers-api-openapi.yml
- filename: valjeanspecialty-appetite-api-openapi.yml
  format: yaml
  label: Valjean Specialty Appetite API
  slug: valjeanspecialty-appetite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-appetite-api-openapi.yml
- filename: valjeanspecialty-bind-api-openapi.yml
  format: yaml
  label: Valjean Specialty Bind API
  slug: valjeanspecialty-bind-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-bind-api-openapi.yml
- filename: valjeanspecialty-documents-api-openapi.yml
  format: yaml
  label: Valjean Specialty Documents API
  slug: valjeanspecialty-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-documents-api-openapi.yml
- filename: valjeanspecialty-events-api-openapi.yml
  format: yaml
  label: Valjean Specialty Events API
  slug: valjeanspecialty-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-events-api-openapi.yml
- filename: valjeanspecialty-instant-quotes-api-openapi.yml
  format: yaml
  label: Valjean Specialty Instant quotes API
  slug: valjeanspecialty-instant-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-instant-quotes-api-openapi.yml
- filename: valjeanspecialty-invoices-api-openapi.yml
  format: yaml
  label: Valjean Specialty Invoices API
  slug: valjeanspecialty-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-invoices-api-openapi.yml
- filename: valjeanspecialty-policies-api-openapi.yml
  format: yaml
  label: Valjean Specialty Policies API
  slug: valjeanspecialty-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-policies-api-openapi.yml
- filename: valjeanspecialty-public-api-openapi.yml
  format: yaml
  label: Valjean Specialty Public API
  slug: valjeanspecialty-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-public-api-openapi.yml
- filename: valjeanspecialty-quotes-api-openapi.yml
  format: yaml
  label: Valjean Specialty Quotes API
  slug: valjeanspecialty-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-quotes-api-openapi.yml
- filename: valjeanspecialty-requirements-api-openapi.yml
  format: yaml
  label: Valjean Specialty Requirements API
  slug: valjeanspecialty-requirements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-requirements-api-openapi.yml
- filename: valjeanspecialty-submissions-api-openapi.yml
  format: yaml
  label: Valjean Specialty Submissions API
  slug: valjeanspecialty-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-submissions-api-openapi.yml
- filename: valjeanspecialty-webhooks-api-openapi.yml
  format: yaml
  label: Valjean Specialty Webhooks API
  slug: valjeanspecialty-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-webhooks-api-openapi.yml
authorization_urls:
- https://api.valjeanspecialty.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Valjeanspecialty Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Valjean Specialty publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Valjean Specialty API on a user''s behalf.


  Tokens are issued from https://api.valjeanspecialty.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Valjean Specialty
provider_slug: valjeanspecialty
schemes:
- description: 'For AI apps that connect by signing in. Authorization code flow with PKCE (S256 only), public clients (no secret), dynamic client registration at https://api.valjeanspecialty.com/oauth/register. Discovery: https://api.valjeanspecialty.com/.well-known/oauth-authorization-server. Access tokens last 1 hour; refresh tokens 30 days and rotate on use. Tokens stop when the API key or portal link that approved them is revoked.'
  flows:
  - authorizationUrl: https://api.valjeanspecialty.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.valjeanspecialty.com/oauth/token
  name: oauth2
  source: openapi/valjeanspecialty-openapi.yaml
scope_count: 2
scope_names:
- read
- submit
scopes:
- description: Appetite, requirements, status, quotes, documents, policies
  flows:
  - authorizationCode
  scope: read
- description: Also send files, answers, documents, bind requests and instant-quote asks
  flows:
  - authorizationCode
  scope: submit
slug: valjeanspecialty-scopes
source_filename: valjeanspecialty-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/valjeanspecialty-openapi.yaml\nschemes:\n- name: oauth2\n  source: openapi/valjeanspecialty-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.valjeanspecialty.com/oauth/authorize\n    tokenUrl: https://api.valjeanspecialty.com/oauth/token\n  description: 'For AI apps that connect by signing in. Authorization code flow with PKCE (S256\n    only), public clients (no secret), dynamic client registration at https://api.valjeanspecialty.com/oauth/register.\n    Discovery: https://api.valjeanspecialty.com/.well-known/oauth-authorization-server. Access\n    tokens last 1 hour; refresh tokens 30 days and rotate on use. Tokens stop when the API key\n    or portal link that approved them is revoked.'\nscopes:\n- scope: read\n  description: Appetite, requirements, status, quotes, documents, policies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/valjeanspecialty-openapi.yaml\n- scope:\
  \ submit\n  description: Also send files, answers, documents, bind requests and instant-quote asks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/valjeanspecialty-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/valjeanspecialty/scopes/valjeanspecialty-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Insurance
- Wholesale
- Brokerage
- E&S
- Insurance Tech
token_bound: false
token_urls:
- https://api.valjeanspecialty.com/oauth/token
---
