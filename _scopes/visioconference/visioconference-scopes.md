---
api_specs:
- filename: zoom-api.yaml
  format: yaml
  label: Zoom API
  slug: zoom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/zoom/api/master/openapi/zoom-api.yaml
authorization_urls:
- https://zoom.us/oauth/authorize
description: ''
docs: https://developers.zoom.us/docs/integrations/oauth-scopes/
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Visioconference Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Visioconference publishes 473 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Visioconference API on a user''s behalf.


  Tokens are issued from https://zoom.us/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Visioconference
provider_slug: visioconference
schemes:
- description: OAuth 2.0 (server-to-server or user OAuth); access tokens valid for one hour
  flows:
  - flow: clientCredentials
    tokenUrl: https://zoom.us/oauth/token
  - authorizationUrl: https://zoom.us/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://zoom.us/oauth/token
  name: oauth2
  source: openapi/visioconference-openapi.yml
scope_count: 473
scope_names:
- account:master
- account:read:admin
- account:write:admin
- billing:master
- calendar:read
- calendar:read:admin
- calendar:write
- calendar:write:admin
- chat:read
- chat:read:admin
- chat:write
- chat:write:admin
- chat_channel:read
- chat_channel:read:admin
- chat_channel:read:member
- chat_channel:write
- chat_channel:write:admin
- chat_contact:read
- chat_contact:write
- chat_contact:write:admin
- chat_event:write
- chat_event:write:admin
- chat_history_legal_hold:read:admin
- chat_history_legal_hold:write:admin
- chat_message:read
- chat_message:read:admin
- chat_message:write
- chat_message:write:admin
- chat_migration:read:admin
- chat_migration:write:admin
- imchat:bot
- imchat:read:admin
- imchat:write
- clips:read
- clips:read:admin
- clips:write
- clips:write:admin
- apiconnector:master
- apiconnector:read:admin
- apiconnector:write:admin
- crc:master
- crc:read:admin
- crc_account:master
- crc_account:read:admin
- crc_account:write:admin
- crc_rooms:master
- crc_rooms:read:admin
- crc_rooms:write:admin
- contact_center_attachment:read:admin
- contact_center_block_list_rules:write:admin
- contact_center_flow:write:admin
- contact_center_follow_up_task:read:admin
- contact_center_follow_up_task:write
- contact_center_messaging:read:admin
- contact_center_messaging:write:admin
- contact_center_outbound_campaign_dnc_list_phones:read:admin
- contact_center_outbound_campaign_dnc_list_phones:write:admin
- contact_center_routing_profile:write:admin
- contact_center_rtms:write:admin
- contact_center_team:read:admin
- contact_center_team:write:admin
- contact_center_user_template:read:admin
- contact_center_user_template:write:admin
- contact_center_asset_library:read:admin
- contact_center_asset_library:write:admin
- contact_center_contact:read:admin
- contact_center_contact:write:admin
- contact_center_disposition:read:admin
- contact_center_disposition:write:admin
- contact_center_engagement:read:admin
- contact_center_engagement:write:admin
- contact_center_flow:read:admin
- contact_center_inbox:read:admin
- contact_center_inbox:write:admin
- contact_center_note:read:admin
- contact_center_note:write
- contact_center_operating_hours:read:admin
- contact_center_operating_hours:write:admin
- contact_center_operation_logs:read:admin
- contact_center_outbound_campaign:delete:admin
- contact_center_outbound_campaign:read:admin
- contact_center_outbound_campaign:update:admin
- contact_center_outbound_campaign:write:admin
- contact_center_outbound_campaign_contactlist:read:admin
- contact_center_outbound_campaign_contactlist:write:admin
- contact_center_outbound_campaign_contacts:read:admin
- contact_center_outbound_campaign_contacts:write:admin
- contact_center_preference:read:admin
- contact_center_preference:write:admin
- contact_center_queue:read:admin
- contact_center_queue:write:admin
- contact_center_recording:read
- contact_center_recording:read:admin
- contact_center_recording:write:admin
- contact_center_region:read:admin
- contact_center_region:write:admin
- contact_center_report:read:admin
- contact_center_role:read:admin
- contact_center_role:write:admin
- contact_center_routing_profile:read:admin
- contact_center_skill:read:admin
- contact_center_skill:write:admin
- contact_center_sms:master
- contact_center_sms:read:admin
- contact_center_user:read:admin
- contact_center_user:write:admin
- contact_center_variable:read:admin
- contact_center_variable:write:admin
- contact_center_variable_log:read:admin
- contact_center_variable_log:write:admin
- contact_center_voice_call:master
- contact_center_voice_call:read:admin
- contact:read
- contact:read:admin
- dashboard:master
- dashboard:read:admin
- dashboard_crc:read:admin
- dashboard_home:read:admin
- dashboard_im:read:admin
- dashboard_meetings:read:admin
- dashboard_webinars:read:admin
- dashboard_zr:read:admin
- device:read:admin
- device:write:admin
- h323:master
- h323:read:admin
- h323:write:admin
- docs:delete
- docs:delete:admin
- docs:read:admin
- docs:write:admin
- docs_collaborator:delete
- docs_collaborator:delete:admin
- docs_collaborator:read
- docs_collaborator:read:admin
- docs_collaborator:write
- docs_collaborator:write:admin
- docs_export:read
- docs_export:read:admin
- docs_export:write
- docs_export:write:admin
- docs_file_owner:write
- docs_file_owner:write:admin
- docs_file_uploads:write
- docs_file_uploads:write:admin
- docs_general_access:read
- docs_general_access:read:admin
- docs_general_access:write
- docs_general_access:write:admin
- docs_import:read
- docs_import:read:admin
- docs_import:write
- docs_import:write:admin
- group:master
- group:read:admin
- group:write:admin
- contact_group:read:admin
- contact_group:write:admin
- imgroup:master
- imgroup:read:admin
- imgroup:write:admin
- clinical_note:read:admin
- clinical_note:update:admin
- mail:read
- mail:read:admin
- mail:write
- mail:write:admin
- marketplace_app:master
- marketplace_app:read
- marketplace_app:read:admin
- marketplace_app:write
- marketplace_app:write:admin
- marketplace_custom_fields:read
- marketplace_custom_fields:read:admin
- marketplace_entitlement:read
- marketplace_entitlement:read:admin
- information_barriers:read:admin
- information_barriers:read:master
- information_barriers:write:admin
- information_barriers:write:master
- meeting:master
- meeting:read
- meeting:read:admin
- meeting:write
- meeting:write:admin
- meeting:write:admin:sip_dialing
- meeting:write:sip_dialing
- meeting_summary:master
- meeting_summary:read
- meeting_summary:read:admin
- meeting_token:read:admin:live_streaming
- meeting_token:read:admin:local_archiving
- meeting_token:read:admin:local_recording
- meeting_token:read:live_streaming
- meeting_token:read:local_recording
- number_management_numbers:read:admin
- number_management_numbers:read:master
- number_management_numbers:write:admin
- number_management_numbers:write:master
- pac:read
- pac:read:admin
- phone:master
- phone:read
- phone:read:admin
- phone:write
- phone:write:admin
- phone_call_log:master
- phone_call_log:read
- phone_call_log:read:admin
- phone_call_log:write
- phone_call_log:write:admin
- phone_peering:master
- phone_peering:read:admin
- phone_peering:write:admin
- phone_recording:master
- phone_recording:read
- phone_recording:read:admin
- phone_recording:write
- phone_recording:write:admin
- phone_sms:master
- phone_sms:read
- phone_sms:read:admin
- phone_sms:write
- phone_sms:write:admin
- phone_voicemail:master
- phone_voicemail:read
- phone_voicemail:read:admin
- phone_voicemail:write
- phone_voicemail:write:admin
- qm_evaluations:read
- qm_evaluations:read:admin
- qm_interactions:read
- qm_interactions:read:admin
- recording:master
- recording:read
- recording:read:admin
- recording:write
- recording:write:admin
- report:master
- report:read:admin
- report_chat:read:admin
- zva_report:read:admin
- role:master
- role:read:admin
- role:write:admin
- room:master
- room:read:admin
- room:write:admin
- room:read:master
- room:write:master
- sip_phone:master
- sip_phone:read:admin
- sip_phone:write:admin
- sip_trunk:master
- contact_center_sms:write:admin
- scheduler:read
- scheduler:read:admin
- scheduler:write
- scheduler:write:admin
- app:deeplink:write
- app:deeplink:write:admin
- app:notification:read
- app:notification:write
- survey:master
- survey:read:admin
- tsp:master
- tsp:read
- tsp:read:admin
- tsp:write
- tsp:write:admin
- tasks:delete
- tasks:delete:admin
- tasks:read
- tasks:read:admin
- tasks:write
- tasks:write:admin
- tasks_assignee:read
- tasks_assignee:read:admin
- tasks_assignee:write
- tasks_assignee:write:admin
- tasks_collaborator:read
- tasks_collaborator:read:admin
- tasks_collaborator:write
- tasks_collaborator:write:admin
- tasks_comment:read
- tasks_comment:read:admin
- tasks_comment:write
- tasks_comment:write:admin
- tracking_fields:master
- tracking_fields:read:admin
- tracking_fields:write:admin
- user:master
- user:read
- user:read:admin
- user:write
- user:write:admin
- user_info:read
- user_zak:read
- visitor_management:read
- visitor_management:write
- visitor_management:write:admin
- webinar:master
- webinar:read
- webinar:read:admin
- webinar:write
- webinar:write:admin
- webinar:write:admin:sip_dialing
- webinar:write:sip_dialing
- webinar_token:read:admin:live_streaming
- webinar_token:read:admin:local_archiving
- webinar_token:read:admin:local_recording
- webinar_token:read:live_streaming
- webinar_token:read:local_recording
- whiteboard:read
- whiteboard:read:admin
- whiteboard:write
- whiteboard:write:admin
- whiteboard_classification_labels:read
- whiteboard_classification_labels:read:admin
- whiteboard_classification_labels:write:admin
- whiteboard_collaborator:read
- whiteboard_collaborator:read:admin
- whiteboard_collaborator:write
- whiteboard_collaborator:write:admin
- whiteboard_content:read
- whiteboard_content:read:admin
- whiteboard_export:write
- whiteboard_export:write:admin
- whiteboard_file:read
- whiteboard_file:read:admin
- whiteboard_file:write
- whiteboard_file:write:admin
- whiteboard_import:read
- whiteboard_import:read:admin
- whiteboard_import:write
- whiteboard_import:write:admin
- whiteboard_project:read
- whiteboard_project:read:admin
- whiteboard_project:write
- whiteboard_project:write:admin
- whiteboard_project_collaborator:read
- whiteboard_project_collaborator:read:admin
- whiteboard_project_collaborator:write
- whiteboard_project_collaborator:write:admin
- whiteboard_share_setting:write
- whiteboard_share_setting:write:admin
- workspace:read
- workspace:read:admin
- workspace:write
- workspace:write:admin
- aic_archive:read:admin
- dashboard_aic:read:admin
- data_request:read:admin
- data_request:write:admin
- dialer:read:admin
- dialer:write:admin
- clips:read:master
- docs:read
- docs:write
- zoom_events_access_links:read
- zoom_events_access_links:read:admin
- zoom_events_access_links:write
- zoom_events_access_links:write:admin
- zoom_events_attendee_actions:read
- zoom_events_attendee_actions:read:admin
- zoom_events_attendee_actions:write
- zoom_events_attendee_actions:write:admin
- zoom_events_basic:read
- zoom_events_basic:read:admin
- zoom_events_basic:write
- zoom_events_basic:write:admin
- zoom_events_coeditor:write
- zoom_events_coeditor:write:admin
- zoom_events_coeditors:read
- zoom_events_coeditors:read:admin
- zoom_events_email:read
- zoom_events_email:read:admin
- zoom_events_exhibitors:read
- zoom_events_exhibitors:read:admin
- zoom_events_exhibitors:write
- zoom_events_exhibitors:write:admin
- zoom_events_file:write
- zoom_events_file:write:admin
- zoom_events_hub:write
- zoom_events_hub:write:admin
- zoom_events_hubs:read
- zoom_events_hubs:read:admin
- zoom_events_insights:read
- zoom_events_insights:read:admin
- zoom_events_registrants:read
- zoom_events_registrants:read:admin
- zoom_events_reports:read
- zoom_events_reports:read:admin
- zoom_events_sessions:read
- zoom_events_sessions:read:admin
- zoom_events_sessions:write
- zoom_events_sessions:write:admin
- zoom_events_speakers:read
- zoom_events_speakers:read:admin
- zoom_events_speakers:write
- zoom_events_speakers:write:admin
- zoom_events_ticket_types:read
- zoom_events_ticket_types:read:admin
- zoom_events_ticket_types:write
- zoom_events_ticket_types:write:admin
- zoom_events_tickets:read
- zoom_events_tickets:read:admin
- zoom_events_tickets:write
- zoom_events_tickets:write:admin
- zoom_events_videos:read
- zoom_events_videos:read:admin
- zoom_events_videos:write
- zoom_events_videos:write:admin
- zoom_events_vod_channels:read
- zoom_events_vod_channels:read:admin
- zoom_events_vod_channels:write
- zoom_events_vod_channels:write:admin
- zoom_events_vod_registration:read
- zoom_events_vod_registration:read:admin
- zoom_events_vod_registration:write
- zoom_events_vod_registration:write:admin
- zoom_events_vod_reports:read
- zoom_events_vod_reports:read:admin
- iq_account:read:admin
- iq_coaching:read
- iq_coaching:read:admin
- iq_comment:read
- iq_comment:read:admin
- iq_comment:write
- iq_comment:write:admin
- iq_conversation:read
- iq_conversation:read:admin
- iq_conversation:write
- iq_conversation:write:admin
- iq_deal:read
- iq_deal:read:admin
- iq_deal:write
- iq_deal:write:admin
- iq_playlist:read
- iq_playlist:read:admin
- iq_team:read
- iq_team:read:admin
- iq_team:write:admin
- meeting_summary:write
- meeting_summary:write:admin
- qm_interactions:write
- qm_interactions:write:admin
- iq_crm:read:admin
- iq_crm:write:admin
- division:read:admin
- division:wirte:admin
- video_mgmt_channels:read
- video_mgmt_channels:read:admin
- video_mgmt_channels:write
- video_mgmt_channels:write:admin
- video_mgmt_file:write
- video_mgmt_file:write:admin
- video_mgmt_playlists:read
- video_mgmt_playlists:read:admin
- video_mgmt_playlists:write
- video_mgmt_playlists:write:admin
- video_mgmt_videos:read
- video_mgmt_videos:read:admin
- video_mgmt_videos:write
- video_mgmt_videos:write:admin
- zoom_commerce:read:admin
- zoom_commerce:write:admin
- zva:read:km_kbs
- zva:write:km_kbs
- zva_report:read
- contact_center_block_list_rules:read:admin
- workforce_management:write:admin
- workforce_management:read:admin
scopes:
- description: View and manage sub accounts
  flows: []
  scope: account:master
