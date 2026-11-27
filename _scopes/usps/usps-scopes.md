---
api_specs:
- filename: usps-addresses-api-openapi.yml
  format: yaml
  label: United States Postal Service Addresses API
  slug: usps-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-addresses-api-openapi.yml
- filename: usps-carrier-pickup-api-openapi.yml
  format: yaml
  label: United States Postal Service Carrier Pickup API
  slug: usps-carrier-pickup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-carrier-pickup-api-openapi.yml
- filename: usps-domestic-prices-api-openapi.yml
  format: yaml
  label: United States Postal Service Domestic Prices API
  slug: usps-domestic-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-domestic-prices-api-openapi.yml
- filename: usps-files-api-openapi.yml
  format: yaml
  label: United States Postal Service Files API
  slug: usps-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-files-api-openapi.yml
- filename: usps-listener-url-specification-api-openapi.yml
  format: yaml
  label: United States Postal Service Listener URL Specification API
  slug: usps-listener-url-specification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-listener-url-specification-api-openapi.yml
- filename: usps-resources-api-openapi.yml
  format: yaml
  label: United States Postal Service Resources API
  slug: usps-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-resources-api-openapi.yml
- filename: usps-tracking-api-openapi.yml
  format: yaml
  label: United States Postal Service Tracking API
  slug: usps-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usps/openapi/usps-tracking-api-openapi.yml
authorization_urls:
- /oauth2/v3/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: United States Postal Service Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'United States Postal Service publishes 44 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the United States Postal Service API on a user''s behalf.


  Tokens are issued from /oauth2/v3/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: United States Postal Service
provider_slug: usps
schemes:
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-addresses-openapi.yml
- description: The specificed APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-adjustments-openapi.yml
- description: 'The specificed APIs accept an access token formatted as a JSON Web

    Token. The relative path to the OAuth2 version 3 API which supplies this

    access token is provided below for reference.'
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-appointments-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-carrier-pickup-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-containers-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-domestic-labels-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-domestic-prices-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: OAuth
  source: openapi/usps-informed-delivery-mail-campaigns-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: OAuth
  source: openapi/usps-informed-delivery-package-campaigns-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-international-labels-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-international-prices-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-international-service-standards-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-locations-openapi.yml
- description: OAuth2 security scheme for shipment tracking.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-logistics-shipments-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-ncoa-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: OAuth
  source: openapi/usps-payments-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-pmod-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-qr-codes-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-reconciliation-adjustments-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-scan-forms-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-service-standards-directory-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-service-standards-files-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-service-standards-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-ship-enrollment-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-shipping-options-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-subscriptions-addresses-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-subscriptions-adjustments-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-subscriptions-disputes-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-subscriptions-ncoa-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-subscriptions-package-transaction-details-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-subscriptions-tracking-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-subscriptions-tracking-v3r2-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-subscriptions-unpaid-packages-openapi.yml
- description: The specified APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-tracking-openapi.yml
- description: The specificed APIs accept an access token formatted as a JSON Web Token. The relative path to the OAuth2 version 3 API which supplies this access token is provided below for reference.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-tracking-v3r2-openapi.yml
- description: 'The specified APIs accept an access token placed in the Authorization header using the Bearer Authentication security scheme. The relative path to the OAuth2 API which supply this access token is provided here for reference.

    Access tokens issued by either the OAuth __Client Credentials__ or __Authorization Code__ flows are supported.

    The ''openid'' scope is required either as an input or assigned to the client applicatiion upoon registration.'
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/v3/token
  - authorizationUrl: /oauth2/v3/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v3/token
  name: OAuth
  source: openapi/usps-userinfo-openapi.yml
scope_count: 44
scope_names:
- address
- addresses
- adjustments
- campaigns
- carrier-pickup
- containers
- email
- fast-appointments
- international-labels
- international-prices
- international-service-standard
- labels
- locations
- locations-files
- logistics
- ncoa-data-services
- oauth2-oidc
- openid
- parcel-locker
- payments
- pickup
- pmod
- prices
- profile
- qr-code
- reconciliation-adjustments
- scan-forms
- service-standards
- service-standards-directory
- service-standards-files
- ship-enrollment
- shipments
- subscriptions-address
- subscriptions-addresses
- subscriptions-adjustments
- subscriptions-disputes
- subscriptions-ncoa
- subscriptions-package-transaction-details
- subscriptions-tracking
- subscriptions-unpaid-packages
- tracking
- usps:MIDs
- usps:contract_rates
- usps:payment_methods
scopes:
- description: The OpenID Connect industry standard, United States Postal Service authorized access the user's address.
  flows:
  - authorizationCode
  - clientCredentials
  scope: address
- description: read-only access to all addresses endpoints
  flows:
  - authorizationCode
  - clientCredentials
  scope: addresses
