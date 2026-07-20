---
api_specs:
- filename: hugging-face-transformers-openapi.json
  format: json
  label: Hugging Face Hub API
  slug: hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hugging-face-transformers/refs/heads/main/openapi/hugging-face-transformers-openapi.json
authorization_urls:
- https://huggingface.co/oauth/authorize
description: ''
docs: https://huggingface.co/docs/hub/oauth
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Hugging Face Transformers Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hugging Face Transformers publishes 15 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hugging Face Transformers API on a user''s behalf.


  Tokens are issued from https://huggingface.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hugging Face Transformers
provider_slug: hugging-face-transformers
schemes:
- flows:
  - authorizationUrl: https://huggingface.co/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://huggingface.co/oauth/token
  - deviceAuthorizationUrl: https://huggingface.co/oauth/device
    flow: deviceCode
    tokenUrl: https://huggingface.co/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  issuer: https://huggingface.co
  name: OAuth2 / OIDC
  source: https://huggingface.co/.well-known/openid-configuration
scope_count: 15
scope_names:
- openid
- profile
- email
- read-billing
- read-repos
- gated-repos
- contribute-repos
- write-repos
- manage-repos
- read-collections
- write-collections
- inference-api
- jobs
- webhooks
- write-discussions
scopes:
- description: Get the ID token in addition to the access token.
  flows: []
  scope: openid
- description: Get the user's profile information (username, avatar, etc.).
  flows: []
  scope: profile
- description: Get the user's email address.
  flows: []
  scope: email
- description: Know whether the user has a payment method set up.
  flows: []
  scope: read-billing
- description: Get read access to the user's personal repos.
  flows: []
  scope: read-repos
- description: Get read access to the content of public gated repos the user has been granted access to. Does not grant access to private repos.
  flows: []
  scope: gated-repos
- description: Create repositories and access those created by this app; cannot access other repositories unless additional permissions are granted.
  flows: []
  scope: contribute-repos
- description: Get write/read access to the user's personal repos.
  flows: []
  scope: write-repos
- description: Full access to the user's personal repos, including repo creation and deletion.
  flows: []
  scope: manage-repos
- description: Get read access to the user's personal collections.
  flows: []
  scope: read-collections
- description: Write/read access to the user's personal collections, including creation and deletion.
  flows: []
  scope: write-collections
- description: Access Inference Providers and make inference requests on behalf of the user.
  flows: []
  scope: inference-api
- description: Run jobs.
  flows: []
  scope: jobs
- description: Manage webhooks.
  flows: []
  scope: webhooks
- description: Open discussions and Pull Requests on behalf of the user and interact with discussions (reactions, comments, closing, etc.).
  flows: []
  scope: write-discussions
slug: hugging-face-transformers-scopes
source_filename: hugging-face-transformers-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/hugging-face-transformers-openapi.json\ndocs: https://huggingface.co/docs/hub/oauth\nnotes: >-\n  The Hub OpenAPI declares only http bearer (User Access Token) auth, but\n  Hugging Face runs a full OAuth 2.0 / OIDC authorization server (Sign in with\n  Hugging Face) whose scopes are documented at the docs URL above and whose\n  discovery metadata is at /.well-known/openid-configuration. PKCE (S256) is\n  supported; public apps may omit a client secret. Enterprise plans add\n  RFC 8693 token exchange for keyless per-member token issuance.\nschemes:\n  - name: OAuth2 / OIDC\n    source: https://huggingface.co/.well-known/openid-configuration\n    issuer: https://huggingface.co\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://huggingface.co/oauth/authorize\n        tokenUrl: https://huggingface.co/oauth/token\n        pkce: S256\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://huggingface.co/oauth/device\n\
  \        tokenUrl: https://huggingface.co/oauth/token\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\nscopes:\n  - scope: openid\n    description: Get the ID token in addition to the access token.\n  - scope: profile\n    description: Get the user's profile information (username, avatar, etc.).\n  - scope: email\n    description: Get the user's email address.\n  - scope: read-billing\n    description: Know whether the user has a payment method set up.\n  - scope: read-repos\n    description: Get read access to the user's personal repos.\n  - scope: gated-repos\n    description: >-\n      Get read access to the content of public gated repos the user has been\n      granted access to. Does not grant access to private repos.\n  - scope: contribute-repos\n    description: >-\n      Create repositories and access those created by this app; cannot access\n    \
  \  other repositories unless additional permissions are granted.\n  - scope: write-repos\n    description: Get write/read access to the user's personal repos.\n  - scope: manage-repos\n    description: >-\n      Full access to the user's personal repos, including repo creation and\n      deletion.\n  - scope: read-collections\n    description: Get read access to the user's personal collections.\n  - scope: write-collections\n    description: >-\n      Write/read access to the user's personal collections, including creation\n      and deletion.\n  - scope: inference-api\n    description: >-\n      Access Inference Providers and make inference requests on behalf of the\n      user.\n  - scope: jobs\n    description: Run jobs.\n  - scope: webhooks\n    description: Manage webhooks.\n  - scope: write-discussions\n    description: >-\n      Open discussions and Pull Requests on behalf of the user and interact\n      with discussions (reactions, comments, closing, etc.).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hugging-face-transformers/refs/heads/main/scopes/hugging-face-transformers-scopes.yml
summary_line: 15 scopes · authorizationCode/deviceCode
tags:
- Artificial Intelligence
- Computer Vision
- Deep Learning
- Machine Learning
- Natural Language Processing
- Open Source
- Transformers
token_urls:
- https://huggingface.co/oauth/token
---
