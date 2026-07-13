---
api_specs:
- filename: sap-sd-sales-order-openapi.yml
  format: yaml
  label: Sales Order API
  slug: sales-order
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-order-openapi.yml
- filename: sap-sd-customer-master-data-openapi.yml
  format: yaml
  label: Customer Master Data API
  slug: customer-master-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-master-data-openapi.yml
- filename: sap-sd-outbound-delivery-openapi.yml
  format: yaml
  label: Outbound Delivery API
  slug: outbound-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-outbound-delivery-openapi.yml
- filename: sap-sd-billing-document-openapi.yml
  format: yaml
  label: Billing Document API
  slug: billing-document
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-billing-document-openapi.yml
- filename: sap-sd-pricing-openapi.yml
  format: yaml
  label: Pricing API
  slug: pricing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-pricing-openapi.yml
- filename: sap-sd-sales-quotation-openapi.yml
  format: yaml
  label: Sales Quotation API
  slug: sales-quotation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-quotation-openapi.yml
- filename: sap-sd-credit-management-openapi.yml
  format: yaml
  label: Credit Management API
  slug: credit-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-credit-management-openapi.yml
- filename: sap-sd-material-master-openapi.yml
  format: yaml
  label: Material Master API
  slug: material-master
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-material-master-openapi.yml
- filename: sap-sd-credit-memo-request-openapi.yml
  format: yaml
  label: Credit Memo Request API
  slug: credit-memo-request
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-credit-memo-request-openapi.yml
- filename: sap-sd-debit-memo-request-openapi.yml
  format: yaml
  label: Debit Memo Request API
  slug: debit-memo-request
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-debit-memo-request-openapi.yml
- filename: sap-sd-sales-contract-openapi.yml
  format: yaml
  label: Sales Contract API
  slug: sales-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-contract-openapi.yml
- filename: sap-sd-sales-inquiry-openapi.yml
  format: yaml
  label: Sales Inquiry API
  slug: sales-inquiry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-inquiry-openapi.yml
- filename: sap-sd-sales-scheduling-agreement-openapi.yml
  format: yaml
  label: Sales Scheduling Agreement API
  slug: sales-scheduling-agreement
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-sales-scheduling-agreement-openapi.yml
- filename: sap-sd-customer-return-openapi.yml
  format: yaml
  label: Customer Return API
  slug: customer-return
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-return-openapi.yml
- filename: sap-sd-customer-returns-delivery-openapi.yml
  format: yaml
  label: Customer Returns Delivery API
  slug: customer-returns-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-returns-delivery-openapi.yml
- filename: sap-sd-customer-material-openapi.yml
  format: yaml
  label: Customer Material API
  slug: customer-material
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-customer-material-openapi.yml
- filename: sap-sd-inbound-delivery-openapi.yml
  format: yaml
  label: Inbound Delivery API
  slug: inbound-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/openapi/sap-sd-inbound-delivery-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Sales And Distribution Sd Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAP Sales and Distribution (SD) publishes 17 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP Sales and Distribution (SD) API on a user''s behalf.


  Tokens are issued from https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-billing-document-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-credit-management-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-credit-memo-request-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-customer-master-data-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-customer-material-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-customer-return-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-customer-returns-delivery-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-debit-memo-request-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-inbound-delivery-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-material-master-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-outbound-delivery-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-pricing-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-sales-contract-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-sales-inquiry-openapi.yml
- description: OAuth 2.0 authentication for SAP S/4HANA Cloud
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-sales-order-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-sales-quotation-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-sd-sales-scheduling-agreement-openapi.yml
scope_count: 17
scope_names:
- API_BILLING_DOCUMENT_SRV
- API_BUSINESS_PARTNER
- API_CREDIT_MANAGEMENT
- API_CREDIT_MEMO_REQUEST_SRV
- API_CUSTOMER_MATERIAL_SRV
- API_CUSTOMER_RETURN_DELIVERY_SRV
- API_CUSTOMER_RETURN_SRV
- API_DEBIT_MEMO_REQUEST_SRV
- API_INBOUND_DELIVERY_SRV
- API_OUTBOUND_DELIVERY_SRV
- API_PRODUCT_SRV
- API_SALES_CONTRACT_SRV
- API_SALES_INQUIRY_SRV
- API_SALES_ORDER_SRV
- API_SALES_QUOTATION_SRV
- API_SALES_SCHEDULING_AGREEMENT
- API_SLSPRCGCONDITIONRECORD_SRV
scopes:
- description: Access to Billing Document API
  flows:
  - clientCredentials
  scope: API_BILLING_DOCUMENT_SRV
- description: Access to Business Partner API
  flows:
  - clientCredentials
  scope: API_BUSINESS_PARTNER
- description: Access to Credit Management API
  flows:
  - clientCredentials
  scope: API_CREDIT_MANAGEMENT
- description: Access to Credit Memo Request API
  flows:
  - clientCredentials
  scope: API_CREDIT_MEMO_REQUEST_SRV
- description: Access to Customer Material API
  flows:
  - clientCredentials
  scope: API_CUSTOMER_MATERIAL_SRV
- description: Access to Returns Delivery API
  flows:
  - clientCredentials
  scope: API_CUSTOMER_RETURN_DELIVERY_SRV
- description: Access to Customer Return API
  flows:
  - clientCredentials
  scope: API_CUSTOMER_RETURN_SRV
- description: Access to Debit Memo Request API
  flows:
  - clientCredentials
  scope: API_DEBIT_MEMO_REQUEST_SRV