- description: Get adjustments for a tracking number.
  flows:
  - authorizationCode
  - clientCredentials
  scope: adjustments
- description: read/write access to all campaigns endpoints
  flows:
  - clientCredentials
  scope: campaigns
- description: ''
  flows: []
  scope: carrier-pickup
- description: Both read and create access to containers API.
  flows:
  - clientCredentials
  scope: containers
- description: The OpenID Connect industry standard, United States Postal Service authorized access the user's email address.
  flows:
  - authorizationCode
  - clientCredentials
  scope: email
- description: check for available slots and create appointments
  flows:
  - authorizationCode
  - clientCredentials
  scope: fast-appointments
- description: Read, create, and cancel access to Labels.
  flows:
  - authorizationCode
  - clientCredentials
  scope: international-labels
- description: get prices based on ingredients
  flows:
  - authorizationCode
  - clientCredentials
  scope: international-prices
- description: Read access to Service Standard.
  flows:
  - clientCredentials
  scope: international-service-standard
- description: Read, create, and cancel access to Labels.
  flows:
  - authorizationCode
  - clientCredentials
  scope: labels
- description: read location resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: locations
- description: ''
  flows: []
  scope: locations-files
- description: read-only access to all shipments endpoints
  flows:
  - authorizationCode
  - clientCredentials
  scope: logistics
- description: change of address
  flows:
  - authorizationCode
  - clientCredentials
  scope: ncoa-data-services
- description: ''
  flows: []
  scope: oauth2-oidc
- description: OpenID Connnect industry standard scope to utilize this API.
  flows:
  - authorizationCode
  - clientCredentials
  scope: openid
- description: ''
  flows: []
  scope: parcel-locker
- description: Both read and write access to the payments API.
  flows:
  - clientCredentials
  scope: payments
- description: read write access to all pickup endpoints
  flows:
  - authorizationCode
  - clientCredentials
  scope: pickup
- description: Read, create and cancel access to Open and Distribute.
  flows:
  - authorizationCode
  - clientCredentials
  scope: pmod
- description: get prices based on ingredients
  flows:
  - authorizationCode
  - clientCredentials
  scope: prices
- description: The OpenID Connect industry standard, United States Postal Service authorized access the user's name and company.
  flows:
  - authorizationCode
  - clientCredentials
  scope: profile
- description: read QR Code resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: qr-code
- description: read reconciliation adjustments resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: reconciliation-adjustments
- description: Both read and create access to Scan Forms API.
  flows:
  - authorizationCode
  - clientCredentials
  scope: scan-forms
- description: Read access to Service Standards.
  flows:
  - authorizationCode
  - clientCredentials
  scope: service-standards
- description: get service standards directory
  flows:
  - clientCredentials
  scope: service-standards-directory
- description: ''
  flows: []
  scope: service-standards-files
- description: Read access to Ship Enrollment.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ship-enrollment
- description: Read access to Shipping Options API.
  flows:
  - clientCredentials
  scope: shipments
- description: Read, and write access to resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: subscriptions-address
- description: ''
  flows: []
  scope: subscriptions-addresses
- description: Read, and write access to resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: subscriptions-adjustments
- description: Read, and write access to resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: subscriptions-disputes
- description: Read, and write access to resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: subscriptions-ncoa
- description: Read, and write access to resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: subscriptions-package-transaction-details
- description: Read, and write access to resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: subscriptions-tracking
- description: Read, and write access to resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: subscriptions-unpaid-packages
- description: Get tracking information and create tracking notifications.
  flows:
  - authorizationCode
  - clientCredentials
  scope: tracking
- description: United States Postal Service authorized access to the user's mailer IDs.
  flows:
  - authorizationCode
  - clientCredentials
  scope: usps:MIDs
- description: United States Postal Service authorized access to the user's contract rates.
  flows:
  - authorizationCode
  - clientCredentials
  scope: usps:contract_rates
- description: United States Postal Service authorized access to the user's payment methods.
  flows:
  - authorizationCode
  - clientCredentials
  scope: usps:payment_methods
