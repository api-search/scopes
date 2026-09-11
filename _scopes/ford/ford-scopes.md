---
api_specs:
- filename: ford-charging-api-openapi.yml
  format: yaml
  label: Ford Charging API
  slug: ford-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-charging-api-openapi.yml
- filename: ford-commands-api-openapi.yml
  format: yaml
  label: Ford Commands API
  slug: ford-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-commands-api-openapi.yml
- filename: ford-images-api-openapi.yml
  format: yaml
  label: Ford Images API
  slug: ford-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-images-api-openapi.yml
- filename: ford-oauth-api-openapi.yml
  format: yaml
  label: Ford OAuth API
  slug: ford-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-oauth-api-openapi.yml
- filename: ford-status-api-openapi.yml
  format: yaml
  label: Ford Status API
  slug: ford-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-status-api-openapi.yml
- filename: ford-vehicles-api-openapi.yml
  format: yaml
  label: Ford Vehicles API
  slug: ford-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/openapi/ford-vehicles-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.ford.com/apis
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ford Scopes
name_suffix: OAuth Scopes
note: 'Ford does not publish a conventional OAuth scope string list. Authorization on FordConnect is granted as DATA CATEGORIES: an application declares the categories it needs on the ''API & Scope Info'' step of credential creation (''Data categories in scope'', ''At least one Data Category must be selected''), and the vehicle owner consents to those categories in the FordPass account-linking flow. The categories below are Ford''s own, harvested verbatim from the developer portal. The OIDC layer itself advertises only the ''openid'' scope — confirmed from Ford''s own Azure AD B2C discovery document — so the category list, not an OAuth scope string, is the real permission surface. The single ''access'' scope previously recorded here was derived from an API Evangelist documentation-derived OpenAPI, not from Ford.'
overview: 'Ford publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ford API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ford
provider_slug: ford
schemes:
- authorizationUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/authorize
  consent_url: https://fordconnect.cv.ford.com/common/login
  flow: authorizationCode
  issuer: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/v2.0/
  jwks_uri: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/discovery/v2.0/keys
  name: oauth2
  policy: B2C_1A_signup_signin_common
  source: well-known/ford-openid-configuration.json
  tokenUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/token
  type: oauth2
scope_count: 14
scope_names:
- chargingData
- drivingData
- evData
- tripData
- upfitterData
- vehicleData
- vehicleHealth
- vehicleLocation
- vehicleSecurity
- dynamicCharging
- vehicleCommands
- vehicleBasicInfo
- customerInfo
- rewards
scopes:
- description: Information related to the vehicle’s charging process, including voltage, current, charger type, and plug status.
  flows:
  - authorizationCode
  scope: chargingData
- description: Real-time sensor and driver input data, such as acceleration, pedal position, gear lever, and wheel torque.
  flows:
  - authorizationCode
  scope: drivingData
- description: Key electric vehicle metrics, including battery charge level, energy capacity, temperature, and motor voltage.
  flows:
  - authorizationCode
  scope: evData
- description: Insights into journey specifics, such as fuel consumption, total distance, and electric-only travel range.
  flows:
  - authorizationCode
  scope: tripData
- description: High-level details about Specialty Vehicle Manufacturer-installed modules such as input and output status of those modules.
  flows:
  - authorizationCode
  scope: upfitterData
- description: Core vehicle performance and system status, including battery levels, fuel, and coolant temperature.
  flows:
  - authorizationCode
  scope: vehicleData
- description: Diagnostic and maintenance-related information, including tire pressure, oil life, and Diesel exhaust system status.
  flows:
  - authorizationCode
  scope: vehicleHealth
- description: Positional and movement data, including GPS coordinates, compass direction, and wheel speed.
  flows:
  - authorizationCode
  scope: vehicleLocation
- description: Status of security systems, including alarms, door locks, and window positions.
  flows:
  - authorizationCode
  scope: vehicleSecurity
- description: Dynamic charging vehicle’s data includes start charging, stop charging, set vehicle home.
  flows:
  - authorizationCode
  scope: dynamicCharging
- description: Commands to interact with the vehicle, such as lock and unlock.
  flows:
  - authorizationCode
  scope: vehicleCommands
- description: Vehicle identity information including VIN, Make, Model, Year, and Drivetrain configuration.
  flows:
  - authorizationCode
  scope: vehicleBasicInfo
- description: Name and email address.
  flows:
  - authorizationCode
  scope: customerInfo