- description: View account info
  flows: []
  scope: account:read:admin
- description: View and manage account info
  flows: []
  scope: account:write:admin
- description: View and manage sub account's billing info
  flows: []
  scope: billing:master
- description: View calendar
  flows: []
  scope: calendar:read
- description: View calendar
  flows: []
  scope: calendar:read:admin
- description: Manage calendar
  flows: []
  scope: calendar:write
- description: Manage calendar
  flows: []
  scope: calendar:write:admin
- description: View Chat Message Info
  flows: []
  scope: chat:read
- description: View Chat Message Info
  flows: []
  scope: chat:read:admin
- description: Manage Chat Message Info
  flows: []
  scope: chat:write
- description: Manage Chat Message Info
  flows: []
  scope: chat:write:admin
- description: View current user's team chat channels
  flows: []
  scope: chat_channel:read
- description: View all users' team chat channels
  flows: []
  scope: chat_channel:read:admin
- description: View team chat channels as a member
  flows: []
  scope: chat_channel:read:member
- description: View and manage current user's team chat channels
  flows: []
  scope: chat_channel:write
- description: View and manage all users' team chat channels
  flows: []
  scope: chat_channel:write:admin
- description: View current user's team chat contact information
  flows: []
  scope: chat_contact:read
- description: Send Contact Invitation
  flows: []
  scope: chat_contact:write
- description: Send contact invitation
  flows: []
  scope: chat_contact:write:admin
- description: Manage your chat event info
  flows: []
  scope: chat_event:write
- description: Manage account's chat event info
  flows: []
  scope: chat_event:write:admin
- description: View Chat History Legal Hold Info
  flows: []
  scope: chat_history_legal_hold:read:admin
- description: Manage Chat History Legal Hold Info
  flows: []
  scope: chat_history_legal_hold:write:admin
- description: View current user's team chat messages
  flows: []
  scope: chat_message:read
- description: View all users' team chat messages
  flows: []
  scope: chat_message:read:admin
- description: View and manage current user's team chat messages
  flows: []
  scope: chat_message:write
- description: View and manage all users' team chat messages
  flows: []
  scope: chat_message:write:admin
- description: View information about a chat history migration
  flows: []
  scope: chat_migration:read:admin
