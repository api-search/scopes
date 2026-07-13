---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Sendcloud Shipments API v3
  slug: shipments-api-v3
  spec_type: OpenAPI
  url: https://sendcloud.dev/.openapi/v3/shipments/openapi.yaml
- filename: sendcloud-v3-orders-openapi.yml
  format: yaml
  label: Sendcloud Orders API v3
  slug: orders-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-orders-openapi.yml
- filename: sendcloud-v3-ship-an-order-openapi.yml
  format: yaml
  label: Sendcloud Ship an Order API v3
  slug: ship-an-order-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-ship-an-order-openapi.yml
- filename: sendcloud-v3-returns-openapi.yml
  format: yaml
  label: Sendcloud Returns API v3
  slug: returns-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-returns-openapi.yml
- filename: sendcloud-v3-service-points-openapi.yml
  format: yaml
  label: Sendcloud Service Points API v3
  slug: service-points-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-service-points-openapi.yml
- filename: sendcloud-v3-parcel-tracking-openapi.yml
  format: yaml
  label: Sendcloud Parcel Tracking API v3
  slug: parcel-tracking-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-parcel-tracking-openapi.yml
- filename: sendcloud-v3-parcel-documents-openapi.yml
  format: yaml
  label: Sendcloud Parcel Documents API v3
  slug: parcel-documents-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-parcel-documents-openapi.yml
- filename: sendcloud-v3-webhooks-openapi.yml
  format: yaml
  label: Sendcloud Webhooks API v3
  slug: webhooks-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-webhooks-openapi.yml
- filename: sendcloud-v3-event-subscriptions-openapi.yml
  format: yaml
  label: Sendcloud Event Subscriptions API v3
  slug: event-subscriptions-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-event-subscriptions-openapi.yml
- filename: sendcloud-v3-integrations-openapi.yml
  format: yaml
  label: Sendcloud Integrations API v3
  slug: integrations-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-integrations-openapi.yml
- filename: sendcloud-v3-analytics-openapi.yml
  format: yaml
  label: Sendcloud Analytics API v3
  slug: analytics-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-analytics-openapi.yml
- filename: sendcloud-v3-reporting-openapi.yml
  format: yaml
  label: Sendcloud Reporting API v3
  slug: reporting-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v3-reporting-openapi.yml
- filename: sendcloud-v2-parcels-openapi.yml
  format: yaml
  label: Sendcloud Parcels API v2
  slug: parcels-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-parcels-openapi.yml
- filename: sendcloud-v2-labels-openapi.yml
  format: yaml
  label: Sendcloud Labels API v2
  slug: labels-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-labels-openapi.yml
- filename: sendcloud-v2-tracking-openapi.yml
  format: yaml
  label: Sendcloud Tracking API v2
  slug: tracking-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-tracking-openapi.yml
- filename: sendcloud-v2-webhooks-openapi.yml
  format: yaml
  label: Sendcloud Webhooks API v2
  slug: webhooks-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-webhooks-openapi.yml
- filename: sendcloud-v2-integrations-openapi.yml
  format: yaml
  label: Sendcloud Integrations API v2
  slug: integrations-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-integrations-openapi.yml
- filename: sendcloud-v2-analytics-openapi.yml
  format: yaml
  label: Sendcloud Analytics API v2
  slug: analytics-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-analytics-openapi.yml
- filename: sendcloud-v2-reporting-openapi.yml
  format: yaml
  label: Sendcloud Reporting API v2
  slug: reporting-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-reporting-openapi.yml
- filename: sendcloud-v2-parcel-documents-openapi.yml
  format: yaml
  label: Sendcloud Parcel Documents API v2
  slug: parcel-documents-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/openapi/sendcloud-v2-parcel-documents-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sendcloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sendcloud publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sendcloud API on a user''s behalf.


  Tokens are issued from https://account.sendcloud.com/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sendcloud
provider_slug: sendcloud
schemes:
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-shipments-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v2-analytics-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v2-integrations-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v2-labels-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v2-parcel-documents-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v2-parcels-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v2-reporting-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v2-tracking-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-analytics-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-event-subscriptions-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-integrations-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-orders-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-parcel-documents-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-parcel-tracking-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-reporting-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-returns-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-service-points-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-ship-an-order-openapi.yml
- description: OAuth2 is a standardized protocol for authorization that allows users to share their private resources stored on one site with another site without having to provide their credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for server-to-server interactions that require authorization to access specific resources.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.sendcloud.com/oauth2/token/
  name: OAuth2ClientCreds
  source: openapi/sendcloud-v3-webhooks-openapi.yml
