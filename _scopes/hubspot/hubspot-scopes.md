---
authorization_urls:
- https://app.hubspot.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hubspot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HubSpot publishes 16 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HubSpot API on a user''s behalf.


  Tokens are issued from https://api.hubapi.com/oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HubSpot
provider_slug: hubspot
schemes:
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: OAuth2
  source: openapi/hubspot-analytics-events-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: OAuth2
  source: openapi/hubspot-authors-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: OAuth2
  source: openapi/hubspot-blog-posts-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: oauth2Auth
  source: openapi/hubspot-commerce-payments-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: OAuth2
  source: openapi/hubspot-conversations-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: OAuth2
  source: openapi/hubspot-crm-associations-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: oauth2
  source: openapi/hubspot-custom-workflow-actions-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: OAuth2
  source: openapi/hubspot-domains-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: OAuth2
  source: openapi/hubspot-engagement-calls-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: OAuth2
  source: openapi/hubspot-engagement-notes-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: OAuth2
  source: openapi/hubspot-marketing-emal-api-openapi.yml
- flows:
  - authorizationUrl: https://app.hubspot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubapi.com/oauth/v1/token
  name: oauth2
  source: openapi/hubspot-source-code-api-openapi.yml
scope_count: 16
scope_names:
- analytics.read
- automation
- cms.domains.read
- cms.domains.write
- content
- conversations.read
- conversations.write
- crm.objects.commerce_payments.read
- crm.objects.commerce_payments.write
- crm.objects.companies.read
- crm.objects.companies.write
- crm.objects.contacts.read
- crm.objects.contacts.write
- crm.objects.deals.read
- crm.objects.deals.write
- transactional-email
scopes:
- description: Read analytics data
  flows:
  - authorizationCode
  scope: analytics.read
- description: Access to automation API
  flows:
  - authorizationCode
  scope: automation
- description: Read domains
  flows:
  - authorizationCode
  scope: cms.domains.read
- description: Create or update domains
  flows:
  - authorizationCode
  scope: cms.domains.write
- description: Read from and write to content
  flows:
  - authorizationCode
  scope: content
- description: Read access to conversations
  flows:
  - authorizationCode
  scope: conversations.read
- description: Write access to conversations
  flows:
  - authorizationCode
  scope: conversations.write
- description: Read commerce payments
  flows:
  - authorizationCode
  scope: crm.objects.commerce_payments.read
- description: Write commerce payments
  flows:
  - authorizationCode
  scope: crm.objects.commerce_payments.write
- description: Read companies
  flows:
  - authorizationCode
  scope: crm.objects.companies.read
- description: Write companies
  flows:
  - authorizationCode
  scope: crm.objects.companies.write
- description: Read contacts
  flows:
  - authorizationCode
  scope: crm.objects.contacts.read
- description: Write contacts
  flows:
  - authorizationCode
  scope: crm.objects.contacts.write
- description: Read deals
  flows:
  - authorizationCode
  scope: crm.objects.deals.read
- description: Write deals
  flows:
  - authorizationCode
  scope: crm.objects.deals.write
- description: Send transactional emails and manage SMTP tokens
  flows:
  - authorizationCode
  scope: transactional-email
slug: hubspot-scopes
source_filename: hubspot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hubspot-analytics-events-api-openapi.yml, openapi/hubspot-authors-api-openapi.yml,\n  openapi/hubspot-blog-posts-api-openapi.yml, openapi/hubspot-commerce-payments-api-openapi.yml,\n  openapi/hubspot-conversations-api-openapi.yml, openapi/hubspot-crm-associations-api-openapi.yml,\n  openapi/hubspot-custom-workflow-actions-api-openapi.yml, openapi/hubspot-domains-api-openapi.yml,\n  openapi/hubspot-engagement-calls-api-openapi.yml, openapi/hubspot-engagement-notes-openapi.yml,\n  openapi/hubspot-marketing-emal-api-openapi.yml, openapi/hubspot-source-code-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/hubspot-analytics-events-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: OAuth2\n  source: openapi/hubspot-authors-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: OAuth2\n  source: openapi/hubspot-blog-posts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: oauth2Auth\n  source: openapi/hubspot-commerce-payments-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: OAuth2\n  source: openapi/hubspot-conversations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: OAuth2\n  source: openapi/hubspot-crm-associations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n\
  - name: oauth2\n  source: openapi/hubspot-custom-workflow-actions-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: OAuth2\n  source: openapi/hubspot-domains-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: OAuth2\n  source: openapi/hubspot-engagement-calls-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: OAuth2\n  source: openapi/hubspot-engagement-notes-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: OAuth2\n  source: openapi/hubspot-marketing-emal-api-openapi.yml\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\n- name: oauth2\n  source: openapi/hubspot-source-code-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hubspot.com/oauth/authorize\n    tokenUrl: https://api.hubapi.com/oauth/v1/token\nscopes:\n- scope: analytics.read\n  description: Read analytics data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-analytics-events-api-openapi.yml\n- scope: automation\n  description: Access to automation API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-custom-workflow-actions-api-openapi.yml\n- scope: cms.domains.read\n  description: Read domains\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-domains-api-openapi.yml\n- scope: cms.domains.write\n  description: Create or update domains\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-domains-api-openapi.yml\n\
  - scope: content\n  description: Read from and write to content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-authors-api-openapi.yml\n  - openapi/hubspot-blog-posts-api-openapi.yml\n  - openapi/hubspot-source-code-api-openapi.yml\n- scope: conversations.read\n  description: Read access to conversations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-conversations-api-openapi.yml\n- scope: conversations.write\n  description: Write access to conversations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-conversations-api-openapi.yml\n- scope: crm.objects.commerce_payments.read\n  description: Read commerce payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-commerce-payments-api-openapi.yml\n- scope: crm.objects.commerce_payments.write\n  description: Write commerce payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-commerce-payments-api-openapi.yml\n- scope: crm.objects.companies.read\n\
  \  description: Read companies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-crm-associations-api-openapi.yml\n- scope: crm.objects.companies.write\n  description: Write companies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-crm-associations-api-openapi.yml\n- scope: crm.objects.contacts.read\n  description: Read contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-crm-associations-api-openapi.yml\n  - openapi/hubspot-engagement-calls-api-openapi.yml\n  - openapi/hubspot-engagement-notes-openapi.yml\n- scope: crm.objects.contacts.write\n  description: Write contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-crm-associations-api-openapi.yml\n  - openapi/hubspot-engagement-calls-api-openapi.yml\n  - openapi/hubspot-engagement-notes-openapi.yml\n- scope: crm.objects.deals.read\n  description: Read deals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-crm-associations-api-openapi.yml\n\
  - scope: crm.objects.deals.write\n  description: Write deals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-crm-associations-api-openapi.yml\n- scope: transactional-email\n  description: Send transactional emails and manage SMTP tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubspot-marketing-emal-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/scopes/hubspot-scopes.yml
summary_line: 16 scopes · authorizationCode
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
token_urls:
- https://api.hubapi.com/oauth/v1/token
---
