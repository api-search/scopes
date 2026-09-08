---
api_specs:
- filename: eci-solutions-erp-v2-1-openapi.json
  format: json
  label: ECI Manufacturing ERP API
  slug: eci-solutions-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-erp-v2-1-openapi.json
- filename: eci-solutions-jobboss2-openapi.json
  format: json
  label: JobBOSS² Public API
  slug: eci-solutions-jobboss2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-jobboss2-openapi.json
- filename: eci-solutions-m1-openapi.json
  format: json
  label: M1 Public API
  slug: eci-solutions-m1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-m1-openapi.json
- filename: eci-solutions-management-openapi.json
  format: json
  label: ECI MFG Integration Management API
  slug: eci-solutions-integration-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-management-openapi.json
- filename: eci-solutions-authentication-openapi.json
  format: json
  label: ECI Authentication API
  slug: eci-solutions-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-authentication-openapi.json
- filename: eci-solutions-payment-openapi.json
  format: json
  label: ECI MFG Payment API
  slug: eci-solutions-payment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-payment-openapi.json
- filename: eci-solutions-financial-v2-openapi.json
  format: json
  label: ECI Financial Integration API
  slug: eci-solutions-financial
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-financial-v2-openapi.json
- filename: eci-solutions-ecommerce-openapi.json
  format: json
  label: ECI EvolutionX Ecommerce API
  slug: eci-solutions-ecommerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-ecommerce-openapi.json
- filename: eci-solutions-einvoice-openapi.json
  format: json
  label: ECI Einvoice API
  slug: eci-solutions-einvoice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-einvoice-openapi.json
- filename: eci-solutions-shipping-openapi.json
  format: json
  label: ECI Shipping API
  slug: eci-solutions-shipping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-shipping-openapi.json
- filename: eci-solutions-currency-openapi.json
  format: json
  label: ECI Currency Data API
  slug: eci-solutions-currency
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-currency-openapi.json
- filename: eci-solutions-apar-commerce-openapi.json
  format: json
  label: ECI AP/AR Commerce Automation API
  slug: eci-solutions-apar-commerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-apar-commerce-openapi.json
- filename: eci-solutions-office-openapi.json
  format: json
  label: ECI Office Integration API
  slug: eci-solutions-office
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-office-openapi.json
- filename: eci-solutions-notification-openapi.json
  format: json
  label: ECI Notification API
  slug: eci-solutions-notification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-notification-openapi.json
- filename: eci-solutions-lasso-crm-openapi.yml
  format: yaml
  label: Lasso CRM API
  slug: eci-solutions-lasso-crm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/openapi/eci-solutions-lasso-crm-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Eci Solutions Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ECI Solutions publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ECI Solutions API on a user''s behalf.


  Tokens are issued from https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ECI Solutions
provider_slug: eci-solutions
schemes:
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-apar-commerce-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-currency-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-ecommerce-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-einvoice-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-erp-v1-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-erp-v2-1-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-erp-v2-openapi.json
- description: Use the Authentication API OAuth endpoints
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-financial-v1-openapi.json
- description: Use the Authentication API OAuth endpoints
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-financial-v2-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-jobboss2-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: oauth2
  source: openapi/eci-solutions-m1-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users from Integration Engine
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: ClientToken
  source: openapi/eci-solutions-notification-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-office-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-payment-openapi.json
- description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine Management Console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
  name: Bearer
  source: openapi/eci-solutions-shipping-openapi.json
scope_count: 1
scope_names:
- openid
scopes:
- description: openid
  flows:
  - clientCredentials
  scope: openid
slug: eci-solutions-scopes
source_filename: eci-solutions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/eci-solutions-apar-commerce-openapi.json, openapi/eci-solutions-currency-openapi.json,\n  openapi/eci-solutions-ecommerce-openapi.json, openapi/eci-solutions-einvoice-openapi.json,\n  openapi/eci-solutions-erp-v1-openapi.json, openapi/eci-solutions-erp-v2-1-openapi.json, openapi/eci-solutions-erp-v2-openapi.json,\n  openapi/eci-solutions-financial-v1-openapi.json, openapi/eci-solutions-financial-v2-openapi.json,\n  openapi/eci-solutions-jobboss2-openapi.json, openapi/eci-solutions-m1-openapi.json, openapi/eci-solutions-notification-openapi.json,\n  openapi/eci-solutions-office-openapi.json, openapi/eci-solutions-payment-openapi.json, openapi/eci-solutions-shipping-openapi.json\nschemes:\n- name: Bearer\n  source: openapi/eci-solutions-apar-commerce-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client\
  \ Credentials Flow with API Users issued from Integration Engine\n    Management Console\n- name: Bearer\n  source: openapi/eci-solutions-currency-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine\n    Management Console\n- name: Bearer\n  source: openapi/eci-solutions-ecommerce-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine\n    Management Console\n- name: Bearer\n  source: openapi/eci-solutions-einvoice-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from\
  \ Integration Engine\n    Management Console\n- name: Bearer\n  source: openapi/eci-solutions-erp-v1-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine\n    Management Console\n- name: Bearer\n  source: openapi/eci-solutions-erp-v2-1-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine\n    Management Console\n- name: Bearer\n  source: openapi/eci-solutions-erp-v2-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine\n    Management Console\n- name:\
  \ Bearer\n  source: openapi/eci-solutions-financial-v1-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: Use the Authentication API OAuth endpoints\n- name: Bearer\n  source: openapi/eci-solutions-financial-v2-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: Use the Authentication API OAuth endpoints\n- name: Bearer\n  source: openapi/eci-solutions-jobboss2-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine\n    Management Console\n- name: oauth2\n  source: openapi/eci-solutions-m1-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n\
  \  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine\n    Management Console\n- name: ClientToken\n  source: openapi/eci-solutions-notification-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users from Integration Engine\n- name: Bearer\n  source: openapi/eci-solutions-office-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine\n    Management Console\n- name: Bearer\n  source: openapi/eci-solutions-payment-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued\
  \ from Integration Engine\n    Management Console\n- name: Bearer\n  source: openapi/eci-solutions-shipping-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token\n  description: OAuth 2.0 Client Credentials Flow with API Users issued from Integration Engine\n    Management Console\nscopes:\n- scope: openid\n  description: openid\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/eci-solutions-apar-commerce-openapi.json\n  - openapi/eci-solutions-currency-openapi.json\n  - openapi/eci-solutions-ecommerce-openapi.json\n  - openapi/eci-solutions-einvoice-openapi.json\n  - openapi/eci-solutions-erp-v1-openapi.json\n  - openapi/eci-solutions-erp-v2-1-openapi.json\n  - openapi/eci-solutions-erp-v2-openapi.json\n  - openapi/eci-solutions-financial-v1-openapi.json\n  - openapi/eci-solutions-financial-v2-openapi.json\n  - openapi/eci-solutions-jobboss2-openapi.json\n  - openapi/eci-solutions-m1-openapi.json\n\
  \  - openapi/eci-solutions-notification-openapi.json\n  - openapi/eci-solutions-office-openapi.json\n  - openapi/eci-solutions-payment-openapi.json\n  - openapi/eci-solutions-shipping-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/scopes/eci-solutions-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Accounting
- Building Supply
- Business Management
- CRM
- Construction
- Distribution
- E-Commerce
- ERP
- Field Service
- Inventory
- Manufacturing
- Payments
- Retail
- Shipping
token_urls:
- https://api-user.integrations.ecimanufacturing.com/oauth2/api-user/token
---