- description: Migrate chat history from another vendor
  flows: []
  scope: chat_migration:write:admin
- description: Enable Chatbot within Zoom Team Chat Client
  flows: []
  scope: imchat:bot
- description: View all users history and channels
  flows: []
  scope: imchat:read:admin
- description: Send a team chat message to a Zoom Team Chat user or channel
  flows: []
  scope: imchat:write
- description: View your clips information
  flows: []
  scope: clips:read
- description: View your clips information
  flows: []
  scope: clips:read:admin
- description: Manage your clips information
  flows: []
  scope: clips:write
- description: Manage your clips information
  flows: []
  scope: clips:write:admin
- description: This scope allows an app to view and manage sub account’s API Connector information
  flows: []
  scope: apiconnector:master
- description: This scope allow an app to view all API Connector information
  flows: []
  scope: apiconnector:read:admin
- description: This scope allow an app to view and manage all API Connector information
  flows: []
  scope: apiconnector:write:admin
- description: View and manage sub account's CRC configuration
  flows: []
  scope: crc:master
- description: View and manage CRC configuration
  flows: []
  scope: crc:read:admin
- description: View and manage all sub account's Cisco/Polycom room account setting
  flows: []
  scope: crc_account:master
- description: View Cisco/Polycom rooms account setting
  flows: []
  scope: crc_account:read:admin
- description: View and manage Cisco/Polycom rooms account setting
  flows: []
  scope: crc_account:write:admin
- description: View and manage sub account’s managed Cisco and Polycom rooms information
  flows: []
  scope: crc_rooms:master
- description: View all managed Cisco and Polycom rooms information
  flows: []
  scope: crc_rooms:read:admin
- description: View and manage all managed Cisco and Polycom rooms information
  flows: []
  scope: crc_rooms:write:admin
- description: View your contact center attachment information
  flows: []
  scope: contact_center_attachment:read:admin
- description: Edit Block List Rules
  flows: []
  scope: contact_center_block_list_rules:write:admin
- description: flow write
  flows: []
  scope: contact_center_flow:write:admin
- description: View a follow-up task
  flows: []
  scope: contact_center_follow_up_task:read:admin
- description: Update a follow-up task
  flows: []
  scope: contact_center_follow_up_task:write
- description: Get message
  flows: []
  scope: contact_center_messaging:read:admin
- description: send message
  flows: []
  scope: contact_center_messaging:write:admin
- description: Get campaign dnc list phone
  flows: []
  scope: contact_center_outbound_campaign_dnc_list_phones:read:admin
- description: Write campaign dnc list phone
  flows: []
  scope: contact_center_outbound_campaign_dnc_list_phones:write:admin
- description: Edit agent routing profile.
  flows: []
  scope: contact_center_routing_profile:write:admin
- description: Scope to control RTMS
  flows: []
  scope: contact_center_rtms:write:admin
- description: View your contact center team information
  flows: []
  scope: contact_center_team:read:admin
- description: Manage your contact center team information
  flows: []
  scope: contact_center_team:write:admin
- description: View all contact center user template’s details.
  flows: []
  scope: contact_center_user_template:read:admin
- description: View and manage all contact center user template's details.
  flows: []
  scope: contact_center_user_template:write:admin
- description: View your contact center asset library information
  flows: []
  scope: contact_center_asset_library:read:admin
- description: Manage your contact center asset library information
  flows: []
  scope: contact_center_asset_library:write:admin
- description: View address book information
  flows: []
  scope: contact_center_contact:read:admin
- description: Update address book information
  flows: []
  scope: contact_center_contact:write:admin
- description: View your contact center disposition information
  flows: []
  scope: contact_center_disposition:read:admin
- description: Manage your contact center disposition information
  flows: []
  scope: contact_center_disposition:write:admin
- description: View all contact center engagement information
  flows: []
  scope: contact_center_engagement:read:admin
- description: Manage all contact center engagement information
  flows: []
  scope: contact_center_engagement:write:admin
- description: View all contact center flow information
  flows: []
  scope: contact_center_flow:read:admin
- description: View all contact center inbox information
  flows: []
  scope: contact_center_inbox:read:admin
- description: Manage all contact center inbox information
  flows: []
  scope: contact_center_inbox:write:admin
- description: View all contact center note information
  flows: []
  scope: contact_center_note:read:admin
- description: Manage all contact center note information
  flows: []
  scope: contact_center_note:write
- description: View all contact center operating hours information
  flows: []
  scope: contact_center_operating_hours:read:admin
- description: Manage all contact center operating hours information
  flows: []
  scope: contact_center_operating_hours:write:admin
- description: Read permission for Operation logs
  flows: []
  scope: contact_center_operation_logs:read:admin
- description: Delete an Outbound Campaign.
  flows: []
  scope: contact_center_outbound_campaign:delete:admin
- description: View an Outbound Campaign.
  flows: []
  scope: contact_center_outbound_campaign:read:admin
- description: Update an Outbound Campaign
  flows: []
  scope: contact_center_outbound_campaign:update:admin
- description: Create an Outbound Campaign
  flows: []
  scope: contact_center_outbound_campaign:write:admin
- description: Get campaign contact list
  flows: []
  scope: contact_center_outbound_campaign_contactlist:read:admin
- description: Create campaign contact list
  flows: []
  scope: contact_center_outbound_campaign_contactlist:write:admin
- description: Get campaign contact list contact
  flows: []
  scope: contact_center_outbound_campaign_contacts:read:admin
- description: Create campaign contact list contact
  flows: []
  scope: contact_center_outbound_campaign_contacts:write:admin
- description: View your contact center preference information
  flows: []
  scope: contact_center_preference:read:admin
- description: Manage your contact center preference information
  flows: []
  scope: contact_center_preference:write:admin
- description: View your contact center queue information
  flows: []
  scope: contact_center_queue:read:admin
- description: Manage your contact center queue information
  flows: []
  scope: contact_center_queue:write:admin
- description: View your contact center recording information.
  flows: []
  scope: contact_center_recording:read
- description: View all contact center recording information
  flows: []
  scope: contact_center_recording:read:admin
- description: Manage all contact center recording information
  flows: []
  scope: contact_center_recording:write:admin
- description: View all contact center region information
  flows: []
  scope: contact_center_region:read:admin
- description: Manage all contact center region information
  flows: []
  scope: contact_center_region:write:admin
- description: View all contact center report information
  flows: []
  scope: contact_center_report:read:admin
- description: View your contact center role information
  flows: []
  scope: contact_center_role:read:admin
- description: Manage your contact center role information
  flows: []
  scope: contact_center_role:write:admin
- description: View routing profile information.
  flows: []
  scope: contact_center_routing_profile:read:admin
- description: View all contact center skill information
  flows: []
  scope: contact_center_skill:read:admin
- description: Manage all contact center skill information
  flows: []
  scope: contact_center_skill:write:admin
- description: View sub account’s SMS log information
  flows: []
  scope: contact_center_sms:master
- description: View all contact center SMS log information
  flows: []
  scope: contact_center_sms:read:admin
- description: View all contact center user’s details
  flows: []
  scope: contact_center_user:read:admin
- description: View and manage all contact center user's details
  flows: []
  scope: contact_center_user:write:admin
- description: View all contact center variable information
  flows: []
  scope: contact_center_variable:read:admin
- description: Manage all contact center variable information
  flows: []
  scope: contact_center_variable:write:admin
- description: View variable log information
  flows: []
  scope: contact_center_variable_log:read:admin
- description: Manage variable log information
  flows: []
  scope: contact_center_variable_log:write:admin
- description: View sub account’s voice call information
  flows: []
  scope: contact_center_voice_call:master
- description: view voice call information
  flows: []
  scope: contact_center_voice_call:read:admin
- description: View current user's contacts
  flows: []
  scope: contact:read
- description: View all users' contacts
  flows: []
  scope: contact:read:admin
- description: View sub account's Dashboard data
  flows: []
  scope: dashboard:master
- description: View Dashboard data
  flows: []
  scope: dashboard:read:admin
- description: View all users' usage statistics of CRC
  flows: []
  scope: dashboard_crc:read:admin
- description: View overview of usage statistics for Meetings and Zoom Rooms
  flows: []
  scope: dashboard_home:read:admin
- description: View all users' usage statistics of team chat messages and message types
  flows: []
  scope: dashboard_im:read:admin
- description: View all users' meetings information on Dashboard
  flows: []
  scope: dashboard_meetings:read:admin
- description: View all users' webinar information on Dashboard
  flows: []
  scope: dashboard_webinars:read:admin
- description: View all users' Zoom Room usage statistics and information
  flows: []
  scope: dashboard_zr:read:admin
