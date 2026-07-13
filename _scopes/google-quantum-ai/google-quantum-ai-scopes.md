---
api_specs:
- filename: quantum-engine-api-openapi.yml
  format: yaml
  label: Google Quantum Engine API
  slug: quantum-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/quantum-engine-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Quantum Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Quantum AI publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Quantum AI API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Quantum AI
provider_slug: google-quantum-ai
schemes:
- description: OAuth 2.0 via Google Cloud Application Default Credentials.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: googleOAuth
  source: openapi/quantum-engine-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: Read/write access to Google Cloud resources, including Quantum Engine.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-quantum-ai-scopes
source_filename: google-quantum-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quantum-engine-api-openapi.yml\nschemes:\n- name: googleOAuth\n  source: openapi/quantum-engine-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 via Google Cloud Application Default Credentials.\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Read/write access to Google Cloud resources, including Quantum Engine.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quantum-engine-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/scopes/google-quantum-ai-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Quantum Computing
- Quantum
- Hardware
- NISQ
- Error Correction
- Willow
- Sycamore
- Cirq
- Quantum Engine
- Superconducting Qubits
- Google Cloud
token_urls:
- https://oauth2.googleapis.com/token
---
