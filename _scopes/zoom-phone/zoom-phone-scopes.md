---
api_specs:
- filename: zoom-phone-api-openapi.json
  format: json
  label: Zoom Phone API
  slug: zoom-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/openapi/zoom-phone-api-openapi.json
- filename: zoom-phone-webhooks-openapi.json
  format: json
  label: Zoom Phone Webhooks
  slug: zoom-phone-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/openapi/zoom-phone-webhooks-openapi.json
- filename: zoom-phone-number-management-openapi.json
  format: json
  label: Zoom Phone Number Management API
  slug: zoom-phone-number-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/openapi/zoom-phone-number-management-openapi.json
authorization_urls:
- /
description: ''
docs: https://developers.zoom.us/docs/integrations/oauth-scopes-granular/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Zoom Phone Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoom Phone publishes 435 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoom Phone API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoom Phone
provider_slug: zoom-phone
schemes:
- flows:
  - authorizationUrl: /
    flow: authorizationCode
  name: openapi_oauth
  source: openapi/zoom-phone-api-openapi.json
- flows:
  - authorizationUrl: /
    flow: authorizationCode
  name: openapi_oauth
  source: openapi/zoom-phone-number-management-openapi.json
scope_count: 435
scope_names:
- number_management:delete:numbers:admin
- number_management:delete:peering_number:admin
- number_management:delete:sms_consent:admin
- number_management:read:list_carrier_peering_numbers:admin
- number_management:read:list_numbers:admin
- number_management:read:list_peering_numbers:admin
- number_management:read:list_ported_numbers:admin
- number_management:read:list_sip_groups:admin
- number_management:read:list_sip_trunks:admin
- number_management:read:list_sms_campaigns:admin
- number_management:read:numbers:admin
- number_management:read:numbers_plan:admin
- number_management:read:ported_number:admin
- number_management:read:sms_campaign:admin
- number_management:read:sms_consent:admin
- number_management:update:numbers:admin
- number_management:update:peering_number:admin
- number_management:update:sms_consent:admin
- number_management:write:byoc_numbers:admin
- number_management:write:numbers:admin
- number_management:write:peering_number:admin
- number_management:write:sms_consent:admin
- number_management_numbers:read:admin
- number_management_numbers:write:admin
- number_management_numbers:write:master
- phone:delete:alert_setting:admin
- phone:delete:audio
- phone:delete:audio:admin
- phone:delete:auto_receptionist:admin
- phone:delete:auto_receptionist_number:admin
- phone:delete:auto_receptionist_policy:admin
- phone:delete:auto_receptionist_setting:admin
- phone:delete:blocked_list:admin
- phone:delete:call_handling_setting:admin
- phone:delete:call_log
- phone:delete:call_log:admin
- phone:delete:call_pickup_group:admin
- phone:delete:call_pickup_group_member:admin
- phone:delete:call_queue:admin
- phone:delete:call_queue_custom_group:admin
- phone:delete:call_queue_custom_group:master
- phone:delete:call_queue_custom_group_member:admin
- phone:delete:call_queue_member:admin
- phone:delete:call_queue_number:admin
- phone:delete:call_queue_policy:admin
- phone:delete:call_queue_setting:admin
- phone:delete:call_recording
- phone:delete:call_recording:admin
- phone:delete:carrier_number:admin
- phone:delete:common_area:admin
- phone:delete:common_area_calling_plan:admin
- phone:delete:common_area_number:admin
- phone:delete:common_area_outbound_calling_rule:admin
- phone:delete:common_area_setting:admin
- phone:delete:customized_number:admin
- phone:delete:device:admin
- phone:delete:device_extension:admin
- phone:delete:directory:admin
- phone:delete:emergency_address:admin
- phone:delete:emergency_location:admin
- phone:delete:extension_inbound_block_rule
- phone:delete:extension_inbound_block_rule:admin
- phone:delete:extension_inbound_block_rule_stat:admin
- phone:delete:external_contact:admin
- phone:delete:fax_log
- phone:delete:fax_log:admin
- phone:delete:firmware_update_rule:admin
- phone:delete:inbound_block_rule:admin
- phone:delete:line_keys
- phone:delete:line_keys:admin
- phone:delete:monitoring_group:admin
- phone:delete:monitoring_group_member:admin
- phone:delete:number:admin
- phone:delete:outbound_calling_rule:admin
- phone:delete:peering_number:admin
- phone:delete:private_directory_member:admin
- phone:delete:provision_template:admin
- phone:delete:role:admin
- phone:delete:role_member:admin
- phone:delete:room:admin
- phone:delete:room_calling_plan:admin
- phone:delete:room_phone_number:admin
- phone:delete:routing_rule:admin
- phone:delete:shared_line_group:admin
- phone:delete:shared_line_group_number:admin
- phone:delete:shared_line_group_policy:admin
- phone:delete:shared_line_group_setting:admin
- phone:delete:shared_line_member:admin
- phone:delete:shared_setting
- phone:delete:shared_setting:admin
- phone:delete:site:admin
- phone:delete:site_customized_number:admin
- phone:delete:site_outbound_calling_rule:admin
- phone:delete:site_setting:admin
- phone:delete:sms_campaign_number:admin
- phone:delete:user_call_handling_setting
- phone:delete:user_call_handling_setting:admin
- phone:delete:user_customized_number
- phone:delete:user_customized_number:admin
- phone:delete:user_number
- phone:delete:user_number:admin
- phone:delete:user_outbound_calling_rule:admin
- phone:delete:user_setting
- phone:delete:user_setting:admin
- phone:delete:users_calling_plan
- phone:delete:users_calling_plan:admin
- phone:delete:voicemail
- phone:delete:voicemail:admin
- phone:master
- phone:patch:alert_setting:admin
- phone:read
- phone:read:admin
- phone:read:ai_call_summary
- phone:read:ai_call_summary:admin
- phone:read:alert_setting:admin
- phone:read:audio
- phone:read:audio:admin
- phone:read:auto_receptionist:admin
- phone:read:auto_receptionist_call_handling_setting:admin
- phone:read:auto_receptionist_ivr:admin
- phone:read:auto_receptionist_policy:admin
- phone:read:auto_receptionist_setting:admin
- phone:read:billing_account:admin
- phone:read:blocked_list:admin
- phone:read:call_charges:admin
- phone:read:call_log:admin
- phone:read:call_pickup_group:admin
- phone:read:call_pickup_group_member:admin
- phone:read:call_qos:admin
- phone:read:call_queue:admin
- phone:read:call_queue_call_handling_setting:admin
- phone:read:call_queue_custom_group:admin
- phone:read:call_queue_custom_group:master
- phone:read:call_queue_policy:admin
- phone:read:call_queue_setting:admin
- phone:read:call_recording
- phone:read:call_recording:admin
- phone:read:common_area:admin
- phone:read:common_area_call_handling_setting:admin
- phone:read:common_area_outbound_calling_rule:admin
- phone:read:default_emergency_address:admin
- phone:read:detectable_personal_location:admin
- phone:read:device:admin
- phone:read:device_line_keys
- phone:read:device_line_keys:admin
- phone:read:directory:admin
- phone:read:emergency_address:admin
- phone:read:emergency_location:admin
- phone:read:external_contact:admin
- phone:read:fax_charges:admin
- phone:read:fax_log
- phone:read:fax_log:admin
- phone:read:firmware_update_rule:admin
- phone:read:group_policy:admin
- phone:read:group_setting:admin
- phone:read:line_keys
- phone:read:line_keys:admin
- phone:read:list_account_settings:admin
- phone:read:list_alert_settings:admin
- phone:read:list_audios
- phone:read:list_audios:admin
- phone:read:list_auto_receptionists:admin
- phone:read:list_billing_accounts:admin
- phone:read:list_blocked_lists:admin
- phone:read:list_call_handling_settings:admin
- phone:read:list_call_logs
- phone:read:list_call_logs:admin
- phone:read:list_call_pickup_groups:admin
- phone:read:list_call_queue_members:admin
- phone:read:list_call_queue_recordings:admin
- phone:read:list_call_queues:admin
- phone:read:list_call_recordings:admin
- phone:read:list_calling_plans:admin
- phone:read:list_carrier_numbers:admin
- phone:read:list_common_area_activation_codes:admin
- phone:read:list_common_area_settings:admin
- phone:read:list_customized_number:admin
- phone:read:list_devices:admin
- phone:read:list_emergency_addresses:admin
- phone:read:list_emergency_locations:admin
- phone:read:list_extension_inbound_block_rules
- phone:read:list_extension_inbound_block_rules:admin
- phone:read:list_extension_inbound_block_rules_stat:admin
- phone:read:list_external_contacts:admin
- phone:read:list_fax_log
- phone:read:list_fax_log:admin
- phone:read:list_firmware_update_rules:admin
- phone:read:list_firmwares:admin
- phone:read:list_inbound_block_rules:admin
- phone:read:list_monitoring_group_members:admin
- phone:read:list_monitoring_groups:admin
- phone:read:list_numbers:admin
- phone:read:list_outbound_calling_rules:admin
- phone:read:list_peering_numbers:admin
- phone:read:list_ported_numbers:admin
- phone:read:list_private_directory_members:admin
- phone:read:list_provision_templates:admin
- phone:read:list_recordings
- phone:read:list_recordings:admin
- phone:read:list_roles:admin
- phone:read:list_rooms:admin
- phone:read:list_routing_rules:admin
- phone:read:list_setting_templates:admin
- phone:read:list_shared_line_appearances:admin
- phone:read:list_shared_line_groups:admin
- phone:read:list_sip_groups:admin
- phone:read:list_sip_trunks:admin
- phone:read:list_site_customized_number:admin
- phone:read:list_sites:admin
- phone:read:list_sms_campaigns:admin
- phone:read:list_sms_sessions
- phone:read:list_sms_sessions:admin
- phone:read:list_tracked_locations:admin
- phone:read:list_user_customized_number
- phone:read:list_user_customized_number:admin
- phone:read:list_users:admin
- phone:read:list_voicemails
- phone:read:list_voicemails:admin
- phone:read:location_sharing_permission:admin
- phone:read:monitoring_group:admin
- phone:read:nomadic_emergency_services:admin
- phone:read:numbers:admin
- phone:read:operation_logs:admin
- phone:read:policy:admin
- phone:read:ported_number:admin
- phone:read:provision_template:admin
- phone:read:realtime_location_devices:admin
- phone:read:realtime_location_users:admin
- phone:read:recording_transcript
- phone:read:recording_transcript:admin
- phone:read:role:admin
- phone:read:role_member:admin
- phone:read:room:admin
- phone:read:routing_rule:admin
- phone:read:setting_template:admin
- phone:read:settings:admin
- phone:read:shared_line_group:admin
- phone:read:shared_line_group_call_handling_setting:admin
- phone:read:shared_line_group_policy:admin
- phone:read:shared_line_group_setting:admin
- phone:read:site:admin
- phone:read:site_outbound_calling_rule:admin
- phone:read:site_setting:admin
- phone:read:sms_campaign:admin
- phone:read:sms_campaign_number_opt_status
- phone:read:sms_campaign_number_opt_status:admin
- phone:read:sms_charges:admin
- phone:read:sms_consent_number_opt_status:admin
- phone:read:sms_message
- phone:read:sms_message:admin
- phone:read:sms_session
- phone:read:sms_session:admin
- phone:read:user
- phone:read:user:admin
- phone:read:user_call_handling_setting
- phone:read:user_call_handling_setting:admin
- phone:read:user_outbound_calling_rule:admin
- phone:read:user_policy:admin
- phone:read:user_setting
- phone:read:user_setting:admin
- phone:read:voicemail
- phone:read:voicemail:admin
- phone:update:audio
- phone:update:audio:admin
- phone:update:auto_receptionist:admin
- phone:update:auto_receptionist_call_handling_setting:admin
- phone:update:auto_receptionist_ivr:admin
- phone:update:auto_receptionist_policy:admin
- phone:update:auto_receptionist_setting:admin
- phone:update:batch_users:admin
- phone:update:blocked_list:admin
- phone:update:call_handling_setting:admin
- phone:update:call_log:admin
- phone:update:call_pickup_group:admin
- phone:update:call_queue:admin
- phone:update:call_queue_call_handling_setting:admin
- phone:update:call_queue_custom_group:admin
- phone:update:call_queue_policy:admin
- phone:update:call_queue_setting:admin
- phone:update:call_recording
- phone:update:call_recording:admin
- phone:update:calling_plan
- phone:update:calling_plan:admin
- phone:update:carrier_number:admin
- phone:update:common_area:admin
- phone:update:common_area_call_handling_setting:admin
- phone:update:common_area_outbound_calling_rule:admin
- phone:update:common_area_setting:admin
- phone:update:device:admin
- phone:update:device_line_keys
- phone:update:device_line_keys:admin
- phone:update:device_provision_template:admin
- phone:update:emergency_address:admin
- phone:update:emergency_location:admin
- phone:update:external_contact:admin
- phone:update:firmware_update_rule:admin
- phone:update:group_policy:admin
- phone:update:inbound_block_rule:admin
- phone:update:inbound_blocked_for_all:admin
- phone:update:line_keys
- phone:update:line_keys:admin
- phone:update:monitoring_group:admin
- phone:update:number:admin
- phone:update:outbound_calling_rule:admin
- phone:update:peering_number:admin
- phone:update:policy:admin
- phone:update:private_directory_member:admin
- phone:update:provision_template:admin
- phone:update:role:admin
- phone:update:room:admin
- phone:update:routing_rule:admin
- phone:update:setting_template:admin
- phone:update:settings:admin
- phone:update:shared_line_group:admin
- phone:update:shared_line_group_call_handling_setting:admin
- phone:update:shared_line_group_policy:admin
- phone:update:shared_line_group_setting:admin
- phone:update:shared_setting
- phone:update:shared_setting:admin
- phone:update:site:admin
- phone:update:site_number:admin
- phone:update:site_outbound_calling_rule:admin
- phone:update:site_setting:admin
- phone:update:sms_campaign_number_opt_status:admin
- phone:update:user
- phone:update:user:admin
- phone:update:user_call_handling_setting
- phone:update:user_call_handling_setting:admin
- phone:update:user_outbound_calling_rule:admin
- phone:update:user_policy:admin
- phone:update:user_setting
- phone:update:user_setting:admin
- phone:update:voicemail
- phone:update:voicemail:admin
- phone:write
- phone:write:admin
- phone:write:alert_setting:admin
- phone:write:apply_template_to_common_areas:admin
- phone:write:audio
- phone:write:audio:admin
- phone:write:auto_receptionist:admin
- phone:write:auto_receptionist_number:admin
- phone:write:auto_receptionist_policy:admin
- phone:write:auto_receptionist_setting:admin
- phone:write:batch_audios
- phone:write:batch_audios:admin
- phone:write:batch_emergency_locations:admin
- phone:write:batch_users:admin
- phone:write:blocked_list:admin
- phone:write:byo_carrier_number:admin
- phone:write:call_handling_setting:admin
- phone:write:call_pickup_group:admin
- phone:write:call_pickup_group_member:admin
- phone:write:call_queue:admin
- phone:write:call_queue_custom_group:admin
- phone:write:call_queue_custom_group_member:admin
- phone:write:call_queue_member:admin
- phone:write:call_queue_number:admin
- phone:write:call_queue_policy:admin
- phone:write:call_queue_setting:admin
- phone:write:calling_plan
- phone:write:calling_plan:admin
- phone:write:carrier_number:admin
- phone:write:common_area:admin
- phone:write:common_area_calling_plan:admin
- phone:write:common_area_number:admin
- phone:write:common_area_outbound_calling_rule:admin
- phone:write:common_area_setting:admin
- phone:write:customized_number:admin
- phone:write:device:admin
- phone:write:device_extension:admin
- phone:write:directory:admin
- phone:write:emergency_address:admin
- phone:write:emergency_location:admin
- phone:write:extension_inbound_block_rule
- phone:write:extension_inbound_block_rule:admin
- phone:write:external_contact:admin
- phone:write:firmware_update_rule:admin
- phone:write:inbound_block_rule:admin
- phone:write:monitoring_group:admin
- phone:write:monitoring_group_member:admin
- phone:write:outbound_calling_rule:admin
- phone:write:peering_number:admin
- phone:write:private_directory_member:admin
- phone:write:provision_template:admin
- phone:write:reboot_device:admin
- phone:write:role:admin
- phone:write:role_member:admin
- phone:write:room:admin
- phone:write:room_calling_plan:admin
- phone:write:room_phone_number:admin
- phone:write:routing_rule:admin
- phone:write:send_fax
- phone:write:send_fax:admin
- phone:write:setting_template:admin
- phone:write:shared_line_group:admin
- phone:write:shared_line_group_number:admin
- phone:write:shared_line_group_policy:admin
- phone:write:shared_line_group_setting:admin
- phone:write:shared_line_member:admin
- phone:write:shared_setting
- phone:write:shared_setting:admin
- phone:write:site:admin
- phone:write:site_customized_number:admin
- phone:write:site_outbound_calling_rule:admin
- phone:write:site_setting:admin
- phone:write:sms_campaign_number:admin
- phone:write:sync_device:admin
- phone:write:user_call_handling_setting
- phone:write:user_call_handling_setting:admin
- phone:write:user_customized_number
- phone:write:user_customized_number:admin
- phone:write:user_number
- phone:write:user_number:admin
- phone:write:user_outbound_calling_rule:admin
- phone:write:user_setting
- phone:write:user_setting:admin
- phone_call_log:read
- phone_call_log:read:admin
- phone_call_log:write
- phone_call_log:write:admin
- phone_peering:read:admin
- phone_peering:write:admin
- phone_recording:read
- phone_recording:read:admin
- phone_recording:write
- phone_recording:write:admin
- phone_sms:read
- phone_sms:read:admin
- phone_sms:write
- phone_sms:write:admin
- phone_voicemail:read
- phone_voicemail:read:admin
- phone_voicemail:write
- phone_voicemail:write:admin
scopes:
- description: number_management:delete:numbers:admin
  flows:
  - authorizationCode
  scope: number_management:delete:numbers:admin
