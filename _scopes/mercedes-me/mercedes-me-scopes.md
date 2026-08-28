---
api_specs:
- filename: mercedes-me-components-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Components API
  slug: mercedes-me-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-components-api-openapi.yml
- filename: mercedes-me-configurations-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Configurations API
  slug: mercedes-me-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-configurations-api-openapi.yml
- filename: mercedes-me-dealer-search-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Dealer search API
  slug: mercedes-me-dealer-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-dealer-search-api-openapi.yml
- filename: mercedes-me-diagnostic-trouble-code-dtc-snapshots-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Diagnostic Trouble Code (DTC) Snapshots API
  slug: mercedes-me-diagnostic-trouble-code-dtc-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-diagnostic-trouble-code-dtc-snapshots-api-openapi.yml
- filename: mercedes-me-diagnostic-trouble-codes-dtc-s-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Diagnostic Trouble Codes (DTC's) API
  slug: mercedes-me-diagnostic-trouble-codes-dtc-s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-diagnostic-trouble-codes-dtc-s-api-openapi.yml
- filename: mercedes-me-electronical-control-units-ecu-s-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Electronical Control Units (ECU's) API
  slug: mercedes-me-electronical-control-units-ecu-s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-electronical-control-units-ecu-s-api-openapi.yml
- filename: mercedes-me-images-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Images API
  slug: mercedes-me-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-images-api-openapi.yml
- filename: mercedes-me-perspectives-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Perspectives API
  slug: mercedes-me-perspectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-perspectives-api-openapi.yml
- filename: mercedes-me-references-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me References API
  slug: mercedes-me-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-references-api-openapi.yml
- filename: mercedes-me-resources-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Resources API
  slug: mercedes-me-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-resources-api-openapi.yml
- filename: mercedes-me-saved-configurations-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Saved configurations API
  slug: mercedes-me-saved-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-saved-configurations-api-openapi.yml
authorization_urls: []
description: The Mercedes-Benz connected-vehicle APIs authenticate against the Mercedes-Benz customer identity provider at https://id.mercedes-benz.com (PingFederate). Its OpenID Connect discovery document is public and unauthenticated, and it publishes the complete scopes_supported list — 81 scopes, of which 38 are Mercedes-Benz product scopes. This artifact records those scopes verbatim as probed, together with the API product each scope string names. Mercedes-Benz publishes NO OpenAPI securitySchemes for the connected-vehicle products (the four Swagger 2.0 documents in openapi/ carry no securityDefinitions at all), so the discovery document is the only machine-readable scope reference the provider publishes.
docs: https://developer.mercedes-benz.com/content-page/oauth-documentation
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Mercedes Me Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mercedes-Benz Mercedes me publishes 38 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mercedes-Benz Mercedes me API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mercedes-Benz Mercedes me
provider_slug: mercedes-me
schemes: []
scope_count: 38
scope_names:
- mb:vehicle:mbdata:vehiclestatus
- mb:vehicle:mbdata:vehiclestatus15
- mb:vehicle:mbdata:vehiclelock
- mb:vehicle:mbdata:fuelstatus
- mb:vehicle:mbdata:evstatus
- mb:vehicle:mbdata:evstatus2.0
- mb:vehicle:mbdata:evstatus3.0
- mb:vehicle:mbdata:payasyoudrive
- mb:vehicle:mbdata:payasyoudrive2.0
- mb:vehicle:image
- mb:vehicle:rds:reader
- mb:vehicle:rms:reader
- mb:vehicle:action:doors
- mb:vehicle:action:general
- mb:vehicle:status:writer
- mb:vehicle:status:general
- mb:vehicle:status:location
- mb:user:pool:reader
- mb:user:cv_exp:reader
- mb:vehicle:cv_exp:general
- mb.vehicle
- mb:vehicle:mbdata:euda:vehicleoperation
- mb:vehicle:mbdata:euda:maintenancediagnostic
- mb:vehicle:mbdata:euda:navigationpositioning
- mb:vehicle:mbdata:euda:bodyfeature
- mb:vehicle:mbdata:euda:bodymountingwork
- mb:vehicle:mbdata:euda:climatecomfort
- mb:vehicle:mbdata:euda:energyconsumption
- mb:vehicle:mbdata:euda:infotainmentuserinteraction
- mb:wallbox:mbdata:euda:wallbox
- mb:digital:eqready:userdata
- mb:service:incardelivery
- mb:company-id
- mb:internal
- mb:rduhackathon
- oneapi:vehicle:light
- oneapi:testapi
- oneapi:nil
scopes:
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:vehiclestatus
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:vehiclestatus15
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:vehiclelock
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:fuelstatus
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:evstatus
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:evstatus2.0
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:evstatus3.0
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:payasyoudrive
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:payasyoudrive2.0
- description: ''
  flows: []
  scope: mb:vehicle:image
- description: ''
  flows: []
  scope: mb:vehicle:rds:reader
- description: ''
  flows: []
  scope: mb:vehicle:rms:reader
- description: ''
  flows: []
  scope: mb:vehicle:action:doors
- description: ''
  flows: []
  scope: mb:vehicle:action:general
- description: ''
  flows: []
  scope: mb:vehicle:status:writer
- description: ''
  flows: []
  scope: mb:vehicle:status:general
- description: ''
  flows: []
  scope: mb:vehicle:status:location
- description: ''
  flows: []
  scope: mb:user:pool:reader
- description: ''
  flows: []
  scope: mb:user:cv_exp:reader
- description: ''
  flows: []
  scope: mb:vehicle:cv_exp:general
- description: ''
  flows: []
  scope: mb.vehicle
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:euda:vehicleoperation
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:euda:maintenancediagnostic
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:euda:navigationpositioning
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:euda:bodyfeature
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:euda:bodymountingwork
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:euda:climatecomfort
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:euda:energyconsumption
- description: ''
  flows: []
  scope: mb:vehicle:mbdata:euda:infotainmentuserinteraction
- description: ''
  flows: []
  scope: mb:wallbox:mbdata:euda:wallbox
- description: ''
  flows: []
  scope: mb:digital:eqready:userdata
- description: ''
  flows: []
  scope: mb:service:incardelivery
- description: ''
  flows: []
  scope: mb:company-id
- description: ''
  flows: []
  scope: mb:internal
- description: ''
  flows: []
  scope: mb:rduhackathon
- description: ''
  flows: []
  scope: oneapi:vehicle:light
- description: ''
  flows: []
  scope: oneapi:testapi
- description: ''
  flows: []
  scope: oneapi:nil
slug: mercedes-me-scopes
source_filename: mercedes-me-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://id.mercedes-benz.com/.well-known/openid-configuration\ndocs: https://developer.mercedes-benz.com/content-page/oauth-documentation\nevidence:\n  - url: https://id.mercedes-benz.com/.well-known/openid-configuration\n    status: 200\n    content_type: application/json\n    note: saved verbatim to well-known/mercedes-me-id-openid-configuration.json\n  - url: https://id.mercedes-benz.com/.well-known/oauth-authorization-server\n    status: 200\n    content_type: application/json\n    note: saved verbatim to well-known/mercedes-me-id-oauth-authorization-server.json\ndescription: >-\n  The Mercedes-Benz connected-vehicle APIs authenticate against the Mercedes-Benz customer identity\n  provider at https://id.mercedes-benz.com (PingFederate). Its OpenID Connect discovery document is\n  public and unauthenticated, and it publishes the complete scopes_supported list — 81 scopes, of\n  which 38 are Mercedes-Benz product scopes. This\
  \ artifact records those scopes verbatim as probed,\n  together with the API product each scope string names. Mercedes-Benz publishes NO OpenAPI\n  securitySchemes for the connected-vehicle products (the four Swagger 2.0 documents in openapi/\n  carry no securityDefinitions at all), so the discovery document is the only machine-readable\n  scope reference the provider publishes.\nauthorization_server:\n  issuer: https://id.mercedes-benz.com\n  authorization_endpoint: https://id.mercedes-benz.com/as/authorization.oauth2\n  token_endpoint: https://id.mercedes-benz.com/as/token.oauth2\n  revocation_endpoint: https://id.mercedes-benz.com/as/revoke_token.oauth2\n  introspection_endpoint: https://id.mercedes-benz.com/as/introspect.oauth2\n  userinfo_endpoint: https://id.mercedes-benz.com/idp/userinfo.openid\n  jwks_uri: https://id.mercedes-benz.com/pf/JWKS\n  registration_endpoint: https://id.mercedes-benz.com/as/clients.oauth2\n  pushed_authorization_request_endpoint_present: true\n  device_authorization_endpoint_present:\
  \ true\n  end_session_endpoint_present: true\n  code_challenge_methods_supported: [plain, S256]\n  grant_types_supported:\n    - authorization_code\n    - refresh_token\n    - client_credentials\n    - implicit\n    - password\n    - urn:ietf:params:oauth:grant-type:jwt-bearer\n    - urn:ietf:params:oauth:grant-type:saml2-bearer\n    - urn:ietf:params:oauth:grant-type:device_code\n    - urn:ietf:params:oauth:grant-type:token-exchange\n    - urn:openid:params:grant-type:ciba\n    - urn:pingidentity.com:oauth2:grant_type:validate_bearer\n  token_endpoint_auth_methods_supported:\n    - client_secret_basic\n    - client_secret_post\n    - client_secret_jwt\n    - private_key_jwt\n    - tls_client_auth\n    - none\nscope_count: 81\nproduct_scope_count: 38\nscopes:\n  # --- Connected vehicle data products (the Mercedes me / connected-vehicle API family) ---\n  - scope: mb:vehicle:mbdata:vehiclestatus\n    product: Vehicle Status API\n    grants: Door, window, deck-lid, sunroof, tyre-pressure\
  \ and overall lock state by VIN.\n    mapping_confidence: high\n    mapping_basis: scope string names the product (mbdata + vehiclestatus)\n  - scope: mb:vehicle:mbdata:vehiclestatus15\n    product: Vehicle Status API\n    grants: Extended Vehicle Status signal set (15-signal variant).\n    mapping_confidence: medium\n    mapping_basis: scope string names the product; the \"15\" suffix is not explained in any public Mercedes-Benz document we could read\n  - scope: mb:vehicle:mbdata:vehiclelock\n    product: Vehicle Lock Status API\n    grants: Door-lock, deck-lid and position-lock state by VIN.\n    mapping_confidence: high\n    mapping_basis: scope string names the product\n  - scope: mb:vehicle:mbdata:fuelstatus\n    product: Fuel Status API\n    grants: Tank level and remaining fuel range by VIN.\n    mapping_confidence: high\n    mapping_basis: scope string names the product\n  - scope: mb:vehicle:mbdata:evstatus\n    product: Electric Vehicle Status API (v1)\n    grants: State of\
  \ charge, electric range and charge status.\n    mapping_confidence: high\n    mapping_basis: scope string names the product\n  - scope: mb:vehicle:mbdata:evstatus2.0\n    product: Electric Vehicle Status API (v2)\n    grants: v2 signal set, including remote charge control surface.\n    mapping_confidence: high\n    mapping_basis: scope string names the product and its version\n  - scope: mb:vehicle:mbdata:evstatus3.0\n    product: Electric Vehicle Status API (v3)\n    grants: v3 signal set — the version currently listed on the developer portal.\n    mapping_confidence: high\n    mapping_basis: scope string names the product and its version\n  - scope: mb:vehicle:mbdata:payasyoudrive\n    product: Pay As You Drive Insurance API (v1)\n    grants: Odometer reading and geographic position for usage-based insurance.\n    mapping_confidence: high\n    mapping_basis: scope string names the product\n  - scope: mb:vehicle:mbdata:payasyoudrive2.0\n    product: Pay As You Drive 2.0 API\n    grants:\
  \ v2 odometer + position signal set.\n    mapping_confidence: high\n    mapping_basis: scope string names the product and its version\n  - scope: mb:vehicle:image\n    product: Vehicle Images API\n    grants: Vehicle and component imagery for a FIN/VIN or configuration.\n    mapping_confidence: high\n    mapping_basis: scope string names the product\n  - scope: mb:vehicle:rds:reader\n    product: Remote Diagnostic Support API\n    grants: Read access to DTC, DTC-snapshot, ECU and resource readouts. (rds = Remote Diagnostic Support.)\n    mapping_confidence: high\n    mapping_basis: acronym matches the product name and the readout operations in openapi/mercedes-me-*-readouts specs\n  - scope: mb:vehicle:rms:reader\n    product: unmapped\n    grants: Read scope on an \"rms\" vehicle service.\n    mapping_confidence: low\n    mapping_basis: no Mercedes-Benz public document we could read expands \"rms\"; recorded because it is published, not because we can attribute it\n  # --- Vehicle command\
  \ / action scopes ---\n  - scope: mb:vehicle:action:doors\n    product: Remote door commands\n    grants: Remote lock/unlock of vehicle doors. WRITE scope — a safety-relevant actuation.\n    mapping_confidence: high\n    mapping_basis: scope string names the action\n  - scope: mb:vehicle:action:general\n    product: Remote vehicle commands (general)\n    grants: General remote-command surface. WRITE scope.\n    mapping_confidence: high\n    mapping_basis: scope string names the action\n  - scope: mb:vehicle:status:writer\n    product: Vehicle status write\n    grants: Write access to vehicle status. WRITE scope.\n    mapping_confidence: medium\n    mapping_basis: scope string names a writer role on vehicle status; no public reference page describes it\n  - scope: mb:vehicle:status:general\n    product: Vehicle status (general)\n    grants: General vehicle-status read scope. Commonly paired with mb:user:pool:reader in Mercedes-Benz OAuth examples.\n    mapping_confidence: medium\n    mapping_basis:\
  \ scope string; pairing observed in third-party integration write-ups, not in a Mercedes-Benz reference page we could read\n  - scope: mb:vehicle:status:location\n    product: Vehicle location\n    grants: Vehicle geographic position.\n    mapping_confidence: high\n    mapping_basis: scope string names the signal\n  # --- Vehicle / user pool ---\n  - scope: mb:user:pool:reader\n    product: Vehicle pool\n    grants: Read the set of vehicles the consenting customer has assigned to the application.\n    mapping_confidence: high\n    mapping_basis: scope string\n  - scope: mb:user:cv_exp:reader\n    product: Connected-vehicle experience (read)\n    mapping_confidence: low\n    mapping_basis: scope string only\n  - scope: mb:vehicle:cv_exp:general\n    product: Connected-vehicle experience (general)\n    mapping_confidence: low\n    mapping_basis: scope string only\n  - scope: mb.vehicle\n    product: unmapped legacy scope\n    mapping_confidence: low\n    mapping_basis: dot-delimited legacy\
  \ form; recorded verbatim as published\n  # --- EUDA (EU Data Act) vehicle-data categories ---\n  - scope: mb:vehicle:mbdata:euda:vehicleoperation\n    product: EU Data Act vehicle-data category — vehicle operation\n    mapping_confidence: high\n    mapping_basis: 'the \"euda\" segment plus the category name'\n  - scope: mb:vehicle:mbdata:euda:maintenancediagnostic\n    product: EU Data Act vehicle-data category — maintenance and diagnostics\n    mapping_confidence: high\n    mapping_basis: 'the \"euda\" segment plus the category name'\n  - scope: mb:vehicle:mbdata:euda:navigationpositioning\n    product: EU Data Act vehicle-data category — navigation and positioning\n    mapping_confidence: high\n    mapping_basis: 'the \"euda\" segment plus the category name'\n  - scope: mb:vehicle:mbdata:euda:bodyfeature\n    product: EU Data Act vehicle-data category — body features\n    mapping_confidence: high\n    mapping_basis: 'the \"euda\" segment plus the category name'\n  - scope: mb:vehicle:mbdata:euda:bodymountingwork\n\
  \    product: EU Data Act vehicle-data category — body mounting work (van upfitters)\n    mapping_confidence: high\n    mapping_basis: 'the \"euda\" segment plus the category name'\n  - scope: mb:vehicle:mbdata:euda:climatecomfort\n    product: EU Data Act vehicle-data category — climate and comfort\n    mapping_confidence: high\n    mapping_basis: 'the \"euda\" segment plus the category name'\n  - scope: mb:vehicle:mbdata:euda:energyconsumption\n    product: EU Data Act vehicle-data category — energy consumption\n    mapping_confidence: high\n    mapping_basis: 'the \"euda\" segment plus the category name'\n  - scope: mb:vehicle:mbdata:euda:infotainmentuserinteraction\n    product: EU Data Act vehicle-data category — infotainment user interaction\n    mapping_confidence: high\n    mapping_basis: 'the \"euda\" segment plus the category name'\n  - scope: mb:wallbox:mbdata:euda:wallbox\n    product: EU Data Act data category — home wallbox charger\n    mapping_confidence: high\n    mapping_basis:\
  \ 'the \"euda\" segment plus the category name'\n  # --- Adjacent Mercedes-Benz products ---\n  - scope: mb:digital:eqready:userdata\n    product: EQ Ready\n    mapping_confidence: medium\n    mapping_basis: scope string names the Mercedes-Benz EQ Ready app\n  - scope: mb:service:incardelivery\n    product: In-car delivery service\n    mapping_confidence: medium\n    mapping_basis: scope string names the service\n  - scope: mb:company-id\n    product: Company identifier claim\n    mapping_confidence: medium\n    mapping_basis: matches the company-id claim in claims_supported\n  - scope: mb:internal\n    product: internal\n    mapping_confidence: high\n    mapping_basis: not for third-party use — published in discovery but named internal\n  - scope: mb:rduhackathon\n    product: hackathon scope\n    mapping_confidence: high\n    mapping_basis: scope string; not a production product\n  - scope: oneapi:vehicle:light\n    product: OneAPI vehicle (light)\n    mapping_confidence: low\n    mapping_basis:\
  \ scope string only\n  - scope: oneapi:testapi\n    product: OneAPI test\n    mapping_confidence: high\n    mapping_basis: test scope, not a production product\n  - scope: oneapi:nil\n    product: OneAPI placeholder\n    mapping_confidence: high\n    mapping_basis: placeholder scope\nstandard_scopes:\n  - openid\n  - profile\n  - email\n  - phone\n  - address\n  - offline_access\nnotes:\n  - >-\n    Scope-to-product mapping is stated with an explicit confidence on every row. Where Mercedes-Benz\n    publishes no readable reference for a scope string, the row says so rather than guessing —\n    the developer portal is a client-rendered SPA whose reference pages return an empty HTML shell\n    to any non-browser client, so the per-product scope tables could not be read.\n  - >-\n    The eleven Car Configurator / Dealer / Vehicle Images / Remote Diagnostic Support OpenAPI\n    documents in openapi/ authenticate with an API key, not OAuth — their 401 response description\n    reads \"Failed\
  \ to resolve API Key query parameter / Invalid API Key\". The OAuth scopes above\n    apply to the connected-vehicle product family, which publishes no OpenAPI.\n  - >-\n    The presence of an mb:vehicle:mbdata:euda:* scope family is a substantive finding: Mercedes-Benz\n    has provisioned EU Data Act in-vehicle data categories as first-class OAuth scopes on its\n    production identity provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/scopes/mercedes-me-scopes.yml
summary_line: 38 scopes
tags:
- Automotive
- Connected Car
- Connected Vehicle
- Daimler
- Fleet Management
- Mercedes me
- Mercedes-Benz
- OEM
- Telematics
- Vehicle Data
token_urls: []
---
