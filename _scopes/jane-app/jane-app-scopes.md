---
authorization_urls:
- https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/auth?response_type=code&resource=https://jdpdocsdemo.jane.qa&prompt=consent
description: ''
docs: https://developers.jane.app/docs/getting-started
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Jane App Scopes
name_suffix: OAuth Scopes
note: Scopes are resource:action OAuth2 scopes gated by user consent at authorization. This is standard OAuth2/OIDC, not SMART-on-FHIR scope grammar.
overview: 'Jane publishes 30 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jane API on a user''s behalf.


  Tokens are issued from https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jane
provider_slug: jane-app
schemes:
- description: 'OAuth2 authorization code flow with PKCE (Proof Key for Code Exchange) support.


    **PKCE Flow Required**: All integrations must use PKCE flow for authentication.


    **PKCE Benefits:**

    - Enhanced security against authorization code interception attacks

    - S256 code challenge method supported

    - Industry best practice for OAuth2 implementations


    **Implementation**: Use the authorization code flow with PKCE extension as defined in RFC 7636.'
  flows:
  - authorizationUrl: https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/auth?response_type=code&resource=https://jdpdocsdemo.jane.qa&prompt=consent
    flow: authorizationCode
    tokenUrl: https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/token
  name: OAuth2
  source: openapi/jane-app-jdp-openapi.yml
scope_count: 30
scope_names:
- appointments:read
- care_plans:create
- care_plans:read
- care_plans:update
- companies:read
- conversations:read
- conversations:write
- disciplines:read
- document_uploads:create
- document_uploads:read
- extensions:install
- extensions:uninstall
- locations:read
- medications:create
- medications:read
- medications:update
- messages:read
- messages:write
- observations:create
- observations:read
- observations:update
- partner_extensions:create
- partner_extensions:delete
- patients:read
- staff_members:read
- treatments:read
- webhooks:create
- webhooks:delete
- webhooks:read
- webhooks:update
scopes:
- description: Read appointment information
  flows:
  - authorizationCode
  scope: appointments:read
- description: Create care plans
  flows:
  - authorizationCode
  scope: care_plans:create
- description: Read care plans
  flows:
  - authorizationCode
  scope: care_plans:read
- description: Update care plans
  flows:
  - authorizationCode
  scope: care_plans:update
- description: Read company information
  flows:
  - authorizationCode
  scope: companies:read
- description: Read conversation information
  flows:
  - authorizationCode
  scope: conversations:read
- description: Create and update conversations
  flows:
  - authorizationCode
  scope: conversations:write
- description: Read discipline information
  flows:
  - authorizationCode
  scope: disciplines:read
- description: Create document uploads
  flows:
  - authorizationCode
  scope: document_uploads:create
- description: Read document uploads
  flows:
  - authorizationCode
  scope: document_uploads:read
- description: Install extensions
  flows:
  - authorizationCode
  scope: extensions:install
- description: Uninstall extensions
  flows:
  - authorizationCode
  scope: extensions:uninstall
- description: Read location information
  flows:
  - authorizationCode
  scope: locations:read
- description: Create medication records
  flows:
  - authorizationCode
  scope: medications:create
- description: Read medication information
  flows:
  - authorizationCode
  scope: medications:read
- description: Update medication records
  flows:
  - authorizationCode
  scope: medications:update
- description: Read message information
  flows:
  - authorizationCode
  scope: messages:read
- description: Create and update messages
  flows:
  - authorizationCode
  scope: messages:write
- description: Create observations
  flows:
  - authorizationCode
  scope: observations:create
- description: Read observations
  flows:
  - authorizationCode
  scope: observations:read
- description: Update observations
  flows:
  - authorizationCode
  scope: observations:update
- description: Create partner extensions
  flows:
  - authorizationCode
  scope: partner_extensions:create
- description: Delete partner extensions
  flows:
  - authorizationCode
  scope: partner_extensions:delete
- description: Read patient information
  flows:
  - authorizationCode
  scope: patients:read