- description: Manage device
  flows: []
  scope: device:read:admin
- description: View and manage device
  flows: []
  scope: device:write:admin
- description: View and manage sub account's H.323 devices
  flows: []
  scope: h323:master
- description: View all users' H.323 devices
  flows: []
  scope: h323:read:admin
- description: View and manage all users' H.323 devices
  flows: []
  scope: h323:write:admin
- description: Delete a file
  flows: []
  scope: docs:delete
- description: Delete a file
  flows: []
  scope: docs:delete:admin
- description: Get basic info of the file
  flows: []
  scope: docs:read:admin
- description: Edit basic info of a file
  flows: []
  scope: docs:write:admin
- description: Remove collaborators of a file
  flows: []
  scope: docs_collaborator:delete
- description: Remove collaborators of a file
  flows: []
  scope: docs_collaborator:delete:admin
- description: Get collaborators of a file
  flows: []
  scope: docs_collaborator:read
- description: Get collaborator of a file
  flows: []
  scope: docs_collaborator:read:admin
- description: scope to manage collaborator in Docs
  flows: []
  scope: docs_collaborator:write
- description: scope for admin to manage collaborators
  flows: []
  scope: docs_collaborator:write:admin
- description: Get file export status
  flows: []
  scope: docs_export:read
- description: Get file export status
  flows: []
  scope: docs_export:read:admin
- description: Create a file export
  flows: []
  scope: docs_export:write
- description: Create a file export
  flows: []
  scope: docs_export:write:admin
- description: Transfer ownership of a file
  flows: []
  scope: docs_file_owner:write
- description: Transfer ownership of a file
  flows: []
  scope: docs_file_owner:write:admin
- description: Create a file upload
  flows: []
  scope: docs_file_uploads:write
- description: Create a file upload
  flows: []
  scope: docs_file_uploads:write:admin
- description: Get general access of a file
  flows: []
  scope: docs_general_access:read
- description: Get general access of a file
  flows: []
  scope: docs_general_access:read:admin
- description: Update general access of a file
  flows: []
  scope: docs_general_access:write
- description: Update general access of a file
  flows: []
  scope: docs_general_access:write:admin
- description: Get import task status
  flows: []
  scope: docs_import:read
- description: Get import task status
  flows: []
  scope: docs_import:read:admin
- description: Create new file by import
  flows: []
  scope: docs_import:write
- description: Create new file by import
  flows: []
  scope: docs_import:write:admin
- description: View and manage sub account's groups
  flows: []
  scope: group:master
- description: View groups
  flows: []
  scope: group:read:admin
- description: View and manage groups
  flows: []
  scope: group:write:admin
- description: View all contact group information
  flows: []
  scope: contact_group:read:admin
- description: Manage all contact group information
  flows: []
  scope: contact_group:write:admin
- description: View and manage sub account's Zoom Team Chat Groups
  flows: []
  scope: imgroup:master
- description: View Zoom Team Chat Group information
  flows: []
  scope: imgroup:read:admin
- description: View and manage Zoom Team Chat Groups
  flows: []
  scope: imgroup:write:admin
- description: Read Clinical Notes
  flows: []
  scope: clinical_note:read:admin
- description: Update Clinical Notes
  flows: []
  scope: clinical_note:update:admin
- description: Read user’s own mailbox content.
  flows: []
  scope: mail:read
- description: Read all mailboxes' content under the account, and account level settings.
  flows: []
  scope: mail:read:admin
- description: Read and write user’s own mailbox content.
  flows: []
  scope: mail:write
- description: Read and write all mailboxes' content under the account, and account level settings.
  flows: []
  scope: mail:write:admin
- description: View and manage sub accounts' marketplace app info
  flows: []
  scope: marketplace_app:master
- description: View your marketplace app information
  flows: []
  scope: marketplace_app:read
- description: View marketplace app information for the account
  flows: []
  scope: marketplace_app:read:admin
- description: Edit marketplace app
  flows: []
  scope: marketplace_app:write
- description: View and Manage marketplace app information for the account
  flows: []
  scope: marketplace_app:write:admin
- description: Read custom field values
  flows: []
  scope: marketplace_custom_fields:read
- description: Read custom field values
  flows: []
  scope: marketplace_custom_fields:read:admin
- description: View entitlements
  flows: []
  scope: marketplace_entitlement:read
- description: View entitlements
  flows: []
  scope: marketplace_entitlement:read:admin
- description: View information barriers
  flows: []
  scope: information_barriers:read:admin
- description: View information barriers
  flows: []
  scope: information_barriers:read:master
- description: View and manage information barriers
  flows: []
  scope: information_barriers:write:admin
- description: View and manage information barriers
  flows: []
  scope: information_barriers:write:master
- description: View and manage sub account's user meetings
  flows: []
  scope: meeting:master
- description: View your meetings
  flows: []
  scope: meeting:read
- description: View all user meetings
  flows: []
  scope: meeting:read:admin
- description: View and manage your meetings
  flows: []
  scope: meeting:write
- description: View and manage all user meetings
  flows: []
  scope: meeting:write:admin
- description: Get CRC dial string with passcode
  flows: []
  scope: meeting:write:admin:sip_dialing
- description: Get CRC dial string with passcode
  flows: []
  scope: meeting:write:sip_dialing
- description: View and manage sub account's user meeting summaries
  flows: []
  scope: meeting_summary:master
- description: View your meeting summaries
  flows: []
  scope: meeting_summary:read
- description: View all user meeting summaries
  flows: []
  scope: meeting_summary:read:admin
- description: View live streaming meeting token information
  flows: []
  scope: meeting_token:read:admin:live_streaming
- description: View local archiving meeting token information
  flows: []
  scope: meeting_token:read:admin:local_archiving
- description: This scope allows an app to view an account's users' local recording meeting token information
  flows: []
  scope: meeting_token:read:admin:local_recording
- description: View live streaming meeting token information
  flows: []
  scope: meeting_token:read:live_streaming
- description: This scope allows an app to view a user's local recording meeting token information
  flows: []
  scope: meeting_token:read:local_recording
- description: View all phone number detail in "Number Management".
  flows: []
  scope: number_management_numbers:read:admin
- description: View and manage sub account's phone number detail in "Number Management".
  flows: []
  scope: number_management_numbers:read:master
- description: Manage phone number detail in "Number Management".
  flows: []
  scope: number_management_numbers:write:admin
- description: Manage sub account's phone number detail in "Number Management".
  flows: []
  scope: number_management_numbers:write:master
- description: View your audio conference info
  flows: []
  scope: pac:read
- description: View all users' audio conference info
  flows: []
  scope: pac:read:admin
- description: View and manage all sub accounts' Zoom Phone information
  flows: []
  scope: phone:master
- description: View your phone information
  flows: []
  scope: phone:read
- description: View all users' phone information
  flows: []
  scope: phone:read:admin
- description: View and manage your phone information
  flows: []
  scope: phone:write
- description: View and manage all users' phone information
  flows: []
  scope: phone:write:admin
- description: View and manage all subaccounts' call logs
  flows: []
  scope: phone_call_log:master
- description: View your call history information
  flows: []
  scope: phone_call_log:read
- description: View all users' call history information
  flows: []
  scope: phone_call_log:read:admin
- description: View and manage your call log information
  flows: []
  scope: phone_call_log:write
- description: View and manage all users' call log information
  flows: []
  scope: phone_call_log:write:admin
- description: View and manage subaccounts' E164 numbers sent via peering API
  flows: []
  scope: phone_peering:master
- description: View the E164 numbers sent via peering API
  flows: []
  scope: phone_peering:read:admin
- description: View and manage the E164 numbers sent via peering API
  flows: []
  scope: phone_peering:write:admin
- description: View and manage subaccounts' call recording information
  flows: []
  scope: phone_recording:master
- description: View your call recording information
  flows: []
  scope: phone_recording:read
- description: View all users' recording information
  flows: []
  scope: phone_recording:read:admin
- description: View and manage your call recording information
  flows: []
  scope: phone_recording:write
- description: View and manage all users' call recording information
  flows: []
  scope: phone_recording:write:admin
- description: View and manage all sub accounts' Zoom Phone SMS information
  flows: []
  scope: phone_sms:master
- description: View your Zoom Phone SMS information
  flows: []
  scope: phone_sms:read
- description: View all users' Zoom Phone SMS information
  flows: []
  scope: phone_sms:read:admin
- description: View and manage your Zoom Phone SMS information
  flows: []
  scope: phone_sms:write
- description: View and manage all users' Zoom Phone SMS information
  flows: []
  scope: phone_sms:write:admin
- description: View and manage subaccounts' call voicemails
  flows: []
  scope: phone_voicemail:master