- description: number_management:delete:peering_number:admin
  flows:
  - authorizationCode
  scope: number_management:delete:peering_number:admin
- description: number_management:delete:sms_consent:admin
  flows:
  - authorizationCode
  scope: number_management:delete:sms_consent:admin
- description: number_management:read:list_carrier_peering_numbers:admin
  flows:
  - authorizationCode
  scope: number_management:read:list_carrier_peering_numbers:admin
- description: number_management:read:list_numbers:admin
  flows:
  - authorizationCode
  scope: number_management:read:list_numbers:admin
- description: number_management:read:list_peering_numbers:admin
  flows:
  - authorizationCode
  scope: number_management:read:list_peering_numbers:admin
- description: number_management:read:list_ported_numbers:admin
  flows:
  - authorizationCode
  scope: number_management:read:list_ported_numbers:admin
- description: number_management:read:list_sip_groups:admin
  flows:
  - authorizationCode
  scope: number_management:read:list_sip_groups:admin
- description: number_management:read:list_sip_trunks:admin
  flows:
  - authorizationCode
  scope: number_management:read:list_sip_trunks:admin
- description: number_management:read:list_sms_campaigns:admin
  flows:
  - authorizationCode
  scope: number_management:read:list_sms_campaigns:admin
- description: number_management:read:numbers:admin
  flows:
  - authorizationCode
  scope: number_management:read:numbers:admin
- description: number_management:read:numbers_plan:admin
  flows:
  - authorizationCode
  scope: number_management:read:numbers_plan:admin
- description: number_management:read:ported_number:admin
  flows:
  - authorizationCode
  scope: number_management:read:ported_number:admin
- description: number_management:read:sms_campaign:admin
  flows:
  - authorizationCode
  scope: number_management:read:sms_campaign:admin
- description: number_management:read:sms_consent:admin
  flows:
  - authorizationCode
  scope: number_management:read:sms_consent:admin
- description: number_management:update:numbers:admin
  flows:
  - authorizationCode
  scope: number_management:update:numbers:admin
- description: number_management:update:peering_number:admin
  flows:
  - authorizationCode
  scope: number_management:update:peering_number:admin
