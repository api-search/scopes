---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Brim Billing And Revenue Innovation Management Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAP BRIM (Billing and Revenue Innovation Management) publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP BRIM (Billing and Revenue Innovation Management) API on a user''s behalf.


  Tokens are issued from https://auth.sap.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP BRIM (Billing and Revenue Innovation Management)
provider_slug: sap-brim-billing-and-revenue-innovation-management
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sap.com/oauth/token
  name: OAuth2
  source: openapi/sap-brim-convergent-charging-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sap.com/oauth/token
  name: OAuth2
  source: openapi/sap-brim-subscription-billing-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to charging and rating resources
  flows:
  - clientCredentials
  scope: read
- description: Write access to charging and rating resources
  flows:
  - clientCredentials
  scope: write
slug: sap-brim-billing-and-revenue-innovation-management-scopes
source_filename: sap-brim-billing-and-revenue-innovation-management-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-brim-convergent-charging-openapi.yml, openapi/sap-brim-subscription-billing-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/sap-brim-convergent-charging-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sap.com/oauth/token\n- name: OAuth2\n  source: openapi/sap-brim-subscription-billing-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sap.com/oauth/token\nscopes:\n- scope: read\n  description: Read access to charging and rating resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-brim-convergent-charging-openapi.yml\n  - openapi/sap-brim-subscription-billing-openapi.yml\n- scope: write\n  description: Write access to charging and rating resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-brim-convergent-charging-openapi.yml\n  - openapi/sap-brim-subscription-billing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/scopes/sap-brim-billing-and-revenue-innovation-management-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Billing
- Enterprise
- Order to Cash
- Revenue Management
- SAP
- Subscription Management
- Usage-Based Pricing
token_urls:
- https://auth.sap.com/oauth/token
---