- description: View your call voicemail information
  flows: []
  scope: phone_voicemail:read
- description: View all users' call voicemail information
  flows: []
  scope: phone_voicemail:read:admin
- description: View and manage your call voicemail information
  flows: []
  scope: phone_voicemail:write
- description: View and manage all users' call voicemail information
  flows: []
  scope: phone_voicemail:write:admin
- description: Read evaluations
  flows: []
  scope: qm_evaluations:read
- description: Read evaluations
  flows: []
  scope: qm_evaluations:read:admin
- description: View interactions
  flows: []
  scope: qm_interactions:read
- description: View interactions
  flows: []
  scope: qm_interactions:read:admin
- description: View and manage sub account's user recordings
  flows: []
  scope: recording:master
- description: View your recordings
  flows: []
  scope: recording:read
- description: View all user recordings
  flows: []
  scope: recording:read:admin
- description: View and manage your recordings
  flows: []
  scope: recording:write
- description: View and manage all user recordings
  flows: []
  scope: recording:write:admin
- description: View sub account's report data
  flows: []
  scope: report:master
- description: View report data
  flows: []
  scope: report:read:admin
- description: View your team chat history report
  flows: []
  scope: report_chat:read:admin
- description: View zva engagements
  flows: []
  scope: zva_report:read:admin
- description: View and manage sub account user roles
  flows: []
  scope: role:master
- description: View all user roles
  flows: []
  scope: role:read:admin
- description: View and manage all user roles
  flows: []
  scope: role:write:admin
- description: View and manage sub account's Zoom Rooms information
  flows: []
  scope: room:master
- description: View all users' Zoom Rooms information
  flows: []
  scope: room:read:admin
- description: View and manage all users' Zoom Rooms information
  flows: []
  scope: room:write:admin
- description: View sub account's Zoom Rooms information
  flows: []
  scope: room:read:master
- description: Manage sub account's Zoom Rooms information
  flows: []
  scope: room:write:master
- description: View and manage sub account's SIP phone information
  flows: []
  scope: sip_phone:master
- description: View all users' SIP phone information
  flows: []
  scope: sip_phone:read:admin
- description: View and manage all users' SIP phone information
  flows: []
  scope: sip_phone:write:admin
- description: View and manage sub account's SIP trunk information
  flows: []
  scope: sip_trunk:master
- description: send sms
  flows: []
  scope: contact_center_sms:write:admin
- description: View scheduler
  flows: []
  scope: scheduler:read
- description: View scheduler
  flows: []
  scope: scheduler:read:admin
- description: Manage scheduler
  flows: []
  scope: scheduler:write
- description: Manage scheduler
  flows: []
  scope: scheduler:write:admin
- description: Generate an app deeplink
  flows: []
  scope: app:deeplink:write
- description: Generate an app deeplink
  flows: []
  scope: app:deeplink:write:admin
- description: View chat app notification
  flows: []
  scope: app:notification:read
- description: View and Manage chat app notification
  flows: []
  scope: app:notification:write
- description: View survey information
  flows: []
  scope: survey:master
- description: View survey information
  flows: []
  scope: survey:read:admin
- description: View and manage sub account's TSP account info
  flows: []
  scope: tsp:master
- description: View your TSP account info
  flows: []
  scope: tsp:read
- description: View TSP info
  flows: []
  scope: tsp:read:admin
- description: View and manage your TSP account info
  flows: []
  scope: tsp:write
- description: View and manage TSP info
  flows: []
  scope: tsp:write:admin
- description: Delete user's task(s)
  flows: []
  scope: tasks:delete
- description: Delete account's task(s)
  flows: []
  scope: tasks:delete:admin
- description: Get user’s task(s)
  flows: []
  scope: tasks:read
- description: Get account's task(s)
  flows: []
  scope: tasks:read:admin
- description: Update or trash tasks
  flows: []
  scope: tasks:write
- description: Management the account's task
  flows: []
  scope: tasks:write:admin
- description: View task's assignee(s)
  flows: []
  scope: tasks_assignee:read
- description: View account's task assignees
  flows: []
  scope: tasks_assignee:read:admin
- description: Add or remove task's assignee
  flows: []
  scope: tasks_assignee:write
- description: Add or update task's assignees
  flows: []
  scope: tasks_assignee:write:admin
- description: View user's task collaborator information
  flows: []
  scope: tasks_collaborator:read
- description: View account's task collaborators
  flows: []
  scope: tasks_collaborator:read:admin
- description: Add or update task's collaborator
  flows: []
  scope: tasks_collaborator:write
- description: View and update account's task collaborator information
  flows: []
  scope: tasks_collaborator:write:admin
- description: Read user's task comment
  flows: []
  scope: tasks_comment:read
- description: View account's task comment
  flows: []
  scope: tasks_comment:read:admin
- description: Manage and view the user's task comments
  flows: []
  scope: tasks_comment:write
- description: View and manage account's task comment.
  flows: []
  scope: tasks_comment:write:admin
- description: View and manage sub account user tracking fields
  flows: []
  scope: tracking_fields:master
- description: View all users' tracking fields
  flows: []
  scope: tracking_fields:read:admin
- description: View and manage all users' tracking fields
  flows: []
  scope: tracking_fields:write:admin
- description: View and manage sub account's user information
  flows: []
  scope: user:master
- description: View your user information
  flows: []
  scope: user:read
- description: View all user information
  flows: []
  scope: user:read:admin
- description: View and manage your user information
  flows: []
  scope: user:write
- description: View users information and manage users
  flows: []
  scope: user:write:admin
- description: View user info
  flows: []
  scope: user_info:read
- description: View user’s zak token
  flows: []
  scope: user_zak:read
- description: View visitor management information
  flows: []
  scope: visitor_management:read
- description: Update visitor management information
  flows: []
  scope: visitor_management:write
- description: Update visitor management information
  flows: []
  scope: visitor_management:write:admin
- description: View and manage sub account's user webinars
  flows: []
  scope: webinar:master
- description: View your webinars
  flows: []
  scope: webinar:read
- description: View all user Webinars
  flows: []
  scope: webinar:read:admin
- description: View and manage your webinars
  flows: []
  scope: webinar:write
- description: View and manage all user Webinars
  flows: []
  scope: webinar:write:admin
- description: Get CRC dial string with passcode
  flows: []
  scope: webinar:write:admin:sip_dialing
- description: Get CRC dial string with passcode
  flows: []
  scope: webinar:write:sip_dialing
- description: View live streaming webinar token information
  flows: []
  scope: webinar_token:read:admin:live_streaming
- description: View local archiving webinar token information
  flows: []
  scope: webinar_token:read:admin:local_archiving
- description: This scope allows an app to view an account's users' local recording webinar token information
  flows: []
  scope: webinar_token:read:admin:local_recording
- description: View live streaming webinar token information
  flows: []
  scope: webinar_token:read:live_streaming
- description: This scope allows an app to view a user's local recording webinar token information
  flows: []
  scope: webinar_token:read:local_recording
- description: Get my whiteboard(s)
  flows: []
  scope: whiteboard:read
- description: Get account’s whiteboard(s)
  flows: []
  scope: whiteboard:read:admin
- description: Update or trash my whiteboard
  flows: []
  scope: whiteboard:write
- description: Update or trash my whiteboard
  flows: []
  scope: whiteboard:write:admin
- description: Read whiteboard classification labels
  flows: []
  scope: whiteboard_classification_labels:read
- description: View account classification labels
  flows: []
  scope: whiteboard_classification_labels:read:admin
- description: View and manage account classification labels
  flows: []
  scope: whiteboard_classification_labels:write:admin
- description: View user's whiteboard collaborator information
  flows: []
  scope: whiteboard_collaborator:read
- description: View account's whiteboard collaborator information
  flows: []
  scope: whiteboard_collaborator:read:admin
- description: View and add collaborator information to the whiteboard
  flows: []
  scope: whiteboard_collaborator:write
- description: View and manage account's whiteboard collaborator information
  flows: []
  scope: whiteboard_collaborator:write:admin
- description: View and export whiteboard content
  flows: []
  scope: whiteboard_content:read
- description: View and export account’s whiteboard(s) content
  flows: []
  scope: whiteboard_content:read:admin
- description: Create my whiteboard export data
  flows: []
  scope: whiteboard_export:write
- description: Create account's whiteboard export data
  flows: []
  scope: whiteboard_export:write:admin
- description: View whiteboard file information
  flows: []
  scope: whiteboard_file:read
- description: View whiteboard file information
  flows: []
  scope: whiteboard_file:read:admin
- description: View and manage whiteboard file informanation
  flows: []
  scope: whiteboard_file:write