slug: usps-scopes
source_filename: usps-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/usps-addresses-openapi.yml, openapi/usps-adjustments-openapi.yml, openapi/usps-appointments-openapi.yml,\n  openapi/usps-carrier-pickup-openapi.yml, openapi/usps-containers-openapi.yml, openapi/usps-domestic-labels-openapi.yml,\n  openapi/usps-domestic-prices-openapi.yml, openapi/usps-informed-delivery-mail-campaigns-openapi.yml,\n  openapi/usps-informed-delivery-package-campaigns-openapi.yml, openapi/usps-international-labels-openapi.yml,\n  openapi/usps-international-prices-openapi.yml, openapi/usps-international-service-standards-openapi.yml,\n  openapi/usps-locations-openapi.yml, openapi/usps-logistics-shipments-openapi.yml, openapi/usps-ncoa-openapi.yml,\n  openapi/usps-payments-openapi.yml, openapi/usps-pmod-openapi.yml, openapi/usps-qr-codes-openapi.yml,\n  openapi/usps-reconciliation-adjustments-openapi.yml, openapi/usps-scan-forms-openapi.yml,\n  openapi/usps-service-standards-directory-openapi.yml, openapi/usps-service-standards-files-openapi.yml,\n\
  \  openapi/usps-service-standards-openapi.yml, openapi/usps-ship-enrollment-openapi.yml, openapi/usps-shipping-options-openapi.yml,\n  openapi/usps-subscriptions-addresses-openapi.yml, openapi/usps-subscriptions-adjustments-openapi.yml,\n  openapi/usps-subscriptions-disputes-openapi.yml, openapi/usps-subscriptions-ncoa-openapi.yml,\n  openapi/usps-subscriptions-package-transaction-details-openapi.yml, openapi/usps-subscriptions-tracking-openapi.yml,\n  openapi/usps-subscriptions-tracking-v3r2-openapi.yml, openapi/usps-subscriptions-unpaid-packages-openapi.yml,\n  openapi/usps-tracking-openapi.yml, openapi/usps-tracking-v3r2-openapi.yml, openapi/usps-userinfo-openapi.yml\nschemes:\n- name: OAuth\n  source: openapi/usps-addresses-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON\
  \ Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-adjustments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specificed APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-appointments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: |-\n    The specificed APIs accept an access token formatted as a JSON Web\n    Token. The relative path to the OAuth2 version 3 API which supplies this\n   \
  \ access token is provided below for reference.\n- name: OAuth\n  source: openapi/usps-carrier-pickup-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-containers-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-domestic-labels-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n\
  \    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-domestic-prices-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-informed-delivery-mail-campaigns-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n- name: OAuth\n  source: openapi/usps-informed-delivery-package-campaigns-openapi.yml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: /oauth2/token\n- name: OAuth\n  source: openapi/usps-international-labels-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-international-prices-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-international-service-standards-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-locations-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-logistics-shipments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: OAuth2\
  \ security scheme for shipment tracking.\n- name: OAuth\n  source: openapi/usps-ncoa-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-payments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n- name: OAuth\n  source: openapi/usps-pmod-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this\
  \ access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-qr-codes-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-reconciliation-adjustments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-scan-forms-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-service-standards-directory-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-service-standards-files-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n\
  \  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-service-standards-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-ship-enrollment-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n\
  \    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-shipping-options-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-subscriptions-addresses-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-subscriptions-adjustments-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-subscriptions-disputes-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-subscriptions-ncoa-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow:\
  \ authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-subscriptions-package-transaction-details-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-subscriptions-tracking-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n\
  \    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-subscriptions-tracking-v3r2-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-subscriptions-unpaid-packages-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs\
  \ accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-tracking-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specified APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-tracking-v3r2-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: The specificed APIs accept an access token formatted as a JSON Web Token. The\n    relative path to the OAuth2 version\
  \ 3 API which supplies this access token is provided below\n    for reference.\n- name: OAuth\n  source: openapi/usps-userinfo-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v3/token\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v3/authorize\n    tokenUrl: /oauth2/v3/token\n  description: |-\n    The specified APIs accept an access token placed in the Authorization header using the Bearer Authentication security scheme. The relative path to the OAuth2 API which supply this access token is provided here for reference.\n    Access tokens issued by either the OAuth __Client Credentials__ or __Authorization Code__ flows are supported.\n    The 'openid' scope is required either as an input or assigned to the client applicatiion upoon registration.\nscopes:\n- scope: address\n  description: The OpenID Connect industry standard, United States Postal Service authorized\n    access the user's address.\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/usps-userinfo-openapi.yml\n- scope: addresses\n  description: read-only access to all addresses endpoints\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-addresses-openapi.yml\n- scope: adjustments\n  description: Get adjustments for a tracking number.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-adjustments-openapi.yml\n- scope: campaigns\n  description: read/write access to all campaigns endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/usps-informed-delivery-mail-campaigns-openapi.yml\n  - openapi/usps-informed-delivery-package-campaigns-openapi.yml\n- scope: carrier-pickup\n  sources:\n  - openapi/usps-carrier-pickup-openapi.yml\n- scope: containers\n  description: Both read and create access to containers API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/usps-containers-openapi.yml\n- scope: email\n  description: The OpenID Connect industry standard,\
  \ United States Postal Service authorized\n    access the user's email address.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-userinfo-openapi.yml\n- scope: fast-appointments\n  description: check for available slots and create appointments\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-appointments-openapi.yml\n- scope: international-labels\n  description: Read, create, and cancel access to Labels.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-international-labels-openapi.yml\n- scope: international-prices\n  description: get prices based on ingredients\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-international-prices-openapi.yml\n- scope: international-service-standard\n  description: Read access to Service Standard.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/usps-international-service-standards-openapi.yml\n- scope:\
  \ labels\n  description: Read, create, and cancel access to Labels.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-domestic-labels-openapi.yml\n- scope: locations\n  description: read location resources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-locations-openapi.yml\n- scope: locations-files\n  sources:\n  - openapi/usps-locations-openapi.yml\n- scope: logistics\n  description: read-only access to all shipments endpoints\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-logistics-shipments-openapi.yml\n- scope: ncoa-data-services\n  description: change of address\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-ncoa-openapi.yml\n- scope: oauth2-oidc\n  sources:\n  - openapi/usps-userinfo-openapi.yml\n- scope: openid\n  description: OpenID Connnect industry standard scope to utilize this API.\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/usps-userinfo-openapi.yml\n- scope: parcel-locker\n  sources:\n  - openapi/usps-locations-openapi.yml\n- scope: payments\n  description: Both read and write access to the payments API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/usps-payments-openapi.yml\n- scope: pickup\n  description: read write access to all pickup endpoints\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-carrier-pickup-openapi.yml\n- scope: pmod\n  description: Read, create and cancel access to Open and Distribute.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-pmod-openapi.yml\n- scope: prices\n  description: get prices based on ingredients\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-domestic-prices-openapi.yml\n- scope: profile\n  description: The OpenID Connect industry standard, United States Postal Service authorized\n    access the user's name and company.\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-userinfo-openapi.yml\n- scope: qr-code\n  description: read QR Code resources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-qr-codes-openapi.yml\n- scope: reconciliation-adjustments\n  description: read reconciliation adjustments resources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-reconciliation-adjustments-openapi.yml\n- scope: scan-forms\n  description: Both read and create access to Scan Forms API.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-scan-forms-openapi.yml\n- scope: service-standards\n  description: Read access to Service Standards.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-service-standards-files-openapi.yml\n  - openapi/usps-service-standards-openapi.yml\n- scope: service-standards-directory\n  description: get service standards\
  \ directory\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/usps-service-standards-directory-openapi.yml\n- scope: service-standards-files\n  sources:\n  - openapi/usps-service-standards-files-openapi.yml\n- scope: ship-enrollment\n  description: Read access to Ship Enrollment.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-ship-enrollment-openapi.yml\n- scope: shipments\n  description: Read access to Shipping Options API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/usps-shipping-options-openapi.yml\n- scope: subscriptions-address\n  description: Read, and write access to resources.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-subscriptions-addresses-openapi.yml\n- scope: subscriptions-addresses\n  sources:\n  - openapi/usps-subscriptions-addresses-openapi.yml\n- scope: subscriptions-adjustments\n  description: Read, and write access to resources.\n  flows:\n  - authorizationCode\n \
  \ - clientCredentials\n  sources:\n  - openapi/usps-subscriptions-adjustments-openapi.yml\n- scope: subscriptions-disputes\n  description: Read, and write access to resources.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-subscriptions-disputes-openapi.yml\n- scope: subscriptions-ncoa\n  description: Read, and write access to resources.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-subscriptions-ncoa-openapi.yml\n- scope: subscriptions-package-transaction-details\n  description: Read, and write access to resources.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-subscriptions-package-transaction-details-openapi.yml\n- scope: subscriptions-tracking\n  description: Read, and write access to resources.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-subscriptions-tracking-openapi.yml\n  - openapi/usps-subscriptions-tracking-v3r2-openapi.yml\n\
  - scope: subscriptions-unpaid-packages\n  description: Read, and write access to resources.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-subscriptions-unpaid-packages-openapi.yml\n- scope: tracking\n  description: Get tracking information and create tracking notifications.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-tracking-openapi.yml\n  - openapi/usps-tracking-v3r2-openapi.yml\n- scope: usps:MIDs\n  description: United States Postal Service authorized access to the user's mailer IDs.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-userinfo-openapi.yml\n- scope: usps:contract_rates\n  description: United States Postal Service authorized access to the user's contract rates.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-userinfo-openapi.yml\n- scope: usps:payment_methods\n  description: United States Postal Service authorized access\
  \ to the user's payment methods.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/usps-userinfo-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/usps/scopes/usps-scopes.yml
summary_line: 44 scopes · clientCredentials/authorizationCode
tags:
- Government
- Postal Service
- Shipping
- Logistics
- Address Validation
- Package Tracking
token_bound: false
token_urls:
- /oauth2/v3/token
- /oauth2/token
---
