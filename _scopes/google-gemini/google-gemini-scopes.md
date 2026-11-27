---
api_specs:
- filename: google-gemini-auth-tokens-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Auth Tokens API
  slug: google-gemini-auth-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-auth-tokens-api-openapi.yml
- filename: google-gemini-batches-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Batches API
  slug: google-gemini-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-batches-api-openapi.yml
- filename: google-gemini-corpora-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Corpora API
  slug: google-gemini-corpora-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-corpora-api-openapi.yml
- filename: google-gemini-dynamic-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Dynamic API
  slug: google-gemini-dynamic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-dynamic-api-openapi.yml
- filename: google-gemini-environments-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Environments API
  slug: google-gemini-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-environments-api-openapi.yml
- filename: google-gemini-files-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Files API
  slug: google-gemini-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-files-api-openapi.yml
- filename: google-gemini-media-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Media API
  slug: google-gemini-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-media-api-openapi.yml
- filename: google-gemini-models-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Models API
  slug: google-gemini-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-models-api-openapi.yml
- filename: google-gemini-cachedcontents-api-openapi.yml
  format: yaml
  label: Google Gemini Cached Contents API
  slug: google-gemini-cachedcontents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-cachedcontents-api-openapi.yml
- filename: google-gemini-filesearchstores-api-openapi.yml
  format: yaml
  label: Google Gemini File Search Stores API
  slug: google-gemini-filesearchstores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-filesearchstores-api-openapi.yml
- filename: google-gemini-generatedfiles-api-openapi.yml
  format: yaml
  label: Google Gemini Generated Files API
  slug: google-gemini-generatedfiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-generatedfiles-api-openapi.yml
- filename: google-gemini-tunedmodels-api-openapi.yml
  format: yaml
  label: Google Gemini Tuned Models API
  slug: google-gemini-tunedmodels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-tunedmodels-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Gemini Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Gemini publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Gemini API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Gemini
provider_slug: google-gemini
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-auth-tokens-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-batches-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-cached-contents-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-corpora-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-dynamic-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-environments-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-file-search-stores-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-files-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-generated-files-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-media-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-models-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-gemini-tuned-models-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/devstorage.read_only
scopes:
- description: View your data in Google Cloud Storage
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/devstorage.read_only
slug: google-gemini-scopes
source_filename: google-gemini-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-gemini-auth-tokens-api-openapi.yml, openapi/google-gemini-batches-api-openapi.yml,\n  openapi/google-gemini-cached-contents-api-openapi.yml, openapi/google-gemini-corpora-api-openapi.yml,\n  openapi/google-gemini-dynamic-api-openapi.yml, openapi/google-gemini-environments-api-openapi.yml,\n  openapi/google-gemini-file-search-stores-api-openapi.yml, openapi/google-gemini-files-api-openapi.yml,\n  openapi/google-gemini-generated-files-api-openapi.yml, openapi/google-gemini-media-api-openapi.yml,\n  openapi/google-gemini-models-api-openapi.yml, openapi/google-gemini-tuned-models-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-gemini-auth-tokens-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-batches-api-openapi.yml\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-cached-contents-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-corpora-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-dynamic-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-environments-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n\
  \    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-file-search-stores-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-files-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-generated-files-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-media-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source:\
  \ openapi/google-gemini-models-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-gemini-tuned-models-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/devstorage.read_only\n  description: View your data in Google Cloud Storage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-gemini-auth-tokens-api-openapi.yml\n  - openapi/google-gemini-batches-api-openapi.yml\n  - openapi/google-gemini-cached-contents-api-openapi.yml\n  - openapi/google-gemini-corpora-api-openapi.yml\n  - openapi/google-gemini-dynamic-api-openapi.yml\n  - openapi/google-gemini-environments-api-openapi.yml\n  - openapi/google-gemini-file-search-stores-api-openapi.yml\n  - openapi/google-gemini-files-api-openapi.yml\n\
  \  - openapi/google-gemini-generated-files-api-openapi.yml\n  - openapi/google-gemini-media-api-openapi.yml\n  - openapi/google-gemini-models-api-openapi.yml\n  - openapi/google-gemini-tuned-models-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-gemini/scopes/google-gemini-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- AI Agents
- Artificial Intelligence
- Code Generation
- Embeddings
- Generative AI
- Image Generation
- LLM
- Machine Learning
- Multi-Modal
- Real-Time
- Foundation Models
- Agents
- Audio Understanding
- Batch Processing
- Deep Research
- Document Understanding
- Function Calling
- Structured Output
- Text-to-Speech
- Video Generation
- Video Understanding
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