- description: number_management:update:sms_consent:admin
  flows:
  - authorizationCode
  scope: number_management:update:sms_consent:admin
- description: number_management:write:byoc_numbers:admin
  flows:
  - authorizationCode
  scope: number_management:write:byoc_numbers:admin
- description: number_management:write:numbers:admin
  flows:
  - authorizationCode
  scope: number_management:write:numbers:admin
- description: number_management:write:peering_number:admin
  flows:
  - authorizationCode
  scope: number_management:write:peering_number:admin
- description: number_management:write:sms_consent:admin
  flows:
  - authorizationCode
  scope: number_management:write:sms_consent:admin
- description: number_management_numbers:read:admin
  flows:
  - authorizationCode
  scope: number_management_numbers:read:admin
- description: number_management_numbers:write:admin
  flows:
  - authorizationCode
  scope: number_management_numbers:write:admin
- description: number_management_numbers:write:master
  flows:
  - authorizationCode
  scope: number_management_numbers:write:master
- description: phone:delete:alert_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:alert_setting:admin
- description: phone:delete:audio
  flows:
  - authorizationCode
  scope: phone:delete:audio
- description: phone:delete:audio:admin
  flows:
  - authorizationCode
  scope: phone:delete:audio:admin
- description: phone:delete:auto_receptionist:admin
  flows:
  - authorizationCode
  scope: phone:delete:auto_receptionist:admin
- description: phone:delete:auto_receptionist_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:auto_receptionist_number:admin
- description: phone:delete:auto_receptionist_policy:admin
  flows:
  - authorizationCode
  scope: phone:delete:auto_receptionist_policy:admin
- description: phone:delete:auto_receptionist_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:auto_receptionist_setting:admin
- description: phone:delete:blocked_list:admin
  flows:
  - authorizationCode
  scope: phone:delete:blocked_list:admin
- description: phone:delete:call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_handling_setting:admin
- description: phone:delete:call_log
  flows:
  - authorizationCode
  scope: phone:delete:call_log
- description: phone:delete:call_log:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_log:admin
- description: phone:delete:call_pickup_group:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_pickup_group:admin
- description: phone:delete:call_pickup_group_member:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_pickup_group_member:admin
- description: phone:delete:call_queue:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_queue:admin
- description: phone:delete:call_queue_custom_group:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_queue_custom_group:admin
- description: phone:delete:call_queue_custom_group:master
  flows:
  - authorizationCode
  scope: phone:delete:call_queue_custom_group:master
- description: phone:delete:call_queue_custom_group_member:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_queue_custom_group_member:admin
- description: phone:delete:call_queue_member:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_queue_member:admin
- description: phone:delete:call_queue_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_queue_number:admin
- description: phone:delete:call_queue_policy:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_queue_policy:admin
- description: phone:delete:call_queue_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_queue_setting:admin
- description: phone:delete:call_recording
  flows:
  - authorizationCode
  scope: phone:delete:call_recording
- description: phone:delete:call_recording:admin
  flows:
  - authorizationCode
  scope: phone:delete:call_recording:admin
- description: phone:delete:carrier_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:carrier_number:admin
- description: phone:delete:common_area:admin
  flows:
  - authorizationCode
  scope: phone:delete:common_area:admin
- description: phone:delete:common_area_calling_plan:admin
  flows:
  - authorizationCode
  scope: phone:delete:common_area_calling_plan:admin
- description: phone:delete:common_area_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:common_area_number:admin
- description: phone:delete:common_area_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:delete:common_area_outbound_calling_rule:admin
- description: phone:delete:common_area_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:common_area_setting:admin
- description: phone:delete:customized_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:customized_number:admin
- description: phone:delete:device:admin
  flows:
  - authorizationCode
  scope: phone:delete:device:admin
- description: phone:delete:device_extension:admin
  flows:
  - authorizationCode
  scope: phone:delete:device_extension:admin
- description: phone:delete:directory:admin
  flows:
  - authorizationCode
  scope: phone:delete:directory:admin
- description: phone:delete:emergency_address:admin
  flows:
  - authorizationCode
  scope: phone:delete:emergency_address:admin
- description: phone:delete:emergency_location:admin
  flows:
  - authorizationCode
  scope: phone:delete:emergency_location:admin
- description: phone:delete:extension_inbound_block_rule
  flows:
  - authorizationCode
  scope: phone:delete:extension_inbound_block_rule
- description: phone:delete:extension_inbound_block_rule:admin
  flows:
  - authorizationCode
  scope: phone:delete:extension_inbound_block_rule:admin
- description: phone:delete:extension_inbound_block_rule_stat:admin
  flows:
  - authorizationCode
  scope: phone:delete:extension_inbound_block_rule_stat:admin
- description: phone:delete:external_contact:admin
  flows:
  - authorizationCode
  scope: phone:delete:external_contact:admin
- description: phone:delete:fax_log
  flows:
  - authorizationCode
  scope: phone:delete:fax_log
- description: phone:delete:fax_log:admin
  flows:
  - authorizationCode
  scope: phone:delete:fax_log:admin
- description: phone:delete:firmware_update_rule:admin
  flows:
  - authorizationCode
  scope: phone:delete:firmware_update_rule:admin
- description: phone:delete:inbound_block_rule:admin
  flows:
  - authorizationCode
  scope: phone:delete:inbound_block_rule:admin
- description: phone:delete:line_keys
  flows:
  - authorizationCode
  scope: phone:delete:line_keys
- description: phone:delete:line_keys:admin
  flows:
  - authorizationCode
  scope: phone:delete:line_keys:admin
- description: phone:delete:monitoring_group:admin
  flows:
  - authorizationCode
  scope: phone:delete:monitoring_group:admin
- description: phone:delete:monitoring_group_member:admin
  flows:
  - authorizationCode
  scope: phone:delete:monitoring_group_member:admin
- description: phone:delete:number:admin
  flows:
  - authorizationCode
  scope: phone:delete:number:admin
- description: phone:delete:outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:delete:outbound_calling_rule:admin
- description: phone:delete:peering_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:peering_number:admin
- description: phone:delete:private_directory_member:admin
  flows:
  - authorizationCode
  scope: phone:delete:private_directory_member:admin
- description: phone:delete:provision_template:admin
  flows:
  - authorizationCode
  scope: phone:delete:provision_template:admin
- description: phone:delete:role:admin
  flows:
  - authorizationCode
  scope: phone:delete:role:admin
- description: phone:delete:role_member:admin
  flows:
  - authorizationCode
  scope: phone:delete:role_member:admin
- description: phone:delete:room:admin
  flows:
  - authorizationCode
  scope: phone:delete:room:admin
- description: phone:delete:room_calling_plan:admin
  flows:
  - authorizationCode
  scope: phone:delete:room_calling_plan:admin
- description: phone:delete:room_phone_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:room_phone_number:admin
- description: phone:delete:routing_rule:admin
  flows:
  - authorizationCode
  scope: phone:delete:routing_rule:admin
- description: phone:delete:shared_line_group:admin
  flows:
  - authorizationCode
  scope: phone:delete:shared_line_group:admin
- description: phone:delete:shared_line_group_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:shared_line_group_number:admin
- description: phone:delete:shared_line_group_policy:admin
  flows:
  - authorizationCode
  scope: phone:delete:shared_line_group_policy:admin
- description: phone:delete:shared_line_group_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:shared_line_group_setting:admin
- description: phone:delete:shared_line_member:admin
  flows:
  - authorizationCode
  scope: phone:delete:shared_line_member:admin
- description: phone:delete:shared_setting
  flows:
  - authorizationCode
  scope: phone:delete:shared_setting
- description: phone:delete:shared_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:shared_setting:admin
- description: phone:delete:site:admin
  flows:
  - authorizationCode
  scope: phone:delete:site:admin
- description: phone:delete:site_customized_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:site_customized_number:admin
- description: phone:delete:site_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:delete:site_outbound_calling_rule:admin
- description: phone:delete:site_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:site_setting:admin
- description: phone:delete:sms_campaign_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:sms_campaign_number:admin
- description: phone:delete:user_call_handling_setting
  flows:
  - authorizationCode
  scope: phone:delete:user_call_handling_setting
- description: phone:delete:user_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:user_call_handling_setting:admin
- description: phone:delete:user_customized_number
  flows:
  - authorizationCode
  scope: phone:delete:user_customized_number
- description: phone:delete:user_customized_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:user_customized_number:admin
- description: phone:delete:user_number
  flows:
  - authorizationCode
  scope: phone:delete:user_number
- description: phone:delete:user_number:admin
  flows:
  - authorizationCode
  scope: phone:delete:user_number:admin
- description: phone:delete:user_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:delete:user_outbound_calling_rule:admin
- description: phone:delete:user_setting
  flows:
  - authorizationCode
  scope: phone:delete:user_setting
- description: phone:delete:user_setting:admin
  flows:
  - authorizationCode
  scope: phone:delete:user_setting:admin
- description: phone:delete:users_calling_plan
  flows:
  - authorizationCode
  scope: phone:delete:users_calling_plan
- description: phone:delete:users_calling_plan:admin
  flows:
  - authorizationCode
  scope: phone:delete:users_calling_plan:admin
- description: phone:delete:voicemail
  flows:
  - authorizationCode
  scope: phone:delete:voicemail
- description: phone:delete:voicemail:admin
  flows:
  - authorizationCode
  scope: phone:delete:voicemail:admin
- description: phone:master
  flows:
  - authorizationCode
  scope: phone:master
- description: phone:patch:alert_setting:admin
  flows:
  - authorizationCode
  scope: phone:patch:alert_setting:admin
- description: phone:read
  flows:
  - authorizationCode
  scope: phone:read
- description: phone:read:admin
  flows:
  - authorizationCode
  scope: phone:read:admin
- description: phone:read:ai_call_summary
  flows:
  - authorizationCode
  scope: phone:read:ai_call_summary
- description: phone:read:ai_call_summary:admin
  flows:
  - authorizationCode
  scope: phone:read:ai_call_summary:admin
- description: phone:read:alert_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:alert_setting:admin
- description: phone:read:audio
  flows:
  - authorizationCode
  scope: phone:read:audio
- description: phone:read:audio:admin
  flows:
  - authorizationCode
  scope: phone:read:audio:admin
