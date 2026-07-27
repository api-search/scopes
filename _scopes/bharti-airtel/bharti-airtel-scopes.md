---
api_specs:
- filename: bharti-airtel-iq-sms-openapi.yml
  format: yaml
  label: Airtel IQ SMS API
  slug: airtel-iq-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-iq-sms-openapi.yml
- filename: bharti-airtel-iq-reporting-openapi.yml
  format: yaml
  label: Airtel IQ Reporting API
  slug: airtel-iq-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-iq-reporting-openapi.yml
- filename: bharti-airtel-iot-openapi.yml
  format: yaml
  label: Airtel IoT API
  slug: airtel-iot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-iot-openapi.yml
- filename: bharti-airtel-locate-openapi.yml
  format: yaml
  label: Airtel Locate API
  slug: airtel-locate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-locate-openapi.yml
authorization_urls: []
description: ''
docs: https://www.airtel.in/m2m/business/b2b/locate-solution/documentation/locate-solution/
flows:
- clientCredentials
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Bharti Airtel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bharti Airtel publishes 4 OAuth 2.0 scopes via the clientCredentials, authorizationCode, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bharti Airtel API on a user''s behalf.


  Tokens are issued from https://openapi.airtel.in/locate/apis/customers/{customerBaId}/oauth2_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bharti Airtel
provider_slug: bharti-airtel
schemes:
- flows:
  - flow: clientCredentials
    scope_parameter: request body field `scope` on AccessTokenRequest (required)
    tokenUrl: https://openapi.airtel.in/locate/apis/customers/{customerBaId}/oauth2_token
  name: Airtel Locate OAuth 2.0
  source: openapi/bharti-airtel-locate-openapi.yml
- flows:
  - flow: authorizationCode
    scope_parameter: ?scope={scope} on the authorization request
  - flow: implicit
    scope_parameter: ?scope={scope} on the authorization request
  name: Airtel Smart API OAuth 2.0 (legacy)
  source: https://openapi.airtel.in/smartapi/#/docs/developerAuth
  status: legacy
scope_count: 4
scope_names:
- location
- resource
- ChargeAmount
- subscription
scopes:
- description: 'Required to call the Airtel Locate Location API. Per the specification: "The access token must be generated with ''location'' scope for using this API."'
  flows:
  - clientCredentials
  scope: location
- description: The second value of the AccessTokenRequest.scope enum, covering the Resource Consent and resource-management surface (register, search, modify, delete MSISDNs and their consent).
  flows:
  - clientCredentials
  scope: resource
- description: Legacy Smart API carrier-billing scope required for the charge-amount operation. Published verbatim in the 2017 partner documentation's worked authorization example.
  flows:
  - authorizationCode
  - implicit
  scope: ChargeAmount
- description: Legacy Smart API subscription scope used for subscription activation and deactivation.
  flows:
  - authorizationCode
  - implicit
  scope: subscription
slug: bharti-airtel-scopes
source_filename: bharti-airtel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  openapi/bharti-airtel-locate-openapi.yml (AccessTokenRequest.scope enum) and the legacy Smart API\n  partner documentation at https://openapi.airtel.in/smartapi/#/docs/developerAuth\ndocs: https://www.airtel.in/m2m/business/b2b/locate-solution/documentation/locate-solution/\nderive_note: >-\n  0-working/derive-oauth-scopes.py yields nothing for this provider because no harvested\n  specification declares an oauth2 securityScheme. The scopes below are real and published, but\n  they are carried in a request-body enum and in prose documentation rather than in a\n  securityScheme flows map.\nschemes:\n  - name: Airtel Locate OAuth 2.0\n    source: openapi/bharti-airtel-locate-openapi.yml\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://openapi.airtel.in/locate/apis/customers/{customerBaId}/oauth2_token\n        scope_parameter: request body field `scope` on AccessTokenRequest (required)\n  - name:\
  \ Airtel Smart API OAuth 2.0 (legacy)\n    source: https://openapi.airtel.in/smartapi/#/docs/developerAuth\n    status: legacy\n    flows:\n      - flow: authorizationCode\n        scope_parameter: '?scope={scope} on the authorization request'\n      - flow: implicit\n        scope_parameter: '?scope={scope} on the authorization request'\nscopes:\n  - scope: location\n    api: locate\n    description: >-\n      Required to call the Airtel Locate Location API. Per the specification: \"The access token\n      must be generated with 'location' scope for using this API.\"\n    flows:\n      - clientCredentials\n    sources:\n      - openapi/bharti-airtel-locate-openapi.yml\n    grants:\n      - openapi/bharti-airtel-locate-openapi.yml#getLocationUsingGET_3\n      - openapi/bharti-airtel-locate-openapi.yml#getLocationForTenantsUsingGET_1\n  - scope: resource\n    api: locate\n    description: >-\n      The second value of the AccessTokenRequest.scope enum, covering the Resource Consent and\n\
  \      resource-management surface (register, search, modify, delete MSISDNs and their consent).\n    flows:\n      - clientCredentials\n    sources:\n      - openapi/bharti-airtel-locate-openapi.yml\n  - scope: ChargeAmount\n    api: smart-api\n    description: >-\n      Legacy Smart API carrier-billing scope required for the charge-amount operation. Published\n      verbatim in the 2017 partner documentation's worked authorization example.\n    flows:\n      - authorizationCode\n      - implicit\n    status: legacy\n    sources:\n      - https://openapi.airtel.in/smartapi/#/docs/payment\n  - scope: subscription\n    api: smart-api\n    description: >-\n      Legacy Smart API subscription scope used for subscription activation and deactivation.\n    flows:\n      - authorizationCode\n      - implicit\n    status: legacy\n    sources:\n      - https://openapi.airtel.in/smartapi/#/docs/subscriptions\nscope_administration: >-\n  Per the Smart API documentation, \"scopes are configured when\
  \ the service is provisioned by the\n  platform administrator\" — Airtel scopes are provisioned per partner, not self-selected.\ncounts:\n  scopes: 4\n  active: 2\n  legacy: 2\ngaps:\n  - >-\n    Airtel IoT issues client-credentials tokens (POST /auth/v2/generate/authtoken) but publishes no\n    scope vocabulary at all — its 43 operations are all reachable with one undifferentiated token.\n  - >-\n    Airtel IQ (SMS, Voice, CDR) uses HTTP Basic and has no scope surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/scopes/bharti-airtel-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode/implicit
tags:
- Telecommunications
- India
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- CPaaS
- Messaging
- SMS
- RCS
- Voice
- IoT
- M2M
- Device Location
- Broadband
- 5G
- Identity Verification
- Carrier Billing
- Consent Management
token_urls:
- https://openapi.airtel.in/locate/apis/customers/{customerBaId}/oauth2_token
---