- description: Read staff member information
  flows:
  - authorizationCode
  scope: staff_members:read
- description: Read treatment information
  flows:
  - authorizationCode
  scope: treatments:read
- description: Register a webhook subscription
  flows:
  - authorizationCode
  scope: webhooks:create
- description: Deregister a webhook subscription
  flows:
  - authorizationCode
  scope: webhooks:delete
- description: List webhook subscriptions
  flows:
  - authorizationCode
  scope: webhooks:read
- description: Update a webhook subscription
  flows:
  - authorizationCode
  scope: webhooks:update
slug: jane-app-scopes
source_filename: jane-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/jane-app-jdp-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/jane-app-jdp-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/auth?response_type=code&resource=https://jdpdocsdemo.jane.qa&prompt=consent\n    tokenUrl: https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/token\n  description: 'OAuth2 authorization code flow with PKCE (Proof Key for Code Exchange) support.\n\n\n    **PKCE Flow Required**: All integrations must use PKCE flow for authentication.\n\n\n    **PKCE Benefits:**\n\n    - Enhanced security against authorization code interception attacks\n\n    - S256 code challenge method supported\n\n    - Industry best practice for OAuth2 implementations\n\n\n    **Implementation**: Use the authorization code flow with PKCE extension as defined in RFC 7636.'\nscopes:\n- scope:\
  \ appointments:read\n  description: Read appointment information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: care_plans:create\n  description: Create care plans\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: care_plans:read\n  description: Read care plans\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: care_plans:update\n  description: Update care plans\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: companies:read\n  description: Read company information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: conversations:read\n  description: Read conversation information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: conversations:write\n  description: Create and update conversations\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: disciplines:read\n  description: Read discipline information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: document_uploads:create\n  description: Create document uploads\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: document_uploads:read\n  description: Read document uploads\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: extensions:install\n  description: Install extensions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: extensions:uninstall\n  description: Uninstall extensions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: locations:read\n  description: Read location information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: medications:create\n  sources:\n\
  \  - openapi/jane-app-jdp-openapi.yml\n  description: Create medication records\n  flows:\n  - authorizationCode\n- scope: medications:read\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n  description: Read medication information\n  flows:\n  - authorizationCode\n- scope: medications:update\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n  description: Update medication records\n  flows:\n  - authorizationCode\n- scope: messages:read\n  description: Read message information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: messages:write\n  description: Create and update messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: observations:create\n  description: Create observations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: observations:read\n  description: Read observations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n\
  - scope: observations:update\n  description: Update observations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: partner_extensions:create\n  description: Create partner extensions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: partner_extensions:delete\n  description: Delete partner extensions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: patients:read\n  description: Read patient information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: staff_members:read\n  description: Read staff member information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: treatments:read\n  description: Read treatment information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: webhooks:create\n  description: Register a webhook subscription\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: webhooks:delete\n  description: Deregister a webhook subscription\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: webhooks:read\n  description: List webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\n- scope: webhooks:update\n  description: Update a webhook subscription\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jane-app-jdp-openapi.yml\ndocs: https://developers.jane.app/docs/getting-started\nproduction_realm:\n  authorizationUrl: https://login.id.janeapp.com/realms/jane/protocol/openid-connect/auth\n  tokenUrl: https://login.id.janeapp.com/realms/jane/protocol/openid-connect/token\n  note: Documented URLs in the OpenAPI use the jane_partner_sandbox realm; swap realm to `jane` for production.\nnote: Scopes are resource:action OAuth2 scopes gated by user consent at authorization. This\
  \ is standard\n  OAuth2/OIDC, not SMART-on-FHIR scope grammar.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/scopes/jane-app-scopes.yml
summary_line: 30 scopes · authorizationCode
tags:
- Healthcare
- Canada
- Practice Management
- EHR
- EMR
- Scheduling
- Clinical Documentation
- Telehealth
- Health and Wellness
- REST API
- OAuth2
- Webhooks
token_urls:
- https://login.id.janeapp.com/realms/jane_partner_sandbox/protocol/openid-connect/token
---
