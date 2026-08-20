---
api_specs:
- filename: sadq-holding-limited-archiving-delegations-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Archiving & Delegations API
  slug: sadq-holding-limited-archiving-delegations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-archiving-delegations-api-openapi.yml
- filename: sadq-holding-limited-authentication-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Authentication API
  slug: sadq-holding-limited-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-authentication-api-openapi.yml
- filename: sadq-holding-limited-configuration-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Configuration API
  slug: sadq-holding-limited-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-configuration-api-openapi.yml
- filename: sadq-holding-limited-documents-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Documents API
  slug: sadq-holding-limited-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-documents-api-openapi.yml
- filename: sadq-holding-limited-envelopes-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Envelopes API
  slug: sadq-holding-limited-envelopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-envelopes-api-openapi.yml
- filename: sadq-holding-limited-esign-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited eSign API
  slug: sadq-holding-limited-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-esign-api-openapi.yml
- filename: sadq-holding-limited-invitations-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Invitations API
  slug: sadq-holding-limited-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-invitations-api-openapi.yml
- filename: sadq-holding-limited-kyb-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited KYB API
  slug: sadq-holding-limited-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-kyb-api-openapi.yml
- filename: sadq-holding-limited-reports-requests-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Reports & Requests API
  slug: sadq-holding-limited-reports-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-reports-requests-api-openapi.yml
- filename: sadq-holding-limited-sign-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Sign API
  slug: sadq-holding-limited-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-sign-api-openapi.yml
- filename: sadq-holding-limited-templates-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Templates API
  slug: sadq-holding-limited-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-templates-api-openapi.yml
- filename: sadq-holding-limited-users-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Users API
  slug: sadq-holding-limited-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-users-api-openapi.yml
- filename: sadq-holding-limited-webhooks-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Webhooks API
  slug: sadq-holding-limited-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-webhooks-api-openapi.yml
- filename: sadq-holding-limited-workflows-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Workflows API
  slug: sadq-holding-limited-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-workflows-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.sadq.sa/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Sadq Holding Limited Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares only BearerAuth (JWT), but the docs host publishes full OAuth 2.0 authorization-server metadata (RFC 8414), OIDC discovery, and an auth.md. Scopes are captured from those searched discovery documents.
overview: 'Sadq Holding Limited publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sadq Holding Limited API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sadq Holding Limited
provider_slug: sadq-holding-limited
schemes:
- authorizationServer: https://identity.sadq.sa
  flow: clientCredentials
  name: OAuth2ClientCredentials
  tokenUrl: https://identity.sadq.sa/connect/token
scope_count: 4
scope_names:
- Integrationscope
- openid
- profile
- email
scopes:
- description: Full access to the Sadq Integration API (the scope agents/services request).
  flows:
  - clientCredentials
  scope: Integrationscope
- description: OIDC — issue an ID token / subject identifier.
  flows:
  - authorizationCode
  scope: openid
- description: OIDC — access to profile claims (name, given_name, family_name).
  flows:
  - authorizationCode
  scope: profile
- description: OIDC — access to the email claim.
  flows:
  - authorizationCode
  scope: email
slug: sadq-holding-limited-scopes
source_filename: sadq-holding-limited-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sadq.sa/.well-known/oauth-authorization-server\ndocs: https://docs.sadq.sa/auth.md\nnote: >-\n  The OpenAPI declares only BearerAuth (JWT), but the docs host publishes full\n  OAuth 2.0 authorization-server metadata (RFC 8414), OIDC discovery, and an\n  auth.md. Scopes are captured from those searched discovery documents.\nschemes:\n- name: OAuth2ClientCredentials\n  flow: clientCredentials\n  authorizationServer: https://identity.sadq.sa\n  tokenUrl: https://identity.sadq.sa/connect/token\nscopes:\n- scope: Integrationscope\n  description: Full access to the Sadq Integration API (the scope agents/services request).\n  flows: [clientCredentials]\n  sources: [https://docs.sadq.sa/.well-known/oauth-protected-resource]\n- scope: openid\n  description: OIDC — issue an ID token / subject identifier.\n  flows: [authorizationCode]\n  sources: [https://docs.sadq.sa/.well-known/openid-configuration]\n- scope: profile\n\
  \  description: OIDC — access to profile claims (name, given_name, family_name).\n  flows: [authorizationCode]\n  sources: [https://docs.sadq.sa/.well-known/openid-configuration]\n- scope: email\n  description: OIDC — access to the email claim.\n  flows: [authorizationCode]\n  sources: [https://docs.sadq.sa/.well-known/openid-configuration]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/scopes/sadq-holding-limited-scopes.yml
summary_line: 4 scopes
tags:
- Company
- E-Signature
- Digital Signature
- Identity
- KYB
- Document-Management
- Saudi Arabia
- Nafath
- Webhook
- Agent Ready
token_urls: []
---