- description: View and manage account's whiteboard file information
  flows: []
  scope: whiteboard_file:write:admin
- description: View user's whiteboard import information
  flows: []
  scope: whiteboard_import:read
- description: View account's whiteboard import information
  flows: []
  scope: whiteboard_import:read:admin
- description: View and manage user's whiteboard import information
  flows: []
  scope: whiteboard_import:write
- description: view and manage account's whiteboard import information
  flows: []
  scope: whiteboard_import:write:admin
- description: View user's project information
  flows: []
  scope: whiteboard_project:read
- description: View account's project information
  flows: []
  scope: whiteboard_project:read:admin
- description: View and manage user's project information
  flows: []
  scope: whiteboard_project:write
- description: View and manage account's project information
  flows: []
  scope: whiteboard_project:write:admin
- description: View user's project collaborator information
  flows: []
  scope: whiteboard_project_collaborator:read
- description: View account's project collaborator information
  flows: []
  scope: whiteboard_project_collaborator:read:admin
- description: View and update user's project collaborator information
  flows: []
  scope: whiteboard_project_collaborator:write
- description: View and update account's project collaborator information
  flows: []
  scope: whiteboard_project_collaborator:write:admin
- description: View and manage your whiteboard sharing settings
  flows: []
  scope: whiteboard_share_setting:write
- description: View and manage account's whiteboard sharing settings
  flows: []
  scope: whiteboard_share_setting:write:admin
- description: View workspace reservation information
  flows: []
  scope: workspace:read
- description: View workspace reservation information for the account
  flows: []
  scope: workspace:read:admin
- description: Edit workspace reservation information
  flows: []
  scope: workspace:write
- description: Edit workspace reservation information for the account
  flows: []
  scope: workspace:write:admin
- description: View all user's AIC archive files
  flows: []
  scope: aic_archive:read:admin
- description: View users' AIC information on Dashboard
  flows: []
  scope: dashboard_aic:read:admin
- description: Allows viewing and downloading data request information
  flows: []
  scope: data_request:read:admin
- description: Allows creation and modification of data requests
  flows: []
  scope: data_request:write:admin
- description: View Dialer
  flows: []
  scope: dialer:read:admin
- description: Manage Dialer
  flows: []
  scope: dialer:write:admin
- description: view your subAccount clips info
  flows: []
  scope: clips:read:master
- description: Get basic info of the file
  flows: []
  scope: docs:read
- description: Edit basic info of a file
  flows: []
  scope: docs:write
- description: View event's Access Link
  flows: []
  scope: zoom_events_access_links:read
- description: View event's Access Link
  flows: []
  scope: zoom_events_access_links:read:admin
- description: View and Manage Zoom Event's access links
  flows: []
  scope: zoom_events_access_links:write
- description: View and Manage Zoom Event's access links
  flows: []
  scope: zoom_events_access_links:write:admin
- description: View attendee actions performed by host for an event/session
  flows: []
  scope: zoom_events_attendee_actions:read
- description: View attendee actions performed by host for an event/session
  flows: []
  scope: zoom_events_attendee_actions:read:admin
- description: View and manage attendee actions performed by host for an event/session
  flows: []
  scope: zoom_events_attendee_actions:write
- description: View and manage attendee actions performed by host for an event/session
  flows: []
  scope: zoom_events_attendee_actions:write:admin
- description: View your Zoom events
  flows: []
  scope: zoom_events_basic:read
- description: View all events information
  flows: []
  scope: zoom_events_basic:read:admin
- description: Manage your Zoom events
  flows: []
  scope: zoom_events_basic:write
- description: View and manage events information
  flows: []
  scope: zoom_events_basic:write:admin
- description: View and manage coeditor information
  flows: []
  scope: zoom_events_coeditor:write
- description: View and manage coeditor information
  flows: []
  scope: zoom_events_coeditor:write:admin
- description: View Zoom event coeditors information
  flows: []
  scope: zoom_events_coeditors:read
- description: View Zoom events coeditor information
  flows: []
  scope: zoom_events_coeditors:read:admin
- description: View emails for an event
  flows: []
  scope: zoom_events_email:read
- description: View emails for an event
  flows: []
  scope: zoom_events_email:read:admin
- description: View exhibitor information for an event
  flows: []
  scope: zoom_events_exhibitors:read
- description: View exhibitor information for an event
  flows: []
  scope: zoom_events_exhibitors:read:admin
- description: View and manage exhibitor information for an event
  flows: []
  scope: zoom_events_exhibitors:write
- description: View and manage exhibitor information for an event
  flows: []
  scope: zoom_events_exhibitors:write:admin
- description: zoom events file upload
  flows: []
  scope: zoom_events_file:write
- description: zoom events file upload account level
  flows: []
  scope: zoom_events_file:write:admin
- description: Update Zoom Events hub configuration
  flows: []
  scope: zoom_events_hub:write
- description: Update Zoom Events hub information
  flows: []
  scope: zoom_events_hub:write:admin
- description: View all hubs information
  flows: []
  scope: zoom_events_hubs:read
- description: View all hubs information
  flows: []
  scope: zoom_events_hubs:read:admin
- description: View Insights data
  flows: []
  scope: zoom_events_insights:read
- description: View Insights data
  flows: []
  scope: zoom_events_insights:read:admin
- description: View event registrants information
  flows: []
  scope: zoom_events_registrants:read
- description: View event registrants information
  flows: []
  scope: zoom_events_registrants:read:admin
- description: View Zoom events report
  flows: []
  scope: zoom_events_reports:read
- description: View Zoom events reports
  flows: []
  scope: zoom_events_reports:read:admin
- description: View event session information
  flows: []
  scope: zoom_events_sessions:read
- description: View event session information
  flows: []
  scope: zoom_events_sessions:read:admin
- description: View and manage event session information
  flows: []
  scope: zoom_events_sessions:write
- description: View and manage event session information
  flows: []
  scope: zoom_events_sessions:write:admin
- description: View event speaker information
  flows: []
  scope: zoom_events_speakers:read
- description: View event speaker information
  flows: []
  scope: zoom_events_speakers:read:admin
- description: Manage event speaker information
  flows: []
  scope: zoom_events_speakers:write
- description: Manage event speaker information
  flows: []
  scope: zoom_events_speakers:write:admin
- description: View all event ticket types
  flows: []
  scope: zoom_events_ticket_types:read
- description: View all event ticket types
  flows: []
  scope: zoom_events_ticket_types:read:admin
- description: View and manage event ticket types
  flows: []
  scope: zoom_events_ticket_types:write
- description: View and manage event ticket types
  flows: []
  scope: zoom_events_ticket_types:write:admin
- description: View event tickets and event ticket details
  flows: []
  scope: zoom_events_tickets:read
- description: View event tickets information
  flows: []
  scope: zoom_events_tickets:read:admin
- description: Create event tickets
  flows: []
  scope: zoom_events_tickets:write
- description: View and manage event tickets information
  flows: []
  scope: zoom_events_tickets:write:admin
- description: View video details
  flows: []
  scope: zoom_events_videos:read
- description: View video information
  flows: []
  scope: zoom_events_videos:read:admin
- description: Manage video information
  flows: []
  scope: zoom_events_videos:write
- description: Manage video information
  flows: []
  scope: zoom_events_videos:write:admin
- description: View on-demand video channels
  flows: []
  scope: zoom_events_vod_channels:read
- description: View on-demand video channels
  flows: []
  scope: zoom_events_vod_channels:read:admin
- description: View and manage on-demand video channels
  flows: []
  scope: zoom_events_vod_channels:write
- description: View and manage on-demand video channels
  flows: []
  scope: zoom_events_vod_channels:write:admin
- description: Read VOD channel registrations
  flows: []
  scope: zoom_events_vod_registration:read
- description: Read VOD channel registration settings
  flows: []
  scope: zoom_events_vod_registration:read:admin
- description: Update VOD channel registrations
  flows: []
  scope: zoom_events_vod_registration:write
- description: Update VOD channel registrations
  flows: []
  scope: zoom_events_vod_registration:write:admin
- description: Zoom Events VOD reports
  flows: []
  scope: zoom_events_vod_reports:read
- description: Zoom events VOD reports
  flows: []
  scope: zoom_events_vod_reports:read:admin
- description: View all account settings information
  flows: []
  scope: iq_account:read:admin
- description: View your coaching information
  flows: []
  scope: iq_coaching:read
- description: View all coaching information
  flows: []
  scope: iq_coaching:read:admin
- description: View your comments information
  flows: []
  scope: iq_comment:read
- description: Manage all comments information
  flows: []
  scope: iq_comment:read:admin
- description: Mangage your comments information
  flows: []
  scope: iq_comment:write
