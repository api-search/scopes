---
api_specs:
- filename: angelcam-openapi-original.yml
  format: yaml
  label: Angelcam API
  slug: angelcam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/angelcam/refs/heads/main/openapi/angelcam-openapi-original.yml
authorization_urls:
- https://my.angelcam.com/oauth/authorize/
description: ''
docs: https://developers.angelcam.com/guides/authentication/
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: searched
name: Angelcam Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AngelCam publishes 51 OAuth 2.0 scopes via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AngelCam API on a user''s behalf.


  Tokens are issued from https://my.angelcam.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AngelCam
provider_slug: angelcam
schemes:
- description: See the Authentication section above for full documentation.
  flows:
  - authorizationUrl: https://my.angelcam.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://my.angelcam.com/oauth/token/
  - flow: password
    tokenUrl: https://api.angelcam.com/oauth/token/
  name: OAuth2
  source: openapi/angelcam-openapi-original.yml
scope_count: 51
scope_names:
- active_services_access
- active_services_manage
- arrow_client_access
- arrow_client_manage
- audio_message_access
- audio_message_manage
- audio_messages_play
- broadcasting_access
- broadcasting_start_stop
- camera_access
- camera_create
- camera_delete
- camera_guest_access
- camera_guest_manage
- camera_manage
- client_access
- client_create
- client_manage
- event_access
- incidents_access
- locations_access
- messages_access
- messages_manage
- notifications_methods_access
- notifications_methods_manage
- notifications_rules_access
- notifications_rules_manage
- orders_access
- public_cameras_access
- recording_access
- recording_clips_access
- recording_clips_create
- recording_clips_share
- recording_start_stop
- rts_arming_manage
- rts_settings_access
- rts_settings_manage
- sensor_access
- sensor_manage
- services_access
- sites_access
- sites_manage
- space_access
- space_permissions_access
- speaker_access
- speaker_manage
- streams_detect
- trials_access
- trials_activate
- user_access
- user_delete
scopes:
- description: Permission to access active services
  flows:
  - authorizationCode
  - password
  scope: active_services_access
- description: Permission to manage active services
  flows:
  - authorizationCode
  - password
  scope: active_services_manage
- description: Permission to access Arrow clients
  flows:
  - authorizationCode
  - password
  scope: arrow_client_access
- description: Permission to manage Arrow clients
  flows:
  - authorizationCode
  - password
  scope: arrow_client_manage
- description: ''
  flows: []
  scope: audio_message_access
- description: ''
  flows: []
  scope: audio_message_manage
- description: ''
  flows: []
  scope: audio_messages_play
- description: Permission to see general broadcasting information and access broadcasting streams
  flows:
  - authorizationCode
  - password
  scope: broadcasting_access
- description: Permission to start and stop public broadcasting on camera
  flows:
  - authorizationCode
  - password
  scope: broadcasting_start_stop
- description: Permission to list cameras and to get details of a specific camera
  flows:
  - authorizationCode
  - password
  scope: camera_access
- description: Permission to create cameras
  flows:
  - authorizationCode
  - password
  scope: camera_create
- description: Permission to delete cameras
  flows:
  - authorizationCode
  - password
  scope: camera_delete
- description: Permission to access camera guest
  flows:
  - authorizationCode
  - password
  scope: camera_guest_access
- description: Permission to manage camera guest
  flows:
  - authorizationCode
  - password
  scope: camera_guest_manage
- description: Permission to update cameras
  flows:
  - authorizationCode
  - password
  scope: camera_manage
- description: Permission to list resellers clients and get details of a specific client
  flows:
  - authorizationCode
  - password
  scope: client_access
- description: Permission to create client account
  flows:
  - authorizationCode
  - password
  scope: client_create
- description: Permission to update clients detail
  flows:
  - authorizationCode
  - password
  scope: client_manage
- description: Permission to access events
  flows:
  - authorizationCode
  - password
  scope: event_access
- description: Permission to access Incidents
  flows:
  - authorizationCode
  - password
  scope: incidents_access
- description: ''
  flows: []
  scope: locations_access
- description: Permission to access RTS messages
  flows:
  - authorizationCode
  - password
  scope: messages_access
- description: Permission to manage RTS messages
  flows:
  - authorizationCode
  - password
  scope: messages_manage
- description: ''
  flows: []
  scope: notifications_methods_access
- description: ''
  flows: []
  scope: notifications_methods_manage
- description: ''
  flows: []
  scope: notifications_rules_access
- description: ''
  flows: []
  scope: notifications_rules_manage
- description: Permission to access orders
  flows:
  - authorizationCode
  - password
  scope: orders_access
- description: Permission to access public cameras
  flows:
  - authorizationCode
  scope: public_cameras_access
- description: Permission to access camera recordings
  flows:
  - authorizationCode
  - password
  scope: recording_access
- description: Permission to access recording clips
  flows:
  - authorizationCode
  - password
  scope: recording_clips_access
- description: Permission to create recording clips
  flows:
  - authorizationCode
  - password
  scope: recording_clips_create
- description: Permission to share recording clips
  flows:
  - authorizationCode
  - password
  scope: recording_clips_share
- description: Permission to start and stop recording on camera
  flows:
  - authorizationCode
  - password
  scope: recording_start_stop
- description: Permission to arm and disarm RTS
  flows:
  - password
  scope: rts_arming_manage
- description: Permission to access RTS settings
  flows:
  - password
  scope: rts_settings_access