- description: Ford/Lincoln Rewards member number and points information.
  flows:
  - authorizationCode
  scope: rewards
slug: ford-scopes
source_filename: ford-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: https://developer.ford.com/assets/i18n/en.json\ndocs: https://developer.ford.com/apis\nnote: 'Ford does not publish a conventional OAuth scope string list. Authorization on FordConnect is granted\n  as DATA CATEGORIES: an application declares the categories it needs on the ''API & Scope Info'' step\n  of credential creation (''Data categories in scope'', ''At least one Data Category must be selected''),\n  and the vehicle owner consents to those categories in the FordPass account-linking flow. The categories\n  below are Ford''s own, harvested verbatim from the developer portal. The OIDC layer itself advertises\n  only the ''openid'' scope — confirmed from Ford''s own Azure AD B2C discovery document — so the category\n  list, not an OAuth scope string, is the real permission surface. The single ''access'' scope previously\n  recorded here was derived from an API Evangelist documentation-derived OpenAPI, not from Ford.'\nschemes:\n\
  - name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  issuer: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/v2.0/\n  authorizationUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/authorize\n  tokenUrl: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/oauth2/v2.0/token\n  jwks_uri: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/b2c_1a_signup_signin_common/discovery/v2.0/keys\n  policy: B2C_1A_signup_signin_common\n  consent_url: https://fordconnect.cv.ford.com/common/login\n  source: well-known/ford-openid-configuration.json\noidc_scopes_supported:\n- openid\npermission_model: data-categories\nscope_count: 14\nscopes:\n- scope: chargingData\n  name: Charging Data\n  description: Information related to the vehicle’s charging process, including voltage, current, charger\n    type, and plug status.\n  kind: data-category\n\
  \  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: drivingData\n  name: Driving Data\n  description: Real-time sensor and driver input data, such as acceleration, pedal position, gear lever,\n    and wheel torque.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: evData\n  name: EV Data\n  description: Key electric vehicle metrics, including battery charge level, energy capacity, temperature,\n    and motor voltage.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: tripData\n  name: Trip Data\n  description: Insights into journey specifics, such as fuel consumption, total distance, and electric-only\n    travel\
  \ range.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: upfitterData\n  name: Specialty Vehicle Manufacturer Data\n  description: High-level details about Specialty Vehicle Manufacturer-installed modules such as input\n    and output status of those modules.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: vehicleData\n  name: Vehicle Data\n  description: Core vehicle performance and system status, including battery levels, fuel, and coolant\n    temperature.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: vehicleHealth\n  name: Vehicle Health\n  description: Diagnostic and maintenance-related\
  \ information, including tire pressure, oil life, and\n    Diesel exhaust system status.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: vehicleLocation\n  name: Vehicle Location\n  description: Positional and movement data, including GPS coordinates, compass direction, and wheel speed.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: vehicleSecurity\n  name: Vehicle Security\n  description: Status of security systems, including alarms, door locks, and window positions.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: dynamicCharging\n  name: Dynamic Charging\n  description: Dynamic\
  \ charging vehicle’s data includes start charging, stop charging, set vehicle home.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: vehicleCommands\n  name: Vehicle Commands\n  description: Commands to interact with the vehicle, such as lock and unlock.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: vehicleBasicInfo\n  name: Vehicle Basic Info\n  description: Vehicle identity information including VIN, Make, Model, Year, and Drivetrain configuration.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: customerInfo\n  name: Customer Information\n  description: Name and email address.\n\
  \  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\n- scope: rewards\n  name: Rewards Information\n  description: Ford/Lincoln Rewards member number and points information.\n  kind: data-category\n  flows:\n  - authorizationCode\n  consent: vehicle owner, via FordPass account linking\n  sources:\n  - https://developer.ford.com/assets/i18n/en.json\nx-evidence:\n- url: https://developer.ford.com/assets/i18n/en.json\n  http_status: 200\n  fetched: '2026-09-10'\n- url: https://dah2vb2cprod.b2clogin.com/914d88b1-3523-4bf6-9be4-1b96b4f6f919/B2C_1A_signup_signin_common/v2.0/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-09-10'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ford/refs/heads/main/scopes/ford-scopes.yml
summary_line: 14 scopes
tags:
- Automobiles
- Cars
- Vehicles
- Connected Vehicle
- Automotive
- Telematics
- Electric Vehicles
- Fleet
token_urls: []
---