- description: Manage all comments information
  flows: []
  scope: iq_comment:write:admin
- description: View your conversations information
  flows: []
  scope: iq_conversation:read
- description: View all conversations information
  flows: []
  scope: iq_conversation:read:admin
- description: Manage your conversations information
  flows: []
  scope: iq_conversation:write
- description: Manage all conversations information
  flows: []
  scope: iq_conversation:write:admin
- description: Retrieve ZoomIQ Deal information with activity
  flows: []
  scope: iq_deal:read
- description: Retrieve ZoomIQ Deal information with activity
  flows: []
  scope: iq_deal:read:admin
- description: View and manage deal activities
  flows: []
  scope: iq_deal:write
- description: View and manage deal activities
  flows: []
  scope: iq_deal:write:admin
- description: View all playlists information
  flows: []
  scope: iq_playlist:read
- description: View all playlists information
  flows: []
  scope: iq_playlist:read:admin
- description: Get team info in User level
  flows: []
  scope: iq_team:read
- description: Get team info
  flows: []
  scope: iq_team:read:admin
- description: team resource read&edit
  flows: []
  scope: iq_team:write:admin
- description: View and manage your meeting summaries
  flows: []
  scope: meeting_summary:write
- description: View and manage all user meeting summaries
  flows: []
  scope: meeting_summary:write:admin
- description: Manage the interactions.
  flows: []
  scope: qm_interactions:write
- description: Manage the interactions.
  flows: []
  scope: qm_interactions:write:admin
- description: View CRM objects and metadata
  flows: []
  scope: iq_crm:read:admin
- description: Edit CRM objects and metadata
  flows: []
  scope: iq_crm:write:admin
- description: View divisions
  flows: []
  scope: division:read:admin
- description: View and manage divisions
  flows: []
  scope: division:wirte:admin
- description: View video channels information
  flows: []
  scope: video_mgmt_channels:read
- description: View video channels information
  flows: []
  scope: video_mgmt_channels:read:admin
- description: Manage video channels
  flows: []
  scope: video_mgmt_channels:write
- description: Manage video channels
  flows: []
  scope: video_mgmt_channels:write:admin
- description: Upload file to video management
  flows: []
  scope: video_mgmt_file:write
- description: upload a file to video management
  flows: []
  scope: video_mgmt_file:write:admin
- description: View playlists
  flows: []
  scope: video_mgmt_playlists:read
- description: View playlists
  flows: []
  scope: video_mgmt_playlists:read:admin
- description: Manage playlists
  flows: []
  scope: video_mgmt_playlists:write
- description: Manage playlists
  flows: []
  scope: video_mgmt_playlists:write:admin
- description: View videos information
  flows: []
  scope: video_mgmt_videos:read
- description: View videos information
  flows: []
  scope: video_mgmt_videos:read:admin
- description: Manage video content and metadata
  flows: []
  scope: video_mgmt_videos:write
- description: Manage video content and metadata
  flows: []
  scope: video_mgmt_videos:write:admin
- description: Zoom commerce API read access for account admin
  flows: []
  scope: zoom_commerce:read:admin
- description: Zoom Commerce API write access for account admin
  flows: []
  scope: zoom_commerce:write:admin
- description: View your knowledge bases and articles
  flows: []
  scope: zva:read:km_kbs
- description: View and manage your knowledge bases and articles
  flows: []
  scope: zva:write:km_kbs
- description: View zva engagements
  flows: []
  scope: zva_report:read
- description: Read Block List Rules
  flows: []
  scope: contact_center_block_list_rules:read:admin
- description: Create workforce management information
  flows: []
  scope: workforce_management:write:admin
- description: View workforce management information
  flows: []
  scope: workforce_management:read:admin