- description: Permission to manage RTS settings
  flows:
  - password
  scope: rts_settings_manage
- description: Permission to list sensors and to get details of a specific sensor
  flows:
  - authorizationCode
  - password
  scope: sensor_access
- description: Permission to create, update and delete sensors
  flows:
  - authorizationCode
  - password
  scope: sensor_manage
- description: Permission to access available services
  flows:
  - authorizationCode
  - password
  scope: services_access
- description: Permission to access sites
  flows:
  - authorizationCode
  - password
  scope: sites_access
- description: Permission to create, update and delete sites
  flows:
  - authorizationCode
  - password
  scope: sites_manage
- description: Permission to list and activate spaces
  flows:
  - authorizationCode
  - password
  scope: space_access
- description: Permission to view space permissions
  flows:
  - authorizationCode
  - password
  scope: space_permissions_access
- description: ''
  flows: []
  scope: speaker_access
- description: ''
  flows: []
  scope: speaker_manage
- description: Permission to detect camera streams
  flows:
  - authorizationCode
  - password
  scope: streams_detect
- description: Permission to access available trials
  flows:
  - authorizationCode
  - password
  scope: trials_access
- description: Permission to activate a trial
  flows:
  - authorizationCode
  - password
  scope: trials_activate
- description: Permission to access user information
  flows:
  - authorizationCode
  - password
  scope: user_access
- description: Permission to delete the current user account
  flows:
  - authorizationCode
  - password
  scope: user_delete
slug: angelcam-scopes
source_filename: angelcam-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/angelcam-openapi-original.yml\nschemes:\n- name: OAuth2\n  source: openapi/angelcam-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://my.angelcam.com/oauth/authorize/\n    tokenUrl: https://my.angelcam.com/oauth/token/\n  - flow: password\n    tokenUrl: https://api.angelcam.com/oauth/token/\n  description: See the Authentication section above for full documentation.\nscopes:\n- scope: active_services_access\n  description: Permission to access active services\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: active_services_manage\n  description: Permission to manage active services\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: arrow_client_access\n  description: Permission to access Arrow clients\n  flows:\n  - authorizationCode\n  - password\n  sources:\n\
  \  - openapi/angelcam-openapi-original.yml\n- scope: arrow_client_manage\n  description: Permission to manage Arrow clients\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: audio_message_access\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: audio_message_manage\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: audio_messages_play\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: broadcasting_access\n  description: Permission to see general broadcasting information and access broadcasting streams\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: broadcasting_start_stop\n  description: Permission to start and stop public broadcasting on camera\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: camera_access\n  description: Permission to list cameras and to get\
  \ details of a specific camera\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: camera_create\n  description: Permission to create cameras\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: camera_delete\n  description: Permission to delete cameras\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: camera_guest_access\n  description: Permission to access camera guest\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: camera_guest_manage\n  description: Permission to manage camera guest\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: camera_manage\n  description: Permission to update cameras\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n\
  - scope: client_access\n  description: Permission to list resellers clients and get details of a specific client\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: client_create\n  description: Permission to create client account\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: client_manage\n  description: Permission to update clients detail\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: event_access\n  description: Permission to access events\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: incidents_access\n  description: Permission to access Incidents\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: locations_access\n  sources:\n  - openapi/angelcam-openapi-original.yml\n\
  - scope: messages_access\n  description: Permission to access RTS messages\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: messages_manage\n  description: Permission to manage RTS messages\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: notifications_methods_access\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: notifications_methods_manage\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: notifications_rules_access\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: notifications_rules_manage\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: orders_access\n  description: Permission to access orders\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: public_cameras_access\n  description: Permission to access public cameras\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: recording_access\n  description: Permission to access camera recordings\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: recording_clips_access\n  description: Permission to access recording clips\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: recording_clips_create\n  description: Permission to create recording clips\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: recording_clips_share\n  description: Permission to share recording clips\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: recording_start_stop\n  description: Permission to start and stop recording on camera\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n\
  - scope: rts_arming_manage\n  description: Permission to arm and disarm RTS\n  flows:\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: rts_settings_access\n  description: Permission to access RTS settings\n  flows:\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: rts_settings_manage\n  description: Permission to manage RTS settings\n  flows:\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: sensor_access\n  description: Permission to list sensors and to get details of a specific sensor\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: sensor_manage\n  description: Permission to create, update and delete sensors\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: services_access\n  description: Permission to access available services\n  flows:\n  - authorizationCode\n  - password\n\
  \  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: sites_access\n  description: Permission to access sites\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: sites_manage\n  description: Permission to create, update and delete sites\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: space_access\n  description: Permission to list and activate spaces\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: space_permissions_access\n  description: Permission to view space permissions\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: speaker_access\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: speaker_manage\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: streams_detect\n  description: Permission to detect\
  \ camera streams\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: trials_access\n  description: Permission to access available trials\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: trials_activate\n  description: Permission to activate a trial\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: user_access\n  description: Permission to access user information\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- scope: user_delete\n  description: Permission to delete the current user account\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/angelcam-openapi-original.yml\ndocs: https://developers.angelcam.com/guides/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angelcam/refs/heads/main/scopes/angelcam-scopes.yml
summary_line: 51 scopes · authorizationCode/password
tags:
- Company
- Video Surveillance
- Cameras
- IP Camera
- Cloud Recording
- Video Streaming
- IoT
- ONVIF
- Security
- Webhooks
token_urls:
- https://my.angelcam.com/oauth/token/
- https://api.angelcam.com/oauth/token/
---
