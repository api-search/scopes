---
api_specs:
- filename: stellantis-grouping-api-openapi.yml
  format: yaml
  label: Stellantis Grouping API
  slug: stellantis-grouping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-grouping-api-openapi.yml
- filename: stellantis-data-stream-api-openapi.yml
  format: yaml
  label: Stellantis Data Stream API
  slug: stellantis-data-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-data-stream-api-openapi.yml
- filename: stellantis-auth-api-openapi.yml
  format: yaml
  label: Stellantis Auth API
  slug: stellantis-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-auth-api-openapi.yml
- filename: stellantis-bugs-api-openapi.yml
  format: yaml
  label: Stellantis Bugs API
  slug: stellantis-bugs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-bugs-api-openapi.yml
- filename: stellantis-cloud-data-treatment-api-openapi.yml
  format: yaml
  label: Stellantis Vehicles API
  slug: stellantis-cloud-data-treatment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-cloud-data-treatment-api-openapi.yml
- filename: stellantis-cloud-docg-device-management-api-openapi.yml
  format: yaml
  label: Stellantis Cloud Docg Device Management API
  slug: stellantis-cloud-docg-device-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-cloud-docg-device-management-api-openapi.yml
- filename: stellantis-cloud-notification-center-api-openapi.yml
  format: yaml
  label: Stellantis Cloud Notification Center API
  slug: stellantis-cloud-notification-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-cloud-notification-center-api-openapi.yml
- filename: stellantis-connected-car-b2b-api-openapi.yml
  format: yaml
  label: Stellantis Capabilities API
  slug: stellantis-connected-car-b2b-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-connected-car-b2b-api-openapi.yml
- filename: stellantis-connected-car-b2c-api-openapi.yml
  format: yaml
  label: Stellantis Connected Car B2C API
  slug: stellantis-connected-car-b2c-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-connected-car-b2c-api-openapi.yml
- filename: stellantis-data-api-openapi.yml
  format: yaml
  label: Stellantis Data API
  slug: stellantis-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-data-api-openapi.yml
- filename: stellantis-feedback-api-openapi.yml
  format: yaml
  label: Stellantis Feedback API
  slug: stellantis-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-feedback-api-openapi.yml
- filename: stellantis-geofence-breaches-api-openapi.yml
  format: yaml
  label: Stellantis Geofence Breaches API
  slug: stellantis-geofence-breaches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-geofence-breaches-api-openapi.yml
- filename: stellantis-geofence-collection-api-openapi.yml
  format: yaml
  label: Stellantis Geofence Collection API
  slug: stellantis-geofence-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-geofence-collection-api-openapi.yml
- filename: stellantis-geofencing-notifications-api-openapi.yml
  format: yaml
  label: Stellantis Geofencing Notifications API
  slug: stellantis-geofencing-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-geofencing-notifications-api-openapi.yml
- filename: stellantis-hackathon-register-api-openapi.yml
  format: yaml
  label: Stellantis Hackathon Register API
  slug: stellantis-hackathon-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-hackathon-register-api-openapi.yml
- filename: stellantis-hackathon-unsubscribe-api-openapi.yml
  format: yaml
  label: Stellantis Hackathon Unsubscribe API
  slug: stellantis-hackathon-unsubscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-hackathon-unsubscribe-api-openapi.yml
- filename: stellantis-popup-api-openapi.yml
  format: yaml
  label: Stellantis Popup API
  slug: stellantis-popup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-popup-api-openapi.yml
- filename: stellantis-remote-api-openapi.yml
  format: yaml
  label: Stellantis Remote API
  slug: stellantis-remote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-remote-api-openapi.yml
- filename: stellantis-stream-api-openapi.yml
  format: yaml
  label: Stellantis Stream API
  slug: stellantis-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stellantis/openapi/stellantis-stream-api-openapi.yml