slug: visioconference-scopes
source_filename: visioconference-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/visioconference-openapi.yml\ndocs: https://developers.zoom.us/docs/integrations/oauth-scopes/\nschemes:\n- name: oauth2\n  source: openapi/visioconference-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://zoom.us/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://zoom.us/oauth/authorize\n    tokenUrl: https://zoom.us/oauth/token\n  description: OAuth 2.0 (server-to-server or user OAuth); access tokens valid for one hour\nscopes:\n- scope: account:master\n  description: View and manage sub accounts\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: account:read:admin\n  description: View account info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: account:write:admin\n  description: View and manage account info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: billing:master\n\
  \  description: View and manage sub account's billing info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: calendar:read\n  description: View calendar\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: calendar:read:admin\n  description: View calendar\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: calendar:write\n  description: Manage calendar\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: calendar:write:admin\n  description: Manage calendar\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat:read\n  description: View Chat Message Info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat:read:admin\n  description: View Chat Message Info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat:write\n  description: Manage Chat Message\
  \ Info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat:write:admin\n  description: Manage Chat Message Info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_channel:read\n  description: View current user's team chat channels\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_channel:read:admin\n  description: View all users' team chat channels\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_channel:read:member\n  description: View team chat channels as a member\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_channel:write\n  description: View and manage current user's team chat channels\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_channel:write:admin\n  description: View and manage all users' team chat channels\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: chat_contact:read\n  description: View current user's team chat contact information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_contact:write\n  description: Send Contact Invitation\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_contact:write:admin\n  description: Send contact invitation\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_event:write\n  description: Manage your chat event info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_event:write:admin\n  description: Manage account's chat event info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_history_legal_hold:read:admin\n  description: View Chat History Legal Hold Info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_history_legal_hold:write:admin\n  description:\
  \ Manage Chat History Legal Hold Info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_message:read\n  description: View current user's team chat messages\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_message:read:admin\n  description: View all users' team chat messages\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_message:write\n  description: View and manage current user's team chat messages\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_message:write:admin\n  description: View and manage all users' team chat messages\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_migration:read:admin\n  description: View information about a chat history migration\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: chat_migration:write:admin\n  description:\
  \ Migrate chat history from another vendor\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: imchat:bot\n  description: Enable Chatbot within Zoom Team Chat Client\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: imchat:read:admin\n  description: View all users history and channels\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: imchat:write\n  description: Send a team chat message to a Zoom Team Chat user or channel\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: clips:read\n  description: View your clips information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: clips:read:admin\n  description: View your clips information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: clips:write\n  description: Manage your clips information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: clips:write:admin\n  description: Manage your clips information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: apiconnector:master\n  description: This scope allows an app to view and manage sub account’s API Connector information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: apiconnector:read:admin\n  description: This scope allow an app to view all API Connector information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: apiconnector:write:admin\n  description: This scope allow an app to view and manage all API Connector information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: crc:master\n  description: View and manage sub account's CRC configuration\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: crc:read:admin\n  description: View and manage CRC configuration\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: crc_account:master\n  description: View and manage all sub account's Cisco/Polycom room account setting\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: crc_account:read:admin\n  description: View Cisco/Polycom rooms account setting\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: crc_account:write:admin\n  description: View and manage Cisco/Polycom rooms account setting\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: crc_rooms:master\n  description: View and manage sub account’s managed Cisco and Polycom rooms information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: crc_rooms:read:admin\n  description: View all managed Cisco and Polycom rooms information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: crc_rooms:write:admin\n  description: View and manage all managed Cisco and Polycom rooms\
  \ information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_attachment:read:admin\n  description: View your contact center attachment information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_block_list_rules:write:admin\n  description: Edit Block List Rules\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_flow:write:admin\n  description: flow write\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_follow_up_task:read:admin\n  description: View a follow-up task\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_follow_up_task:write\n  description: Update a follow-up task\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_messaging:read:admin\n  description: Get message\n  sources:\n\
  \  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_messaging:write:admin\n  description: send message\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign_dnc_list_phones:read:admin\n  description: Get campaign dnc list phone\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign_dnc_list_phones:write:admin\n  description: Write campaign dnc list phone\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_routing_profile:write:admin\n  description: Edit agent routing profile.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_rtms:write:admin\n  description: Scope to control RTMS\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_team:read:admin\n  description: View your contact\
  \ center team information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_team:write:admin\n  description: Manage your contact center team information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_user_template:read:admin\n  description: View all contact center user template’s details.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_user_template:write:admin\n  description: View and manage all contact center user template's details.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_asset_library:read:admin\n  description: View your contact center asset library information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_asset_library:write:admin\n  description: Manage your contact center asset library information\n  sources:\n\
  \  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_contact:read:admin\n  description: View address book information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_contact:write:admin\n  description: Update address book information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_disposition:read:admin\n  description: View your contact center disposition information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_disposition:write:admin\n  description: Manage your contact center disposition information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_engagement:read:admin\n  description: View all contact center engagement information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_engagement:write:admin\n\
  \  description: Manage all contact center engagement information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_flow:read:admin\n  description: View all contact center flow information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_inbox:read:admin\n  description: View all contact center inbox information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_inbox:write:admin\n  description: Manage all contact center inbox information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_note:read:admin\n  description: View all contact center note information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_note:write\n  description: Manage all contact center note information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: contact_center_operating_hours:read:admin\n  description: View all contact center operating hours information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_operating_hours:write:admin\n  description: Manage all contact center operating hours information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_operation_logs:read:admin\n  description: Read permission for Operation logs\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign:delete:admin\n  description: Delete an Outbound Campaign.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign:read:admin\n  description: View an Outbound Campaign.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign:update:admin\n  description: Update\
  \ an Outbound Campaign\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign:write:admin\n  description: Create an Outbound Campaign\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign_contactlist:read:admin\n  description: Get campaign contact list\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign_contactlist:write:admin\n  description: Create campaign contact list\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign_contacts:read:admin\n  description: Get campaign contact list contact\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_outbound_campaign_contacts:write:admin\n  description: Create campaign contact list contact\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: contact_center_preference:read:admin\n  description: View your contact center preference information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_preference:write:admin\n  description: Manage your contact center preference information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_queue:read:admin\n  description: View your contact center queue information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_queue:write:admin\n  description: Manage your contact center queue information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_recording:read\n  description: View your contact center recording information.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_recording:read:admin\n  description: View all contact center recording\
  \ information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_recording:write:admin\n  description: Manage all contact center recording information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_region:read:admin\n  description: View all contact center region information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_region:write:admin\n  description: Manage all contact center region information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_report:read:admin\n  description: View all contact center report information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_role:read:admin\n  description: View your contact center role information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_role:write:admin\n\
  \  description: Manage your contact center role information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_routing_profile:read:admin\n  description: View routing profile information.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_skill:read:admin\n  description: View all contact center skill information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_skill:write:admin\n  description: Manage all contact center skill information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_sms:master\n  description: View sub account’s SMS log information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_sms:read:admin\n  description: View all contact center SMS log information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: contact_center_user:read:admin\n  description: View all contact center user’s details\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_user:write:admin\n  description: View and manage all contact center user's details\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_variable:read:admin\n  description: View all contact center variable information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_variable:write:admin\n  description: Manage all contact center variable information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_variable_log:read:admin\n  description: View variable log information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_variable_log:write:admin\n  description: Manage variable log information\n  sources:\n\
  \  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_voice_call:master\n  description: View sub account’s voice call information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_center_voice_call:read:admin\n  description: view voice call information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact:read\n  description: View current user's contacts\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact:read:admin\n  description: View all users' contacts\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: dashboard:master\n  description: View sub account's Dashboard data\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: dashboard:read:admin\n  description: View Dashboard data\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope:\
  \ dashboard_crc:read:admin\n  description: View all users' usage statistics of CRC\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: dashboard_home:read:admin\n  description: View overview of usage statistics for Meetings and Zoom Rooms\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: dashboard_im:read:admin\n  description: View all users' usage statistics of team chat messages and message types\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: dashboard_meetings:read:admin\n  description: View all users' meetings information on Dashboard\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: dashboard_webinars:read:admin\n  description: View all users' webinar information on Dashboard\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: dashboard_zr:read:admin\n  description: View all users' Zoom Room usage statistics\
  \ and information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: device:read:admin\n  description: Manage device\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: device:write:admin\n  description: View and manage device\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: h323:master\n  description: View and manage sub account's H.323 devices\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: h323:read:admin\n  description: View all users' H.323 devices\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: h323:write:admin\n  description: View and manage all users' H.323 devices\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs:delete\n  description: Delete a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs:delete:admin\n  description:\
  \ Delete a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs:read:admin\n  description: Get basic info of the file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs:write:admin\n  description: Edit basic info of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_collaborator:delete\n  description: Remove collaborators of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_collaborator:delete:admin\n  description: Remove collaborators of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_collaborator:read\n  description: Get collaborators of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_collaborator:read:admin\n  description: Get collaborator of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: docs_collaborator:write\n  description: scope to manage collaborator in Docs\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_collaborator:write:admin\n  description: scope for admin to manage collaborators\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_export:read\n  description: Get file export status\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_export:read:admin\n  description: Get file export status\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_export:write\n  description: Create a file export\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_export:write:admin\n  description: Create a file export\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_file_owner:write\n  description: Transfer ownership of a file\n  sources:\n\
  \  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_file_owner:write:admin\n  description: Transfer ownership of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_file_uploads:write\n  description: Create a file upload\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_file_uploads:write:admin\n  description: Create a file upload\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_general_access:read\n  description: Get general access of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_general_access:read:admin\n  description: Get general access of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_general_access:write\n  description: Update general access of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: docs_general_access:write:admin\n  description: Update general access of a file\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_import:read\n  description: Get import task status\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_import:read:admin\n  description: Get import task status\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_import:write\n  description: Create new file by import\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: docs_import:write:admin\n  description: Create new file by import\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: group:master\n  description: View and manage sub account's groups\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: group:read:admin\n  description: View groups\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: group:write:admin\n  description: View and manage groups\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_group:read:admin\n  description: View all contact group information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: contact_group:write:admin\n  description: Manage all contact group information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: imgroup:master\n  description: View and manage sub account's Zoom Team Chat Groups\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: imgroup:read:admin\n  description: View Zoom Team Chat Group information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: imgroup:write:admin\n  description: View and manage Zoom Team Chat Groups\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: clinical_note:read:admin\n  description:\
  \ Read Clinical Notes\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: clinical_note:update:admin\n  description: Update Clinical Notes\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: mail:read\n  description: Read user’s own mailbox content.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: mail:read:admin\n  description: Read all mailboxes' content under the account, and account level settings.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: mail:write\n  description: Read and write user’s own mailbox content.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: mail:write:admin\n  description: Read and write all mailboxes' content under the account, and account level settings.\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: marketplace_app:master\n  description: View\
  \ and manage sub accounts' marketplace app info\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: marketplace_app:read\n  description: View your marketplace app information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: marketplace_app:read:admin\n  description: View marketplace app information for the account\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: marketplace_app:write\n  description: Edit marketplace app\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: marketplace_app:write:admin\n  description: View and Manage marketplace app information for the account\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: marketplace_custom_fields:read\n  description: Read custom field values\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: marketplace_custom_fields:read:admin\n\
  \  description: Read custom field values\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: marketplace_entitlement:read\n  description: View entitlements\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: marketplace_entitlement:read:admin\n  description: View entitlements\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: information_barriers:read:admin\n  description: View information barriers\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: information_barriers:read:master\n  description: View information barriers\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: information_barriers:write:admin\n  description: View and manage information barriers\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: information_barriers:write:master\n  description: View and manage information\
  \ barriers\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting:master\n  description: View and manage sub account's user meetings\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting:read\n  description: View your meetings\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting:read:admin\n  description: View all user meetings\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting:write\n  description: View and manage your meetings\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting:write:admin\n  description: View and manage all user meetings\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting:write:admin:sip_dialing\n  description: Get CRC dial string with passcode\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope:\
  \ meeting:write:sip_dialing\n  description: Get CRC dial string with passcode\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting_summary:master\n  description: View and manage sub account's user meeting summaries\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting_summary:read\n  description: View your meeting summaries\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting_summary:read:admin\n  description: View all user meeting summaries\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting_token:read:admin:live_streaming\n  description: View live streaming meeting token information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting_token:read:admin:local_archiving\n  description: View local archiving meeting token information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: meeting_token:read:admin:local_recording\n  description: This scope allows an app to view an account's users' local recording meeting token information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting_token:read:live_streaming\n  description: View live streaming meeting token information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: meeting_token:read:local_recording\n  description: This scope allows an app to view a user's local recording meeting token information\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: number_management_numbers:read:admin\n  description: View all phone number detail in \"Number Management\".\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n- scope: number_management_numbers:read:master\n  description: View and manage sub account's phone number detail in \"Number Management\".\n  sources:\n  - https://developers.zoom.us/docs/integrations/oauth-scopes/\n\
  - scope: number_management_numbers:write:admin\n  description: Manage phone number detail in \"Number Management\".\n  sources:\n  - ht\n\n# --- truncated at 32 KB (74 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/visioconference/refs/heads/main/scopes/visioconference-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visioconference/refs/heads/main/scopes/visioconference-scopes.yml
summary_line: 473 scopes · clientCredentials/authorizationCode
tags:
- Audio
- Chat
- Collaboration
- Communication
- Conferencing
- Live Streaming
- Real-Time
- Remote Work
- Screen Sharing
- Video
- WebRTC
token_urls:
- https://zoom.us/oauth/token
---