- description: phone:read:auto_receptionist:admin
  flows:
  - authorizationCode
  scope: phone:read:auto_receptionist:admin
- description: phone:read:auto_receptionist_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:auto_receptionist_call_handling_setting:admin
- description: phone:read:auto_receptionist_ivr:admin
  flows:
  - authorizationCode
  scope: phone:read:auto_receptionist_ivr:admin
- description: phone:read:auto_receptionist_policy:admin
  flows:
  - authorizationCode
  scope: phone:read:auto_receptionist_policy:admin
- description: phone:read:auto_receptionist_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:auto_receptionist_setting:admin
- description: phone:read:billing_account:admin
  flows:
  - authorizationCode
  scope: phone:read:billing_account:admin
- description: phone:read:blocked_list:admin
  flows:
  - authorizationCode
  scope: phone:read:blocked_list:admin
- description: phone:read:call_charges:admin
  flows:
  - authorizationCode
  scope: phone:read:call_charges:admin
- description: phone:read:call_log:admin
  flows:
  - authorizationCode
  scope: phone:read:call_log:admin
- description: phone:read:call_pickup_group:admin
  flows:
  - authorizationCode
  scope: phone:read:call_pickup_group:admin
- description: phone:read:call_pickup_group_member:admin
  flows:
  - authorizationCode
  scope: phone:read:call_pickup_group_member:admin
- description: phone:read:call_qos:admin
  flows:
  - authorizationCode
  scope: phone:read:call_qos:admin
- description: phone:read:call_queue:admin
  flows:
  - authorizationCode
  scope: phone:read:call_queue:admin
- description: phone:read:call_queue_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:call_queue_call_handling_setting:admin
- description: phone:read:call_queue_custom_group:admin
  flows:
  - authorizationCode
  scope: phone:read:call_queue_custom_group:admin
- description: phone:read:call_queue_custom_group:master
  flows:
  - authorizationCode
  scope: phone:read:call_queue_custom_group:master
- description: phone:read:call_queue_policy:admin
  flows:
  - authorizationCode
  scope: phone:read:call_queue_policy:admin
- description: phone:read:call_queue_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:call_queue_setting:admin
- description: phone:read:call_recording
  flows:
  - authorizationCode
  scope: phone:read:call_recording
- description: phone:read:call_recording:admin
  flows:
  - authorizationCode
  scope: phone:read:call_recording:admin
- description: phone:read:common_area:admin
  flows:
  - authorizationCode
  scope: phone:read:common_area:admin
- description: phone:read:common_area_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:common_area_call_handling_setting:admin
- description: phone:read:common_area_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:read:common_area_outbound_calling_rule:admin
- description: phone:read:default_emergency_address:admin
  flows:
  - authorizationCode
  scope: phone:read:default_emergency_address:admin
- description: phone:read:detectable_personal_location:admin
  flows:
  - authorizationCode
  scope: phone:read:detectable_personal_location:admin
- description: phone:read:device:admin
  flows:
  - authorizationCode
  scope: phone:read:device:admin
- description: phone:read:device_line_keys
  flows:
  - authorizationCode
  scope: phone:read:device_line_keys
- description: phone:read:device_line_keys:admin
  flows:
  - authorizationCode
  scope: phone:read:device_line_keys:admin
- description: phone:read:directory:admin
  flows:
  - authorizationCode
  scope: phone:read:directory:admin
- description: phone:read:emergency_address:admin
  flows:
  - authorizationCode
  scope: phone:read:emergency_address:admin
- description: phone:read:emergency_location:admin
  flows:
  - authorizationCode
  scope: phone:read:emergency_location:admin
- description: phone:read:external_contact:admin
  flows:
  - authorizationCode
  scope: phone:read:external_contact:admin
- description: phone:read:fax_charges:admin
  flows:
  - authorizationCode
  scope: phone:read:fax_charges:admin
- description: phone:read:fax_log
  flows:
  - authorizationCode
  scope: phone:read:fax_log
- description: phone:read:fax_log:admin
  flows:
  - authorizationCode
  scope: phone:read:fax_log:admin
- description: phone:read:firmware_update_rule:admin
  flows:
  - authorizationCode
  scope: phone:read:firmware_update_rule:admin
- description: phone:read:group_policy:admin
  flows:
  - authorizationCode
  scope: phone:read:group_policy:admin
- description: phone:read:group_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:group_setting:admin
- description: phone:read:line_keys
  flows:
  - authorizationCode
  scope: phone:read:line_keys
- description: phone:read:line_keys:admin
  flows:
  - authorizationCode
  scope: phone:read:line_keys:admin
- description: phone:read:list_account_settings:admin
  flows:
  - authorizationCode
  scope: phone:read:list_account_settings:admin
- description: phone:read:list_alert_settings:admin
  flows:
  - authorizationCode
  scope: phone:read:list_alert_settings:admin
- description: phone:read:list_audios
  flows:
  - authorizationCode
  scope: phone:read:list_audios
- description: phone:read:list_audios:admin
  flows:
  - authorizationCode
  scope: phone:read:list_audios:admin
- description: phone:read:list_auto_receptionists:admin
  flows:
  - authorizationCode
  scope: phone:read:list_auto_receptionists:admin
- description: phone:read:list_billing_accounts:admin
  flows:
  - authorizationCode
  scope: phone:read:list_billing_accounts:admin
- description: phone:read:list_blocked_lists:admin
  flows:
  - authorizationCode
  scope: phone:read:list_blocked_lists:admin
- description: phone:read:list_call_handling_settings:admin
  flows:
  - authorizationCode
  scope: phone:read:list_call_handling_settings:admin
- description: phone:read:list_call_logs
  flows:
  - authorizationCode
  scope: phone:read:list_call_logs
- description: phone:read:list_call_logs:admin
  flows:
  - authorizationCode
  scope: phone:read:list_call_logs:admin
- description: phone:read:list_call_pickup_groups:admin
  flows:
  - authorizationCode
  scope: phone:read:list_call_pickup_groups:admin
- description: phone:read:list_call_queue_members:admin
  flows:
  - authorizationCode
  scope: phone:read:list_call_queue_members:admin
- description: phone:read:list_call_queue_recordings:admin
  flows:
  - authorizationCode
  scope: phone:read:list_call_queue_recordings:admin
- description: phone:read:list_call_queues:admin
  flows:
  - authorizationCode
  scope: phone:read:list_call_queues:admin
- description: phone:read:list_call_recordings:admin
  flows:
  - authorizationCode
  scope: phone:read:list_call_recordings:admin
- description: phone:read:list_calling_plans:admin
  flows:
  - authorizationCode
  scope: phone:read:list_calling_plans:admin
- description: phone:read:list_carrier_numbers:admin
  flows:
  - authorizationCode
  scope: phone:read:list_carrier_numbers:admin
- description: phone:read:list_common_area_activation_codes:admin
  flows:
  - authorizationCode
  scope: phone:read:list_common_area_activation_codes:admin
- description: phone:read:list_common_area_settings:admin
  flows:
  - authorizationCode
  scope: phone:read:list_common_area_settings:admin
- description: phone:read:list_customized_number:admin
  flows:
  - authorizationCode
  scope: phone:read:list_customized_number:admin
- description: phone:read:list_devices:admin
  flows:
  - authorizationCode
  scope: phone:read:list_devices:admin
- description: phone:read:list_emergency_addresses:admin
  flows:
  - authorizationCode
  scope: phone:read:list_emergency_addresses:admin
- description: phone:read:list_emergency_locations:admin
  flows:
  - authorizationCode
  scope: phone:read:list_emergency_locations:admin
- description: phone:read:list_extension_inbound_block_rules
  flows:
  - authorizationCode
  scope: phone:read:list_extension_inbound_block_rules
- description: phone:read:list_extension_inbound_block_rules:admin
  flows:
  - authorizationCode
  scope: phone:read:list_extension_inbound_block_rules:admin
- description: phone:read:list_extension_inbound_block_rules_stat:admin
  flows:
  - authorizationCode
  scope: phone:read:list_extension_inbound_block_rules_stat:admin
- description: phone:read:list_external_contacts:admin
  flows:
  - authorizationCode
  scope: phone:read:list_external_contacts:admin
- description: phone:read:list_fax_log
  flows:
  - authorizationCode
  scope: phone:read:list_fax_log
- description: phone:read:list_fax_log:admin
  flows:
  - authorizationCode
  scope: phone:read:list_fax_log:admin
- description: phone:read:list_firmware_update_rules:admin
  flows:
  - authorizationCode
  scope: phone:read:list_firmware_update_rules:admin
- description: phone:read:list_firmwares:admin
  flows:
  - authorizationCode
  scope: phone:read:list_firmwares:admin
- description: phone:read:list_inbound_block_rules:admin
  flows:
  - authorizationCode
  scope: phone:read:list_inbound_block_rules:admin
- description: phone:read:list_monitoring_group_members:admin
  flows:
  - authorizationCode
  scope: phone:read:list_monitoring_group_members:admin
- description: phone:read:list_monitoring_groups:admin
  flows:
  - authorizationCode
  scope: phone:read:list_monitoring_groups:admin
- description: phone:read:list_numbers:admin
  flows:
  - authorizationCode
  scope: phone:read:list_numbers:admin
- description: phone:read:list_outbound_calling_rules:admin
  flows:
  - authorizationCode
  scope: phone:read:list_outbound_calling_rules:admin
- description: phone:read:list_peering_numbers:admin
  flows:
  - authorizationCode
  scope: phone:read:list_peering_numbers:admin
- description: phone:read:list_ported_numbers:admin
  flows:
  - authorizationCode
  scope: phone:read:list_ported_numbers:admin
- description: phone:read:list_private_directory_members:admin
  flows:
  - authorizationCode
  scope: phone:read:list_private_directory_members:admin
- description: phone:read:list_provision_templates:admin
  flows:
  - authorizationCode
  scope: phone:read:list_provision_templates:admin
- description: phone:read:list_recordings
  flows:
  - authorizationCode
  scope: phone:read:list_recordings
- description: phone:read:list_recordings:admin
  flows:
  - authorizationCode
  scope: phone:read:list_recordings:admin
