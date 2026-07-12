---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Oracle Retail Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Oracle Retail publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Oracle Retail API on a user''s behalf.


  Tokens are issued from https://identity.oraclecloud.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oracle Retail
provider_slug: oracle-retail
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token
  name: oauth2
  source: openapi/oracle-retail-merchandising-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token
  name: oauth2
  source: openapi/oracle-retail-order-management-openapi.yml
scope_count: 4
scope_names:
- oms.read
- oms.write
- retail.read
- retail.write
scopes:
- description: Read order data
  flows:
  - clientCredentials
  scope: oms.read
- description: Write order data
  flows:
  - clientCredentials
  scope: oms.write
- description: Read retail data
  flows:
  - clientCredentials
  scope: retail.read
- description: Write retail data
  flows:
  - clientCredentials
  scope: retail.write
slug: oracle-retail-scopes
source_filename: oracle-retail-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-retail-merchandising-openapi.yml, openapi/oracle-retail-order-management-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/oracle-retail-merchandising-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token\n- name: oauth2\n  source: openapi/oracle-retail-order-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token\nscopes:\n- scope: oms.read\n  description: Read order data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oracle-retail-order-management-openapi.yml\n- scope: oms.write\n  description: Write order data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oracle-retail-order-management-openapi.yml\n- scope: retail.read\n  description: Read retail data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oracle-retail-merchandising-openapi.yml\n\
  - scope: retail.write\n  description: Write retail data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oracle-retail-merchandising-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-retail/refs/heads/main/scopes/oracle-retail-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Retail
- Merchandising
- Order Management
- Pricing
- Inventory
- Point of Sale
- Omnichannel
- Oracle
token_urls:
- https://identity.oraclecloud.com/oauth2/v1/token
---
