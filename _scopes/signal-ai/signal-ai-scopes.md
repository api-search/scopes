---
api_specs:
- filename: signal-ai-openapi-original.json
  format: json
  label: Signal AI API
  slug: signal-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/openapi/signal-ai-openapi-original.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Signal Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Signal AI publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Signal AI API on a user''s behalf.


  Tokens are issued from https://api.signal-ai.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Signal AI
provider_slug: signal-ai
schemes:
- description: "To obtain the Bearer Token using the Client ID / Secret pair provided to you:\n\n```bash\ncurl -X POST \\\n  -d 'grant_type=client_credentials' \\\n  -d 'client_id=YOUR_CLIENT_ID' \\\n  -d 'client_secret=YOUR_CLIENT_SECRET' \\\n  https://api.signal-ai.com/auth/token\n```\n\nThis will return the following JSON response:\n\n```json\n{\n    \"access_token\": \"eyJhbGciOi…\",\n    \"expires_in\": 86400,\n    …\n}\n```\n\nYou must send the `access_token` from this response in the Authorization header when making requests to other API endpoints:\n\n```bash\ncurl -H \"Authorization: Bearer eyJhbGciOi…\" \\\n  https://api.signal-ai.com/…\n```\n\nAccess tokens will expire 24 hours from the time they were issued."
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.signal-ai.com/auth/token
  name: OAuth2
  source: openapi/signal-ai-openapi-original.json
scope_count: 6
scope_names:
- affinity
- default
- events
- metrics
- risk-events
- search
scopes:
- description: Access to concept affinity endpoints
  flows:
  - clientCredentials
  scope: affinity
- description: Access to discovery endpoints
  flows:
  - clientCredentials
  scope: default
- description: Access to events endpoint
  flows:
  - clientCredentials
  scope: events
- description: Access to content metrics endpoint
  flows:
  - clientCredentials
  scope: metrics
- description: Access to risk events
  flows:
  - clientCredentials
  scope: risk-events
- description: Access to content search endpoint
  flows:
  - clientCredentials
  scope: search
slug: signal-ai-scopes
source_filename: signal-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/signal-ai-openapi-original.json\nschemes:\n- name: OAuth2\n  source: openapi/signal-ai-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.signal-ai.com/auth/token\n  description: |-\n    To obtain the Bearer Token using the Client ID / Secret pair provided to you:\n\n    ```bash\n    curl -X POST \\\n      -d 'grant_type=client_credentials' \\\n      -d 'client_id=YOUR_CLIENT_ID' \\\n      -d 'client_secret=YOUR_CLIENT_SECRET' \\\n      https://api.signal-ai.com/auth/token\n    ```\n\n    This will return the following JSON response:\n\n    ```json\n    {\n        \"access_token\": \"eyJhbGciOi…\",\n        \"expires_in\": 86400,\n        …\n    }\n    ```\n\n    You must send the `access_token` from this response in the Authorization header when making requests to other API endpoints:\n\n    ```bash\n    curl -H \"Authorization: Bearer eyJhbGciOi…\" \\\n      https://api.signal-ai.com/…\n\
  \    ```\n\n    Access tokens will expire 24 hours from the time they were issued.\nscopes:\n- scope: affinity\n  description: Access to concept affinity endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/signal-ai-openapi-original.json\n- scope: default\n  description: Access to discovery endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/signal-ai-openapi-original.json\n- scope: events\n  description: Access to events endpoint\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/signal-ai-openapi-original.json\n- scope: metrics\n  description: Access to content metrics endpoint\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/signal-ai-openapi-original.json\n- scope: risk-events\n  description: Access to risk events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/signal-ai-openapi-original.json\n- scope: search\n  description: Access to content search endpoint\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/signal-ai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signal-ai/refs/heads/main/scopes/signal-ai-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Company
- Media Intelligence
- Reputation Management
- Risk Intelligence
- News
- Content Search
- Knowledge Graph
- ESG
- Artificial Intelligence
- Analytics
token_urls:
- https://api.signal-ai.com/auth/token
---