- description: phone:read:list_roles:admin
  flows:
  - authorizationCode
  scope: phone:read:list_roles:admin
- description: phone:read:list_rooms:admin
  flows:
  - authorizationCode
  scope: phone:read:list_rooms:admin
- description: phone:read:list_routing_rules:admin
  flows:
  - authorizationCode
  scope: phone:read:list_routing_rules:admin
- description: phone:read:list_setting_templates:admin
  flows:
  - authorizationCode
  scope: phone:read:list_setting_templates:admin
- description: phone:read:list_shared_line_appearances:admin
  flows:
  - authorizationCode
  scope: phone:read:list_shared_line_appearances:admin
- description: phone:read:list_shared_line_groups:admin
  flows:
  - authorizationCode
  scope: phone:read:list_shared_line_groups:admin
- description: phone:read:list_sip_groups:admin
  flows:
  - authorizationCode
  scope: phone:read:list_sip_groups:admin
- description: phone:read:list_sip_trunks:admin
  flows:
  - authorizationCode
  scope: phone:read:list_sip_trunks:admin
- description: phone:read:list_site_customized_number:admin
  flows:
  - authorizationCode
  scope: phone:read:list_site_customized_number:admin
- description: phone:read:list_sites:admin
  flows:
  - authorizationCode
  scope: phone:read:list_sites:admin
- description: phone:read:list_sms_campaigns:admin
  flows:
  - authorizationCode
  scope: phone:read:list_sms_campaigns:admin
- description: phone:read:list_sms_sessions
  flows:
  - authorizationCode
  scope: phone:read:list_sms_sessions
- description: phone:read:list_sms_sessions:admin
  flows:
  - authorizationCode
  scope: phone:read:list_sms_sessions:admin
- description: phone:read:list_tracked_locations:admin
  flows:
  - authorizationCode
  scope: phone:read:list_tracked_locations:admin
- description: phone:read:list_user_customized_number
  flows:
  - authorizationCode
  scope: phone:read:list_user_customized_number
- description: phone:read:list_user_customized_number:admin
  flows:
  - authorizationCode
  scope: phone:read:list_user_customized_number:admin
- description: phone:read:list_users:admin
  flows:
  - authorizationCode
  scope: phone:read:list_users:admin
- description: phone:read:list_voicemails
  flows:
  - authorizationCode
  scope: phone:read:list_voicemails
- description: phone:read:list_voicemails:admin
  flows:
  - authorizationCode
  scope: phone:read:list_voicemails:admin
- description: phone:read:location_sharing_permission:admin
  flows:
  - authorizationCode
  scope: phone:read:location_sharing_permission:admin
- description: phone:read:monitoring_group:admin
  flows:
  - authorizationCode
  scope: phone:read:monitoring_group:admin
- description: phone:read:nomadic_emergency_services:admin
  flows:
  - authorizationCode
  scope: phone:read:nomadic_emergency_services:admin
- description: phone:read:numbers:admin
  flows:
  - authorizationCode
  scope: phone:read:numbers:admin
- description: phone:read:operation_logs:admin
  flows:
  - authorizationCode
  scope: phone:read:operation_logs:admin
- description: phone:read:policy:admin
  flows:
  - authorizationCode
  scope: phone:read:policy:admin
- description: phone:read:ported_number:admin
  flows:
  - authorizationCode
  scope: phone:read:ported_number:admin
- description: phone:read:provision_template:admin
  flows:
  - authorizationCode
  scope: phone:read:provision_template:admin
- description: phone:read:realtime_location_devices:admin
  flows:
  - authorizationCode
  scope: phone:read:realtime_location_devices:admin
- description: phone:read:realtime_location_users:admin
  flows:
  - authorizationCode
  scope: phone:read:realtime_location_users:admin
- description: phone:read:recording_transcript
  flows:
  - authorizationCode
  scope: phone:read:recording_transcript
- description: phone:read:recording_transcript:admin
  flows:
  - authorizationCode
  scope: phone:read:recording_transcript:admin
- description: phone:read:role:admin
  flows:
  - authorizationCode
  scope: phone:read:role:admin
- description: phone:read:role_member:admin
  flows:
  - authorizationCode
  scope: phone:read:role_member:admin
- description: phone:read:room:admin
  flows:
  - authorizationCode
  scope: phone:read:room:admin
- description: phone:read:routing_rule:admin
  flows:
  - authorizationCode
  scope: phone:read:routing_rule:admin
- description: phone:read:setting_template:admin
  flows:
  - authorizationCode
  scope: phone:read:setting_template:admin
- description: phone:read:settings:admin
  flows:
  - authorizationCode
  scope: phone:read:settings:admin
- description: phone:read:shared_line_group:admin
  flows:
  - authorizationCode
  scope: phone:read:shared_line_group:admin
- description: phone:read:shared_line_group_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:shared_line_group_call_handling_setting:admin
- description: phone:read:shared_line_group_policy:admin
  flows:
  - authorizationCode
  scope: phone:read:shared_line_group_policy:admin
- description: phone:read:shared_line_group_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:shared_line_group_setting:admin
- description: phone:read:site:admin
  flows:
  - authorizationCode
  scope: phone:read:site:admin
- description: phone:read:site_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:read:site_outbound_calling_rule:admin
- description: phone:read:site_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:site_setting:admin
- description: phone:read:sms_campaign:admin
  flows:
  - authorizationCode
  scope: phone:read:sms_campaign:admin
- description: phone:read:sms_campaign_number_opt_status
  flows:
  - authorizationCode
  scope: phone:read:sms_campaign_number_opt_status
- description: phone:read:sms_campaign_number_opt_status:admin
  flows:
  - authorizationCode
  scope: phone:read:sms_campaign_number_opt_status:admin
- description: phone:read:sms_charges:admin
  flows:
  - authorizationCode
  scope: phone:read:sms_charges:admin
- description: phone:read:sms_consent_number_opt_status:admin
  flows:
  - authorizationCode
  scope: phone:read:sms_consent_number_opt_status:admin
- description: phone:read:sms_message
  flows:
  - authorizationCode
  scope: phone:read:sms_message
- description: phone:read:sms_message:admin
  flows:
  - authorizationCode
  scope: phone:read:sms_message:admin
- description: phone:read:sms_session
  flows:
  - authorizationCode
  scope: phone:read:sms_session
- description: phone:read:sms_session:admin
  flows:
  - authorizationCode
  scope: phone:read:sms_session:admin
- description: phone:read:user
  flows:
  - authorizationCode
  scope: phone:read:user
- description: phone:read:user:admin
  flows:
  - authorizationCode
  scope: phone:read:user:admin
- description: phone:read:user_call_handling_setting
  flows:
  - authorizationCode
  scope: phone:read:user_call_handling_setting
- description: phone:read:user_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:user_call_handling_setting:admin
- description: phone:read:user_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:read:user_outbound_calling_rule:admin
- description: phone:read:user_policy:admin
  flows:
  - authorizationCode
  scope: phone:read:user_policy:admin
- description: phone:read:user_setting
  flows:
  - authorizationCode
  scope: phone:read:user_setting
- description: phone:read:user_setting:admin
  flows:
  - authorizationCode
  scope: phone:read:user_setting:admin
- description: phone:read:voicemail
  flows:
  - authorizationCode
  scope: phone:read:voicemail
- description: phone:read:voicemail:admin
  flows:
  - authorizationCode
  scope: phone:read:voicemail:admin
- description: phone:update:audio
  flows:
  - authorizationCode
  scope: phone:update:audio
- description: phone:update:audio:admin
  flows:
  - authorizationCode
  scope: phone:update:audio:admin
- description: phone:update:auto_receptionist:admin
  flows:
  - authorizationCode
  scope: phone:update:auto_receptionist:admin
- description: phone:update:auto_receptionist_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:auto_receptionist_call_handling_setting:admin
- description: phone:update:auto_receptionist_ivr:admin
  flows:
  - authorizationCode
  scope: phone:update:auto_receptionist_ivr:admin
- description: phone:update:auto_receptionist_policy:admin
  flows:
  - authorizationCode
  scope: phone:update:auto_receptionist_policy:admin
- description: phone:update:auto_receptionist_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:auto_receptionist_setting:admin
- description: phone:update:batch_users:admin
  flows:
  - authorizationCode
  scope: phone:update:batch_users:admin
- description: phone:update:blocked_list:admin
  flows:
  - authorizationCode
  scope: phone:update:blocked_list:admin
- description: phone:update:call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:call_handling_setting:admin
- description: phone:update:call_log:admin
  flows:
  - authorizationCode
  scope: phone:update:call_log:admin
- description: phone:update:call_pickup_group:admin
  flows:
  - authorizationCode
  scope: phone:update:call_pickup_group:admin
- description: phone:update:call_queue:admin
  flows:
  - authorizationCode
  scope: phone:update:call_queue:admin
- description: phone:update:call_queue_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:call_queue_call_handling_setting:admin
- description: phone:update:call_queue_custom_group:admin
  flows:
  - authorizationCode
  scope: phone:update:call_queue_custom_group:admin
- description: phone:update:call_queue_policy:admin
  flows:
  - authorizationCode
  scope: phone:update:call_queue_policy:admin
- description: phone:update:call_queue_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:call_queue_setting:admin
- description: phone:update:call_recording
  flows:
  - authorizationCode
  scope: phone:update:call_recording
- description: phone:update:call_recording:admin
  flows:
  - authorizationCode
  scope: phone:update:call_recording:admin
- description: phone:update:calling_plan
  flows:
  - authorizationCode
  scope: phone:update:calling_plan
- description: phone:update:calling_plan:admin
  flows:
  - authorizationCode
  scope: phone:update:calling_plan:admin
- description: phone:update:carrier_number:admin
  flows:
  - authorizationCode
  scope: phone:update:carrier_number:admin
- description: phone:update:common_area:admin
  flows:
  - authorizationCode
  scope: phone:update:common_area:admin
- description: phone:update:common_area_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:common_area_call_handling_setting:admin
- description: phone:update:common_area_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:update:common_area_outbound_calling_rule:admin
- description: phone:update:common_area_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:common_area_setting:admin
- description: phone:update:device:admin
  flows:
  - authorizationCode
  scope: phone:update:device:admin
