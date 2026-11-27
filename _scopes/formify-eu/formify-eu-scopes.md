---
api_specs:
- filename: formify-eu-account-api-openapi.yml
  format: yaml
  label: Formify Account API
  slug: formify-eu-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-account-api-openapi.yml
- filename: formify-eu-auth-api-openapi.yml
  format: yaml
  label: Formify Auth API
  slug: formify-eu-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-auth-api-openapi.yml
- filename: formify-eu-docs-api-openapi.yml
  format: yaml
  label: Formify Docs API
  slug: formify-eu-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-docs-api-openapi.yml
- filename: formify-eu-drafts-api-openapi.yml
  format: yaml
  label: Formify Drafts API
  slug: formify-eu-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-drafts-api-openapi.yml
- filename: formify-eu-files-api-openapi.yml
  format: yaml
  label: Formify Files API
  slug: formify-eu-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-files-api-openapi.yml
- filename: formify-eu-links-api-openapi.yml
  format: yaml
  label: Formify Links API
  slug: formify-eu-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-links-api-openapi.yml
- filename: formify-eu-oauth-api-openapi.yml
  format: yaml
  label: Formify OAuth API
  slug: formify-eu-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-oauth-api-openapi.yml
- filename: formify-eu-templates-api-openapi.yml
  format: yaml
  label: Formify Templates API
  slug: formify-eu-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-templates-api-openapi.yml
- filename: formify-eu-user-api-openapi.yml
  format: yaml
  label: Formify User API
  slug: formify-eu-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-user-api-openapi.yml
- filename: formify-eu-webhooks-api-openapi.yml
  format: yaml
  label: Formify Webhooks API
  slug: formify-eu-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formify-eu/openapi/formify-eu-webhooks-api-openapi.yml
authorization_urls:
- https://docs-api.formify.eu/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Formify Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Formify publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Formify API on a user''s behalf.


  Tokens are issued from https://docs-api.formify.eu/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Formify
provider_slug: formify-eu
schemes:
- description: OAuth2 Authentication. Allows third-party systems to access the API on behalf of the user and their account after authorization.
  flows:
  - authorizationUrl: https://docs-api.formify.eu/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://docs-api.formify.eu/v1/oauth/token
  name: OAuth2
  source: openapi/formify-eu-openapi.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Allows reading documents and their metadata
  flows:
  - authorizationCode
  scope: read
- description: Allows modifying documents and sending signature requests
  flows:
  - authorizationCode
  scope: write
slug: formify-eu-scopes
source_filename: formify-eu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/formify-eu-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/formify-eu-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docs-api.formify.eu/v1/oauth/authorize\n    tokenUrl: https://docs-api.formify.eu/v1/oauth/token\n  description: OAuth2 Authentication. Allows third-party systems to access the API on behalf\n    of the user and their account after authorization.\nscopes:\n- scope: read\n  description: Allows reading documents and their metadata\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formify-eu-openapi.json\n- scope: write\n  description: Allows modifying documents and sending signature requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formify-eu-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/formify-eu/scopes/formify-eu-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- E-signing
- Legal Tech
- Multilingual
token_bound: false
token_urls:
- https://docs-api.formify.eu/v1/oauth/token
---
