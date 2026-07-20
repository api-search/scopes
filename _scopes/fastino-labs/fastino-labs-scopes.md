---
api_specs:
- filename: pioneer-openapi-original.json
  format: json
  label: Pioneer Inference API
  slug: pioneer-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastino-labs/refs/heads/main/openapi/pioneer-openapi-original.json
authorization_urls: []
description: ''
docs: https://api.pioneer.ai/.well-known/oauth-protected-resource
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fastino Labs Scopes
name_suffix: OAuth Scopes
note: Pioneer delegates OAuth2/OIDC to a Supabase authorization server. The Pioneer REST API is primarily accessed with an X-API-Key (pio_sk_) key; the OAuth path exposes only the standard OIDC scopes below. The OpenAPI itself declares the bearer token as http/bearer (JWT), not an oauth2 scheme, so no resource-level scopes are published beyond these.
overview: 'Fastino Labs publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fastino Labs API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fastino Labs
provider_slug: fastino-labs
schemes:
- authorizationUrl: https://pwgztilbkupvjmomwbjr.supabase.co/auth/v1/authorize
  flow: authorizationCode
  name: Supabase-OIDC
  pkce:
  - S256
  - plain
  tokenUrl: https://pwgztilbkupvjmomwbjr.supabase.co/auth/v1/token
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access basic profile claims.
  flows: []
  scope: profile
- description: Access the user's email claim.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
slug: fastino-labs-scopes
source_filename: fastino-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.pioneer.ai/.well-known/openid-configuration\ndocs: https://api.pioneer.ai/.well-known/oauth-protected-resource\nnote: >-\n  Pioneer delegates OAuth2/OIDC to a Supabase authorization server. The Pioneer\n  REST API is primarily accessed with an X-API-Key (pio_sk_) key; the OAuth path\n  exposes only the standard OIDC scopes below. The OpenAPI itself declares the\n  bearer token as http/bearer (JWT), not an oauth2 scheme, so no resource-level\n  scopes are published beyond these.\nschemes:\n- name: Supabase-OIDC\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://pwgztilbkupvjmomwbjr.supabase.co/auth/v1/authorize\n  tokenUrl: https://pwgztilbkupvjmomwbjr.supabase.co/auth/v1/token\n  pkce: [S256, plain]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n- scope: profile\n  description: Access basic profile claims.\n- scope: email\n  description: Access the\
  \ user's email claim.\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastino-labs/refs/heads/main/scopes/fastino-labs-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Small Language Models
- Fine-Tuning
- Inference
- Named Entity Recognition
- Information Extraction
- LLM
- Agents
- PII Detection
- Model Training
token_urls: []
---