scope_count: 1
scope_names:
- api
scopes:
- description: Default OAuth scope required to access Sendcloud API.
  flows:
  - clientCredentials
  scope: api
slug: sendcloud-scopes
source_filename: sendcloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sendcloud-shipments-openapi.yml, openapi/sendcloud-v2-analytics-openapi.yml,\n  openapi/sendcloud-v2-integrations-openapi.yml, openapi/sendcloud-v2-labels-openapi.yml, openapi/sendcloud-v2-parcel-documents-openapi.yml,\n  openapi/sendcloud-v2-parcels-openapi.yml, openapi/sendcloud-v2-reporting-openapi.yml, openapi/sendcloud-v2-tracking-openapi.yml,\n  openapi/sendcloud-v3-analytics-openapi.yml, openapi/sendcloud-v3-event-subscriptions-openapi.yml,\n  openapi/sendcloud-v3-integrations-openapi.yml, openapi/sendcloud-v3-orders-openapi.yml, openapi/sendcloud-v3-parcel-documents-openapi.yml,\n  openapi/sendcloud-v3-parcel-tracking-openapi.yml, openapi/sendcloud-v3-reporting-openapi.yml,\n  openapi/sendcloud-v3-returns-openapi.yml, openapi/sendcloud-v3-service-points-openapi.yml,\n  openapi/sendcloud-v3-ship-an-order-openapi.yml, openapi/sendcloud-v3-webhooks-openapi.yml\nschemes:\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-shipments-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v2-analytics-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization\
  \ to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v2-integrations-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v2-labels-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials\
  \ Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v2-parcel-documents-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v2-parcels-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private\
  \ resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v2-reporting-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v2-tracking-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n\
  \  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-analytics-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-event-subscriptions-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-integrations-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization\
  \ to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-orders-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-parcel-documents-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client\
  \ Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-parcel-tracking-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-reporting-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n\
  \    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-returns-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-service-points-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n\
  \  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-ship-an-order-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\n- name: OAuth2ClientCreds\n  source: openapi/sendcloud-v3-webhooks-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.sendcloud.com/oauth2/token/\n  description: OAuth2 is a standardized protocol for authorization that allows users to share\n    their private resources stored on one site with another site without having to provide their\n    credentials. OAuth2 Client Credentials Grant workflow. This workflow is typically used for\n    server-to-server interactions that require authorization to access specific resources.\nscopes:\n- scope: api\n  description: Default OAuth scope required to access Sendcloud API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sendcloud-shipments-openapi.yml\n  - openapi/sendcloud-v2-analytics-openapi.yml\n  - openapi/sendcloud-v2-integrations-openapi.yml\n  - openapi/sendcloud-v2-labels-openapi.yml\n  - openapi/sendcloud-v2-parcel-documents-openapi.yml\n  - openapi/sendcloud-v2-parcels-openapi.yml\n  - openapi/sendcloud-v2-reporting-openapi.yml\n  - openapi/sendcloud-v2-tracking-openapi.yml\n\
  \  - openapi/sendcloud-v3-analytics-openapi.yml\n  - openapi/sendcloud-v3-event-subscriptions-openapi.yml\n  - openapi/sendcloud-v3-integrations-openapi.yml\n  - openapi/sendcloud-v3-orders-openapi.yml\n  - openapi/sendcloud-v3-parcel-documents-openapi.yml\n  - openapi/sendcloud-v3-parcel-tracking-openapi.yml\n  - openapi/sendcloud-v3-reporting-openapi.yml\n  - openapi/sendcloud-v3-returns-openapi.yml\n  - openapi/sendcloud-v3-service-points-openapi.yml\n  - openapi/sendcloud-v3-ship-an-order-openapi.yml\n  - openapi/sendcloud-v3-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/scopes/sendcloud-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Shipping
- Logistics
- Ecommerce
- Carriers
- Labels
- Returns
- Tracking
- Europe
token_urls:
- https://account.sendcloud.com/oauth2/token/
---