- description: Access to Inbound Delivery API
  flows:
  - clientCredentials
  scope: API_INBOUND_DELIVERY_SRV
- description: Access to Outbound Delivery API
  flows:
  - clientCredentials
  scope: API_OUTBOUND_DELIVERY_SRV
- description: Access to Product API
  flows:
  - clientCredentials
  scope: API_PRODUCT_SRV
- description: Access to Sales Contract API
  flows:
  - clientCredentials
  scope: API_SALES_CONTRACT_SRV
- description: Access to Sales Inquiry API
  flows:
  - clientCredentials
  scope: API_SALES_INQUIRY_SRV
- description: Access to Sales Order API
  flows:
  - clientCredentials
  scope: API_SALES_ORDER_SRV
- description: Access to Sales Quotation API
  flows:
  - clientCredentials
  scope: API_SALES_QUOTATION_SRV
- description: Access to Scheduling Agreement API
  flows:
  - clientCredentials
  scope: API_SALES_SCHEDULING_AGREEMENT
- description: Access to Pricing API
  flows:
  - clientCredentials
  scope: API_SLSPRCGCONDITIONRECORD_SRV
slug: sap-sales-and-distribution-sd-scopes
source_filename: sap-sales-and-distribution-sd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-sd-billing-document-openapi.yml, openapi/sap-sd-credit-management-openapi.yml,\n  openapi/sap-sd-credit-memo-request-openapi.yml, openapi/sap-sd-customer-master-data-openapi.yml,\n  openapi/sap-sd-customer-material-openapi.yml, openapi/sap-sd-customer-return-openapi.yml,\n  openapi/sap-sd-customer-returns-delivery-openapi.yml, openapi/sap-sd-debit-memo-request-openapi.yml,\n  openapi/sap-sd-inbound-delivery-openapi.yml, openapi/sap-sd-material-master-openapi.yml, openapi/sap-sd-outbound-delivery-openapi.yml,\n  openapi/sap-sd-pricing-openapi.yml, openapi/sap-sd-sales-contract-openapi.yml, openapi/sap-sd-sales-inquiry-openapi.yml,\n  openapi/sap-sd-sales-order-openapi.yml, openapi/sap-sd-sales-quotation-openapi.yml, openapi/sap-sd-sales-scheduling-agreement-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/sap-sd-billing-document-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n\
  - name: oauth2\n  source: openapi/sap-sd-credit-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-credit-memo-request-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-customer-master-data-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-customer-material-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-customer-return-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n\
  - name: oauth2\n  source: openapi/sap-sd-customer-returns-delivery-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-debit-memo-request-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-inbound-delivery-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-material-master-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-outbound-delivery-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n\
  - name: oauth2\n  source: openapi/sap-sd-pricing-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-sales-contract-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-sales-inquiry-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-sd-sales-order-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n  description: OAuth 2.0 authentication for SAP S/4HANA Cloud\n- name: oauth2\n  source: openapi/sap-sd-sales-quotation-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\n\
  - name: oauth2\n  source: openapi/sap-sd-sales-scheduling-agreement-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token\nscopes:\n- scope: API_BILLING_DOCUMENT_SRV\n  description: Access to Billing Document API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-billing-document-openapi.yml\n- scope: API_BUSINESS_PARTNER\n  description: Access to Business Partner API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-customer-master-data-openapi.yml\n- scope: API_CREDIT_MANAGEMENT\n  description: Access to Credit Management API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-credit-management-openapi.yml\n- scope: API_CREDIT_MEMO_REQUEST_SRV\n  description: Access to Credit Memo Request API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-credit-memo-request-openapi.yml\n- scope: API_CUSTOMER_MATERIAL_SRV\n  description: Access to Customer\
  \ Material API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-customer-material-openapi.yml\n- scope: API_CUSTOMER_RETURN_DELIVERY_SRV\n  description: Access to Returns Delivery API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-customer-returns-delivery-openapi.yml\n- scope: API_CUSTOMER_RETURN_SRV\n  description: Access to Customer Return API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-customer-return-openapi.yml\n- scope: API_DEBIT_MEMO_REQUEST_SRV\n  description: Access to Debit Memo Request API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-debit-memo-request-openapi.yml\n- scope: API_INBOUND_DELIVERY_SRV\n  description: Access to Inbound Delivery API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-inbound-delivery-openapi.yml\n- scope: API_OUTBOUND_DELIVERY_SRV\n  description: Access to Outbound Delivery API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-outbound-delivery-openapi.yml\n\
  - scope: API_PRODUCT_SRV\n  description: Access to Product API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-material-master-openapi.yml\n- scope: API_SALES_CONTRACT_SRV\n  description: Access to Sales Contract API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-sales-contract-openapi.yml\n- scope: API_SALES_INQUIRY_SRV\n  description: Access to Sales Inquiry API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-sales-inquiry-openapi.yml\n- scope: API_SALES_ORDER_SRV\n  description: Access to Sales Order API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-sales-order-openapi.yml\n- scope: API_SALES_QUOTATION_SRV\n  description: Access to Sales Quotation API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-sales-quotation-openapi.yml\n- scope: API_SALES_SCHEDULING_AGREEMENT\n  description: Access to Scheduling Agreement API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-sales-scheduling-agreement-openapi.yml\n\
  - scope: API_SLSPRCGCONDITIONRECORD_SRV\n  description: Access to Pricing API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-sd-pricing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/scopes/sap-sales-and-distribution-sd-scopes.yml
summary_line: 17 scopes · clientCredentials
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
token_urls:
- https://{tenant}.authentication.{landscape}.hana.ondemand.com/oauth/token
---
