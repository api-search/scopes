---
authorization_urls:
- https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Amerisourcebergen Scopes
name_suffix: OAuth Scopes
note: Probed, not derived from an OpenAPI — Cencora publishes no machine-readable contract. These are the scopes the SAP XSUAA authorization server behind api.cencora.com advertises in its OIDC discovery document. They are the standard OIDC identity scopes plus SAP's roles/user_attributes claims; they are NOT Cencora business scopes. Any API-level scope (order, inventory, returns, DSCSA/EPCIS) would live inside the gated developer portal and requires authenticated introspection to enumerate. No Cencora scope reference page is published anywhere on www.cencora.com.
overview: 'AmerisourceBergen publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AmerisourceBergen API on a user''s behalf.


  Tokens are issued from https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AmerisourceBergen
provider_slug: amerisourcebergen
schemes:
- flows:
  - authorizationUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token
  issuer: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token
  name: SAP XSUAA (Cencora developer portal)
  source: well-known/amerisourcebergen-openid-configuration.json
scope_count: 6
scope_names:
- openid
- profile
- email
- phone
- roles
- user_attributes
scopes:
- description: OIDC — issue an ID token for the authenticated subject.
  flows:
  - authorizationCode
  scope: openid
- description: OIDC — basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: OIDC — email address claim.
  flows:
  - authorizationCode
  scope: email
- description: OIDC — phone number claim.
  flows:
  - authorizationCode
  scope: phone
- description: SAP XSUAA — role collections assigned to the subject in the Cencora BTP subaccount.
  flows:
  - authorizationCode
  scope: roles
- description: SAP XSUAA — tenant-defined user attributes used for instance-based authorization.
  flows:
  - authorizationCode
  scope: user_attributes
slug: amerisourcebergen-scopes
source_filename: amerisourcebergen-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Probed, not derived from an OpenAPI — Cencora publishes no machine-readable contract.\n  These are the scopes the SAP XSUAA authorization server behind api.cencora.com advertises\n  in its OIDC discovery document. They are the standard OIDC identity scopes plus SAP's\n  roles/user_attributes claims; they are NOT Cencora business scopes. Any API-level scope\n  (order, inventory, returns, DSCSA/EPCIS) would live inside the gated developer portal and\n  requires authenticated introspection to enumerate. No Cencora scope reference page is\n  published anywhere on www.cencora.com.\nschemes:\n  - name: SAP XSUAA (Cencora developer portal)\n    source: well-known/amerisourcebergen-openid-configuration.json\n    issuer: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token\n    flows:\n\
  \      - flow: authorizationCode\n        authorizationUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/authorize\n        tokenUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token\nscopes:\n  - scope: openid\n    description: OIDC — issue an ID token for the authenticated subject.\n    flows: [authorizationCode]\n    sources: [well-known/amerisourcebergen-openid-configuration.json]\n  - scope: profile\n    description: OIDC — basic profile claims.\n    flows: [authorizationCode]\n    sources: [well-known/amerisourcebergen-openid-configuration.json]\n  - scope: email\n    description: OIDC — email address claim.\n    flows: [authorizationCode]\n    sources: [well-known/amerisourcebergen-openid-configuration.json]\n  - scope: phone\n    description: OIDC — phone number claim.\n    flows: [authorizationCode]\n    sources: [well-known/amerisourcebergen-openid-configuration.json]\n  - scope: roles\n    description: SAP XSUAA — role\
  \ collections assigned to the subject in the Cencora BTP subaccount.\n    flows: [authorizationCode]\n    sources: [well-known/amerisourcebergen-openid-configuration.json]\n  - scope: user_attributes\n    description: SAP XSUAA — tenant-defined user attributes used for instance-based authorization.\n    flows: [authorizationCode]\n    sources: [well-known/amerisourcebergen-openid-configuration.json]\nscope_count: 6\nbusiness_scopes_published: false\nx-evidence:\n  checked: '2026-09-02'\n  probes:\n    - url: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/.well-known/openid-configuration\n      http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amerisourcebergen/refs/heads/main/scopes/amerisourcebergen-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Pharmaceutical Distribution
- Healthcare
- Drug Distribution
- Manufacturer Solutions
- Provider Solutions
- Animal Health
- Life Sciences
- Fortune 100
token_urls:
- https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token
---