- description: phone:update:device_line_keys
  flows:
  - authorizationCode
  scope: phone:update:device_line_keys
- description: phone:update:device_line_keys:admin
  flows:
  - authorizationCode
  scope: phone:update:device_line_keys:admin
- description: phone:update:device_provision_template:admin
  flows:
  - authorizationCode
  scope: phone:update:device_provision_template:admin
- description: phone:update:emergency_address:admin
  flows:
  - authorizationCode
  scope: phone:update:emergency_address:admin
- description: phone:update:emergency_location:admin
  flows:
  - authorizationCode
  scope: phone:update:emergency_location:admin
- description: phone:update:external_contact:admin
  flows:
  - authorizationCode
  scope: phone:update:external_contact:admin
- description: phone:update:firmware_update_rule:admin
  flows:
  - authorizationCode
  scope: phone:update:firmware_update_rule:admin
- description: phone:update:group_policy:admin
  flows:
  - authorizationCode
  scope: phone:update:group_policy:admin
- description: phone:update:inbound_block_rule:admin
  flows:
  - authorizationCode
  scope: phone:update:inbound_block_rule:admin
- description: phone:update:inbound_blocked_for_all:admin
  flows:
  - authorizationCode
  scope: phone:update:inbound_blocked_for_all:admin
- description: phone:update:line_keys
  flows:
  - authorizationCode
  scope: phone:update:line_keys
- description: phone:update:line_keys:admin
  flows:
  - authorizationCode
  scope: phone:update:line_keys:admin
- description: phone:update:monitoring_group:admin
  flows:
  - authorizationCode
  scope: phone:update:monitoring_group:admin
- description: phone:update:number:admin
  flows:
  - authorizationCode
  scope: phone:update:number:admin
- description: phone:update:outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:update:outbound_calling_rule:admin
- description: phone:update:peering_number:admin
  flows:
  - authorizationCode
  scope: phone:update:peering_number:admin
- description: phone:update:policy:admin
  flows:
  - authorizationCode
  scope: phone:update:policy:admin
- description: phone:update:private_directory_member:admin
  flows:
  - authorizationCode
  scope: phone:update:private_directory_member:admin
- description: phone:update:provision_template:admin
  flows:
  - authorizationCode
  scope: phone:update:provision_template:admin
- description: phone:update:role:admin
  flows:
  - authorizationCode
  scope: phone:update:role:admin
- description: phone:update:room:admin
  flows:
  - authorizationCode
  scope: phone:update:room:admin
- description: phone:update:routing_rule:admin
  flows:
  - authorizationCode
  scope: phone:update:routing_rule:admin
- description: phone:update:setting_template:admin
  flows:
  - authorizationCode
  scope: phone:update:setting_template:admin
- description: phone:update:settings:admin
  flows:
  - authorizationCode
  scope: phone:update:settings:admin
- description: phone:update:shared_line_group:admin
  flows:
  - authorizationCode
  scope: phone:update:shared_line_group:admin
- description: phone:update:shared_line_group_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:shared_line_group_call_handling_setting:admin
- description: phone:update:shared_line_group_policy:admin
  flows:
  - authorizationCode
  scope: phone:update:shared_line_group_policy:admin
- description: phone:update:shared_line_group_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:shared_line_group_setting:admin
- description: phone:update:shared_setting
  flows:
  - authorizationCode
  scope: phone:update:shared_setting
- description: phone:update:shared_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:shared_setting:admin
- description: phone:update:site:admin
  flows:
  - authorizationCode
  scope: phone:update:site:admin
- description: phone:update:site_number:admin
  flows:
  - authorizationCode
  scope: phone:update:site_number:admin
- description: phone:update:site_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:update:site_outbound_calling_rule:admin
- description: phone:update:site_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:site_setting:admin
- description: phone:update:sms_campaign_number_opt_status:admin
  flows:
  - authorizationCode
  scope: phone:update:sms_campaign_number_opt_status:admin
- description: phone:update:user
  flows:
  - authorizationCode
  scope: phone:update:user
- description: phone:update:user:admin
  flows:
  - authorizationCode
  scope: phone:update:user:admin
- description: phone:update:user_call_handling_setting
  flows:
  - authorizationCode
  scope: phone:update:user_call_handling_setting
- description: phone:update:user_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:user_call_handling_setting:admin
- description: phone:update:user_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:update:user_outbound_calling_rule:admin
- description: phone:update:user_policy:admin
  flows:
  - authorizationCode
  scope: phone:update:user_policy:admin
- description: phone:update:user_setting
  flows:
  - authorizationCode
  scope: phone:update:user_setting
- description: phone:update:user_setting:admin
  flows:
  - authorizationCode
  scope: phone:update:user_setting:admin
- description: phone:update:voicemail
  flows:
  - authorizationCode
  scope: phone:update:voicemail
- description: phone:update:voicemail:admin
  flows:
  - authorizationCode
  scope: phone:update:voicemail:admin
- description: phone:write
  flows:
  - authorizationCode
  scope: phone:write
- description: phone:write:admin
  flows:
  - authorizationCode
  scope: phone:write:admin
- description: phone:write:alert_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:alert_setting:admin
- description: phone:write:apply_template_to_common_areas:admin
  flows:
  - authorizationCode
  scope: phone:write:apply_template_to_common_areas:admin
- description: phone:write:audio
  flows:
  - authorizationCode
  scope: phone:write:audio
- description: phone:write:audio:admin
  flows:
  - authorizationCode
  scope: phone:write:audio:admin
- description: phone:write:auto_receptionist:admin
  flows:
  - authorizationCode
  scope: phone:write:auto_receptionist:admin
- description: phone:write:auto_receptionist_number:admin
  flows:
  - authorizationCode
  scope: phone:write:auto_receptionist_number:admin
- description: phone:write:auto_receptionist_policy:admin
  flows:
  - authorizationCode
  scope: phone:write:auto_receptionist_policy:admin
- description: phone:write:auto_receptionist_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:auto_receptionist_setting:admin
- description: phone:write:batch_audios
  flows:
  - authorizationCode
  scope: phone:write:batch_audios
- description: phone:write:batch_audios:admin
  flows:
  - authorizationCode
  scope: phone:write:batch_audios:admin
- description: phone:write:batch_emergency_locations:admin
  flows:
  - authorizationCode
  scope: phone:write:batch_emergency_locations:admin
- description: phone:write:batch_users:admin
  flows:
  - authorizationCode
  scope: phone:write:batch_users:admin
- description: phone:write:blocked_list:admin
  flows:
  - authorizationCode
  scope: phone:write:blocked_list:admin
- description: phone:write:byo_carrier_number:admin
  flows:
  - authorizationCode
  scope: phone:write:byo_carrier_number:admin
- description: phone:write:call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:call_handling_setting:admin
- description: phone:write:call_pickup_group:admin
  flows:
  - authorizationCode
  scope: phone:write:call_pickup_group:admin
- description: phone:write:call_pickup_group_member:admin
  flows:
  - authorizationCode
  scope: phone:write:call_pickup_group_member:admin
- description: phone:write:call_queue:admin
  flows:
  - authorizationCode
  scope: phone:write:call_queue:admin
- description: phone:write:call_queue_custom_group:admin
  flows:
  - authorizationCode
  scope: phone:write:call_queue_custom_group:admin
- description: phone:write:call_queue_custom_group_member:admin
  flows:
  - authorizationCode
  scope: phone:write:call_queue_custom_group_member:admin
- description: phone:write:call_queue_member:admin
  flows:
  - authorizationCode
  scope: phone:write:call_queue_member:admin
- description: phone:write:call_queue_number:admin
  flows:
  - authorizationCode
  scope: phone:write:call_queue_number:admin
- description: phone:write:call_queue_policy:admin
  flows:
  - authorizationCode
  scope: phone:write:call_queue_policy:admin
- description: phone:write:call_queue_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:call_queue_setting:admin
- description: phone:write:calling_plan
  flows:
  - authorizationCode
  scope: phone:write:calling_plan
- description: phone:write:calling_plan:admin
  flows:
  - authorizationCode
  scope: phone:write:calling_plan:admin
- description: phone:write:carrier_number:admin
  flows:
  - authorizationCode
  scope: phone:write:carrier_number:admin
- description: phone:write:common_area:admin
  flows:
  - authorizationCode
  scope: phone:write:common_area:admin
- description: phone:write:common_area_calling_plan:admin
  flows:
  - authorizationCode
  scope: phone:write:common_area_calling_plan:admin
- description: phone:write:common_area_number:admin
  flows:
  - authorizationCode
  scope: phone:write:common_area_number:admin
- description: phone:write:common_area_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:write:common_area_outbound_calling_rule:admin
- description: phone:write:common_area_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:common_area_setting:admin
- description: phone:write:customized_number:admin
  flows:
  - authorizationCode
  scope: phone:write:customized_number:admin
- description: phone:write:device:admin
  flows:
  - authorizationCode
  scope: phone:write:device:admin
- description: phone:write:device_extension:admin
  flows:
  - authorizationCode
  scope: phone:write:device_extension:admin
- description: phone:write:directory:admin
  flows:
  - authorizationCode
  scope: phone:write:directory:admin
- description: phone:write:emergency_address:admin
  flows:
  - authorizationCode
  scope: phone:write:emergency_address:admin
- description: phone:write:emergency_location:admin
  flows:
  - authorizationCode
  scope: phone:write:emergency_location:admin
- description: phone:write:extension_inbound_block_rule
  flows:
  - authorizationCode
  scope: phone:write:extension_inbound_block_rule
- description: phone:write:extension_inbound_block_rule:admin
  flows:
  - authorizationCode
  scope: phone:write:extension_inbound_block_rule:admin
- description: phone:write:external_contact:admin
  flows:
  - authorizationCode
  scope: phone:write:external_contact:admin
- description: phone:write:firmware_update_rule:admin
  flows:
  - authorizationCode
  scope: phone:write:firmware_update_rule:admin
- description: phone:write:inbound_block_rule:admin
  flows:
  - authorizationCode
  scope: phone:write:inbound_block_rule:admin
- description: phone:write:monitoring_group:admin
  flows:
  - authorizationCode
  scope: phone:write:monitoring_group:admin