authorization_urls:
- https://api.mpsa.com/api/connectedcar/v2/oauth/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Stellantis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Stellantis publishes 53 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Stellantis API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stellantis
provider_slug: stellantis
schemes:
- description: This API uses OAuth 2 with the implicit grant flow. [More info](https://api.example.com/docs/auth)
  flows:
  - authorizationUrl: https://api.mpsa.com/api/connectedcar/v2/oauth/authorize
    flow: implicit
  name: api_oauth
  source: openapi/stellantis-cloud-data-treatment-api-openapi.yml
- description: This API uses OAuth 2 with the implicit grant flow. [More info](https://api.example.com/docs/auth)
  flows:
  - authorizationUrl: https://api.mpsa.com/api/connectedcar/v2/oauth/authorize
    flow: implicit
  name: api_oauth
  source: openapi/stellantis-connected-car-b2c-api-openapi.yml
scope_count: 53
scope_names:
- channel
- channel:write
- data:alert
- data:collision
- data:position
- data:telemetry
- data:telemetry:environment
- data:telemetry:privacy
- data:telemetry:vehicle
- data:telemetry:vehicle:adas
- data:telemetry:vehicle:alarm
- data:telemetry:vehicle:alert
- data:telemetry:vehicle:battery
- data:telemetry:vehicle:braking
- data:telemetry:vehicle:doorsState
- data:telemetry:vehicle:drivingBehavior
- data:telemetry:vehicle:energies
- data:telemetry:vehicle:engines
- data:telemetry:vehicle:ignition
- data:telemetry:vehicle:kinetic
- data:telemetry:vehicle:lightingSystem
- data:telemetry:vehicle:location
- data:telemetry:vehicle:maintenance
- data:telemetry:vehicle:odometer
- data:telemetry:vehicle:preconditioning
- data:telemetry:vehicle:propulsion
- data:telemetry:vehicle:safety
- data:telemetry:vehicle:transmission
- data:telemetry:vehicle:tyreState
- data:telemetry:vehicle:wipingBlades
- data:trip
- data:vehicle
- data:vehicle:devices:pnc
- monitor
- monitor:write
- remote
- remote:charging
- remote:charging:write
- remote:door:write
- remote:horn
- remote:horn:write
- remote:lights
- remote:lights:write
- remote:locking
- remote:locking:write
- remote:navigation:write
- remote:onboardPersonalData
- remote:onboardPersonalData:write
- remote:preconditioning
- remote:preconditioning:write
- remote:wakeUp
- remote:wakeUp:write
- remote:wakeup:write
scopes:
- description: read calback related data
  flows:
  - implicit
  scope: channel
- description: create, modify or delete channels
  flows:
  - implicit
  scope: channel:write
- description: Read alert related data
  flows:
  - implicit
  scope: data:alert
- description: read Collision related data
  flows:
  - implicit
  scope: data:collision
- description: Read vehicle Location (position) data
  flows:
  - implicit
  scope: data:position
- description: read full telemetry data
  flows:
  - implicit
  scope: data:telemetry
- description: read telemetry environment data
  flows:
  - implicit
  scope: data:telemetry:environment
- description: read telemetry privacy data
  flows:
  - implicit
  scope: data:telemetry:privacy
- description: read full telemetry vehicle data
  flows:
  - implicit
  scope: data:telemetry:vehicle
- description: read telemetry vehicle ADAS data
  flows:
  - implicit
  scope: data:telemetry:vehicle:adas
- description: read telemetry alarm data
  flows:
  - implicit
  scope: data:telemetry:vehicle:alarm
- description: read telemetry alert data
  flows:
  - implicit
  scope: data:telemetry:vehicle:alert
- description: read telemetry vehicle battery status data
  flows:
  - implicit
  scope: data:telemetry:vehicle:battery
- description: read telemetry vehicle braking system data
  flows:
  - implicit
  scope: data:telemetry:vehicle:braking
- description: read telemetry vehicle doors state data
  flows:
  - implicit
  scope: data:telemetry:vehicle:doorsState
- description: read telemetry vehicle driver bihavior data
  flows:
  - implicit
  scope: data:telemetry:vehicle:drivingBehavior
- description: read telemetry vehicle energies data
  flows:
  - implicit
  scope: data:telemetry:vehicle:energies
- description: read telemetry vehicle engines data
  flows:
  - implicit
  scope: data:telemetry:vehicle:engines
- description: read telemetry vehicle ignition data
  flows:
  - implicit
  scope: data:telemetry:vehicle:ignition
- description: read telemetry vehicle kinetic data
  flows:
  - implicit
  scope: data:telemetry:vehicle:kinetic
- description: read telemetry vehicle lighting system data
  flows:
  - implicit
  scope: data:telemetry:vehicle:lightingSystem
- description: read vehicle location data
  flows:
  - implicit
  scope: data:telemetry:vehicle:location
- description: read telemetry vehicle maintenance data
  flows:
  - implicit
  scope: data:telemetry:vehicle:maintenance
- description: read telemetry vehicle odometer data
  flows:
  - implicit
  scope: data:telemetry:vehicle:odometer
- description: read telemetry vehicle preconditioning system data
  flows:
  - implicit
  scope: data:telemetry:vehicle:preconditioning
- description: read telemetry vehicle propulsion mode
  flows:
  - implicit
  scope: data:telemetry:vehicle:propulsion
- description: read telemetry vehicle safety data
  flows:
  - implicit
  scope: data:telemetry:vehicle:safety
- description: read telemetry vehicle transmission data
  flows:
  - implicit
  scope: data:telemetry:vehicle:transmission
- description: read telemetry vehicle tyre data
  flows:
  - implicit
  scope: data:telemetry:vehicle:tyreState
- description: read telemetry vehicle wiping blades data
  flows:
  - implicit
  scope: data:telemetry:vehicle:wipingBlades
- description: read Trip related data
  flows:
  - implicit
  scope: data:trip
- description: read vehicle attributes data
  flows:
  - implicit
  scope: data:vehicle
- description: ''
  flows: []
  scope: data:vehicle:devices:pnc
- description: read monitors
  flows:
  - implicit
  scope: monitor
- description: create, modify or delete Monitors
  flows:
  - implicit
  scope: monitor:write
- description: read full remote state(pending & history)
  flows:
  - implicit
  scope: remote
- description: read charging remote (pending & history)
  flows:
  - implicit
  scope: remote:charging
- description: send charging remote to vehicle
  flows:
  - implicit
  scope: remote:charging:write
- description: Read & send door remote (pending & history)
  flows:
  - implicit
  scope: remote:door:write
- description: read horn remote (pending & history)
  flows:
  - implicit
  scope: remote:horn
- description: send a horn remote to vehicle
  flows:
  - implicit
  scope: remote:horn:write
- description: read lights remote (pending & history)
  flows:
  - implicit
  scope: remote:lights
- description: send remote to switch on/off vehicle lights
  flows:
  - implicit
  scope: remote:lights:write
- description: read door remote (pending & history)
  flows:
  - implicit
  scope: remote:locking
- description: send a door remote to vehicle
  flows:
  - implicit
  scope: remote:locking:write
- description: Read & send navigation remote (pending & history)
  flows:
  - implicit
  scope: remote:navigation:write
- description: read onboardPersonalData remote (pending & history)
  flows:
  - implicit
  scope: remote:onboardPersonalData
- description: send an onboardPersonalData remote to vehicle
  flows:
  - implicit
  scope: remote:onboardPersonalData:write
- description: read preconditioning remote (pending & history)
  flows:
  - implicit
  scope: remote:preconditioning
- description: send a preconditioning remote to vehicle
  flows:
  - implicit
  scope: remote:preconditioning:write
- description: read wakeUp remote (pending & history)
  flows:
  - implicit
  scope: remote:wakeUp
- description: send remote to wakeUp vehicle
  flows:
  - implicit
  scope: remote:wakeUp:write
- description: Read & send weackup remote (pending & history)
  flows:
  - implicit
  scope: remote:wakeup:write
slug: stellantis-scopes
source_filename: stellantis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/stellantis-cloud-data-treatment-api-openapi.yml, openapi/stellantis-connected-car-b2c-api-openapi.yml\nschemes:\n- name: api_oauth\n  source: openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.mpsa.com/api/connectedcar/v2/oauth/authorize\n  description: This API uses OAuth 2 with the implicit grant flow. [More info](https://api.example.com/docs/auth)\n- name: api_oauth\n  source: openapi/stellantis-connected-car-b2c-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.mpsa.com/api/connectedcar/v2/oauth/authorize\n  description: This API uses OAuth 2 with the implicit grant flow. [More info](https://api.example.com/docs/auth)\nscopes:\n- scope: channel\n  description: read calback related data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: channel:write\n  description:\
  \ create, modify or delete channels\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:alert\n  description: Read alert related data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: data:collision\n  description: read Collision related data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: data:position\n  description: Read vehicle Location (position) data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: data:telemetry\n  description: read full telemetry data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: data:telemetry:environment\n  description: read telemetry environment data\n  flows:\n\
  \  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:privacy\n  description: read telemetry privacy data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle\n  description: read full telemetry vehicle data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:adas\n  description: read telemetry vehicle ADAS data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:alarm\n  description: read telemetry alarm data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:alert\n  description: read telemetry alert data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:battery\n\
  \  description: read telemetry vehicle battery status data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:braking\n  description: read telemetry vehicle braking system data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:doorsState\n  description: read telemetry vehicle doors state data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:drivingBehavior\n  description: read telemetry vehicle driver bihavior data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:energies\n  description: read telemetry vehicle energies data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:engines\n  description:\
  \ read telemetry vehicle engines data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:ignition\n  description: read telemetry vehicle ignition data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:kinetic\n  description: read telemetry vehicle kinetic data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:lightingSystem\n  description: read telemetry vehicle lighting system data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:location\n  description: read vehicle location data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:maintenance\n  description: read telemetry vehicle maintenance\
  \ data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:odometer\n  description: read telemetry vehicle odometer data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:preconditioning\n  description: read telemetry vehicle preconditioning system data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:propulsion\n  description: read telemetry vehicle propulsion mode\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:safety\n  description: read telemetry vehicle safety data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:transmission\n  description: read telemetry vehicle transmission data\n  flows:\n\
  \  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:tyreState\n  description: read telemetry vehicle tyre data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:telemetry:vehicle:wipingBlades\n  description: read telemetry vehicle wiping blades data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:trip\n  description: read Trip related data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: data:vehicle\n  description: read vehicle attributes data\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: data:vehicle:devices:pnc\n  sources:\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: monitor\n  description: read\
  \ monitors\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: monitor:write\n  description: create, modify or delete Monitors\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote\n  description: read full remote state(pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:charging\n  description: read charging remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:charging:write\n  description: send charging remote to vehicle\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: remote:door:write\n  description: Read & send door remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n\
  - scope: remote:horn\n  description: read horn remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:horn:write\n  description: send a horn remote to vehicle\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: remote:lights\n  description: read lights remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:lights:write\n  description: send remote to switch on/off vehicle lights\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: remote:locking\n  description: read door  remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n-\
  \ scope: remote:locking:write\n  description: send a door remote to vehicle\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:navigation:write\n  description: Read & send navigation remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: remote:onboardPersonalData\n  description: read onboardPersonalData remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:onboardPersonalData:write\n  description: send an onboardPersonalData remote to vehicle\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:preconditioning\n  description: read preconditioning remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:preconditioning:write\n\
  \  description: send a preconditioning remote to vehicle\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n- scope: remote:wakeUp\n  description: read wakeUp remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:wakeUp:write\n  description: send remote to wakeUp vehicle\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-cloud-data-treatment-api-openapi.yml\n- scope: remote:wakeup:write\n  description: Read & send weackup remote (pending & history)\n  flows:\n  - implicit\n  sources:\n  - openapi/stellantis-connected-car-b2c-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/stellantis/scopes/stellantis-scopes.yml
summary_line: 53 scopes · implicit
tags:
- Company
- Automotive
- Manufacturing
- Mobility
- Sustainability
token_bound: false
token_urls: []
---
