---
api_specs:
- filename: home-connect-appliances-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Appliances API
  slug: home-connect-appliances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-appliances-api-openapi.yml
- filename: home-connect-commands-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Commands API
  slug: home-connect-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-commands-api-openapi.yml
- filename: home-connect-events-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Events API
  slug: home-connect-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-events-api-openapi.yml
- filename: home-connect-images-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Images API
  slug: home-connect-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-images-api-openapi.yml
- filename: home-connect-map-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Map API
  slug: home-connect-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-map-api-openapi.yml
- filename: home-connect-programs-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Programs API
  slug: home-connect-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-programs-api-openapi.yml
- filename: home-connect-settings-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Settings API
  slug: home-connect-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-settings-api-openapi.yml
- filename: home-connect-status-api-openapi.yml
  format: yaml
  label: Home Connect (BSH appliances) Status API
  slug: home-connect-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/home-connect/openapi/home-connect-status-api-openapi.yml
authorization_urls:
- https://api.home-connect.com/security/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Home Connect Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Home Connect (BSH appliances) publishes 63 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Home Connect (BSH appliances) API on a user''s behalf.


  Tokens are issued from https://api.home-connect.com/security/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Home Connect (BSH appliances)
provider_slug: home-connect
schemes:
- description: 'The Home Connect API uses the authorization code grant flow of the OAuth2

    Authorization Framework as specified in RFC 6749 (https://tools.ietf.org/html/rfc6749).

    Authorization tokens have to be transmitted in the HTTP headers as defined

    in RFC 6750 (https://tools.ietf.org/html/rfc6750).'
  flows:
  - authorizationUrl: https://api.home-connect.com/security/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.home-connect.com/security/oauth/token
  name: homeconnect_auth
  source: openapi/home-connect-openapi.yaml
scope_count: 63
scope_names:
- CleaningRobot
- CleaningRobot-Control
- CleaningRobot-Map
- CleaningRobot-Monitor
- CleaningRobot-Settings
- CoffeeMaker
- CoffeeMaker-Control
- CoffeeMaker-Monitor
- CoffeeMaker-Settings
- Control
- CookProcessor
- CookProcessor-Control
- CookProcessor-Monitor
- CookProcessor-Settings
- Dishwasher
- Dishwasher-Control
- Dishwasher-Monitor
- Dishwasher-Settings
- Dryer
- Dryer-Control
- Dryer-Monitor
- Dryer-Settings
- Freezer
- Freezer-Control
- Freezer-Monitor
- Freezer-Settings
- FridgeFreezer
- FridgeFreezer-Control
- FridgeFreezer-Images
- FridgeFreezer-Monitor
- FridgeFreezer-Settings
- Hob
- Hob-Control
- Hob-Monitor
- Hob-Settings
- Hood
- Hood-Control
- Hood-Monitor
- Hood-Settings
- IdentifyAppliance
- Images
- Monitor
- Oven
- Oven-Control
- Oven-Monitor
- Oven-Settings
- Refrigerator
- Refrigerator-Control
- Refrigerator-Monitor
- Refrigerator-Settings
- Settings
- Washer
- Washer-Control
- Washer-Monitor
- Washer-Settings
- WasherDryer
- WasherDryer-Control
- WasherDryer-Monitor
- WasherDryer-Settings
- WineCooler
- WineCooler-Control
- WineCooler-Monitor
- WineCooler-Settings
scopes:
- description: Grants access to read or modify all resources under /api/homeappliances on cleaning robots
  flows:
  - authorizationCode
  scope: CleaningRobot
- description: Grants access to modify resources under under /api/homeappliances except images and settings on cleaning robots
  flows:
  - authorizationCode
  scope: CleaningRobot-Control
- description: Grants access to read resources under /api/homeappliances/{haId}/map on cleaning robots
  flows:
  - authorizationCode
  scope: CleaningRobot-Map
- description: Grants access to read resources under /api/homeappliances except images and settings on cleaning robots
  flows:
  - authorizationCode
  scope: CleaningRobot-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on cleaning robots
  flows:
  - authorizationCode
  scope: CleaningRobot-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on coffee makers
  flows:
  - authorizationCode
  scope: CoffeeMaker
- description: Grants access to modify resources under under /api/homeappliances except images and settings on coffee makers
  flows:
  - authorizationCode
  scope: CoffeeMaker-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on coffee makers
  flows:
  - authorizationCode
  scope: CoffeeMaker-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on coffee makers
  flows:
  - authorizationCode
  scope: CoffeeMaker-Settings
- description: Grants access to modify resources under under /api/homeappliances except images and settings
  flows:
  - authorizationCode
  scope: Control
- description: Grants access to read or modify all resources under /api/homeappliances on cookprocessors
  flows:
  - authorizationCode
  scope: CookProcessor
- description: Grants access to modify resources under under /api/homeappliances except images and settings on cookprocessors
  flows:
  - authorizationCode
  scope: CookProcessor-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on cookprocessors
  flows:
  - authorizationCode
  scope: CookProcessor-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on cookprocessors
  flows:
  - authorizationCode
  scope: CookProcessor-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on dishwashers
  flows:
  - authorizationCode
  scope: Dishwasher
- description: Grants access to modify resources under under /api/homeappliances except images and settings on dishwashers
  flows:
  - authorizationCode
  scope: Dishwasher-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on dishwashers
  flows:
  - authorizationCode
  scope: Dishwasher-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on dishwashers
  flows:
  - authorizationCode
  scope: Dishwasher-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on dryers
  flows:
  - authorizationCode
  scope: Dryer
- description: Grants access to modify resources under under /api/homeappliances except images and settings on dryers
  flows:
  - authorizationCode
  scope: Dryer-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on dryers
  flows:
  - authorizationCode
  scope: Dryer-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on dryers
  flows:
  - authorizationCode
  scope: Dryer-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on freezers
  flows:
  - authorizationCode
  scope: Freezer
- description: Grants access to modify resources under under /api/homeappliances except images and settings on freezers
  flows:
  - authorizationCode
  scope: Freezer-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on freezers
  flows:
  - authorizationCode
  scope: Freezer-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on freezers
  flows:
  - authorizationCode
  scope: Freezer-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on fridgefreezers
  flows:
  - authorizationCode
  scope: FridgeFreezer
- description: Grants access to modify resources under /api/homeappliances except images and settings on fridgefreezers
  flows:
  - authorizationCode
  scope: FridgeFreezer-Control
- description: Grants access to read resources under /api/homeappliances/{haId}/images on fridgefreezers
  flows:
  - authorizationCode
  scope: FridgeFreezer-Images
- description: Grants access to read resources under /api/homeappliances except images and settings on fridgefreezers
  flows:
  - authorizationCode
  scope: FridgeFreezer-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on fridgefreezers
  flows:
  - authorizationCode
  scope: FridgeFreezer-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on hobs
  flows:
  - authorizationCode
  scope: Hob
- description: Grants access to modify resources under under /api/homeappliances except images and settings on hobs
  flows:
  - authorizationCode
  scope: Hob-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on hobs
  flows:
  - authorizationCode
  scope: Hob-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on hobs
  flows:
  - authorizationCode
  scope: Hob-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on hoods
  flows:
  - authorizationCode
  scope: Hood
- description: Grants access to modify resources under under /api/homeappliances except images and settings on hoods
  flows:
  - authorizationCode
  scope: Hood-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on hoods
  flows:
  - authorizationCode
  scope: Hood-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on hoods
  flows:
  - authorizationCode
  scope: Hood-Settings
- description: Grants right to identify a home appliance under /api/homeappliances
  flows:
  - authorizationCode
  scope: IdentifyAppliance
- description: Grants access to read resources under /api/homeappliances/{haId}/images
  flows:
  - authorizationCode
  scope: Images
- description: Grants access to read resources under /api/homeappliances except images and settings
  flows:
  - authorizationCode
  scope: Monitor
- description: Grants access to read or modify all resources under /api/homeappliances on ovens
  flows:
  - authorizationCode
  scope: Oven
- description: Grants access to modify resources under under /api/homeappliances except images and settings on ovens
  flows:
  - authorizationCode
  scope: Oven-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on ovens
  flows:
  - authorizationCode
  scope: Oven-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on ovens
  flows:
  - authorizationCode
  scope: Oven-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on refrigerators
  flows:
  - authorizationCode
  scope: Refrigerator
- description: Grants access to modify resources under under /api/homeappliances except images and settings on refrigerators
  flows:
  - authorizationCode
  scope: Refrigerator-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on refrigerators
  flows:
  - authorizationCode
  scope: Refrigerator-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on refrigerators
  flows:
  - authorizationCode
  scope: Refrigerator-Settings
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings
  flows:
  - authorizationCode
  scope: Settings
- description: Grants access to read or modify all resources under /api/homeappliances on washers
  flows:
  - authorizationCode
  scope: Washer
- description: Grants access to modify resources under under /api/homeappliances except images and settings on washers
  flows:
  - authorizationCode
  scope: Washer-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on washers
  flows:
  - authorizationCode
  scope: Washer-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on washers
  flows:
  - authorizationCode
  scope: Washer-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on washerdryers
  flows:
  - authorizationCode
  scope: WasherDryer
- description: Grants access to modify resources under under /api/homeappliances except images and settings on washerdryers
  flows:
  - authorizationCode
  scope: WasherDryer-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on washerdryers
  flows:
  - authorizationCode
  scope: WasherDryer-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on washerdryers
  flows:
  - authorizationCode
  scope: WasherDryer-Settings
- description: Grants access to read or modify all resources under /api/homeappliances on wine coolers
  flows:
  - authorizationCode
  scope: WineCooler
- description: Grants access to modify resources under under /api/homeappliances except images and settings on wine coolers
  flows:
  - authorizationCode
  scope: WineCooler-Control
- description: Grants access to read resources under /api/homeappliances except images and settings on wine coolers
  flows:
  - authorizationCode
  scope: WineCooler-Monitor
- description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings on wine coolers
  flows:
  - authorizationCode
  scope: WineCooler-Settings
slug: home-connect-scopes
source_filename: home-connect-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/home-connect-openapi.yaml\nschemes:\n- name: homeconnect_auth\n  source: openapi/home-connect-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.home-connect.com/security/oauth/authorize\n    tokenUrl: https://api.home-connect.com/security/oauth/token\n  description: |-\n    The Home Connect API uses the authorization code grant flow of the OAuth2\n    Authorization Framework as specified in RFC 6749 (https://tools.ietf.org/html/rfc6749).\n    Authorization tokens have to be transmitted in the HTTP headers as defined\n    in RFC 6750 (https://tools.ietf.org/html/rfc6750).\nscopes:\n- scope: CleaningRobot\n  description: Grants access to read or modify all resources under /api/homeappliances on cleaning\n    robots\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CleaningRobot-Control\n  description: Grants access to modify resources under\
  \ under /api/homeappliances except images\n    and settings on cleaning robots\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CleaningRobot-Map\n  description: Grants access to read resources under /api/homeappliances/{haId}/map on cleaning\n    robots\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CleaningRobot-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on cleaning robots\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CleaningRobot-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on cleaning robots\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CoffeeMaker\n  description: Grants access to read or modify all resources under /api/homeappliances on coffee\n    makers\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CoffeeMaker-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on coffee makers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CoffeeMaker-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on coffee makers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CoffeeMaker-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on coffee makers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n\
  - scope: CookProcessor\n  description: Grants access to read or modify all resources under /api/homeappliances on cookprocessors\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CookProcessor-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on cookprocessors\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CookProcessor-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on cookprocessors\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: CookProcessor-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on cookprocessors\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Dishwasher\n  description: Grants access to read\
  \ or modify all resources under /api/homeappliances on dishwashers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Dishwasher-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on dishwashers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Dishwasher-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on dishwashers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Dishwasher-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on dishwashers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Dryer\n  description: Grants access to read or modify all resources under /api/homeappliances on dryers\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Dryer-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on dryers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Dryer-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on dryers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Dryer-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on dryers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Freezer\n  description: Grants access to read or modify all resources under /api/homeappliances on freezers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Freezer-Control\n  description: Grants access to modify\
  \ resources under under /api/homeappliances except images\n    and settings on freezers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Freezer-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on freezers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Freezer-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on freezers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: FridgeFreezer\n  description: Grants access to read or modify all resources under /api/homeappliances on fridgefreezers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: FridgeFreezer-Control\n  description: Grants access to modify resources under /api/homeappliances except images and\n    settings on fridgefreezers\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: FridgeFreezer-Images\n  description: Grants access to read resources under /api/homeappliances/{haId}/images on fridgefreezers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: FridgeFreezer-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on fridgefreezers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: FridgeFreezer-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on fridgefreezers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Hob\n  description: Grants access to read or modify all resources under /api/homeappliances on hobs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Hob-Control\n\
  \  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on hobs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Hob-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on hobs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Hob-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on hobs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Hood\n  description: Grants access to read or modify all resources under /api/homeappliances on hoods\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Hood-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on hoods\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Hood-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on hoods\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Hood-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on hoods\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: IdentifyAppliance\n  description: Grants right to identify a home appliance under /api/homeappliances\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Images\n  description: Grants access to read resources under /api/homeappliances/{haId}/images\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Monitor\n  description: Grants access to read resources under /api/homeappliances except\
  \ images and settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Oven\n  description: Grants access to read or modify all resources under /api/homeappliances on ovens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Oven-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on ovens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Oven-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on ovens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Oven-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on ovens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Refrigerator\n\
  \  description: Grants access to read or modify all resources under /api/homeappliances on refrigerators\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Refrigerator-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on refrigerators\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Refrigerator-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on refrigerators\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Refrigerator-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on refrigerators\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Washer\n  description: Grants access to read or modify all resources under /api/homeappliances on washers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Washer-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on washers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Washer-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on washers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: Washer-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on washers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: WasherDryer\n  description:\
  \ Grants access to read or modify all resources under /api/homeappliances on washerdryers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: WasherDryer-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on washerdryers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: WasherDryer-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on washerdryers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: WasherDryer-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on washerdryers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: WineCooler\n  description: Grants access to read or modify all resources under /api/homeappliances\
  \ on wine\n    coolers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: WineCooler-Control\n  description: Grants access to modify resources under under /api/homeappliances except images\n    and settings on wine coolers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: WineCooler-Monitor\n  description: Grants access to read resources under /api/homeappliances except images and settings\n    on wine coolers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n- scope: WineCooler-Settings\n  description: Grants access to read and modify resources under /api/homeappliances/{haId}/settings\n    on wine coolers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/home-connect-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/home-connect/scopes/home-connect-scopes.yml
summary_line: 63 scopes · authorizationCode
tags:
- smart home
- appliances
- connected devices
token_bound: false
token_urls:
- https://api.home-connect.com/security/oauth/token
---