- description: phone:write:monitoring_group_member:admin
  flows:
  - authorizationCode
  scope: phone:write:monitoring_group_member:admin
- description: phone:write:outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:write:outbound_calling_rule:admin
- description: phone:write:peering_number:admin
  flows:
  - authorizationCode
  scope: phone:write:peering_number:admin
- description: phone:write:private_directory_member:admin
  flows:
  - authorizationCode
  scope: phone:write:private_directory_member:admin
- description: phone:write:provision_template:admin
  flows:
  - authorizationCode
  scope: phone:write:provision_template:admin
- description: phone:write:reboot_device:admin
  flows:
  - authorizationCode
  scope: phone:write:reboot_device:admin
- description: phone:write:role:admin
  flows:
  - authorizationCode
  scope: phone:write:role:admin
- description: phone:write:role_member:admin
  flows:
  - authorizationCode
  scope: phone:write:role_member:admin
- description: phone:write:room:admin
  flows:
  - authorizationCode
  scope: phone:write:room:admin
- description: phone:write:room_calling_plan:admin
  flows:
  - authorizationCode
  scope: phone:write:room_calling_plan:admin
- description: phone:write:room_phone_number:admin
  flows:
  - authorizationCode
  scope: phone:write:room_phone_number:admin
- description: phone:write:routing_rule:admin
  flows:
  - authorizationCode
  scope: phone:write:routing_rule:admin
- description: phone:write:send_fax
  flows:
  - authorizationCode
  scope: phone:write:send_fax
- description: phone:write:send_fax:admin
  flows:
  - authorizationCode
  scope: phone:write:send_fax:admin
- description: phone:write:setting_template:admin
  flows:
  - authorizationCode
  scope: phone:write:setting_template:admin
- description: phone:write:shared_line_group:admin
  flows:
  - authorizationCode
  scope: phone:write:shared_line_group:admin
- description: phone:write:shared_line_group_number:admin
  flows:
  - authorizationCode
  scope: phone:write:shared_line_group_number:admin
- description: phone:write:shared_line_group_policy:admin
  flows:
  - authorizationCode
  scope: phone:write:shared_line_group_policy:admin
- description: phone:write:shared_line_group_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:shared_line_group_setting:admin
- description: phone:write:shared_line_member:admin
  flows:
  - authorizationCode
  scope: phone:write:shared_line_member:admin
- description: phone:write:shared_setting
  flows:
  - authorizationCode
  scope: phone:write:shared_setting
- description: phone:write:shared_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:shared_setting:admin
- description: phone:write:site:admin
  flows:
  - authorizationCode
  scope: phone:write:site:admin
- description: phone:write:site_customized_number:admin
  flows:
  - authorizationCode
  scope: phone:write:site_customized_number:admin
- description: phone:write:site_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:write:site_outbound_calling_rule:admin
- description: phone:write:site_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:site_setting:admin
- description: phone:write:sms_campaign_number:admin
  flows:
  - authorizationCode
  scope: phone:write:sms_campaign_number:admin
- description: phone:write:sync_device:admin
  flows:
  - authorizationCode
  scope: phone:write:sync_device:admin
- description: phone:write:user_call_handling_setting
  flows:
  - authorizationCode
  scope: phone:write:user_call_handling_setting
- description: phone:write:user_call_handling_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:user_call_handling_setting:admin
- description: phone:write:user_customized_number
  flows:
  - authorizationCode
  scope: phone:write:user_customized_number
- description: phone:write:user_customized_number:admin
  flows:
  - authorizationCode
  scope: phone:write:user_customized_number:admin
- description: phone:write:user_number
  flows:
  - authorizationCode
  scope: phone:write:user_number
- description: phone:write:user_number:admin
  flows:
  - authorizationCode
  scope: phone:write:user_number:admin
- description: phone:write:user_outbound_calling_rule:admin
  flows:
  - authorizationCode
  scope: phone:write:user_outbound_calling_rule:admin
- description: phone:write:user_setting
  flows:
  - authorizationCode
  scope: phone:write:user_setting
- description: phone:write:user_setting:admin
  flows:
  - authorizationCode
  scope: phone:write:user_setting:admin
- description: phone_call_log:read
  flows:
  - authorizationCode
  scope: phone_call_log:read
- description: phone_call_log:read:admin
  flows:
  - authorizationCode
  scope: phone_call_log:read:admin
- description: phone_call_log:write
  flows:
  - authorizationCode
  scope: phone_call_log:write
- description: phone_call_log:write:admin
  flows:
  - authorizationCode
  scope: phone_call_log:write:admin
- description: phone_peering:read:admin
  flows:
  - authorizationCode
  scope: phone_peering:read:admin
- description: phone_peering:write:admin
  flows:
  - authorizationCode
  scope: phone_peering:write:admin
- description: phone_recording:read
  flows:
  - authorizationCode
  scope: phone_recording:read
- description: phone_recording:read:admin
  flows:
  - authorizationCode
  scope: phone_recording:read:admin
- description: phone_recording:write
  flows:
  - authorizationCode
  scope: phone_recording:write
- description: phone_recording:write:admin
  flows:
  - authorizationCode
  scope: phone_recording:write:admin
- description: phone_sms:read
  flows:
  - authorizationCode
  scope: phone_sms:read
- description: phone_sms:read:admin
  flows:
  - authorizationCode
  scope: phone_sms:read:admin
- description: phone_sms:write
  flows:
  - authorizationCode
  scope: phone_sms:write
- description: phone_sms:write:admin
  flows:
  - authorizationCode
  scope: phone_sms:write:admin
- description: phone_voicemail:read
  flows:
  - authorizationCode
  scope: phone_voicemail:read
- description: phone_voicemail:read:admin
  flows:
  - authorizationCode
  scope: phone_voicemail:read:admin
- description: phone_voicemail:write
  flows:
  - authorizationCode
  scope: phone_voicemail:write
- description: phone_voicemail:write:admin
  flows:
  - authorizationCode
  scope: phone_voicemail:write:admin
