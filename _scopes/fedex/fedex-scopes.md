---
api_specs:
- filename: fedex-authorization-api-openapi.yml
  format: yaml
  label: FedEx API Authorization
  slug: fedex-api-authorization
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-authorization-api-openapi.yml
- filename: fedex-rate-api-openapi.yml
  format: yaml
  label: FedEx Rates and Transit Times API
  slug: fedex-rates-and-transit-times-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-rate-api-openapi.yml
- filename: fedex-ship-api-openapi.yml
  format: yaml
  label: FedEx Ship API
  slug: fedex-ship-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-ship-api-openapi.yml
- filename: fedex-pickup-api-openapi.yml
  format: yaml
  label: FedEx Pickup Request API
  slug: fedex-pickup-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-pickup-api-openapi.yml
- filename: fedex-track-api-openapi.yml
  format: yaml
  label: FedEx Basic Integrated Visibility
  slug: fedex-basic-integrated-visibility
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-track-api-openapi.yml
- filename: fedex-regulatory-api-openapi.yml
  format: yaml
  label: FedEx Regulatory API
  slug: fedex-regulatory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-regulatory-api-openapi.yml
- filename: fedex-address-api-openapi.yml
  format: yaml
  label: FedEx Address API
  slug: fedex-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-address-api-openapi.yml
- filename: fedex-availability-api-openapi.yml
  format: yaml
  label: FedEx Availability API
  slug: fedex-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-availability-api-openapi.yml
- filename: fedex-commodity-api-openapi.yml
  format: yaml
  label: FedEx Commodity API
  slug: fedex-commodity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-commodity-api-openapi.yml
- filename: fedex-country-api-openapi.yml
  format: yaml
  label: FedEx Country API
  slug: fedex-country-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-country-api-openapi.yml
- filename: fedex-documents-api-openapi.yml
  format: yaml
  label: FedEx Documents API
  slug: fedex-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-documents-api-openapi.yml
- filename: fedex-dutytax-api-openapi.yml
  format: yaml
  label: FedEx Dutytax API
  slug: fedex-dutytax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-dutytax-api-openapi.yml
- filename: fedex-globaltrade-api-openapi.yml
  format: yaml
  label: FedEx Globaltrade API
  slug: fedex-globaltrade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-globaltrade-api-openapi.yml
- filename: fedex-irc-api-openapi.yml
  format: yaml
  label: FedEx Irc API
  slug: fedex-irc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-irc-api-openapi.yml
- filename: fedex-location-api-openapi.yml
  format: yaml
  label: FedEx Location API
  slug: fedex-location-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-location-api-openapi.yml
- filename: fedex-webhook-api-openapi.yml
  format: yaml
  label: FedEx Webhook API
  slug: fedex-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fedex/openapi/fedex-webhook-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Fedex Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'FedEx uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://apis.fedex.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FedEx
provider_slug: fedex
schemes:
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-account-number-subscription-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-address-validation-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-close-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-consolidation-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-dutiestaxes-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-global-trade-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-harmonized-code-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-locations-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-ltl-freight-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-open-ship-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-pickup-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-postal-code-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-rate-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-registration-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-regulatory-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-service-availability-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-ship-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-track-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-tracking-number-subscription-api-openapi.yml
- description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization header the fragments declare as a required header parameter.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.fedex.com/oauth/token
  name: oauth2
  source: openapi/fedex-upload-documents-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: fedex-scopes
source_filename: fedex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: none\nsource: openapi/fedex-account-number-subscription-api-openapi.yml, openapi/fedex-address-validation-api-openapi.yml,\n  openapi/fedex-close-api-openapi.yml, openapi/fedex-consolidation-api-openapi.yml, openapi/fedex-dutiestaxes-api-openapi.yml,\n  openapi/fedex-global-trade-api-openapi.yml, openapi/fedex-harmonized-code-api-openapi.yml,\n  openapi/fedex-locations-api-openapi.yml, openapi/fedex-ltl-freight-api-openapi.yml, openapi/fedex-open-ship-api-openapi.yml,\n  openapi/fedex-pickup-api-openapi.yml, openapi/fedex-postal-code-api-openapi.yml, openapi/fedex-rate-api-openapi.yml,\n  openapi/fedex-registration-api-openapi.yml, openapi/fedex-regulatory-api-openapi.yml, openapi/fedex-service-availability-api-openapi.yml,\n  openapi/fedex-ship-api-openapi.yml, openapi/fedex-track-api-openapi.yml, openapi/fedex-tracking-number-subscription-api-openapi.yml,\n  openapi/fedex-upload-documents-api-openapi.yml\nschemes:\n- name: oauth2\n  source:\
  \ openapi/fedex-account-number-subscription-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-address-validation-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments\
  \ declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-close-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-consolidation-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in\
  \ the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-dutiestaxes-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-global-trade-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal).\
  \ Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-harmonized-code-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-locations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key\
  \ issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-ltl-freight-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-open-ship-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials\
  \ | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-pickup-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-postal-code-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n\
  \    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-rate-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-registration-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization\
  \ endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-regulatory-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-service-availability-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description:\
  \ Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-ship-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-track-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n\
  \  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-tracking-number-subscription-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\n- name: oauth2\n  source: openapi/fedex-upload-documents-api-openapi.yml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://apis.fedex.com/oauth/token\n  description: Bearer token from the FedEx API Authorization endpoint (POST /oauth/token, grant_type\n    client_credentials | csp_credentials | client_pc_credentials; API Key + Secret Key issued\n    per project in the Developer Portal). Tokens are valid for one hour. Passed in the authorization\n    header the fragments declare as a required header parameter.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/fedex/scopes/fedex-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Address Validation
- Freight
- Logistics
- Pickup
- Ratings
- Shipping
- Tracking
- Webhook
- Fortune 100
token_bound: false
token_urls:
- https://apis.fedex.com/oauth/token
---
