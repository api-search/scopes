---
authorization_urls: []
description: ''
docs:
- https://docs.developer.comcast.com/docs/endpoints
- https://docs.developer.comcast.com/docs/170-core-capabilities
- https://docs.developer.comcast.com/docs/170-manage-usergrants
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Comcast Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Comcast uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Comcast
provider_slug: comcast
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: comcast-scopes
source_filename: comcast-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# Comcast — authorization scope model\n#\n# TWO SEPARATE AUTHORIZATION MODELS, recorded together because a consumer will\n# meet both:\n#\n#  1. SAT OAuth SCOPES. The Comcast SAT authorization server issues\n#     client_credentials tokens. Its discovery document publishes NO\n#     `scopes_supported` array, so the only scope strings on record are the two\n#     the provider prints in its own Open Ingest token-response example. They\n#     are recorded verbatim and nothing is inferred beyond them.\n#\n#  2. FIREBOLT CAPABILITIES. Firebolt does not use OAuth scopes. Every one of\n#     the 330 methods in the three OpenRPC contracts declares the capability\n#     URNs it uses, manages or provides, in the `capabilities` tag on the method\n#     itself. A capability is granted per-app and per-user through the UserGrants\n#     module, and the pattern is fixed by the contract:\n#     ^xrn:firebolt:capability:([a-z0-9-]+)((:[a-z0-9-]+)?)$\n#     Functionally this IS the permission\
  \ surface an integrator must reason\n#     about, so it is recorded here rather than left unwritten because it is not\n#     spelled \"scope\".\ngenerated: '2026-09-05'\nmethod: searched\nmethod_note: >-\n  derive-oauth-scopes.py reads OpenAPI oauth2 securitySchemes and found none\n  (Comcast publishes OpenRPC). The OAuth scopes below are read from the\n  provider's published token response; the capability list is derived\n  exhaustively from the three OpenRPC contracts in openrpc/.\nsource: >-\n  https://docs.developer.comcast.com/docs/endpoints (HTTP 200, 2026-09-05) and\n  openrpc/comcast-firebolt-{core,manage,discovery}-openrpc.json v1.7.0\ndocs:\n  - https://docs.developer.comcast.com/docs/endpoints\n  - https://docs.developer.comcast.com/docs/170-core-capabilities\n  - https://docs.developer.comcast.com/docs/170-manage-usergrants\nprovider: Comcast\nproviderId: comcast\noauth:\n  api: comcast:authentication-api\n  authorization_server: https://sat-prod.codebig2.net\n  scopes_supported_published:\
  \ false\n  scopes_supported_note: >-\n    The /.well-known/openid-configuration served by sat-prod.codebig2.net omits\n    scopes_supported entirely. There is no published scope catalogue.\n  scopes_observed_in_docs:\n    - name: x1:compass:piws:read\n      source: https://docs.developer.comcast.com/docs/endpoints\n      description: >-\n        Read scope returned in the documented SAT token response for the Open\n        Ingest / Compass PIWS surface. Comcast does not publish a definition\n        beyond the scope string itself.\n    - name: x1:compass:piws:write\n      source: https://docs.developer.comcast.com/docs/endpoints\n      description: >-\n        Write scope returned in the same documented SAT token response, and the\n        scope that authorizes POSTing an asset package to the Open Ingest proxy.\nfirebolt_capabilities:\n  scheme: firebolt-capability-urn\n  namespace_uri: https://meta.comcast.com/firebolt/capabilities\n  pattern: '^xrn:firebolt:capability:([a-z0-9\\-]+)((:[a-z0-9\\\
  -]+)?)$'\n  roles:\n    use: An app consumes the capability.\n    manage: An app changes the setting behind the capability (Manage SDK).\n    provide: An app implements the capability for the platform.\n  granted_through:\n    - Capabilities.info\n    - Capabilities.request\n    - UserGrants.grant\n    - UserGrants.deny\n    - UserGrants.app\n  deny_reasons_defined_in_contract: true\n  count: 62\n  capabilities:\n  - id: xrn:firebolt:capability:accessibility:audiodescriptions\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:accessibility:closedcaptions\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:accessibility:highcontrastui\n    roles: [use]\n  - id: xrn:firebolt:capability:accessibility:voiceguidance\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:account:id\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:account:uid\n    roles: [use]\n  - id: xrn:firebolt:capability:advertising:configuration\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:advertising:identifier\n\
  \    roles: [manage, use]\n  - id: xrn:firebolt:capability:advertising:policy\n    roles: [use]\n  - id: xrn:firebolt:capability:approve:content\n    roles: [use]\n  - id: xrn:firebolt:capability:approve:purchase\n    roles: [use]\n  - id: xrn:firebolt:capability:capabilities:info\n    roles: [use]\n  - id: xrn:firebolt:capability:capabilities:request\n    roles: [use]\n  - id: xrn:firebolt:capability:device:distributor\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:device:id\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:device:info\n    roles: [use]\n  - id: xrn:firebolt:capability:device:make\n    roles: [use]\n  - id: xrn:firebolt:capability:device:model\n    roles: [use]\n  - id: xrn:firebolt:capability:device:name\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:device:sku\n    roles: [use]\n  - id: xrn:firebolt:capability:device:uid\n    roles: [use]\n  - id: xrn:firebolt:capability:discovery:content-access\n    roles: [use]\n  - id: xrn:firebolt:capability:discovery:entity-info\n\
  \    roles: [provide]\n  - id: xrn:firebolt:capability:discovery:interest\n    roles: [provide, use]\n  - id: xrn:firebolt:capability:discovery:navigate-to\n    roles: [use]\n  - id: xrn:firebolt:capability:discovery:policy\n    roles: [use]\n  - id: xrn:firebolt:capability:discovery:purchased-content\n    roles: [provide]\n  - id: xrn:firebolt:capability:discovery:sign-in-status\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:discovery:watch-next\n    roles: [use]\n  - id: xrn:firebolt:capability:discovery:watched\n    roles: [use]\n  - id: xrn:firebolt:capability:grants:state\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:input:keyboard\n    roles: [provide, use]\n  - id: xrn:firebolt:capability:inputs:hdmi\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:lifecycle:initialize\n    roles: [use]\n  - id: xrn:firebolt:capability:lifecycle:launch\n    roles: [use]\n  - id: xrn:firebolt:capability:lifecycle:ready\n    roles: [use]\n  - id: xrn:firebolt:capability:lifecycle:state\n\
  \    roles: [use]\n  - id: xrn:firebolt:capability:localization:additional-info\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:localization:country-code\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:localization:language\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:localization:locale\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:localization:locality\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:localization:location\n    roles: [use]\n  - id: xrn:firebolt:capability:localization:postal-code\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:localization:time-zone\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:metrics:distributor\n    roles: [use]\n  - id: xrn:firebolt:capability:metrics:general\n    roles: [use]\n  - id: xrn:firebolt:capability:metrics:media\n    roles: [use]\n  - id: xrn:firebolt:capability:network:status\n    roles: [use]\n  - id: xrn:firebolt:capability:privacy:settings\n    roles:\
  \ [manage, use]\n  - id: xrn:firebolt:capability:profile:flags\n    roles: [use]\n  - id: xrn:firebolt:capability:protocol:dial\n    roles: [use]\n  - id: xrn:firebolt:capability:protocol:wifi\n    roles: [use]\n  - id: xrn:firebolt:capability:secondscreen:protocol\n    roles: [use]\n  - id: xrn:firebolt:capability:storage:secure\n    roles: [manage, use]\n  - id: xrn:firebolt:capability:token:account\n    roles: [manage]\n  - id: xrn:firebolt:capability:token:device\n    roles: [use]\n  - id: xrn:firebolt:capability:token:platform\n    roles: [use]\n  - id: xrn:firebolt:capability:token:root\n    roles: [use]\n  - id: xrn:firebolt:capability:token:session\n    roles: [use]\n  - id: xrn:firebolt:capability:usergrant:acknowledgechallenge\n    roles: [provide]\n  - id: xrn:firebolt:capability:usergrant:pinchallenge\n    roles: [provide]\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comcast/refs/heads/main/scopes/comcast-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Cable
- Connected Devices
- Entertainment
- Internet
- Media
- Mobile
- Streaming
- Wireless
- Fortune 100
token_urls: []
---