slug: zoom-phone-scopes
source_filename: zoom-phone-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  openapi/zoom-phone-api-openapi.json, openapi/zoom-phone-number-management-openapi.json\n  (oauth2 flows + per-operation x-macro-scopes / x-granular-scopes), confirmed against\n  https://developers.zoom.us/docs/integrations/oauth-scopes-granular/\ndocs: https://developers.zoom.us/docs/integrations/oauth-scopes-granular/\ndocs_classic: https://developers.zoom.us/docs/integrations/oauth-scopes/\ndocs_overview: https://developers.zoom.us/docs/integrations/oauth-scopes-overview/\ndocs_migration: https://developers.zoom.us/docs/integrations/migrate/\nsummary: >-\n  Zoom runs two parallel scope models. CLASSIC scopes are coarse (phone:read, phone:write,\n  phone:read:admin, phone:write:admin, phone:master); GRANULAR scopes are per-operation and\n  follow product:action:resource[:admin|:master] — phone:read:list_users:admin,\n  phone:write:calling_plan:admin, number_management:delete:numbers:admin. Every Zoom Phone\n  operation\
  \ publishes BOTH forms in its spec extension block (x-macro-scopes and\n  x-granular-scopes), which is why 435 distinct scopes are derivable from the two specs. Zoom\n  is actively migrating apps off classic scopes onto granular ones; new apps should request\n  granular scopes only, and the :admin / :master suffixes gate account-level and\n  master-account access respectively.\nauthorization_endpoint: https://zoom.us/oauth/authorize\ntoken_endpoint: https://zoom.us/oauth/token\nmetadata: https://zoom.us/.well-known/oauth-authorization-server\nschemes:\n- name: openapi_oauth\n  source: openapi/zoom-phone-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n- name: openapi_oauth\n  source: openapi/zoom-phone-number-management-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\nscopes:\n- scope: number_management:delete:numbers:admin\n  description: number_management:delete:numbers:admin\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:delete:peering_number:admin\n  description: number_management:delete:peering_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:delete:sms_consent:admin\n  description: number_management:delete:sms_consent:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:list_carrier_peering_numbers:admin\n  description: number_management:read:list_carrier_peering_numbers:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:list_numbers:admin\n  description: number_management:read:list_numbers:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:list_peering_numbers:admin\n \
  \ description: number_management:read:list_peering_numbers:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:list_ported_numbers:admin\n  description: number_management:read:list_ported_numbers:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:list_sip_groups:admin\n  description: number_management:read:list_sip_groups:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:list_sip_trunks:admin\n  description: number_management:read:list_sip_trunks:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:list_sms_campaigns:admin\n  description: number_management:read:list_sms_campaigns:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n\
  - scope: number_management:read:numbers:admin\n  description: number_management:read:numbers:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:numbers_plan:admin\n  description: number_management:read:numbers_plan:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:ported_number:admin\n  description: number_management:read:ported_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:sms_campaign:admin\n  description: number_management:read:sms_campaign:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:read:sms_consent:admin\n  description: number_management:read:sms_consent:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n\
  - scope: number_management:update:numbers:admin\n  description: number_management:update:numbers:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:update:peering_number:admin\n  description: number_management:update:peering_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:update:sms_consent:admin\n  description: number_management:update:sms_consent:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:write:byoc_numbers:admin\n  description: number_management:write:byoc_numbers:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:write:numbers:admin\n  description: number_management:write:numbers:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n\
  - scope: number_management:write:peering_number:admin\n  description: number_management:write:peering_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management:write:sms_consent:admin\n  description: number_management:write:sms_consent:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management_numbers:read:admin\n  description: number_management_numbers:read:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management_numbers:write:admin\n  description: number_management_numbers:write:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n- scope: number_management_numbers:write:master\n  description: number_management_numbers:write:master\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-number-management-openapi.json\n\
  - scope: phone:delete:alert_setting:admin\n  description: phone:delete:alert_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:audio\n  description: phone:delete:audio\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:audio:admin\n  description: phone:delete:audio:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:auto_receptionist:admin\n  description: phone:delete:auto_receptionist:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:auto_receptionist_number:admin\n  description: phone:delete:auto_receptionist_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:auto_receptionist_policy:admin\n  description: phone:delete:auto_receptionist_policy:admin\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:auto_receptionist_setting:admin\n  description: phone:delete:auto_receptionist_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:blocked_list:admin\n  description: phone:delete:blocked_list:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_handling_setting:admin\n  description: phone:delete:call_handling_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_log\n  description: phone:delete:call_log\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_log:admin\n  description: phone:delete:call_log:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_pickup_group:admin\n\
  \  description: phone:delete:call_pickup_group:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_pickup_group_member:admin\n  description: phone:delete:call_pickup_group_member:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_queue:admin\n  description: phone:delete:call_queue:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_queue_custom_group:admin\n  description: phone:delete:call_queue_custom_group:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_queue_custom_group:master\n  description: phone:delete:call_queue_custom_group:master\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_queue_custom_group_member:admin\n  description: phone:delete:call_queue_custom_group_member:admin\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_queue_member:admin\n  description: phone:delete:call_queue_member:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_queue_number:admin\n  description: phone:delete:call_queue_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_queue_policy:admin\n  description: phone:delete:call_queue_policy:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_queue_setting:admin\n  description: phone:delete:call_queue_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:call_recording\n  description: phone:delete:call_recording\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n\
  - scope: phone:delete:call_recording:admin\n  description: phone:delete:call_recording:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:carrier_number:admin\n  description: phone:delete:carrier_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:common_area:admin\n  description: phone:delete:common_area:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:common_area_calling_plan:admin\n  description: phone:delete:common_area_calling_plan:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:common_area_number:admin\n  description: phone:delete:common_area_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:common_area_outbound_calling_rule:admin\n  description:\
  \ phone:delete:common_area_outbound_calling_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:common_area_setting:admin\n  description: phone:delete:common_area_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:customized_number:admin\n  description: phone:delete:customized_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:device:admin\n  description: phone:delete:device:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:device_extension:admin\n  description: phone:delete:device_extension:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:directory:admin\n  description: phone:delete:directory:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n\
  - scope: phone:delete:emergency_address:admin\n  description: phone:delete:emergency_address:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:emergency_location:admin\n  description: phone:delete:emergency_location:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:extension_inbound_block_rule\n  description: phone:delete:extension_inbound_block_rule\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:extension_inbound_block_rule:admin\n  description: phone:delete:extension_inbound_block_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:extension_inbound_block_rule_stat:admin\n  description: phone:delete:extension_inbound_block_rule_stat:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope:\
  \ phone:delete:external_contact:admin\n  description: phone:delete:external_contact:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:fax_log\n  description: phone:delete:fax_log\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:fax_log:admin\n  description: phone:delete:fax_log:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:firmware_update_rule:admin\n  description: phone:delete:firmware_update_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:inbound_block_rule:admin\n  description: phone:delete:inbound_block_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:line_keys\n  description: phone:delete:line_keys\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n\
  - scope: phone:delete:line_keys:admin\n  description: phone:delete:line_keys:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:monitoring_group:admin\n  description: phone:delete:monitoring_group:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:monitoring_group_member:admin\n  description: phone:delete:monitoring_group_member:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:number:admin\n  description: phone:delete:number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:outbound_calling_rule:admin\n  description: phone:delete:outbound_calling_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:peering_number:admin\n  description: phone:delete:peering_number:admin\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:private_directory_member:admin\n  description: phone:delete:private_directory_member:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:provision_template:admin\n  description: phone:delete:provision_template:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:role:admin\n  description: phone:delete:role:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:role_member:admin\n  description: phone:delete:role_member:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:room:admin\n  description: phone:delete:room:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:room_calling_plan:admin\n\
  \  description: phone:delete:room_calling_plan:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:room_phone_number:admin\n  description: phone:delete:room_phone_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:routing_rule:admin\n  description: phone:delete:routing_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:shared_line_group:admin\n  description: phone:delete:shared_line_group:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:shared_line_group_number:admin\n  description: phone:delete:shared_line_group_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:shared_line_group_policy:admin\n  description: phone:delete:shared_line_group_policy:admin\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:shared_line_group_setting:admin\n  description: phone:delete:shared_line_group_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:shared_line_member:admin\n  description: phone:delete:shared_line_member:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:shared_setting\n  description: phone:delete:shared_setting\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:shared_setting:admin\n  description: phone:delete:shared_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:site:admin\n  description: phone:delete:site:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:site_customized_number:admin\n\
  \  description: phone:delete:site_customized_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:site_outbound_calling_rule:admin\n  description: phone:delete:site_outbound_calling_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:site_setting:admin\n  description: phone:delete:site_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:sms_campaign_number:admin\n  description: phone:delete:sms_campaign_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:user_call_handling_setting\n  description: phone:delete:user_call_handling_setting\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:user_call_handling_setting:admin\n  description: phone:delete:user_call_handling_setting:admin\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:user_customized_number\n  description: phone:delete:user_customized_number\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:user_customized_number:admin\n  description: phone:delete:user_customized_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:user_number\n  description: phone:delete:user_number\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:user_number:admin\n  description: phone:delete:user_number:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:user_outbound_calling_rule:admin\n  description: phone:delete:user_outbound_calling_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n\
  - scope: phone:delete:user_setting\n  description: phone:delete:user_setting\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:user_setting:admin\n  description: phone:delete:user_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:users_calling_plan\n  description: phone:delete:users_calling_plan\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:users_calling_plan:admin\n  description: phone:delete:users_calling_plan:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:voicemail\n  description: phone:delete:voicemail\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:delete:voicemail:admin\n  description: phone:delete:voicemail:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n\
  - scope: phone:master\n  description: phone:master\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:patch:alert_setting:admin\n  description: phone:patch:alert_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read\n  description: phone:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:admin\n  description: phone:read:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:ai_call_summary\n  description: phone:read:ai_call_summary\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:ai_call_summary:admin\n  description: phone:read:ai_call_summary:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:alert_setting:admin\n  description: phone:read:alert_setting:admin\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:audio\n  description: phone:read:audio\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:audio:admin\n  description: phone:read:audio:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:auto_receptionist:admin\n  description: phone:read:auto_receptionist:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:auto_receptionist_call_handling_setting:admin\n  description: phone:read:auto_receptionist_call_handling_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:auto_receptionist_ivr:admin\n  description: phone:read:auto_receptionist_ivr:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:auto_receptionist_policy:admin\n\
  \  description: phone:read:auto_receptionist_policy:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:auto_receptionist_setting:admin\n  description: phone:read:auto_receptionist_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:billing_account:admin\n  description: phone:read:billing_account:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:blocked_list:admin\n  description: phone:read:blocked_list:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_charges:admin\n  description: phone:read:call_charges:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_log:admin\n  description: phone:read:call_log:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n\
  - scope: phone:read:call_pickup_group:admin\n  description: phone:read:call_pickup_group:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_pickup_group_member:admin\n  description: phone:read:call_pickup_group_member:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_qos:admin\n  description: phone:read:call_qos:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_queue:admin\n  description: phone:read:call_queue:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_queue_call_handling_setting:admin\n  description: phone:read:call_queue_call_handling_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_queue_custom_group:admin\n  description: phone:read:call_queue_custom_group:admin\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_queue_custom_group:master\n  description: phone:read:call_queue_custom_group:master\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_queue_policy:admin\n  description: phone:read:call_queue_policy:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_queue_setting:admin\n  description: phone:read:call_queue_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_recording\n  description: phone:read:call_recording\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:call_recording:admin\n  description: phone:read:call_recording:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:common_area:admin\n\
  \  description: phone:read:common_area:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:common_area_call_handling_setting:admin\n  description: phone:read:common_area_call_handling_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:common_area_outbound_calling_rule:admin\n  description: phone:read:common_area_outbound_calling_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:default_emergency_address:admin\n  description: phone:read:default_emergency_address:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:detectable_personal_location:admin\n  description: phone:read:detectable_personal_location:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:device:admin\n  description:\
  \ phone:read:device:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:device_line_keys\n  description: phone:read:device_line_keys\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:device_line_keys:admin\n  description: phone:read:device_line_keys:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:directory:admin\n  description: phone:read:directory:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:emergency_address:admin\n  description: phone:read:emergency_address:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:emergency_location:admin\n  description: phone:read:emergency_location:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope:\
  \ phone:read:external_contact:admin\n  description: phone:read:external_contact:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:fax_charges:admin\n  description: phone:read:fax_charges:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:fax_log\n  description: phone:read:fax_log\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:fax_log:admin\n  description: phone:read:fax_log:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:firmware_update_rule:admin\n  description: phone:read:firmware_update_rule:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:group_policy:admin\n  description: phone:read:group_policy:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n\
  - scope: phone:read:group_setting:admin\n  description: phone:read:group_setting:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:line_keys\n  description: phone:read:line_keys\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:line_keys:admin\n  description: phone:read:line_keys:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_account_settings:admin\n  description: phone:read:list_account_settings:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_alert_settings:admin\n  description: phone:read:list_alert_settings:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_audios\n  description: phone:read:list_audios\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n\
  - scope: phone:read:list_audios:admin\n  description: phone:read:list_audios:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_auto_receptionists:admin\n  description: phone:read:list_auto_receptionists:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_billing_accounts:admin\n  description: phone:read:list_billing_accounts:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_blocked_lists:admin\n  description: phone:read:list_blocked_lists:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_call_handling_settings:admin\n  description: phone:read:list_call_handling_settings:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_call_logs\n  description: phone:read:list_call_logs\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_call_logs:admin\n  description: phone:read:list_call_logs:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_call_pickup_groups:admin\n  description: phone:read:list_call_pickup_groups:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_call_queue_members:admin\n  description: phone:read:list_call_queue_members:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_call_queue_recordings:admin\n  description: phone:read:list_call_queue_recordings:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- scope: phone:read:list_call_queues:admin\n  description: phone:read:list_call_queues:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n\
  - scope: phone:read:list_call_recordings:admin\n  description: phone:read:list_call_recordings:admin\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n- \n\n# --- truncated at 32 KB (76 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/scopes/zoom-phone-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/scopes/zoom-phone-scopes.yml
summary_line: 435 scopes · authorizationCode
tags:
- Telecommunications
- United States
- UCaaS
- Cloud PBX
- Voice
- VoIP
- SIP
- Messaging
- SMS
- Phone Numbers
- Number Porting
- BYOC
- Carrier Peering
- Contact Center
- Communications
token_urls: []
---
