---
api_specs:
- filename: canvas-lms-openapi.yml
  format: yaml
  label: Canvas LMS REST API
  slug: canvas-lms-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas/refs/heads/main/openapi/canvas-lms-openapi.yml
- filename: canvas-courses-api-openapi.yml
  format: yaml
  label: Canvas Courses API
  slug: canvas-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas/refs/heads/main/openapi/canvas-courses-api-openapi.yml
authorization_urls:
- https://canvas.instructure.com/login/oauth2/auth
description: ''
docs: https://developerdocs.instructure.com/services/canvas/resources/api_token_scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Canvas Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Canvas publishes 1117 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Canvas API on a user''s behalf.


  Tokens are issued from https://canvas.instructure.com/login/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Canvas
provider_slug: canvas
schemes:
- flows:
  - authorizationUrl: https://canvas.instructure.com/login/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://canvas.instructure.com/login/oauth2/token
  name: oauth2
  source: openapi/canvas-lms-openapi.yml
scope_count: 1117
scope_names:
- url:GET|/api/lti/accounts/:account_id
- url:PUT|/api/lti/asset_processor_eulas/:context_external_tool_id/deployment
- url:DELETE|/api/lti/asset_processor_eulas/:context_external_tool_id/user
- url:POST|/api/lti/asset_processor_eulas/:context_external_tool_id/user
- url:POST|/api/lti/asset_processors/:asset_processor_id/reports
- url:GET|/api/lti/assignments/:assignment_id
- url:GET|/api/lti/assignments/:assignment_id/files/:file_id/originality_report
- url:PUT|/api/lti/assignments/:assignment_id/files/:file_id/originality_report
- url:GET|/api/lti/assignments/:assignment_id/submissions/:submission_id
- url:GET|/api/lti/assignments/:assignment_id/submissions/:submission_id/history
- url:POST|/api/lti/assignments/:assignment_id/submissions/:submission_id/originality_report
- url:GET|/api/lti/assignments/:assignment_id/submissions/:submission_id/originality_report/:id
- url:PUT|/api/lti/assignments/:assignment_id/submissions/:submission_id/originality_report/:id
- url:GET|/api/lti/courses/:course_id/line_items
- url:POST|/api/lti/courses/:course_id/line_items
- url:DELETE|/api/lti/courses/:course_id/line_items/:id
- url:GET|/api/lti/courses/:course_id/line_items/:id
- url:PUT|/api/lti/courses/:course_id/line_items/:id
- url:GET|/api/lti/courses/:course_id/line_items/:line_item_id/results
- url:GET|/api/lti/courses/:course_id/line_items/:line_item_id/results/:id
- url:POST|/api/lti/courses/:course_id/line_items/:line_item_id/scores
- url:GET|/api/lti/courses/:course_id/names_and_roles
- url:GET|/api/lti/courses/:course_id/progress/:id
- url:PUT|/api/lti/developer_key/update_public_jwk
- url:GET|/api/lti/groups/:group_id/names_and_roles
- url:GET|/api/lti/groups/:group_id/users
- url:GET|/api/lti/notice-handlers/:context_external_tool_id
- url:PUT|/api/lti/notice-handlers/:context_external_tool_id
- url:GET|/api/lti/subscriptions
- url:POST|/api/lti/subscriptions
- url:DELETE|/api/lti/subscriptions/:id
- url:GET|/api/lti/subscriptions/:id
- url:PUT|/api/lti/subscriptions/:id
- url:GET|/api/lti/users/:id
- url:GET|/api/lti/uuid_map
- url:POST|/api/quiz/v1/courses/:course_id/accommodations
- url:GET|/api/quiz/v1/courses/:course_id/quizzes
- url:POST|/api/quiz/v1/courses/:course_id/quizzes
- url:DELETE|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id
- url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id
- url:PATCH|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id
- url:POST|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/accommodations
- url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items
- url:POST|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items
- url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/media_upload_url
- url:DELETE|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/:item_id
- url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/:item_id
- url:PATCH|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/:item_id
- url:POST|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/reports
- url:GET|/api/sis/accounts/:account_id/assignments
- url:GET|/api/sis/courses/:course_id/assignments
- url:PUT|/api/sis/courses/:course_id/disable_post_to_sis
- url:GET|/api/v1/account_calendars
- url:GET|/api/v1/account_calendars/:account_id
- url:PUT|/api/v1/account_calendars/:account_id
- url:GET|/api/v1/accounts
- url:GET|/api/v1/accounts/search
- url:GET|/api/v1/accounts/:account_id/account_calendars
- url:PUT|/api/v1/accounts/:account_id/account_calendars
- url:GET|/api/v1/accounts/:account_id/account_notifications
- url:POST|/api/v1/accounts/:account_id/account_notifications
- url:DELETE|/api/v1/accounts/:account_id/account_notifications/:id
- url:GET|/api/v1/accounts/:account_id/account_notifications/:id
- url:PUT|/api/v1/accounts/:account_id/account_notifications/:id
- url:GET|/api/v1/accounts/:account_id/admins
- url:POST|/api/v1/accounts/:account_id/admins
- url:GET|/api/v1/accounts/:account_id/admins/self
- url:DELETE|/api/v1/accounts/:account_id/admins/:user_id
- url:GET|/api/v1/accounts/:account_id/analytics/completed/activity
- url:GET|/api/v1/accounts/:account_id/analytics/completed/grades
- url:GET|/api/v1/accounts/:account_id/analytics/completed/statistics
- url:GET|/api/v1/accounts/:account_id/analytics/completed/statistics_by_subaccount
- url:GET|/api/v1/accounts/:account_id/analytics/current/activity
- url:GET|/api/v1/accounts/:account_id/analytics/current/grades
- url:GET|/api/v1/accounts/:account_id/analytics/current/statistics
- url:GET|/api/v1/accounts/:account_id/analytics/current/statistics_by_subaccount
- url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/activity
- url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/grades
- url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/statistics
- url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/statistics_by_subaccount
- url:GET|/api/v1/accounts/:account_id/app_by_client_id/:client_id
- url:GET|/api/v1/accounts/:account_id/apps
- url:POST|/api/v1/accounts/:account_id/apps
- url:GET|/api/v1/accounts/:account_id/apps/by_utid/:utid
- url:GET|/api/v1/accounts/:account_id/apps/install_status/:client_id
- url:DELETE|/api/v1/accounts/:account_id/apps/:id
- url:GET|/api/v1/accounts/:account_id/apps/:id
- url:PUT|/api/v1/accounts/:account_id/apps/:id
- url:DELETE|/api/v1/accounts/:account_id/apps/:id/bind
- url:POST|/api/v1/accounts/:account_id/apps/:id/bind
- url:GET|/api/v1/accounts/:account_id/apps/:id/history
- url:POST|/api/v1/accounts/:account_id/apps/:id/install_from_template
- url:GET|/api/v1/accounts/:account_id/apps/:id/latest_update_request
- url:GET|/api/v1/accounts/:account_id/apps/:id/overlay_history
- url:PUT|/api/v1/accounts/:account_id/apps/:id/reset
- url:GET|/api/v1/accounts/:account_id/apps/:id/update_requests/:update_request_id
- url:PUT|/api/v1/accounts/:account_id/apps/:id/update_requests/:update_request_id/apply
- url:GET|/api/v1/accounts/:account_id/apps/:registration_id/deployments/:deployment_id/context_search
- url:GET|/api/v1/accounts/:account_id/authentication_providers
- url:POST|/api/v1/accounts/:account_id/authentication_providers
- url:POST|/api/v1/accounts/:account_id/authentication_providers/force_password_reset
- url:DELETE|/api/v1/accounts/:account_id/authentication_providers/:id
- url:GET|/api/v1/accounts/:account_id/authentication_providers/:id
- url:PUT|/api/v1/accounts/:account_id/authentication_providers/:id
- url:PUT|/api/v1/accounts/:account_id/authentication_providers/:id/restore
- url:GET|/api/v1/accounts/:account_id/blackout_dates
- url:POST|/api/v1/accounts/:account_id/blackout_dates
- url:GET|/api/v1/accounts/:account_id/blackout_dates/new
- url:DELETE|/api/v1/accounts/:account_id/blackout_dates/:id
- url:GET|/api/v1/accounts/:account_id/blackout_dates/:id
- url:PUT|/api/v1/accounts/:account_id/blackout_dates/:id
- url:GET|/api/v1/accounts/:account_id/brand_variables
- url:POST|/api/v1/accounts/:account_id/bulk_enrollment
- url:GET|/api/v1/accounts/:account_id/content_migrations
- url:POST|/api/v1/accounts/:account_id/content_migrations
- url:GET|/api/v1/accounts/:account_id/content_migrations/migrators
- url:GET|/api/v1/accounts/:account_id/content_migrations/:content_migration_id/migration_issues
- url:GET|/api/v1/accounts/:account_id/content_migrations/:content_migration_id/migration_issues/:id
- url:PUT|/api/v1/accounts/:account_id/content_migrations/:content_migration_id/migration_issues/:id
- url:GET|/api/v1/accounts/:account_id/content_migrations/:id
- url:PUT|/api/v1/accounts/:account_id/content_migrations/:id
- url:GET|/api/v1/accounts/:account_id/content_migrations/:id/selective_data
- url:GET|/api/v1/accounts/:account_id/courses
- url:POST|/api/v1/accounts/:account_id/courses
- url:PUT|/api/v1/accounts/:account_id/courses
- url:GET|/api/v1/accounts/:account_id/courses/:id
- url:GET|/api/v1/accounts/:account_id/csp_settings
- url:PUT|/api/v1/accounts/:account_id/csp_settings
- url:DELETE|/api/v1/accounts/:account_id/csp_settings/domains
- url:POST|/api/v1/accounts/:account_id/csp_settings/domains
- url:POST|/api/v1/accounts/:account_id/csp_settings/domains/batch_create
- url:PUT|/api/v1/accounts/:account_id/csp_settings/lock
- url:GET|/api/v1/accounts/:account_id/developer_keys
- url:POST|/api/v1/accounts/:account_id/developer_keys
- url:POST|/api/v1/accounts/:account_id/developer_keys/:developer_key_id/developer_key_account_bindings
- url:GET|/api/v1/accounts/:account_id/enrollments/:id
- url:GET|/api/v1/accounts/:account_id/external_tools
- url:POST|/api/v1/accounts/:account_id/external_tools
- url:DELETE|/api/v1/accounts/:account_id/external_tools/rce_favorites/:id
- url:POST|/api/v1/accounts/:account_id/external_tools/rce_favorites/:id
- url:GET|/api/v1/accounts/:account_id/external_tools/sessionless_launch
- url:DELETE|/api/v1/accounts/:account_id/external_tools/top_nav_favorites/:id
- url:POST|/api/v1/accounts/:account_id/external_tools/top_nav_favorites/:id
- url:DELETE|/api/v1/accounts/:account_id/external_tools/:external_tool_id
- url:GET|/api/v1/accounts/:account_id/external_tools/:external_tool_id
- url:PUT|/api/v1/accounts/:account_id/external_tools/:external_tool_id
- url:GET|/api/v1/accounts/:account_id/features
- url:GET|/api/v1/accounts/:account_id/features/enabled
- url:DELETE|/api/v1/accounts/:account_id/features/flags/:feature
- url:GET|/api/v1/accounts/:account_id/features/flags/:feature
- url:PUT|/api/v1/accounts/:account_id/features/flags/:feature
- url:POST|/api/v1/accounts/:account_id/folders
- url:GET|/api/v1/accounts/:account_id/grading_period_sets
- url:POST|/api/v1/accounts/:account_id/grading_period_sets
- url:DELETE|/api/v1/accounts/:account_id/grading_period_sets/:id
- url:PATCH|/api/v1/accounts/:account_id/grading_period_sets/:id
- url:GET|/api/v1/accounts/:account_id/grading_periods
- url:DELETE|/api/v1/accounts/:account_id/grading_periods/:id
- url:GET|/api/v1/accounts/:account_id/grading_standards
- url:POST|/api/v1/accounts/:account_id/grading_standards
- url:DELETE|/api/v1/accounts/:account_id/grading_standards/:grading_standard_id
- url:GET|/api/v1/accounts/:account_id/grading_standards/:grading_standard_id
- url:PUT|/api/v1/accounts/:account_id/grading_standards/:grading_standard_id
- url:GET|/api/v1/accounts/:account_id/group_categories
- url:POST|/api/v1/accounts/:account_id/group_categories
- url:GET|/api/v1/accounts/:account_id/groups
- url:GET|/api/v1/accounts/:account_id/help_links
- url:GET|/api/v1/accounts/:account_id/logins
- url:POST|/api/v1/accounts/:account_id/logins
- url:PUT|/api/v1/accounts/:account_id/logins/:id
- url:GET|/api/v1/accounts/:account_id/lti_apps/launch_definitions
- url:GET|/api/v1/accounts/:account_id/lti_registration_by_client_id/:client_id
- url:GET|/api/v1/accounts/:account_id/lti_registrations
- url:POST|/api/v1/accounts/:account_id/lti_registrations
- url:GET|/api/v1/accounts/:account_id/lti_registrations/by_utid/:utid
- url:GET|/api/v1/accounts/:account_id/lti_registrations/install_status/:client_id
- url:DELETE|/api/v1/accounts/:account_id/lti_registrations/:id
- url:GET|/api/v1/accounts/:account_id/lti_registrations/:id
- url:PUT|/api/v1/accounts/:account_id/lti_registrations/:id
- url:DELETE|/api/v1/accounts/:account_id/lti_registrations/:id/bind
- url:POST|/api/v1/accounts/:account_id/lti_registrations/:id/bind
- url:GET|/api/v1/accounts/:account_id/lti_registrations/:id/history
- url:POST|/api/v1/accounts/:account_id/lti_registrations/:id/install_from_template
- url:GET|/api/v1/accounts/:account_id/lti_registrations/:id/latest_update_request
- url:GET|/api/v1/accounts/:account_id/lti_registrations/:id/overlay_history
- url:PUT|/api/v1/accounts/:account_id/lti_registrations/:id/reset
- url:GET|/api/v1/accounts/:account_id/lti_registrations/:id/update_requests/:update_request_id
- url:PUT|/api/v1/accounts/:account_id/lti_registrations/:id/update_requests/:update_request_id/apply
- url:GET|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls
- url:POST|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls/bulk
- url:DELETE|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls/:id
- url:GET|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls/:id
- url:PUT|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls/:id
- url:GET|/api/v1/accounts/:account_id/lti_registrations/:registration_id/deployments/:deployment_id/context_search
- url:GET|/api/v1/accounts/:account_id/outcome_group_links
- url:GET|/api/v1/accounts/:account_id/outcome_groups
- url:DELETE|/api/v1/accounts/:account_id/outcome_groups/:id
- url:GET|/api/v1/accounts/:account_id/outcome_groups/:id
- url:PUT|/api/v1/accounts/:account_id/outcome_groups/:id
- url:POST|/api/v1/accounts/:account_id/outcome_groups/:id/import
- url:GET|/api/v1/accounts/:account_id/outcome_groups/:id/outcomes
- url:POST|/api/v1/accounts/:account_id/outcome_groups/:id/outcomes
- url:DELETE|/api/v1/accounts/:account_id/outcome_groups/:id/outcomes/:outcome_id
- url:PUT|/api/v1/accounts/:account_id/outcome_groups/:id/outcomes/:outcome_id
- url:GET|/api/v1/accounts/:account_id/outcome_groups/:id/subgroups
- url:POST|/api/v1/accounts/:account_id/outcome_groups/:id/subgroups
- url:POST|/api/v1/accounts/:account_id/outcome_imports
- url:GET|/api/v1/accounts/:account_id/outcome_imports/:id
- url:GET|/api/v1/accounts/:account_id/outcome_imports/:id/created_group_ids
- url:GET|/api/v1/accounts/:account_id/outcome_proficiency
- url:POST|/api/v1/accounts/:account_id/outcome_proficiency
- url:GET|/api/v1/accounts/:account_id/permissions
- url:GET|/api/v1/accounts/:account_id/reports
- url:GET|/api/v1/accounts/:account_id/reports/:report
- url:POST|/api/v1/accounts/:account_id/reports/:report
- url:DELETE|/api/v1/accounts/:account_id/reports/:report/:id
- url:GET|/api/v1/accounts/:account_id/reports/:report/:id
- url:PUT|/api/v1/accounts/:account_id/reports/:report/:id/abort
- url:GET|/api/v1/accounts/:account_id/roles
- url:POST|/api/v1/accounts/:account_id/roles
- url:GET|/api/v1/accounts/:account_id/roles/permissions
- url:DELETE|/api/v1/accounts/:account_id/roles/:id
- url:GET|/api/v1/accounts/:account_id/roles/:id
- url:PUT|/api/v1/accounts/:account_id/roles/:id
- url:POST|/api/v1/accounts/:account_id/roles/:id/activate
- url:GET|/api/v1/accounts/:account_id/root_outcome_group
- url:GET|/api/v1/accounts/:account_id/rubrics
- url:POST|/api/v1/accounts/:account_id/rubrics/upload
- url:GET|/api/v1/accounts/:account_id/rubrics/upload/:id
- url:GET|/api/v1/accounts/:account_id/rubrics/:id
- url:GET|/api/v1/accounts/:account_id/rubrics/:id/used_locations
- url:GET|/api/v1/accounts/:account_id/scopes
- url:POST|/api/v1/accounts/:account_id/self_registration
- url:GET|/api/v1/accounts/:account_id/settings
- url:POST|/api/v1/accounts/:account_id/shared_brand_configs
- url:PUT|/api/v1/accounts/:account_id/shared_brand_configs/:id
- url:GET|/api/v1/accounts/:account_id/sis_import_errors
- url:GET|/api/v1/accounts/:account_id/sis_imports
- url:POST|/api/v1/accounts/:account_id/sis_imports
- url:PUT|/api/v1/accounts/:account_id/sis_imports/abort_all_pending
- url:GET|/api/v1/accounts/:account_id/sis_imports/importing
- url:GET|/api/v1/accounts/:account_id/sis_imports/:id
- url:PUT|/api/v1/accounts/:account_id/sis_imports/:id/abort
- url:GET|/api/v1/accounts/:account_id/sis_imports/:id/errors
- url:PUT|/api/v1/accounts/:account_id/sis_imports/:id/restore_states
- url:GET|/api/v1/accounts/:account_id/sso_settings
- url:PUT|/api/v1/accounts/:account_id/sso_settings
- url:GET|/api/v1/accounts/:account_id/sub_accounts
- url:POST|/api/v1/accounts/:account_id/sub_accounts
- url:DELETE|/api/v1/accounts/:account_id/sub_accounts/:id
- url:GET|/api/v1/accounts/:account_id/tabs
- url:GET|/api/v1/accounts/:account_id/temporary_enrollment_pairings
- url:POST|/api/v1/accounts/:account_id/temporary_enrollment_pairings
- url:GET|/api/v1/accounts/:account_id/temporary_enrollment_pairings/new
- url:DELETE|/api/v1/accounts/:account_id/temporary_enrollment_pairings/:id
- url:GET|/api/v1/accounts/:account_id/temporary_enrollment_pairings/:id
- url:GET|/api/v1/accounts/:account_id/terms
- url:POST|/api/v1/accounts/:account_id/terms
- url:DELETE|/api/v1/accounts/:account_id/terms/:id
- url:GET|/api/v1/accounts/:account_id/terms/:id
- url:PUT|/api/v1/accounts/:account_id/terms/:id
- url:GET|/api/v1/accounts/:account_id/terms_of_service
- url:DELETE|/api/v1/accounts/:account_id/users
- url:GET|/api/v1/accounts/:account_id/users
- url:POST|/api/v1/accounts/:account_id/users
- url:PUT|/api/v1/accounts/:account_id/users/bulk_update
- url:DELETE|/api/v1/accounts/:account_id/users/:user_id
- url:PUT|/api/v1/accounts/:account_id/users/:user_id/restore
- url:GET|/api/v1/accounts/:account_id/visible_calendars_count
- url:POST|/api/v1/accounts/:current_account_id/lti_registrations/:registration_id/controls
- url:GET|/api/v1/accounts/:id
- url:PUT|/api/v1/accounts/:id
- url:GET|/api/v1/announcements
- url:GET|/api/v1/appointment_groups
- url:POST|/api/v1/appointment_groups
- url:GET|/api/v1/appointment_groups/next_appointment
- url:DELETE|/api/v1/appointment_groups/:id
- url:GET|/api/v1/appointment_groups/:id
- url:PUT|/api/v1/appointment_groups/:id
- url:GET|/api/v1/appointment_groups/:id/groups
- url:GET|/api/v1/appointment_groups/:id/users
- url:GET|/api/v1/audit/authentication/accounts/:account_id
- url:GET|/api/v1/audit/authentication/logins/:login_id
- url:GET|/api/v1/audit/authentication/users/:user_id
- url:GET|/api/v1/audit/course/accounts/:account_id
- url:GET|/api/v1/audit/course/courses/:course_id
- url:GET|/api/v1/audit/grade_change
- url:GET|/api/v1/audit/grade_change/assignments/:assignment_id
- url:GET|/api/v1/audit/grade_change/courses/:course_id
- url:GET|/api/v1/audit/grade_change/graders/:grader_id
- url:GET|/api/v1/audit/grade_change/students/:student_id
- url:GET|/api/v1/brand_variables
- url:GET|/api/v1/calendar_events
- url:POST|/api/v1/calendar_events
- url:POST|/api/v1/calendar_events/save_enabled_account_calendars
- url:DELETE|/api/v1/calendar_events/:id
- url:GET|/api/v1/calendar_events/:id
- url:PUT|/api/v1/calendar_events/:id
- url:POST|/api/v1/calendar_events/:id/reservations
- url:POST|/api/v1/calendar_events/:id/reservations/:participant_id
- url:GET|/api/v1/career/enabled
- url:GET|/api/v1/career/experience_summary
- url:POST|/api/v1/career/switch_experience
- url:POST|/api/v1/career/switch_role
- url:GET|/api/v1/career/user_context
- url:GET|/api/v1/collaborations/:id/members
- url:GET|/api/v1/comm_messages
- url:GET|/api/v1/conferences
- url:GET|/api/v1/conversations
- url:POST|/api/v1/conversations
- url:PUT|/api/v1/conversations
- url:GET|/api/v1/conversations/batches
- url:GET|/api/v1/conversations/find_recipients
- url:POST|/api/v1/conversations/mark_all_as_read
- url:GET|/api/v1/conversations/unread_count
- url:DELETE|/api/v1/conversations/:id
- url:GET|/api/v1/conversations/:id
- url:PUT|/api/v1/conversations/:id
- url:POST|/api/v1/conversations/:id/add_message
- url:POST|/api/v1/conversations/:id/add_recipients
- url:POST|/api/v1/conversations/:id/remove_messages
- url:GET|/api/v1/course_accounts
- url:GET|/api/v1/course_creation_accounts
- url:GET|/api/v1/courses
- url:GET|/api/v1/courses/:course_id/activity_stream
- url:GET|/api/v1/courses/:course_id/activity_stream/summary
- url:GET|/api/v1/courses/:course_id/ai_experiences
- url:POST|/api/v1/courses/:course_id/ai_experiences
- url:GET|/api/v1/courses/:course_id/ai_experiences/new
- url:GET|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations
- url:POST|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations
- url:DELETE|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id
- url:GET|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id
- url:GET|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/evaluation
- url:POST|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/evaluation
- url:POST|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/messages
- url:POST|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/messages/:message_id/feedback
- url:DELETE|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/messages/:message_id/feedback/:feedback_id
- url:DELETE|/api/v1/courses/:course_id/ai_experiences/:id
- url:GET|/api/v1/courses/:course_id/ai_experiences/:id
- url:PUT|/api/v1/courses/:course_id/ai_experiences/:id
- url:GET|/api/v1/courses/:course_id/ai_experiences/:id/ai_conversations
- url:GET|/api/v1/courses/:course_id/ai_experiences/:id/ai_conversations/:conversation_id
- url:GET|/api/v1/courses/:course_id/ai_experiences/:id/edit
- url:GET|/api/v1/courses/:course_id/analytics/activity
- url:GET|/api/v1/courses/:course_id/analytics/assignments
- url:GET|/api/v1/courses/:course_id/analytics/student_summaries
- url:GET|/api/v1/courses/:course_id/analytics/users/:student_id/activity
- url:GET|/api/v1/courses/:course_id/analytics/users/:student_id/assignments
- url:GET|/api/v1/courses/:course_id/analytics/users/:student_id/communication
- url:POST|/api/v1/courses/:course_id/assign_outcome_order
- url:GET|/api/v1/courses/:course_id/assignment_groups
- url:POST|/api/v1/courses/:course_id/assignment_groups
- url:DELETE|/api/v1/courses/:course_id/assignment_groups/:assignment_group_id
- url:GET|/api/v1/courses/:course_id/assignment_groups/:assignment_group_id
- url:PUT|/api/v1/courses/:course_id/assignment_groups/:assignment_group_id
- url:GET|/api/v1/courses/:course_id/assignment_groups/:assignment_group_id/assignments
- url:GET|/api/v1/courses/:course_id/assignments
- url:POST|/api/v1/courses/:course_id/assignments
- url:PUT|/api/v1/courses/:course_id/assignments/bulk_update
- url:GET|/api/v1/courses/:course_id/assignments/gradeable_students
- url:GET|/api/v1/courses/:course_id/assignments/overrides
- url:POST|/api/v1/courses/:course_id/assignments/overrides
- url:PUT|/api/v1/courses/:course_id/assignments/overrides
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/allocate
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/anonymous_provisional_grades/status
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/anonymous_submissions/:anonymous_id
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/anonymous_submissions/:anonymous_id
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/date_details
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/date_details
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/duplicate
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/extensions
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/gradeable_students
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/moderated_students
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/moderated_students
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/overrides
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/overrides
- url:DELETE|/api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/peer_reviews
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/bulk_select
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/publish
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/publish_async
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/status
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/:provisional_grade_id/select
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submission_summary
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/update_grades
- url:DELETE|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/annotation_notification
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/comments/files
- url:DELETE|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/comments/:id
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/comments/:id
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/document_annotations/read
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/document_annotations/read
- url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/files
- url:DELETE|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/read
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/read
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/read/:item
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/rubric_assessments/read
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/rubric_assessments/read
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/rubric_comments/read
- url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/rubric_comments/read
- url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/users/:user_id/group_members
- url:DELETE|/api/v1/courses/:course_id/assignments/:id
- url:GET|/api/v1/courses/:course_id/assignments/:id
- url:PUT|/api/v1/courses/:course_id/assignments/:id
- url:GET|/api/v1/courses/:course_id/blackout_dates
- url:POST|/api/v1/courses/:course_id/blackout_dates
- url:PUT|/api/v1/courses/:course_id/blackout_dates
- url:GET|/api/v1/courses/:course_id/blackout_dates/new
- url:DELETE|/api/v1/courses/:course_id/blackout_dates/:id
- url:GET|/api/v1/courses/:course_id/blackout_dates/:id
- url:PUT|/api/v1/courses/:course_id/blackout_dates/:id
- url:GET|/api/v1/courses/:course_id/block_editor_templates
- url:GET|/api/v1/courses/:course_id/blueprint_subscriptions
- url:GET|/api/v1/courses/:course_id/blueprint_subscriptions/:subscription_id/migrations
- url:GET|/api/v1/courses/:course_id/blueprint_subscriptions/:subscription_id/migrations/:id
- url:GET|/api/v1/courses/:course_id/blueprint_subscriptions/:subscription_id/migrations/:id/details
- url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id
- url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/associated_courses
- url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/migrations
- url:POST|/api/v1/courses/:course_id/blueprint_templates/:template_id/migrations
- url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/migrations/:id
- url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/migrations/:id/details
- url:PUT|/api/v1/courses/:course_id/blueprint_templates/:template_id/restrict_item
- url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/unsynced_changes
- url:PUT|/api/v1/courses/:course_id/blueprint_templates/:template_id/update_associations
- url:GET|/api/v1/courses/:course_id/brand_variables
- url:GET|/api/v1/courses/:course_id/bulk_user_progress
- url:GET|/api/v1/courses/:course_id/bulk_user_tags
- url:GET|/api/v1/courses/:course_id/calendar_events/timetable
- url:POST|/api/v1/courses/:course_id/calendar_events/timetable
- url:POST|/api/v1/courses/:course_id/calendar_events/timetable_events
- url:GET|/api/v1/courses/:course_id/collaborations
- url:GET|/api/v1/courses/:course_id/conferences
- url:GET|/api/v1/courses/:course_id/content_exports
- url:POST|/api/v1/courses/:course_id/content_exports
- url:GET|/api/v1/courses/:course_id/content_exports/:id
- url:GET|/api/v1/courses/:course_id/content_licenses
- url:GET|/api/v1/courses/:course_id/content_migrations
- url:POST|/api/v1/courses/:course_id/content_migrations
- url:GET|/api/v1/courses/:course_id/content_migrations/migrators
- url:GET|/api/v1/courses/:course_id/content_migrations/:content_migration_id/migration_issues
- url:GET|/api/v1/courses/:course_id/content_migrations/:content_migration_id/migration_issues/:id
- url:PUT|/api/v1/courses/:course_id/content_migrations/:content_migration_id/migration_issues/:id
- url:GET|/api/v1/courses/:course_id/content_migrations/:id
- url:PUT|/api/v1/courses/:course_id/content_migrations/:id
- url:GET|/api/v1/courses/:course_id/content_migrations/:id/asset_id_mapping
- url:GET|/api/v1/courses/:course_id/content_migrations/:id/selective_data
- url:GET|/api/v1/courses/:course_id/content_share_users
- url:POST|/api/v1/courses/:course_id/course_copy
- url:GET|/api/v1/courses/:course_id/course_copy/:id
- url:POST|/api/v1/courses/:course_id/course_pacing
- url:DELETE|/api/v1/courses/:course_id/course_pacing/:id
- url:GET|/api/v1/courses/:course_id/course_pacing/:id
- url:PUT|/api/v1/courses/:course_id/course_pacing/:id
- url:GET|/api/v1/courses/:course_id/csp_settings
- url:PUT|/api/v1/courses/:course_id/csp_settings
- url:PUT|/api/v1/courses/:course_id/custom_gradebook_column_data
- url:GET|/api/v1/courses/:course_id/custom_gradebook_columns
- url:POST|/api/v1/courses/:course_id/custom_gradebook_columns
- url:POST|/api/v1/courses/:course_id/custom_gradebook_columns/reorder
- url:DELETE|/api/v1/courses/:course_id/custom_gradebook_columns/:id
- url:PUT|/api/v1/courses/:course_id/custom_gradebook_columns/:id
- url:GET|/api/v1/courses/:course_id/custom_gradebook_columns/:id/data
- url:PUT|/api/v1/courses/:course_id/custom_gradebook_columns/:id/data/:user_id
- url:GET|/api/v1/courses/:course_id/discussion_topics
- url:POST|/api/v1/courses/:course_id/discussion_topics
- url:PUT|/api/v1/courses/:course_id/discussion_topics/read_all
- url:POST|/api/v1/courses/:course_id/discussion_topics/reorder
- url:GET|/api/v1/courses/:course_id/discussion_topics/:discussion_topic_id/date_details
- url:PUT|/api/v1/courses/:course_id/discussion_topics/:discussion_topic_id/date_details
- url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id
- url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id
- url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id
- url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/duplicate
- url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries
- url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries
- url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/rating
- url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/read
- url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/read
- url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/replies
- url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/replies
- url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:id
- url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:id
- url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/entry_list
- url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/read
- url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/read
- url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/read_all
- url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/read_all
- url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/subscribed
- url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/subscribed
- url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/summaries
- url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/summaries
- url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/summaries/disable
- url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/summaries/:summary_id/feedback
- url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/view
- url:GET|/api/v1/courses/:course_id/effective_due_dates
- url:POST|/api/v1/courses/:course_id/enqueue_outcome_rollup_calculation
- url:GET|/api/v1/courses/:course_id/enrollments
- url:POST|/api/v1/courses/:course_id/enrollments
- url:DELETE|/api/v1/courses/:course_id/enrollments/:id
- url:POST|/api/v1/courses/:course_id/enrollments/:id/accept
- url:PUT|/api/v1/courses/:course_id/enrollments/:id/reactivate
- url:POST|/api/v1/courses/:course_id/enrollments/:id/reject
- url:POST|/api/v1/courses/:course_id/epub_exports
- url:GET|/api/v1/courses/:course_id/epub_exports/:id
- url:GET|/api/v1/courses/:course_id/external_feeds
- url:POST|/api/v1/courses/:course_id/external_feeds
- url:DELETE|/api/v1/courses/:course_id/external_feeds/:external_feed_id
- url:GET|/api/v1/courses/:course_id/external_tools
- url:POST|/api/v1/courses/:course_id/external_tools
- url:GET|/api/v1/courses/:course_id/external_tools/sessionless_launch
- url:GET|/api/v1/courses/:course_id/external_tools/visible_course_nav_tools
- url:DELETE|/api/v1/courses/:course_id/external_tools/:external_tool_id
- url:GET|/api/v1/courses/:course_id/external_tools/:external_tool_id
- url:PUT|/api/v1/courses/:course_id/external_tools/:external_tool_id
- url:GET|/api/v1/courses/:course_id/features
- url:GET|/api/v1/courses/:course_id/features/enabled
- url:DELETE|/api/v1/courses/:course_id/features/flags/:feature
- url:GET|/api/v1/courses/:course_id/features/flags/:feature
- url:PUT|/api/v1/courses/:course_id/features/flags/:feature
- url:GET|/api/v1/courses/:course_id/files
- url:POST|/api/v1/courses/:course_id/files
- url:GET|/api/v1/courses/:course_id/files/file_ref/:migration_id
- url:GET|/api/v1/courses/:course_id/files/quota
- url:GET|/api/v1/courses/:course_id/files/:attachment_id/date_details
- url:PUT|/api/v1/courses/:course_id/files/:attachment_id/date_details
- url:GET|/api/v1/courses/:course_id/files/:id
- url:GET|/api/v1/courses/:course_id/folders
- url:POST|/api/v1/courses/:course_id/folders
- url:GET|/api/v1/courses/:course_id/folders/by_path
- url:GET|/api/v1/courses/:course_id/folders/by_path/*full_path
- url:GET|/api/v1/courses/:course_id/folders/media
- url:GET|/api/v1/courses/:course_id/folders/:id
- url:GET|/api/v1/courses/:course_id/front_page
- url:PUT|/api/v1/courses/:course_id/front_page
- url:GET|/api/v1/courses/:course_id/gradebook_history/days
- url:GET|/api/v1/courses/:course_id/gradebook_history/feed
- url:GET|/api/v1/courses/:course_id/gradebook_history/:date
- url:GET|/api/v1/courses/:course_id/gradebook_history/:date/graders/:grader_id/assignments/:assignment_id/submissions
- url:GET|/api/v1/courses/:course_id/grading_periods
- url:PATCH|/api/v1/courses/:course_id/grading_periods/batch_update
- url:DELETE|/api/v1/courses/:course_id/grading_periods/:id
- url:GET|/api/v1/courses/:course_id/grading_periods/:id
- url:PUT|/api/v1/courses/:course_id/grading_periods/:id
- url:GET|/api/v1/courses/:course_id/grading_standards
- url:POST|/api/v1/courses/:course_id/grading_standards
- url:DELETE|/api/v1/courses/:course_id/grading_standards/:grading_standard_id
- url:GET|/api/v1/courses/:course_id/grading_standards/:grading_standard_id
- url:PUT|/api/v1/courses/:course_id/grading_standards/:grading_standard_id
- url:GET|/api/v1/courses/:course_id/group_categories
- url:POST|/api/v1/courses/:course_id/group_categories
- url:POST|/api/v1/courses/:course_id/group_categories/bulk_manage_differentiation_tag
- url:GET|/api/v1/courses/:course_id/group_categories/differentiation_tag_candidate_count
- url:GET|/api/v1/courses/:course_id/group_categories/export_tags
- url:POST|/api/v1/courses/:course_id/group_categories/import_tags
- url:GET|/api/v1/courses/:course_id/groups
- url:GET|/api/v1/courses/:course_id/live_assessments
- url:POST|/api/v1/courses/:course_id/live_assessments
- url:GET|/api/v1/courses/:course_id/live_assessments/:assessment_id/results
- url:POST|/api/v1/courses/:course_id/live_assessments/:assessment_id/results
- url:GET|/api/v1/courses/:course_id/lti_apps/launch_definitions
- url:GET|/api/v1/courses/:course_id/lti_resource_links
- url:POST|/api/v1/courses/:course_id/lti_resource_links
- url:POST|/api/v1/courses/:course_id/lti_resource_links/bulk
- url:DELETE|/api/v1/courses/:course_id/lti_resource_links/:id
- url:GET|/api/v1/courses/:course_id/lti_resource_links/:id
- url:PUT|/api/v1/courses/:course_id/lti_resource_links/:id
- url:GET|/api/v1/courses/:course_id/media_attachments
- url:GET|/api/v1/courses/:course_id/media_objects
- url:GET|/api/v1/courses/:course_id/module_item_sequence
- url:GET|/api/v1/courses/:course_id/modules
- url:POST|/api/v1/courses/:course_id/modules
- url:GET|/api/v1/courses/:course_id/modules/:context_module_id/assignment_overrides
- url:PUT|/api/v1/courses/:course_id/modules/:context_module_id/assignment_overrides
- url:GET|/api/v1/courses/:course_id/modules/:context_module_id/date_details
- url:DELETE|/api/v1/courses/:course_id/modules/:id
- url:GET|/api/v1/courses/:course_id/modules/:id
- url:PUT|/api/v1/courses/:course_id/modules/:id
- url:PUT|/api/v1/courses/:course_id/modules/:id/relock
- url:GET|/api/v1/courses/:course_id/modules/:module_id/items
- url:POST|/api/v1/courses/:course_id/modules/:module_id/items
- url:DELETE|/api/v1/courses/:course_id/modules/:module_id/items/:id
- url:GET|/api/v1/courses/:course_id/modules/:module_id/items/:id
- url:PUT|/api/v1/courses/:course_id/modules/:module_id/items/:id
- url:PUT|/api/v1/courses/:course_id/modules/:module_id/items/:id/done
- url:POST|/api/v1/courses/:course_id/modules/:module_id/items/:id/mark_read
- url:POST|/api/v1/courses/:course_id/modules/:module_id/items/:id/select_mastery_path
- url:GET|/api/v1/courses/:course_id/new_quizzes/assignment_overrides
- url:GET|/api/v1/courses/:course_id/outcome_alignments
- url:GET|/api/v1/courses/:course_id/outcome_group_links
- url:GET|/api/v1/courses/:course_id/outcome_groups
- url:DELETE|/api/v1/courses/:course_id/outcome_groups/:id
- url:GET|/api/v1/courses/:course_id/outcome_groups/:id
- url:PUT|/api/v1/courses/:course_id/outcome_groups/:id
- url:POST|/api/v1/courses/:course_id/outcome_groups/:id/import
- url:GET|/api/v1/courses/:course_id/outcome_groups/:id/outcomes
- url:POST|/api/v1/courses/:course_id/outcome_groups/:id/outcomes
- url:DELETE|/api/v1/courses/:course_id/outcome_groups/:id/outcomes/:outcome_id
- url:PUT|/api/v1/courses/:course_id/outcome_groups/:id/outcomes/:outcome_id
- url:GET|/api/v1/courses/:course_id/outcome_groups/:id/subgroups
- url:POST|/api/v1/courses/:course_id/outcome_groups/:id/subgroups
- url:POST|/api/v1/courses/:course_id/outcome_imports
- url:GET|/api/v1/courses/:course_id/outcome_imports/:id
- url:GET|/api/v1/courses/:course_id/outcome_imports/:id/created_group_ids
- url:GET|/api/v1/courses/:course_id/outcome_mastery_distribution
- url:GET|/api/v1/courses/:course_id/outcome_proficiency
- url:POST|/api/v1/courses/:course_id/outcome_proficiency
- url:GET|/api/v1/courses/:course_id/outcome_results
- url:GET|/api/v1/courses/:course_id/outcome_rollups
- url:GET|/api/v1/courses/:course_id/outcomes/:outcome_id/contributing_scores
- url:GET|/api/v1/courses/:course_id/pages
- url:POST|/api/v1/courses/:course_id/pages
- url:DELETE|/api/v1/courses/:course_id/pages/:url_or_id
- url:GET|/api/v1/courses/:course_id/pages/:url_or_id
- url:PUT|/api/v1/courses/:course_id/pages/:url_or_id
- url:GET|/api/v1/courses/:course_id/pages/:url_or_id/date_details
- url:PUT|/api/v1/courses/:course_id/pages/:url_or_id/date_details
- url:POST|/api/v1/courses/:course_id/pages/:url_or_id/duplicate
- url:GET|/api/v1/courses/:course_id/pages/:url_or_id/revisions
- url:GET|/api/v1/courses/:course_id/pages/:url_or_id/revisions/latest
- url:GET|/api/v1/courses/:course_id/pages/:url_or_id/revisions/:revision_id
- url:POST|/api/v1/courses/:course_id/pages/:url_or_id/revisions/:revision_id
- url:GET|/api/v1/courses/:course_id/permissions
- url:GET|/api/v1/courses/:course_id/potential_collaborators
- url:POST|/api/v1/courses/:course_id/preview_html
- url:POST|/api/v1/courses/:course_id/quiz_extensions
- url:GET|/api/v1/courses/:course_id/quizzes
- url:POST|/api/v1/courses/:course_id/quizzes
- url:GET|/api/v1/courses/:course_id/quizzes/assignment_overrides
- url:DELETE|/api/v1/courses/:course_id/quizzes/:id
- url:GET|/api/v1/courses/:course_id/quizzes/:id
- url:PUT|/api/v1/courses/:course_id/quizzes/:id
- url:POST|/api/v1/courses/:course_id/quizzes/:id/reorder
- url:POST|/api/v1/courses/:course_id/quizzes/:id/submission_users/message
- url:POST|/api/v1/courses/:course_id/quizzes/:id/validate_access_code
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/date_details
- url:PUT|/api/v1/courses/:course_id/quizzes/:quiz_id/date_details
- url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/extensions
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/groups
- url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/groups
- url:DELETE|/api/v1/courses/:course_id/quizzes/:quiz_id/groups/:id
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/groups/:id
- url:PUT|/api/v1/courses/:course_id/quizzes/:quiz_id/groups/:id
- url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/groups/:id/reorder
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/ip_filters
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/questions
- url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/questions
- url:DELETE|/api/v1/courses/:course_id/quizzes/:quiz_id/questions/:id
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/questions/:id
- url:PUT|/api/v1/courses/:course_id/quizzes/:quiz_id/questions/:id
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/reports
- url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/reports
- url:DELETE|/api/v1/courses/:course_id/quizzes/:quiz_id/reports/:id
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/reports/:id
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/statistics
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submission
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions
- url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions
- url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/self/files
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id
- url:PUT|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id
- url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id/complete
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id/events
- url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id/events
- url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id/time
- url:GET|/api/v1/courses/:course_id/recent_students
- url:GET|/api/v1/courses/:course_id/reports/:report_type
- url:POST|/api/v1/courses/:course_id/reports/:report_type
- url:GET|/api/v1/courses/:course_id/reports/:report_type/:id
- url:POST|/api/v1/courses/:course_id/reset_content
- url:POST|/api/v1/courses/:course_id/restore/:version_id
- url:GET|/api/v1/courses/:course_id/root_outcome_group
- url:POST|/api/v1/courses/:course_id/rubric_associations
- url:DELETE|/api/v1/courses/:course_id/rubric_associations/:id
- url:PUT|/api/v1/courses/:course_id/rubric_associations/:id
- url:POST|/api/v1/courses/:course_id/rubric_associations/:rubric_association_id/rubric_assessments
- url:DELETE|/api/v1/courses/:course_id/rubric_associations/:rubric_association_id/rubric_assessments/:id
- url:PUT|/api/v1/courses/:course_id/rubric_associations/:rubric_association_id/rubric_assessments/:id
- url:GET|/api/v1/courses/:course_id/rubrics
- url:POST|/api/v1/courses/:course_id/rubrics
- url:POST|/api/v1/courses/:course_id/rubrics/upload
- url:GET|/api/v1/courses/:course_id/rubrics/upload/:id
- url:DELETE|/api/v1/courses/:course_id/rubrics/:id
- url:GET|/api/v1/courses/:course_id/rubrics/:id
- url:PUT|/api/v1/courses/:course_id/rubrics/:id
- url:GET|/api/v1/courses/:course_id/rubrics/:id/used_locations
- url:GET|/api/v1/courses/:course_id/search_users
- url:GET|/api/v1/courses/:course_id/sections
- url:POST|/api/v1/courses/:course_id/sections
- url:GET|/api/v1/courses/:course_id/sections/:id
- url:GET|/api/v1/courses/:course_id/settings
- url:PUT|/api/v1/courses/:course_id/settings
- url:GET|/api/v1/courses/:course_id/smartsearch
- url:GET|/api/v1/courses/:course_id/student_view_student
- url:GET|/api/v1/courses/:course_id/students
- url:GET|/api/v1/courses/:course_id/students/submissions
- url:POST|/api/v1/courses/:course_id/study_assist
- url:PUT|/api/v1/courses/:course_id/submissions/bulk_mark_read
- url:POST|/api/v1/courses/:course_id/submissions/update_grades
- url:PUT|/api/v1/courses/:course_id/submissions/:user_id/clear_unread
- url:GET|/api/v1/courses/:course_id/tabs
- url:PUT|/api/v1/courses/:course_id/tabs/:tab_id
- url:GET|/api/v1/courses/:course_id/todo
- url:DELETE|/api/v1/courses/:course_id/usage_rights
- url:PUT|/api/v1/courses/:course_id/usage_rights
- url:GET|/api/v1/courses/:course_id/users
- url:GET|/api/v1/courses/:course_id/users/:id
- url:PUT|/api/v1/courses/:course_id/users/:user_id/last_attended
- url:GET|/api/v1/courses/:course_id/users/:user_id/progress
- url:PUT|/api/v1/courses/:course_id/what_if_grades/reset
- url:DELETE|/api/v1/courses/:id
- url:GET|/api/v1/courses/:id
- url:PUT|/api/v1/courses/:id
- url:POST|/api/v1/courses/:id/dismiss_migration_limitation_message
- url:GET|/api/v1/courses/:id/late_policy
- url:PATCH|/api/v1/courses/:id/late_policy
- url:POST|/api/v1/courses/:id/late_policy
- url:DELETE|/api/v1/developer_keys/:id
- url:PUT|/api/v1/developer_keys/:id
- url:POST|/api/v1/developer_keys/:id/regenerate_secret
- url:GET|/api/v1/discovery_pages
- url:PUT|/api/v1/discovery_pages
- url:POST|/api/v1/discovery_pages/token
- url:PUT|/api/v1/eportfolios/:eportfolio_id/moderate
- url:GET|/api/v1/eportfolios/:eportfolio_id/pages
- url:PUT|/api/v1/eportfolios/:eportfolio_id/restore
- url:DELETE|/api/v1/eportfolios/:id
- url:GET|/api/v1/eportfolios/:id
- url:GET|/api/v1/epub_exports
- url:POST|/api/v1/error_reports
- url:GET|/api/v1/external_tools/visible_course_nav_tools
- url:GET|/api/v1/features/environment
- url:POST|/api/v1/files/update_word_count
- url:DELETE|/api/v1/files/:id
- url:GET|/api/v1/files/:id
- url:PUT|/api/v1/files/:id
- url:GET|/api/v1/files/:id/icon_metadata
- url:GET|/api/v1/files/:id/public_url
- url:POST|/api/v1/files/:id/reset_verifier
- url:POST|/api/v1/folders/:dest_folder_id/copy_file
- url:POST|/api/v1/folders/:dest_folder_id/copy_folder
- url:POST|/api/v1/folders/:folder_id/files
- url:POST|/api/v1/folders/:folder_id/folders
- url:DELETE|/api/v1/folders/:id
- url:GET|/api/v1/folders/:id
- url:PUT|/api/v1/folders/:id
- url:GET|/api/v1/folders/:id/files
- url:GET|/api/v1/folders/:id/folders
- url:DELETE|/api/v1/global/outcome_groups/:id
- url:GET|/api/v1/global/outcome_groups/:id
- url:PUT|/api/v1/global/outcome_groups/:id
- url:POST|/api/v1/global/outcome_groups/:id/import
- url:GET|/api/v1/global/outcome_groups/:id/outcomes
- url:POST|/api/v1/global/outcome_groups/:id/outcomes
- url:DELETE|/api/v1/global/outcome_groups/:id/outcomes/:outcome_id
- url:PUT|/api/v1/global/outcome_groups/:id/outcomes/:outcome_id
- url:GET|/api/v1/global/outcome_groups/:id/subgroups
- url:POST|/api/v1/global/outcome_groups/:id/subgroups
- url:GET|/api/v1/global/root_outcome_group
- url:PATCH|/api/v1/grading_period_sets/:set_id/grading_periods/batch_update
- url:DELETE|/api/v1/group_categories/:group_category_id
- url:GET|/api/v1/group_categories/:group_category_id
- url:PUT|/api/v1/group_categories/:group_category_id
- url:POST|/api/v1/group_categories/:group_category_id/assign_unassigned_members
- url:GET|/api/v1/group_categories/:group_category_id/export
- url:GET|/api/v1/group_categories/:group_category_id/groups
- url:POST|/api/v1/group_categories/:group_category_id/groups
- url:POST|/api/v1/group_categories/:group_category_id/import
- url:GET|/api/v1/group_categories/:group_category_id/users
- url:POST|/api/v1/groups
- url:DELETE|/api/v1/groups/:group_id
- url:GET|/api/v1/groups/:group_id
- url:PUT|/api/v1/groups/:group_id
- url:GET|/api/v1/groups/:group_id/activity_stream
- url:GET|/api/v1/groups/:group_id/activity_stream/summary
- url:GET|/api/v1/groups/:group_id/assignments/:assignment_id/override
- url:GET|/api/v1/groups/:group_id/collaborations
- url:GET|/api/v1/groups/:group_id/conferences
- url:GET|/api/v1/groups/:group_id/content_exports
- url:POST|/api/v1/groups/:group_id/content_exports
- url:GET|/api/v1/groups/:group_id/content_exports/:id
- url:GET|/api/v1/groups/:group_id/content_licenses
- url:GET|/api/v1/groups/:group_id/content_migrations
- url:POST|/api/v1/groups/:group_id/content_migrations
- url:GET|/api/v1/groups/:group_id/content_migrations/migrators
- url:GET|/api/v1/groups/:group_id/content_migrations/:content_migration_id/migration_issues
- url:GET|/api/v1/groups/:group_id/content_migrations/:content_migration_id/migration_issues/:id
- url:PUT|/api/v1/groups/:group_id/content_migrations/:content_migration_id/migration_issues/:id
- url:GET|/api/v1/groups/:group_id/content_migrations/:id
- url:PUT|/api/v1/groups/:group_id/content_migrations/:id
- url:GET|/api/v1/groups/:group_id/content_migrations/:id/selective_data
- url:GET|/api/v1/groups/:group_id/discussion_topics
- url:POST|/api/v1/groups/:group_id/discussion_topics
- url:PUT|/api/v1/groups/:group_id/discussion_topics/read_all
- url:POST|/api/v1/groups/:group_id/discussion_topics/reorder
- url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id
- url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id
- url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id
- url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/duplicate
- url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries
- url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries
- url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/rating
- url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/read
- url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/read
- url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/replies
- url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/replies
- url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:id
- url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:id
- url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/entry_list
- url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/read
- url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/read
- url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/read_all
- url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/read_all
- url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/subscribed
- url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/subscribed
- url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/summaries
- url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/summaries
- url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/summaries/disable
- url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/summaries/:summary_id/feedback
- url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/view
- url:GET|/api/v1/groups/:group_id/external_feeds
- url:POST|/api/v1/groups/:group_id/external_feeds
- url:DELETE|/api/v1/groups/:group_id/external_feeds/:external_feed_id
- url:GET|/api/v1/groups/:group_id/external_tools
- url:GET|/api/v1/groups/:group_id/files
- url:POST|/api/v1/groups/:group_id/files
- url:GET|/api/v1/groups/:group_id/files/quota
- url:GET|/api/v1/groups/:group_id/files/:id
- url:GET|/api/v1/groups/:group_id/folders
- url:POST|/api/v1/groups/:group_id/folders
- url:GET|/api/v1/groups/:group_id/folders/by_path
- url:GET|/api/v1/groups/:group_id/folders/by_path/*full_path
- url:GET|/api/v1/groups/:group_id/folders/media
- url:GET|/api/v1/groups/:group_id/folders/:id
- url:GET|/api/v1/groups/:group_id/front_page
- url:PUT|/api/v1/groups/:group_id/front_page
- url:POST|/api/v1/groups/:group_id/invite
- url:GET|/api/v1/groups/:group_id/media_attachments
- url:GET|/api/v1/groups/:group_id/media_objects
- url:GET|/api/v1/groups/:group_id/memberships
- url:POST|/api/v1/groups/:group_id/memberships
- url:DELETE|/api/v1/groups/:group_id/memberships/:membership_id
- url:GET|/api/v1/groups/:group_id/memberships/:membership_id
- url:PUT|/api/v1/groups/:group_id/memberships/:membership_id
- url:GET|/api/v1/groups/:group_id/pages
- url:POST|/api/v1/groups/:group_id/pages
- url:DELETE|/api/v1/groups/:group_id/pages/:url_or_id
- url:GET|/api/v1/groups/:group_id/pages/:url_or_id
- url:PUT|/api/v1/groups/:group_id/pages/:url_or_id
- url:GET|/api/v1/groups/:group_id/pages/:url_or_id/revisions
- url:GET|/api/v1/groups/:group_id/pages/:url_or_id/revisions/latest
- url:GET|/api/v1/groups/:group_id/pages/:url_or_id/revisions/:revision_id
- url:POST|/api/v1/groups/:group_id/pages/:url_or_id/revisions/:revision_id
- url:GET|/api/v1/groups/:group_id/permissions
- url:GET|/api/v1/groups/:group_id/potential_collaborators
- url:POST|/api/v1/groups/:group_id/preview_html
- url:GET|/api/v1/groups/:group_id/tabs
- url:DELETE|/api/v1/groups/:group_id/usage_rights
- url:PUT|/api/v1/groups/:group_id/usage_rights
- url:DELETE|/api/v1/groups/:group_id/users
- url:GET|/api/v1/groups/:group_id/users
- url:DELETE|/api/v1/groups/:group_id/users/:user_id
- url:GET|/api/v1/groups/:group_id/users/:user_id
- url:PUT|/api/v1/groups/:group_id/users/:user_id
- url:GET|/api/v1/horizon_accounts
- url:POST|/api/v1/inst_access_tokens
- url:POST|/api/v1/jwts
- url:POST|/api/v1/jwts/refresh
- url:GET|/api/v1/manageable_accounts
- url:GET|/api/v1/manually_created_courses_account
- url:GET|/api/v1/media_attachments
- url:PUT|/api/v1/media_attachments/:attachment_id
- url:GET|/api/v1/media_attachments/:attachment_id/media_tracks
- url:PUT|/api/v1/media_attachments/:attachment_id/media_tracks
- url:GET|/api/v1/media_objects
- url:PUT|/api/v1/media_objects/:media_object_id
- url:GET|/api/v1/media_objects/:media_object_id/media_tracks
- url:PUT|/api/v1/media_objects/:media_object_id/media_tracks
- url:GET|/api/v1/outcomes/:id
- url:PUT|/api/v1/outcomes/:id
- url:GET|/api/v1/permissions/groups
- url:GET|/api/v1/permissions/:context_type/:permission/help
- url:GET|/api/v1/planner/items
- url:GET|/api/v1/planner/overrides
- url:POST|/api/v1/planner/overrides
- url:DELETE|/api/v1/planner/overrides/:id
- url:GET|/api/v1/planner/overrides/:id
- url:PUT|/api/v1/planner/overrides/:id
- url:GET|/api/v1/planner_notes
- url:POST|/api/v1/planner_notes
- url:DELETE|/api/v1/planner_notes/:id
- url:GET|/api/v1/planner_notes/:id
- url:PUT|/api/v1/planner_notes/:id
- url:GET|/api/v1/poll_sessions/closed
- url:GET|/api/v1/poll_sessions/opened
- url:GET|/api/v1/polls
- url:POST|/api/v1/polls
- url:DELETE|/api/v1/polls/:id
- url:GET|/api/v1/polls/:id
- url:PUT|/api/v1/polls/:id
- url:GET|/api/v1/polls/:poll_id/poll_choices
- url:POST|/api/v1/polls/:poll_id/poll_choices
- url:DELETE|/api/v1/polls/:poll_id/poll_choices/:id
- url:GET|/api/v1/polls/:poll_id/poll_choices/:id
- url:PUT|/api/v1/polls/:poll_id/poll_choices/:id
- url:GET|/api/v1/polls/:poll_id/poll_sessions
- url:POST|/api/v1/polls/:poll_id/poll_sessions
- url:DELETE|/api/v1/polls/:poll_id/poll_sessions/:id
- url:GET|/api/v1/polls/:poll_id/poll_sessions/:id
- url:PUT|/api/v1/polls/:poll_id/poll_sessions/:id
- url:GET|/api/v1/polls/:poll_id/poll_sessions/:id/close
- url:GET|/api/v1/polls/:poll_id/poll_sessions/:id/open
- url:POST|/api/v1/polls/:poll_id/poll_sessions/:poll_session_id/poll_submissions
- url:GET|/api/v1/polls/:poll_id/poll_sessions/:poll_session_id/poll_submissions/:id
- url:GET|/api/v1/progress/:id
- url:POST|/api/v1/progress/:id/cancel
- url:GET|/api/v1/question_banks
- url:GET|/api/v1/question_banks/:id
- url:GET|/api/v1/question_banks/:id/questions
- url:GET|/api/v1/quiz_submissions/:quiz_submission_id/questions
- url:POST|/api/v1/quiz_submissions/:quiz_submission_id/questions
- url:PUT|/api/v1/quiz_submissions/:quiz_submission_id/questions/:id/flag
- url:GET|/api/v1/quiz_submissions/:quiz_submission_id/questions/:id/formatted_answer
- url:PUT|/api/v1/quiz_submissions/:quiz_submission_id/questions/:id/unflag
- url:GET|/api/v1/rubrics/upload_template
- url:GET|/api/v1/search/all_courses
- url:GET|/api/v1/search/recipients
- url:GET|/api/v1/sections/:course_section_id/assignments/:assignment_id/override
- url:DELETE|/api/v1/sections/:id
- url:GET|/api/v1/sections/:id
- url:PUT|/api/v1/sections/:id
- url:DELETE|/api/v1/sections/:id/crosslist
- url:POST|/api/v1/sections/:id/crosslist/:new_course_id
- url:GET|/api/v1/sections/:id/users
- url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/anonymous_submissions/:anonymous_id
- url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/anonymous_submissions/:anonymous_id
- url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/peer_reviews
- url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submission_summary
- url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions
- url:POST|/api/v1/sections/:section_id/assignments/:assignment_id/submissions
- url:POST|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/update_grades
- url:DELETE|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- url:POST|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id
- url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id
- url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/document_annotations/read
- url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/document_annotations/read
- url:POST|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/files
- url:DELETE|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/read
- url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/read
- url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/read/:item
- url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/rubric_assessments/read
- url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/rubric_assessments/read
- url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/rubric_comments/read
- url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/rubric_comments/read
- url:GET|/api/v1/sections/:section_id/enrollments
- url:POST|/api/v1/sections/:section_id/enrollments
- url:GET|/api/v1/sections/:section_id/students/submissions
- url:PUT|/api/v1/sections/:section_id/submissions/bulk_mark_read
- url:POST|/api/v1/sections/:section_id/submissions/update_grades
- url:PUT|/api/v1/sections/:section_id/submissions/:user_id/clear_unread
- url:GET|/api/v1/services/kaltura
- url:POST|/api/v1/services/kaltura_session
- url:GET|/api/v1/settings/environment
- url:DELETE|/api/v1/shared_brand_configs/:id
- url:PUT|/api/v1/submissions/:id/what_if_grades
- url:GET|/api/v1/temporary_enrollment_status
- url:GET|/api/v1/users/activity_stream
- url:DELETE|/api/v1/users/mobile_sessions
- url:POST|/api/v1/users/page_views/query
- url:GET|/api/v1/users/page_views/query/:query_id
- url:GET|/api/v1/users/page_views/query/:query_id/results
- url:POST|/api/v1/users/reset_password
- url:DELETE|/api/v1/users/self/activity_stream
- url:GET|/api/v1/users/self/activity_stream
- url:GET|/api/v1/users/self/activity_stream/summary
- url:DELETE|/api/v1/users/self/activity_stream/:id
- url:GET|/api/v1/users/self/bookmarks
- url:POST|/api/v1/users/self/bookmarks
- url:DELETE|/api/v1/users/self/bookmarks/:id
- url:GET|/api/v1/users/self/bookmarks/:id
- url:PUT|/api/v1/users/self/bookmarks/:id
- url:DELETE|/api/v1/users/self/communication_channels/push
- url:PUT|/api/v1/users/self/communication_channels/:communication_channel_id/notification_preference_categories/:category
- url:PUT|/api/v1/users/self/communication_channels/:communication_channel_id/notification_preferences
- url:PUT|/api/v1/users/self/communication_channels/:communication_channel_id/notification_preferences/:notification
- url:PUT|/api/v1/users/self/communication_channels/:type/:address/notification_preferences
- url:PUT|/api/v1/users/self/communication_channels/:type/:address/notification_preferences/:notification
- url:DELETE|/api/v1/users/self/course_nicknames
- url:GET|/api/v1/users/self/course_nicknames
- url:DELETE|/api/v1/users/self/course_nicknames/:course_id
- url:GET|/api/v1/users/self/course_nicknames/:course_id
- url:PUT|/api/v1/users/self/course_nicknames/:course_id
- url:DELETE|/api/v1/users/self/favorites/courses
- url:GET|/api/v1/users/self/favorites/courses
- url:DELETE|/api/v1/users/self/favorites/courses/:id
- url:POST|/api/v1/users/self/favorites/courses/:id
- url:DELETE|/api/v1/users/self/favorites/groups
- url:GET|/api/v1/users/self/favorites/groups
- url:DELETE|/api/v1/users/self/favorites/groups/:id
- url:POST|/api/v1/users/self/favorites/groups/:id
- url:GET|/api/v1/users/self/groups
- url:POST|/api/v1/users/self/pandata_events_token
- url:GET|/api/v1/users/self/todo
- url:GET|/api/v1/users/self/todo_item_count
- url:GET|/api/v1/users/self/upcoming_events
- url:GET|/api/v1/users/:id
- url:PUT|/api/v1/users/:id
- url:GET|/api/v1/users/:id/colors
- url:GET|/api/v1/users/:id/colors/:asset_string
- url:PUT|/api/v1/users/:id/colors/:asset_string
- url:GET|/api/v1/users/:id/dashboard_positions
- url:PUT|/api/v1/users/:id/dashboard_positions
- url:PUT|/api/v1/users/:id/files_ui_version_preference
- url:GET|/api/v1/users/:id/graded_submissions
- url:PUT|/api/v1/users/:id/merge_into/accounts/:destination_account_id/users/:destination_user_id
- url:PUT|/api/v1/users/:id/merge_into/:destination_user_id
- url:DELETE|/api/v1/users/:id/mobile_sessions
- url:DELETE|/api/v1/users/:id/sessions
- url:GET|/api/v1/users/:id/settings
- url:POST|/api/v1/users/:id/split
- url:PUT|/api/v1/users/:id/text_editor_preference
- url:GET|/api/v1/users/:user_id/avatars
- url:GET|/api/v1/users/:user_id/calendar_events
- url:GET|/api/v1/users/:user_id/communication_channels
- url:POST|/api/v1/users/:user_id/communication_channels
- url:GET|/api/v1/users/:user_id/communication_channels/:communication_channel_id/notification_preference_categories
- url:GET|/api/v1/users/:user_id/communication_channels/:communication_channel_id/notification_preferences
- url:GET|/api/v1/users/:user_id/communication_channels/:communication_channel_id/notification_preferences/:notification
- url:DELETE|/api/v1/users/:user_id/communication_channels/:id
- url:DELETE|/api/v1/users/:user_id/communication_channels/:type/:address
- url:GET|/api/v1/users/:user_id/communication_channels/:type/:address/notification_preferences
- url:GET|/api/v1/users/:user_id/communication_channels/:type/:address/notification_preferences/:notification
- url:GET|/api/v1/users/:user_id/content_exports
- url:POST|/api/v1/users/:user_id/content_exports
- url:GET|/api/v1/users/:user_id/content_exports/:id
- url:GET|/api/v1/users/:user_id/content_licenses
- url:GET|/api/v1/users/:user_id/content_migrations
- url:POST|/api/v1/users/:user_id/content_migrations
- url:GET|/api/v1/users/:user_id/content_migrations/migrators
- url:GET|/api/v1/users/:user_id/content_migrations/:content_migration_id/migration_issues
- url:GET|/api/v1/users/:user_id/content_migrations/:content_migration_id/migration_issues/:id
- url:PUT|/api/v1/users/:user_id/content_migrations/:content_migration_id/migration_issues/:id
- url:GET|/api/v1/users/:user_id/content_migrations/:id
- url:PUT|/api/v1/users/:user_id/content_migrations/:id
- url:GET|/api/v1/users/:user_id/content_migrations/:id/selective_data
- url:POST|/api/v1/users/:user_id/content_shares
- url:GET|/api/v1/users/:user_id/content_shares/received
- url:GET|/api/v1/users/:user_id/content_shares/sent
- url:GET|/api/v1/users/:user_id/content_shares/unread_count
- url:DELETE|/api/v1/users/:user_id/content_shares/:id
- url:GET|/api/v1/users/:user_id/content_shares/:id
- url:PUT|/api/v1/users/:user_id/content_shares/:id
- url:POST|/api/v1/users/:user_id/content_shares/:id/add_users
- url:GET|/api/v1/users/:user_id/courses
- url:GET|/api/v1/users/:user_id/courses/:course_id/assignments
- url:DELETE|/api/v1/users/:user_id/custom_data
- url:GET|/api/v1/users/:user_id/custom_data
- url:PUT|/api/v1/users/:user_id/custom_data
- url:POST|/api/v1/users/:user_id/educator_accessibility_course_scan
- url:GET|/api/v1/users/:user_id/educator_accessibility_course_statistics
- url:GET|/api/v1/users/:user_id/educator_accessibility_course_terms
- url:GET|/api/v1/users/:user_id/enrollments
- url:GET|/api/v1/users/:user_id/eportfolios
- url:PUT|/api/v1/users/:user_id/eportfolios
- url:GET|/api/v1/users/:user_id/features
- url:GET|/api/v1/users/:user_id/features/enabled
- url:DELETE|/api/v1/users/:user_id/features/flags/:feature
- url:GET|/api/v1/users/:user_id/features/flags/:feature
- url:PUT|/api/v1/users/:user_id/features/flags/:feature
- url:GET|/api/v1/users/:user_id/files
- url:POST|/api/v1/users/:user_id/files
- url:GET|/api/v1/users/:user_id/files/quota
- url:GET|/api/v1/users/:user_id/files/:id
- url:GET|/api/v1/users/:user_id/folders
- url:POST|/api/v1/users/:user_id/folders
- url:GET|/api/v1/users/:user_id/folders/by_path
- url:GET|/api/v1/users/:user_id/folders/by_path/*full_path
- url:GET|/api/v1/users/:user_id/folders/:id
- url:GET|/api/v1/users/:user_id/history
- url:GET|/api/v1/users/:user_id/logins
- url:DELETE|/api/v1/users/:user_id/logins/:id
- url:GET|/api/v1/users/:user_id/missing_submissions
- url:GET|/api/v1/users/:user_id/observees
- url:POST|/api/v1/users/:user_id/observees
- url:DELETE|/api/v1/users/:user_id/observees/:observee_id
- url:GET|/api/v1/users/:user_id/observees/:observee_id
- url:PUT|/api/v1/users/:user_id/observees/:observee_id
- url:POST|/api/v1/users/:user_id/observer_pairing_codes
- url:GET|/api/v1/users/:user_id/observers
- url:GET|/api/v1/users/:user_id/observers/:observer_id
- url:GET|/api/v1/users/:user_id/page_views
- url:POST|/api/v1/users/:user_id/page_views/query
- url:GET|/api/v1/users/:user_id/page_views/query/:query_id
- url:GET|/api/v1/users/:user_id/page_views/query/:query_id/results
- url:GET|/api/v1/users/:user_id/planner/items
- url:POST|/api/v1/users/:user_id/portfolio_notifications
- url:GET|/api/v1/users/:user_id/profile
- url:GET|/api/v1/users/:user_id/tabs
- url:GET|/api/v1/users/:user_id/temporary_enrollment_status
- url:POST|/api/v1/users/:user_id/tokens
- url:DELETE|/api/v1/users/:user_id/tokens/:id
- url:GET|/api/v1/users/:user_id/tokens/:id
- url:PUT|/api/v1/users/:user_id/tokens/:id
- url:DELETE|/api/v1/users/:user_id/usage_rights
- url:PUT|/api/v1/users/:user_id/usage_rights
- url:GET|/api/v1/users/:user_id/user_generated_tokens
scopes:
- description: Get account
  flows: []
  scope: url:GET|/api/lti/accounts/:account_id
- description: Update Eula Deployment Configuration
  flows: []
  scope: url:PUT|/api/lti/asset_processor_eulas/:context_external_tool_id/deployment
- description: Delete Eula Acceptances for deployment
  flows: []
  scope: url:DELETE|/api/lti/asset_processor_eulas/:context_external_tool_id/user
- description: Create an Eula Acceptance
  flows: []
  scope: url:POST|/api/lti/asset_processor_eulas/:context_external_tool_id/user
- description: Create an Asset Report
  flows: []
  scope: url:POST|/api/lti/asset_processors/:asset_processor_id/reports
- description: Get a single assignment (lti)
  flows: []
  scope: url:GET|/api/lti/assignments/:assignment_id
- description: Show an Originality Report
  flows: []
  scope: url:GET|/api/lti/assignments/:assignment_id/files/:file_id/originality_report
- description: Edit an Originality Report
  flows: []
  scope: url:PUT|/api/lti/assignments/:assignment_id/files/:file_id/originality_report
- description: Get a single submission
  flows: []
  scope: url:GET|/api/lti/assignments/:assignment_id/submissions/:submission_id
- description: Get the history of a single submission
  flows: []
  scope: url:GET|/api/lti/assignments/:assignment_id/submissions/:submission_id/history
- description: Create an Originality Report
  flows: []
  scope: url:POST|/api/lti/assignments/:assignment_id/submissions/:submission_id/originality_report
- description: Show an Originality Report
  flows: []
  scope: url:GET|/api/lti/assignments/:assignment_id/submissions/:submission_id/originality_report/:id
- description: Edit an Originality Report
  flows: []
  scope: url:PUT|/api/lti/assignments/:assignment_id/submissions/:submission_id/originality_report/:id
- description: List line Items
  flows: []
  scope: url:GET|/api/lti/courses/:course_id/line_items
- description: Create a Line Item
  flows: []
  scope: url:POST|/api/lti/courses/:course_id/line_items
- description: Delete a Line Item
  flows: []
  scope: url:DELETE|/api/lti/courses/:course_id/line_items/:id
- description: Show a Line Item
  flows: []
  scope: url:GET|/api/lti/courses/:course_id/line_items/:id
- description: Update a Line Item
  flows: []
  scope: url:PUT|/api/lti/courses/:course_id/line_items/:id
- description: Show a collection of Results
  flows: []
  scope: url:GET|/api/lti/courses/:course_id/line_items/:line_item_id/results
- description: Show a Result
  flows: []
  scope: url:GET|/api/lti/courses/:course_id/line_items/:line_item_id/results/:id
- description: Create a Score
  flows: []
  scope: url:POST|/api/lti/courses/:course_id/line_items/:line_item_id/scores
- description: List Course Memberships
  flows: []
  scope: url:GET|/api/lti/courses/:course_id/names_and_roles
- description: Query progress
  flows: []
  scope: url:GET|/api/lti/courses/:course_id/progress/:id
- description: Update Public JWK
  flows: []
  scope: url:PUT|/api/lti/developer_key/update_public_jwk
- description: List Group Memberships
  flows: []
  scope: url:GET|/api/lti/groups/:group_id/names_and_roles
- description: Get all users in a group (lti)
  flows: []
  scope: url:GET|/api/lti/groups/:group_id/users
- description: Show notice handlers
  flows: []
  scope: url:GET|/api/lti/notice-handlers/:context_external_tool_id
- description: Set notice handler
  flows: []
  scope: url:PUT|/api/lti/notice-handlers/:context_external_tool_id
- description: List all Webhook Subscription for a tool proxy
  flows: []
  scope: url:GET|/api/lti/subscriptions
- description: Create a Webhook Subscription
  flows: []
  scope: url:POST|/api/lti/subscriptions
- description: Delete a Webhook Subscription
  flows: []
  scope: url:DELETE|/api/lti/subscriptions/:id
- description: Show a single Webhook Subscription
  flows: []
  scope: url:GET|/api/lti/subscriptions/:id
- description: Update a Webhook Subscription
  flows: []
  scope: url:PUT|/api/lti/subscriptions/:id
- description: Get a single user (lti)
  flows: []
  scope: url:GET|/api/lti/users/:id
- description: Download UUID Mapping for this Sandbox
  flows: []
  scope: url:GET|/api/lti/uuid_map
- description: Set Course-Level Accommodations
  flows: []
  scope: url:POST|/api/quiz/v1/courses/:course_id/accommodations
- description: List new quizzes
  flows: []
  scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes
- description: Create a new quiz
  flows: []
  scope: url:POST|/api/quiz/v1/courses/:course_id/quizzes
- description: Delete a new quiz
  flows: []
  scope: url:DELETE|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id
- description: Get a new quiz
  flows: []
  scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id
- description: Update a single quiz
  flows: []
  scope: url:PATCH|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id
- description: Set Quiz-Level Accommodations
  flows: []
  scope: url:POST|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/accommodations
- description: List quiz items
  flows: []
  scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items
- description: Create a quiz item
  flows: []
  scope: url:POST|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items
- description: Get items media_upload_url
  flows: []
  scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/media_upload_url
- description: Delete a quiz item
  flows: []
  scope: url:DELETE|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/:item_id
- description: Get a quiz item
  flows: []
  scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/:item_id
- description: Update a quiz item
  flows: []
  scope: url:PATCH|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/:item_id
- description: Create a quiz report
  flows: []
  scope: url:POST|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/reports
- description: Retrieve assignments enabled for grade export to SIS
  flows: []
  scope: url:GET|/api/sis/accounts/:account_id/assignments
- description: Retrieve assignments enabled for grade export to SIS
  flows: []
  scope: url:GET|/api/sis/courses/:course_id/assignments
- description: Disable assignments currently enabled for grade export to SIS
  flows: []
  scope: url:PUT|/api/sis/courses/:course_id/disable_post_to_sis
- description: List available account calendars
  flows: []
  scope: url:GET|/api/v1/account_calendars
- description: Get a single account calendar
  flows: []
  scope: url:GET|/api/v1/account_calendars/:account_id
- description: Update a calendar
  flows: []
  scope: url:PUT|/api/v1/account_calendars/:account_id
- description: List accounts
  flows: []
  scope: url:GET|/api/v1/accounts
- description: Search account domains
  flows: []
  scope: url:GET|/api/v1/accounts/search
- description: List all account calendars
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/account_calendars
- description: Update several calendars
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/account_calendars
- description: Index of active global notification for the user
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/account_notifications
- description: Create a global notification
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/account_notifications
- description: Close notification for user. Destroy notification for admin
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/account_notifications/:id
- description: Show a global notification
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/account_notifications/:id
- description: Update a global notification
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/account_notifications/:id
- description: List account admins
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/admins
- description: Make an account admin
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/admins
- description: List my admin roles
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/admins/self
- description: Remove account admin
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/admins/:user_id
- description: Get department-level participation data
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/completed/activity
- description: Get department-level grade data
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/completed/grades
- description: Get department-level statistics
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/completed/statistics
- description: Get department-level statistics, broken down by subaccount
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/completed/statistics_by_subaccount
- description: Get department-level participation data
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/current/activity
- description: Get department-level grade data
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/current/grades
- description: Get department-level statistics
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/current/statistics
- description: Get department-level statistics, broken down by subaccount
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/current/statistics_by_subaccount
- description: Get department-level participation data
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/activity
- description: Get department-level grade data
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/grades
- description: Get department-level statistics
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/statistics
- description: Get department-level statistics, broken down by subaccount
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/statistics_by_subaccount
- description: Show an LTI Registration (via the client_id)
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/app_by_client_id/:client_id
- description: List LTI Registrations in an account
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/apps
- description: Create an LTI Registration
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/apps
- description: Get LTI Registration by Unified Tool ID
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/apps/by_utid/:utid
- description: Check LTI Registration Install Status
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/apps/install_status/:client_id
- description: Delete an LTI Registration
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/apps/:id
- description: Show an LTI Registration
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/apps/:id
- description: Update an LTI Registration
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/apps/:id
- description: Remove an Inherited LTI Registration
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/apps/:id/bind
- description: Bind an LTI Registration to a Root Account
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/apps/:id/bind
- description: Get LTI Registration History
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/apps/:id/history
- description: Install an LTI Registration from a Template
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/apps/:id/install_from_template
- description: Get Latest LTI Registration Update Request
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/apps/:id/latest_update_request
- description: Get LTI Registration Overlay History
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/apps/:id/overlay_history
- description: Reset an LTI Registration to Defaults
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/apps/:id/reset
- description: Get LTI Registration Update Request
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/apps/:id/update_requests/:update_request_id
- description: Apply LTI Registration Update Requst
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/apps/:id/update_requests/:update_request_id/apply
- description: Search for Accounts and Courses
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/apps/:registration_id/deployments/:deployment_id/context_search
- description: List authentication providers
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/authentication_providers
- description: Add authentication provider
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/authentication_providers
- description: Force password reset
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/authentication_providers/force_password_reset
- description: Delete authentication provider
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/authentication_providers/:id
- description: Get authentication provider
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/authentication_providers/:id
- description: Update authentication provider
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/authentication_providers/:id
- description: Restore a deleted authentication provider
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/authentication_providers/:id/restore
- description: List blackout dates
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/blackout_dates
- description: Create Blackout Date
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/blackout_dates
- description: New Blackout Date
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/blackout_dates/new
- description: Delete Blackout Date
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/blackout_dates/:id
- description: Get a single blackout date
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/blackout_dates/:id
- description: Update Blackout Date
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/blackout_dates/:id
- description: Get the brand config variables for a sub-account or course
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/brand_variables
- description: Enroll multiple users to one or more courses
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/bulk_enrollment
- description: List content migrations
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/content_migrations
- description: Create a content migration
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/content_migrations
- description: List Migration Systems
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/content_migrations/migrators
- description: List migration issues
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/content_migrations/:content_migration_id/migration_issues
- description: Get a migration issue
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/content_migrations/:content_migration_id/migration_issues/:id
- description: Update a migration issue
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/content_migrations/:content_migration_id/migration_issues/:id
- description: Get a content migration
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/content_migrations/:id
- description: Update a content migration
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/content_migrations/:id
- description: List items for selective import
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/content_migrations/:id/selective_data
- description: List active courses in an account
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/courses
- description: Create a new course
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/courses
- description: Update courses
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/courses
- description: Get a single course
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/courses/:id
- description: Get current settings for account or course
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/csp_settings
- description: Enable, disable, or clear explicit CSP setting
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/csp_settings
- description: Remove a domain from account
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/csp_settings/domains
- description: Add an allowed domain to account
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/csp_settings/domains
- description: Add multiple allowed domains to an account
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/csp_settings/domains/batch_create
- description: Lock or unlock current CSP settings for sub-accounts and courses
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/csp_settings/lock
- description: List Developer Keys
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/developer_keys
- description: Create a Developer Key
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/developer_keys
- description: Create a Developer Key Account Binding
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/developer_keys/:developer_key_id/developer_key_account_bindings
- description: Enrollment by ID
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/enrollments/:id
- description: List external tools
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/external_tools
- description: Create an external tool
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/external_tools
- description: Unmark tool as RCE Favorite
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/external_tools/rce_favorites/:id
- description: Mark tool as RCE Favorite
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/external_tools/rce_favorites/:id
- description: Get a sessionless launch url for an external tool.
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/external_tools/sessionless_launch
- description: Remove tool from Top Navigation Favorites
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/external_tools/top_nav_favorites/:id
- description: Add tool to Top Navigation Favorites
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/external_tools/top_nav_favorites/:id
- description: Delete an external tool
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/external_tools/:external_tool_id
- description: Get a single external tool
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/external_tools/:external_tool_id
- description: Edit an external tool
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/external_tools/:external_tool_id
- description: List features
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/features
- description: List enabled features
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/features/enabled
- description: Remove feature flag
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/features/flags/:feature
- description: Get feature flag
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/features/flags/:feature
- description: Set feature flag
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/features/flags/:feature
- description: Create folder
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/folders
- description: List grading period sets
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/grading_period_sets
- description: Create a grading period set
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/grading_period_sets
- description: Delete a grading period set
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/grading_period_sets/:id
- description: Update a grading period set
  flows: []
  scope: url:PATCH|/api/v1/accounts/:account_id/grading_period_sets/:id
- description: List grading periods
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/grading_periods
- description: Delete a grading period
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/grading_periods/:id
- description: List the grading standards available in a context.
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/grading_standards
- description: Create a new grading standard
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/grading_standards
- description: Delete a grading standard
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/grading_standards/:grading_standard_id
- description: Get a single grading standard in a context.
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/grading_standards/:grading_standard_id
- description: Update a grading standard
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/grading_standards/:grading_standard_id
- description: List group categories for a context
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/group_categories
- description: Create a Group Category
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/group_categories
- description: List the groups available in a context.
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/groups
- description: Get help links
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/help_links
- description: List user logins
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/logins
- description: Create a user login
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/logins
- description: Edit a user login
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/logins/:id
- description: List LTI Launch Definitions
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_apps/launch_definitions
- description: Show an LTI Registration (via the client_id)
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registration_by_client_id/:client_id
- description: List LTI Registrations in an account
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations
- description: Create an LTI Registration
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/lti_registrations
- description: Get LTI Registration by Unified Tool ID
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/by_utid/:utid
- description: Check LTI Registration Install Status
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/install_status/:client_id
- description: Delete an LTI Registration
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/lti_registrations/:id
- description: Show an LTI Registration
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/:id
- description: Update an LTI Registration
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/lti_registrations/:id
- description: Remove an Inherited LTI Registration
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/lti_registrations/:id/bind
- description: Bind an LTI Registration to a Root Account
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/lti_registrations/:id/bind
- description: Get LTI Registration History
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/:id/history
- description: Install an LTI Registration from a Template
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/lti_registrations/:id/install_from_template
- description: Get Latest LTI Registration Update Request
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/:id/latest_update_request
- description: Get LTI Registration Overlay History
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/:id/overlay_history
- description: Reset an LTI Registration to Defaults
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/lti_registrations/:id/reset
- description: Get LTI Registration Update Request
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/:id/update_requests/:update_request_id
- description: Apply LTI Registration Update Requst
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/lti_registrations/:id/update_requests/:update_request_id/apply
- description: List All Context Controls
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls
- description: Bulk Create LTI Context Controls
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls/bulk
- description: Delete a Context Control
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls/:id
- description: Show LTI Context Control
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls/:id
- description: Modify a Context Control
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/lti_registrations/:registration_id/controls/:id
- description: Search for Accounts and Courses
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/lti_registrations/:registration_id/deployments/:deployment_id/context_search
- description: Get all outcome links for context
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/outcome_group_links
- description: Get all outcome groups for context
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/outcome_groups
- description: Delete an outcome group
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/outcome_groups/:id
- description: Show an outcome group
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/outcome_groups/:id
- description: Update an outcome group
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/outcome_groups/:id
- description: Import an outcome group
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/outcome_groups/:id/import
- description: List linked outcomes
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/outcome_groups/:id/outcomes
- description: Create/link an outcome
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/outcome_groups/:id/outcomes
- description: Unlink an outcome
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/outcome_groups/:id/outcomes/:outcome_id
- description: Create/link an outcome
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/outcome_groups/:id/outcomes/:outcome_id
- description: List subgroups
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/outcome_groups/:id/subgroups
- description: Create a subgroup
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/outcome_groups/:id/subgroups
- description: Import Outcomes
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/outcome_imports
- description: Get Outcome import status
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/outcome_imports/:id
- description: Get IDs of outcome groups created after successful import
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/outcome_imports/:id/created_group_ids
- description: Get proficiency ratings
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/outcome_proficiency
- description: Create/update proficiency ratings
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/outcome_proficiency
- description: Permissions
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/permissions
- description: List Available Reports
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/reports
- description: Index of Reports
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/reports/:report
- description: Start a Report
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/reports/:report
- description: Delete a Report
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/reports/:report/:id
- description: Status of a Report
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/reports/:report/:id
- description: Abort a Report
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/reports/:report/:id/abort
- description: List roles
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/roles
- description: Create a new role
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/roles
- description: List assignable permissions
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/roles/permissions
- description: Deactivate a role
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/roles/:id
- description: Get a single role
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/roles/:id
- description: Update a role
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/roles/:id
- description: Activate a role
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/roles/:id/activate
- description: Redirect to root outcome group for context
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/root_outcome_group
- description: List rubrics
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/rubrics
- description: Creates a rubric using a CSV file
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/rubrics/upload
- description: Get the status of a rubric import
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/rubrics/upload/:id
- description: Get a single rubric
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/rubrics/:id
- description: Get the courses and assignments for a rubric
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/rubrics/:id/used_locations
- description: List scopes
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/scopes
- description: '[DEPRECATED] Self register a user'
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/self_registration
- description: Settings
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/settings
- description: Share a BrandConfig (Theme)
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/shared_brand_configs
- description: Update a shared theme
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/shared_brand_configs/:id
- description: Get SIS import error list
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/sis_import_errors
- description: Get SIS import list
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/sis_imports
- description: Import SIS data
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/sis_imports
- description: Abort all pending SIS imports
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/sis_imports/abort_all_pending
- description: Get the current importing SIS import
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/sis_imports/importing
- description: Get SIS import status
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/sis_imports/:id
- description: Abort SIS import
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/sis_imports/:id/abort
- description: Get SIS import error list
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/sis_imports/:id/errors
- description: Restore workflow_states of SIS imported items
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/sis_imports/:id/restore_states
- description: Show account auth settings
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/sso_settings
- description: Update account auth settings
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/sso_settings
- description: Get the sub-accounts of an account
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/sub_accounts
- description: Create a new sub-account
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/sub_accounts
- description: Delete a sub-account
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/sub_accounts/:id
- description: List available tabs for a course or group
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/tabs
- description: List temporary enrollment pairings
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/temporary_enrollment_pairings
- description: Create Temporary Enrollment Pairing
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/temporary_enrollment_pairings
- description: New TemporaryEnrollmentPairing
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/temporary_enrollment_pairings/new
- description: Delete Temporary Enrollment Pairing
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/temporary_enrollment_pairings/:id
- description: Get a single temporary enrollment pairing
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/temporary_enrollment_pairings/:id
- description: List enrollment terms
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/terms
- description: Create enrollment term
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/terms
- description: Delete enrollment term
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/terms/:id
- description: Retrieve enrollment term
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/terms/:id
- description: Update enrollment term
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/terms/:id
- description: Get the Terms of Service
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/terms_of_service
- description: Delete multiple users from the root account
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/users
- description: List users in account
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/users
- description: Create a user
  flows: []
  scope: url:POST|/api/v1/accounts/:account_id/users
- description: Update multiple users
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/users/bulk_update
- description: Delete a user from the root account
  flows: []
  scope: url:DELETE|/api/v1/accounts/:account_id/users/:user_id
- description: Restore a deleted user from a root account
  flows: []
  scope: url:PUT|/api/v1/accounts/:account_id/users/:user_id/restore
- description: Count of all visible account calendars
  flows: []
  scope: url:GET|/api/v1/accounts/:account_id/visible_calendars_count
- description: Create LTI Context Control
  flows: []
  scope: url:POST|/api/v1/accounts/:current_account_id/lti_registrations/:registration_id/controls
- description: Get a single account
  flows: []
  scope: url:GET|/api/v1/accounts/:id
- description: Update an account
  flows: []
  scope: url:PUT|/api/v1/accounts/:id
- description: List announcements
  flows: []
  scope: url:GET|/api/v1/announcements
- description: List appointment groups
  flows: []
  scope: url:GET|/api/v1/appointment_groups
- description: Create an appointment group
  flows: []
  scope: url:POST|/api/v1/appointment_groups
- description: Get next appointment
  flows: []
  scope: url:GET|/api/v1/appointment_groups/next_appointment
- description: Delete an appointment group
  flows: []
  scope: url:DELETE|/api/v1/appointment_groups/:id
- description: Get a single appointment group
  flows: []
  scope: url:GET|/api/v1/appointment_groups/:id
- description: Update an appointment group
  flows: []
  scope: url:PUT|/api/v1/appointment_groups/:id
- description: List student group participants
  flows: []
  scope: url:GET|/api/v1/appointment_groups/:id/groups
- description: List user participants
  flows: []
  scope: url:GET|/api/v1/appointment_groups/:id/users
- description: Query by account.
  flows: []
  scope: url:GET|/api/v1/audit/authentication/accounts/:account_id
- description: Query by login.
  flows: []
  scope: url:GET|/api/v1/audit/authentication/logins/:login_id
- description: Query by user.
  flows: []
  scope: url:GET|/api/v1/audit/authentication/users/:user_id
- description: Query by account.
  flows: []
  scope: url:GET|/api/v1/audit/course/accounts/:account_id
- description: Query by course.
  flows: []
  scope: url:GET|/api/v1/audit/course/courses/:course_id
- description: Advanced query
  flows: []
  scope: url:GET|/api/v1/audit/grade_change
- description: Query by assignment
  flows: []
  scope: url:GET|/api/v1/audit/grade_change/assignments/:assignment_id
- description: Query by course
  flows: []
  scope: url:GET|/api/v1/audit/grade_change/courses/:course_id
- description: Query by grader
  flows: []
  scope: url:GET|/api/v1/audit/grade_change/graders/:grader_id
- description: Query by student
  flows: []
  scope: url:GET|/api/v1/audit/grade_change/students/:student_id
- description: Get the brand config variables that should be used for this domain
  flows: []
  scope: url:GET|/api/v1/brand_variables
- description: List calendar events
  flows: []
  scope: url:GET|/api/v1/calendar_events
- description: Create a calendar event
  flows: []
  scope: url:POST|/api/v1/calendar_events
- description: Save enabled account calendars
  flows: []
  scope: url:POST|/api/v1/calendar_events/save_enabled_account_calendars
- description: Delete a calendar event
  flows: []
  scope: url:DELETE|/api/v1/calendar_events/:id
- description: Get a single calendar event or assignment
  flows: []
  scope: url:GET|/api/v1/calendar_events/:id
- description: Update a calendar event
  flows: []
  scope: url:PUT|/api/v1/calendar_events/:id
- description: Reserve a time slot
  flows: []
  scope: url:POST|/api/v1/calendar_events/:id/reservations
- description: Reserve a time slot
  flows: []
  scope: url:POST|/api/v1/calendar_events/:id/reservations/:participant_id
- description: Check if Canvas Career is enabled
  flows: []
  scope: url:GET|/api/v1/career/enabled
- description: Get current and available experiences
  flows: []
  scope: url:GET|/api/v1/career/experience_summary
- description: Switch experience
  flows: []
  scope: url:POST|/api/v1/career/switch_experience
- description: Switch role
  flows: []
  scope: url:POST|/api/v1/career/switch_role
- description: Get career user context
  flows: []
  scope: url:GET|/api/v1/career/user_context
- description: List members of a collaboration.
  flows: []
  scope: url:GET|/api/v1/collaborations/:id/members
- description: List of CommMessages for a user
  flows: []
  scope: url:GET|/api/v1/comm_messages
- description: List conferences for the current user
  flows: []
  scope: url:GET|/api/v1/conferences
- description: List conversations
  flows: []
  scope: url:GET|/api/v1/conversations
- description: Create a conversation
  flows: []
  scope: url:POST|/api/v1/conversations
- description: Batch update conversations
  flows: []
  scope: url:PUT|/api/v1/conversations
- description: Get running batches
  flows: []
  scope: url:GET|/api/v1/conversations/batches
- description: Find recipients
  flows: []
  scope: url:GET|/api/v1/conversations/find_recipients
- description: Mark all as read
  flows: []
  scope: url:POST|/api/v1/conversations/mark_all_as_read
- description: Unread count
  flows: []
  scope: url:GET|/api/v1/conversations/unread_count
- description: Delete a conversation
  flows: []
  scope: url:DELETE|/api/v1/conversations/:id
- description: Get a single conversation
  flows: []
  scope: url:GET|/api/v1/conversations/:id
- description: Edit a conversation
  flows: []
  scope: url:PUT|/api/v1/conversations/:id
- description: Add a message
  flows: []
  scope: url:POST|/api/v1/conversations/:id/add_message
- description: Add recipients
  flows: []
  scope: url:POST|/api/v1/conversations/:id/add_recipients
- description: Delete a message
  flows: []
  scope: url:POST|/api/v1/conversations/:id/remove_messages
- description: List accounts for course admins
  flows: []
  scope: url:GET|/api/v1/course_accounts
- description: Get accounts that users can create courses in
  flows: []
  scope: url:GET|/api/v1/course_creation_accounts
- description: List your courses
  flows: []
  scope: url:GET|/api/v1/courses
- description: Course activity stream
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/activity_stream
- description: Course activity stream summary
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/activity_stream/summary
- description: List AI experiences
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/ai_experiences
- description: Create an AI experience
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/ai_experiences
- description: Show new AI experience form
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/ai_experiences/new
- description: Get active conversation
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations
- description: Create AI conversation
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations
- description: Delete AI conversation
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id
- description: Show conversation
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id
- description: Get conversation evaluation
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/evaluation
- description: Generate conversation evaluation
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/evaluation
- description: Post message to conversation
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/messages
- description: Create feedback on a conversation message
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/messages/:message_id/feedback
- description: Delete feedback on a conversation message
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/ai_experiences/:ai_experience_id/conversations/:id/messages/:message_id/feedback/:feedback_id
- description: Delete an AI experience
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/ai_experiences/:id
- description: Show an AI experience
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/ai_experiences/:id
- description: Update an AI experience
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/ai_experiences/:id
- description: List student AI conversations
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/ai_experiences/:id/ai_conversations
- description: Show student AI conversation
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/ai_experiences/:id/ai_conversations/:conversation_id
- description: Show edit AI experience form
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/ai_experiences/:id/edit
- description: Get course-level participation data
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/analytics/activity
- description: Get course-level assignment data
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/analytics/assignments
- description: Get course-level student summary data
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/analytics/student_summaries
- description: Get user-in-a-course-level participation data
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/analytics/users/:student_id/activity
- description: Get user-in-a-course-level assignment data
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/analytics/users/:student_id/assignments
- description: Get user-in-a-course-level messaging data
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/analytics/users/:student_id/communication
- description: Set outcome ordering for LMGB
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assign_outcome_order
- description: List assignment groups
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignment_groups
- description: Create an Assignment Group
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignment_groups
- description: Destroy an Assignment Group
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/assignment_groups/:assignment_group_id
- description: Get an Assignment Group
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignment_groups/:assignment_group_id
- description: Edit an Assignment Group
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignment_groups/:assignment_group_id
- description: List assignments
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignment_groups/:assignment_group_id/assignments
- description: List assignments
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments
- description: Create an assignment
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments
- description: Bulk update assignment dates
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/bulk_update
- description: List multiple assignments gradeable students
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/gradeable_students
- description: Batch retrieve overrides in a course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/overrides
- description: Batch create overrides in a course
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/overrides
- description: Batch update overrides in a course
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/overrides
- description: Allocate Peer Review
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/allocate
- description: Show provisional grade status for a student
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/anonymous_provisional_grades/status
- description: Get a single submission by anonymous id
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/anonymous_submissions/:anonymous_id
- description: Grade or comment on a submission by anonymous id
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/anonymous_submissions/:anonymous_id
- description: Get a learning object's date information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/date_details
- description: Update a learning object's date information
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/date_details
- description: Duplicate assignment
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/duplicate
- description: Set extensions for student assignment submissions
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/extensions
- description: List gradeable students
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/gradeable_students
- description: List students selected for moderation
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/moderated_students
- description: Select students for moderation
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/moderated_students
- description: List assignment overrides
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/overrides
- description: Create an assignment override
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/overrides
- description: Delete an assignment override
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id
- description: Get a single assignment override
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id
- description: Update an assignment override
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id
- description: Get all Peer Reviews
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/peer_reviews
- description: Bulk select provisional grades
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/bulk_select
- description: Publish provisional grades for an assignment
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/publish
- description: Publish provisional grades for an assignment (asynchronous)
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/publish_async
- description: Show provisional grade status for a student
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/status
- description: Select provisional grade
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/:provisional_grade_id/select
- description: Submission Summary
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submission_summary
- description: List assignment submissions
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions
- description: Submit an assignment
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions
- description: Grade or comment on multiple submissions
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/update_grades
- description: Delete Peer Review
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- description: Get all Peer Reviews
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- description: Create Peer Review
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- description: Get a single submission
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id
- description: Grade or comment on a submission
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id
- description: Send annotation notification
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/annotation_notification
- description: Upload a file
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/comments/files
- description: Delete a submission comment
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/comments/:id
- description: Edit a submission comment
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/comments/:id
- description: Get document annotations read state
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/document_annotations/read
- description: Mark document annotations as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/document_annotations/read
- description: Upload a file
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/files
- description: Mark submission as unread
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/read
- description: Mark submission as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/read
- description: Mark submission item as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/read/:item
- description: Get rubric assessments read state
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/rubric_assessments/read
- description: Mark rubric assessments as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/rubric_assessments/read
- description: Get rubric assessments read state
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/rubric_comments/read
- description: Mark rubric assessments as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id/rubric_comments/read
- description: List group members for a student on an assignment
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:assignment_id/users/:user_id/group_members
- description: Delete an assignment
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/assignments/:id
- description: Get a single assignment
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/assignments/:id
- description: Edit an assignment
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/assignments/:id
- description: List blackout dates
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blackout_dates
- description: Create Blackout Date
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/blackout_dates
- description: Update a list of Blackout Dates
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/blackout_dates
- description: New Blackout Date
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blackout_dates/new
- description: Delete Blackout Date
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/blackout_dates/:id
- description: Get a single blackout date
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blackout_dates/:id
- description: Update Blackout Date
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/blackout_dates/:id
- description: List block templates
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/block_editor_templates
- description: List blueprint subscriptions
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_subscriptions
- description: List blueprint imports
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_subscriptions/:subscription_id/migrations
- description: Show a blueprint import
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_subscriptions/:subscription_id/migrations/:id
- description: Get import details
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_subscriptions/:subscription_id/migrations/:id/details
- description: Get blueprint information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id
- description: Get associated course information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/associated_courses
- description: List blueprint migrations
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/migrations
- description: Begin a migration to push to associated courses
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/blueprint_templates/:template_id/migrations
- description: Show a blueprint migration
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/migrations/:id
- description: Get migration details
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/migrations/:id/details
- description: Set or remove restrictions on a blueprint course object
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/blueprint_templates/:template_id/restrict_item
- description: Get unsynced changes
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/blueprint_templates/:template_id/unsynced_changes
- description: Update associated courses
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/blueprint_templates/:template_id/update_associations
- description: Get the brand config variables for a sub-account or course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/brand_variables
- description: Get bulk user progress
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/bulk_user_progress
- description: Bulk fetch user tags for multiple users in a course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/bulk_user_tags
- description: Get course timetable
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/calendar_events/timetable
- description: Set a course timetable
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/calendar_events/timetable
- description: Create or update events directly for a course timetable
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/calendar_events/timetable_events
- description: List collaborations
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/collaborations
- description: List conferences
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/conferences
- description: List content exports
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_exports
- description: Export content
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/content_exports
- description: Show content export
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_exports/:id
- description: List licenses
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_licenses
- description: List content migrations
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_migrations
- description: Create a content migration
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/content_migrations
- description: List Migration Systems
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_migrations/migrators
- description: List migration issues
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_migrations/:content_migration_id/migration_issues
- description: Get a migration issue
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_migrations/:content_migration_id/migration_issues/:id
- description: Update a migration issue
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/content_migrations/:content_migration_id/migration_issues/:id
- description: Get a content migration
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_migrations/:id
- description: Update a content migration
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/content_migrations/:id
- description: Get asset id mapping
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_migrations/:id/asset_id_mapping
- description: List items for selective import
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_migrations/:id/selective_data
- description: Search for content share users
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/content_share_users
- description: Copy course content
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/course_copy
- description: Get course copy status
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/course_copy/:id
- description: Create a Course pace
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/course_pacing
- description: Delete a Course pace
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/course_pacing/:id
- description: Show a Course pace
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/course_pacing/:id
- description: Update a Course pace
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/course_pacing/:id
- description: Get current settings for account or course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/csp_settings
- description: Enable, disable, or clear explicit CSP setting
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/csp_settings
- description: Bulk update column data
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/custom_gradebook_column_data
- description: List custom gradebook columns
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/custom_gradebook_columns
- description: Create a custom gradebook column
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/custom_gradebook_columns
- description: Reorder custom columns
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/custom_gradebook_columns/reorder
- description: Delete a custom gradebook column
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/custom_gradebook_columns/:id
- description: Update a custom gradebook column
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/custom_gradebook_columns/:id
- description: List entries for a column
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/custom_gradebook_columns/:id/data
- description: Update column data
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/custom_gradebook_columns/:id/data/:user_id
- description: List discussion topics
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/discussion_topics
- description: Create a new discussion topic
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/discussion_topics
- description: Mark all topic as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/discussion_topics/read_all
- description: Reorder pinned topics
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/discussion_topics/reorder
- description: Get a learning object's date information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/discussion_topics/:discussion_topic_id/date_details
- description: Update a learning object's date information
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/discussion_topics/:discussion_topic_id/date_details
- description: Delete a topic
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id
- description: Get a single topic
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id
- description: Update a topic
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id
- description: Duplicate discussion topic
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/duplicate
- description: List topic entries
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries
- description: Post an entry
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries
- description: Rate entry
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/rating
- description: Mark entry as unread
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/read
- description: Mark entry as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/read
- description: List entry replies
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/replies
- description: Post a reply
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:entry_id/replies
- description: Delete an entry
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:id
- description: Update an entry
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/entries/:id
- description: List entries
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/entry_list
- description: Mark topic as unread
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/read
- description: Mark topic as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/read
- description: Mark all entries as unread
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/read_all
- description: Mark all entries as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/read_all
- description: Unsubscribe from a topic
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/discussion_topics/:topic_id/subscribed
- description: Subscribe to a topic
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/subscribed
- description: Find Last Summary
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/summaries
- description: Find or Create Summary
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/summaries
- description: Disable summary
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/discussion_topics/:topic_id/summaries/disable
- description: Summary Feedback
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/discussion_topics/:topic_id/summaries/:summary_id/feedback
- description: Get the full topic
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/discussion_topics/:topic_id/view
- description: Get effective due dates
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/effective_due_dates
- description: Enqueue a delayed Outcome Rollup Calculation Job
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/enqueue_outcome_rollup_calculation
- description: List enrollments
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/enrollments
- description: Enroll a user
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/enrollments
- description: Conclude, deactivate, or delete an enrollment
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/enrollments/:id
- description: Accept Course Invitation
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/enrollments/:id/accept
- description: Re-activate an enrollment
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/enrollments/:id/reactivate
- description: Reject Course Invitation
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/enrollments/:id/reject
- description: Create ePub Export
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/epub_exports
- description: Show ePub export
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/epub_exports/:id
- description: List external feeds
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/external_feeds
- description: Create an external feed
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/external_feeds
- description: Delete an external feed
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/external_feeds/:external_feed_id
- description: List external tools
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/external_tools
- description: Create an external tool
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/external_tools
- description: Get a sessionless launch url for an external tool.
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/external_tools/sessionless_launch
- description: Get visible course navigation tools for a single course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/external_tools/visible_course_nav_tools
- description: Delete an external tool
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/external_tools/:external_tool_id
- description: Get a single external tool
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/external_tools/:external_tool_id
- description: Edit an external tool
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/external_tools/:external_tool_id
- description: List features
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/features
- description: List enabled features
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/features/enabled
- description: Remove feature flag
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/features/flags/:feature
- description: Get feature flag
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/features/flags/:feature
- description: Set feature flag
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/features/flags/:feature
- description: List files
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/files
- description: Upload a file
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/files
- description: Translate file reference
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/files/file_ref/:migration_id
- description: Get quota information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/files/quota
- description: Get a learning object's date information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/files/:attachment_id/date_details
- description: Update a learning object's date information
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/files/:attachment_id/date_details
- description: Get file
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/files/:id
- description: List all folders
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/folders
- description: Create folder
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/folders
- description: Resolve path
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/folders/by_path
- description: Resolve path
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/folders/by_path/*full_path
- description: Get uploaded media folder for user
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/folders/media
- description: Get folder
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/folders/:id
- description: Show front page
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/front_page
- description: Update/create front page
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/front_page
- description: Days in gradebook history for this course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/gradebook_history/days
- description: List uncollated submission versions
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/gradebook_history/feed
- description: Details for a given date in gradebook history for this course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/gradebook_history/:date
- description: Lists submissions
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/gradebook_history/:date/graders/:grader_id/assignments/:assignment_id/submissions
- description: List grading periods
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/grading_periods
- description: Batch update grading periods
  flows: []
  scope: url:PATCH|/api/v1/courses/:course_id/grading_periods/batch_update
- description: Delete a grading period
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/grading_periods/:id
- description: Get a single grading period
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/grading_periods/:id
- description: Update a single grading period
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/grading_periods/:id
- description: List the grading standards available in a context.
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/grading_standards
- description: Create a new grading standard
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/grading_standards
- description: Delete a grading standard
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/grading_standards/:grading_standard_id
- description: Get a single grading standard in a context.
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/grading_standards/:grading_standard_id
- description: Update a grading standard
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/grading_standards/:grading_standard_id
- description: List group categories for a context
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/group_categories
- description: Create a Group Category
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/group_categories
- description: Bulk manage differentiation tags
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/group_categories/bulk_manage_differentiation_tag
- description: Get differentiation tag candidate count
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/group_categories/differentiation_tag_candidate_count
- description: export tags and users in course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/group_categories/export_tags
- description: Import differentiation tags
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/group_categories/import_tags
- description: List the groups available in a context.
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/groups
- description: List live assessments
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/live_assessments
- description: Create or find a live assessment
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/live_assessments
- description: List live assessment results
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/live_assessments/:assessment_id/results
- description: Create live assessment results
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/live_assessments/:assessment_id/results
- description: List LTI Launch Definitions
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/lti_apps/launch_definitions
- description: List LTI Resource Links
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/lti_resource_links
- description: Create an LTI Resource Link
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/lti_resource_links
- description: Bulk Create LTI Resource Links
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/lti_resource_links/bulk
- description: Delete an LTI Resource Link
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/lti_resource_links/:id
- description: Show an LTI Resource Link
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/lti_resource_links/:id
- description: Update an LTI Resource Link
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/lti_resource_links/:id
- description: List Media Objects
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/media_attachments
- description: List Media Objects
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/media_objects
- description: Get module item sequence
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/module_item_sequence
- description: List modules
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/modules
- description: Create a module
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/modules
- description: List a module's overrides
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/modules/:context_module_id/assignment_overrides
- description: Update a module's overrides
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/modules/:context_module_id/assignment_overrides
- description: Get a learning object's date information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/modules/:context_module_id/date_details
- description: Delete module
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/modules/:id
- description: Show module
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/modules/:id
- description: Update a module
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/modules/:id
- description: Re-lock module progressions
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/modules/:id/relock
- description: List module items
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/modules/:module_id/items
- description: Create a module item
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/modules/:module_id/items
- description: Delete module item
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/modules/:module_id/items/:id
- description: Show module item
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/modules/:module_id/items/:id
- description: Update a module item
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/modules/:module_id/items/:id
- description: Mark module item as done/not done
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/modules/:module_id/items/:id/done
- description: Mark module item read
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/modules/:module_id/items/:id/mark_read
- description: Select a mastery path
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/modules/:module_id/items/:id/select_mastery_path
- description: Retrieve assignment-overridden dates for New Quizzes
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/new_quizzes/assignment_overrides
- description: Get outcome alignments for a student or assignment
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_alignments
- description: Get all outcome links for context
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_group_links
- description: Get all outcome groups for context
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_groups
- description: Delete an outcome group
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/outcome_groups/:id
- description: Show an outcome group
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_groups/:id
- description: Update an outcome group
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/outcome_groups/:id
- description: Import an outcome group
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/outcome_groups/:id/import
- description: List linked outcomes
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_groups/:id/outcomes
- description: Create/link an outcome
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/outcome_groups/:id/outcomes
- description: Unlink an outcome
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/outcome_groups/:id/outcomes/:outcome_id
- description: Create/link an outcome
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/outcome_groups/:id/outcomes/:outcome_id
- description: List subgroups
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_groups/:id/subgroups
- description: Create a subgroup
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/outcome_groups/:id/subgroups
- description: Import Outcomes
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/outcome_imports
- description: Get Outcome import status
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_imports/:id
- description: Get IDs of outcome groups created after successful import
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_imports/:id/created_group_ids
- description: Get mastery distribution
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_mastery_distribution
- description: Get proficiency ratings
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_proficiency
- description: Create/update proficiency ratings
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/outcome_proficiency
- description: Get outcome results
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_results
- description: Get outcome result rollups
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcome_rollups
- description: Get contributing scores
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/outcomes/:outcome_id/contributing_scores
- description: List pages
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/pages
- description: Create page
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/pages
- description: Delete page
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/pages/:url_or_id
- description: Show page
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/pages/:url_or_id
- description: Update/create page
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/pages/:url_or_id
- description: Get a learning object's date information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/pages/:url_or_id/date_details
- description: Update a learning object's date information
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/pages/:url_or_id/date_details
- description: Duplicate page
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/pages/:url_or_id/duplicate
- description: List revisions
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/pages/:url_or_id/revisions
- description: Show revision
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/pages/:url_or_id/revisions/latest
- description: Show revision
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/pages/:url_or_id/revisions/:revision_id
- description: Revert to revision
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/pages/:url_or_id/revisions/:revision_id
- description: Permissions
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/permissions
- description: List potential members
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/potential_collaborators
- description: Preview processed html
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/preview_html
- description: Set extensions for student quiz submissions
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quiz_extensions
- description: List quizzes in a course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes
- description: Create a quiz
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes
- description: Retrieve assignment-overridden dates for Classic Quizzes
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/assignment_overrides
- description: Delete a quiz
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/quizzes/:id
- description: Get a single quiz
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:id
- description: Edit a quiz
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/quizzes/:id
- description: Reorder quiz items
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:id/reorder
- description: Send a message to unsubmitted or submitted users for the quiz
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:id/submission_users/message
- description: Validate quiz access code
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:id/validate_access_code
- description: Get a learning object's date information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/date_details
- description: Update a learning object's date information
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/quizzes/:quiz_id/date_details
- description: Set extensions for student quiz submissions
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/extensions
- description: List question groups in a quiz
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/groups
- description: Create a question group
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/groups
- description: Delete a question group
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/quizzes/:quiz_id/groups/:id
- description: Get a single quiz group
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/groups/:id
- description: Update a question group
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/quizzes/:quiz_id/groups/:id
- description: Reorder question groups
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/groups/:id/reorder
- description: Get available quiz IP filters.
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/ip_filters
- description: List questions in a quiz or a submission
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/questions
- description: Create a single quiz question
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/questions
- description: Delete a quiz question
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/quizzes/:quiz_id/questions/:id
- description: Get a single quiz question
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/questions/:id
- description: Update an existing quiz question
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/quizzes/:quiz_id/questions/:id
- description: Retrieve all quiz reports
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/reports
- description: Create a quiz report
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/reports
- description: Abort the generation of a report, or remove a previously generated one
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/quizzes/:quiz_id/reports/:id
- description: Get a quiz report
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/reports/:id
- description: Fetching the latest quiz statistics
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/statistics
- description: Get the quiz submission.
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submission
- description: Get all quiz submissions.
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions
- description: Create the quiz submission (start a quiz-taking session)
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions
- description: Upload a file
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/self/files
- description: Get a single quiz submission.
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id
- description: Update student question scores and comments.
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id
- description: Complete the quiz submission (turn it in).
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id/complete
- description: Retrieve captured events
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id/events
- description: Submit captured events
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id/events
- description: Get current quiz submission times.
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/quizzes/:quiz_id/submissions/:id/time
- description: List recently logged in students
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/recent_students
- description: Status of last Report
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/reports/:report_type
- description: Start a Report
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/reports/:report_type
- description: Status of a Report
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/reports/:report_type/:id
- description: Reset a course
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/reset_content
- description: Restore course syllabus version
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/restore/:version_id
- description: Redirect to root outcome group for context
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/root_outcome_group
- description: Create a RubricAssociation
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/rubric_associations
- description: Delete a RubricAssociation
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/rubric_associations/:id
- description: Update a RubricAssociation
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/rubric_associations/:id
- description: Create a single rubric assessment
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/rubric_associations/:rubric_association_id/rubric_assessments
- description: Delete a single rubric assessment
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/rubric_associations/:rubric_association_id/rubric_assessments/:id
- description: Update a single rubric assessment
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/rubric_associations/:rubric_association_id/rubric_assessments/:id
- description: List rubrics
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/rubrics
- description: Create a single rubric
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/rubrics
- description: Creates a rubric using a CSV file
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/rubrics/upload
- description: Get the status of a rubric import
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/rubrics/upload/:id
- description: Delete a single
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/rubrics/:id
- description: Get a single rubric
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/rubrics/:id
- description: Update a single rubric
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/rubrics/:id
- description: Get the courses and assignments for a rubric
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/rubrics/:id/used_locations
- description: List users in course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/search_users
- description: List course sections
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/sections
- description: Create course section
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/sections
- description: Get section information
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/sections/:id
- description: Get course settings
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/settings
- description: Update course settings
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/settings
- description: Search course content
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/smartsearch
- description: Return test student for course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/student_view_student
- description: List students
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/students
- description: List submissions for multiple assignments
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/students/submissions
- description: Request a study assist response
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/study_assist
- description: Mark bulk submissions as read
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/submissions/bulk_mark_read
- description: Grade or comment on multiple submissions
  flows: []
  scope: url:POST|/api/v1/courses/:course_id/submissions/update_grades
- description: Clear unread status for all submissions.
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/submissions/:user_id/clear_unread
- description: List available tabs for a course or group
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/tabs
- description: Update a tab for a course
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/tabs/:tab_id
- description: Course TODO items
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/todo
- description: Remove usage rights
  flows: []
  scope: url:DELETE|/api/v1/courses/:course_id/usage_rights
- description: Set usage rights
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/usage_rights
- description: List users in course
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/users
- description: Get single user
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/users/:id
- description: Add last attended date
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/users/:user_id/last_attended
- description: Get user progress
  flows: []
  scope: url:GET|/api/v1/courses/:course_id/users/:user_id/progress
- description: Reset the what-if scores for the current user for an entire course and recalculate grades
  flows: []
  scope: url:PUT|/api/v1/courses/:course_id/what_if_grades/reset
- description: Delete/Conclude a course
  flows: []
  scope: url:DELETE|/api/v1/courses/:id
- description: Get a single course
  flows: []
  scope: url:GET|/api/v1/courses/:id
- description: Update a course
  flows: []
  scope: url:PUT|/api/v1/courses/:id
- description: Remove quiz migration alert
  flows: []
  scope: url:POST|/api/v1/courses/:id/dismiss_migration_limitation_message
- description: Get a late policy
  flows: []
  scope: url:GET|/api/v1/courses/:id/late_policy
- description: Patch a late policy
  flows: []
  scope: url:PATCH|/api/v1/courses/:id/late_policy
- description: Create a late policy
  flows: []
  scope: url:POST|/api/v1/courses/:id/late_policy
- description: Delete a Developer Key
  flows: []
  scope: url:DELETE|/api/v1/developer_keys/:id
- description: Update a Developer Key
  flows: []
  scope: url:PUT|/api/v1/developer_keys/:id
- description: Regenerate Developer Key Secret
  flows: []
  scope: url:POST|/api/v1/developer_keys/:id/regenerate_secret
- description: Get Discovery Page
  flows: []
  scope: url:GET|/api/v1/discovery_pages
- description: Update Discovery Page
  flows: []
  scope: url:PUT|/api/v1/discovery_pages
- description: Generate Discovery Page Preview Token
  flows: []
  scope: url:POST|/api/v1/discovery_pages/token
- description: Moderate an ePortfolio
  flows: []
  scope: url:PUT|/api/v1/eportfolios/:eportfolio_id/moderate
- description: Get ePortfolio Pages
  flows: []
  scope: url:GET|/api/v1/eportfolios/:eportfolio_id/pages
- description: Restore a deleted ePortfolio
  flows: []
  scope: url:PUT|/api/v1/eportfolios/:eportfolio_id/restore
- description: Delete an ePortfolio
  flows: []
  scope: url:DELETE|/api/v1/eportfolios/:id
- description: Get an ePortfolio
  flows: []
  scope: url:GET|/api/v1/eportfolios/:id
- description: List courses with their latest ePub export
  flows: []
  scope: url:GET|/api/v1/epub_exports
- description: Create Error Report
  flows: []
  scope: url:POST|/api/v1/error_reports
- description: Get visible course navigation tools
  flows: []
  scope: url:GET|/api/v1/external_tools/visible_course_nav_tools
- description: List environment features
  flows: []
  scope: url:GET|/api/v1/features/environment
- description: Update word count
  flows: []
  scope: url:POST|/api/v1/files/update_word_count
- description: Delete file
  flows: []
  scope: url:DELETE|/api/v1/files/:id
- description: Get file
  flows: []
  scope: url:GET|/api/v1/files/:id
- description: Update file
  flows: []
  scope: url:PUT|/api/v1/files/:id
- description: Get icon metadata
  flows: []
  scope: url:GET|/api/v1/files/:id/icon_metadata
- description: Get public inline preview url
  flows: []
  scope: url:GET|/api/v1/files/:id/public_url
- description: Reset link verifier
  flows: []
  scope: url:POST|/api/v1/files/:id/reset_verifier
- description: Copy a file
  flows: []
  scope: url:POST|/api/v1/folders/:dest_folder_id/copy_file
- description: Copy a folder
  flows: []
  scope: url:POST|/api/v1/folders/:dest_folder_id/copy_folder
- description: Upload a file
  flows: []
  scope: url:POST|/api/v1/folders/:folder_id/files
- description: Create folder
  flows: []
  scope: url:POST|/api/v1/folders/:folder_id/folders
- description: Delete folder
  flows: []
  scope: url:DELETE|/api/v1/folders/:id
- description: Get folder
  flows: []
  scope: url:GET|/api/v1/folders/:id
- description: Update folder
  flows: []
  scope: url:PUT|/api/v1/folders/:id
- description: List files
  flows: []
  scope: url:GET|/api/v1/folders/:id/files
- description: List folders
  flows: []
  scope: url:GET|/api/v1/folders/:id/folders
- description: Delete an outcome group
  flows: []
  scope: url:DELETE|/api/v1/global/outcome_groups/:id
- description: Show an outcome group
  flows: []
  scope: url:GET|/api/v1/global/outcome_groups/:id
- description: Update an outcome group
  flows: []
  scope: url:PUT|/api/v1/global/outcome_groups/:id
- description: Import an outcome group
  flows: []
  scope: url:POST|/api/v1/global/outcome_groups/:id/import
- description: List linked outcomes
  flows: []
  scope: url:GET|/api/v1/global/outcome_groups/:id/outcomes
- description: Create/link an outcome
  flows: []
  scope: url:POST|/api/v1/global/outcome_groups/:id/outcomes
- description: Unlink an outcome
  flows: []
  scope: url:DELETE|/api/v1/global/outcome_groups/:id/outcomes/:outcome_id
- description: Create/link an outcome
  flows: []
  scope: url:PUT|/api/v1/global/outcome_groups/:id/outcomes/:outcome_id
- description: List subgroups
  flows: []
  scope: url:GET|/api/v1/global/outcome_groups/:id/subgroups
- description: Create a subgroup
  flows: []
  scope: url:POST|/api/v1/global/outcome_groups/:id/subgroups
- description: Redirect to root outcome group for context
  flows: []
  scope: url:GET|/api/v1/global/root_outcome_group
- description: Batch update grading periods
  flows: []
  scope: url:PATCH|/api/v1/grading_period_sets/:set_id/grading_periods/batch_update
- description: Delete a Group Category
  flows: []
  scope: url:DELETE|/api/v1/group_categories/:group_category_id
- description: Get a single group category
  flows: []
  scope: url:GET|/api/v1/group_categories/:group_category_id
- description: Update a Group Category
  flows: []
  scope: url:PUT|/api/v1/group_categories/:group_category_id
- description: Assign unassigned members
  flows: []
  scope: url:POST|/api/v1/group_categories/:group_category_id/assign_unassigned_members
- description: export groups in and users in category
  flows: []
  scope: url:GET|/api/v1/group_categories/:group_category_id/export
- description: List groups in group category
  flows: []
  scope: url:GET|/api/v1/group_categories/:group_category_id/groups
- description: Create a group
  flows: []
  scope: url:POST|/api/v1/group_categories/:group_category_id/groups
- description: Import category groups
  flows: []
  scope: url:POST|/api/v1/group_categories/:group_category_id/import
- description: List users in group category
  flows: []
  scope: url:GET|/api/v1/group_categories/:group_category_id/users
- description: Create a group
  flows: []
  scope: url:POST|/api/v1/groups
- description: Delete a group
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id
- description: Get a single group
  flows: []
  scope: url:GET|/api/v1/groups/:group_id
- description: Edit a group
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id
- description: Group activity stream
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/activity_stream
- description: Group activity stream summary
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/activity_stream/summary
- description: Redirect to the assignment override for a group
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/assignments/:assignment_id/override
- description: List collaborations
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/collaborations
- description: List conferences
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/conferences
- description: List content exports
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/content_exports
- description: Export content
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/content_exports
- description: Show content export
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/content_exports/:id
- description: List licenses
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/content_licenses
- description: List content migrations
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/content_migrations
- description: Create a content migration
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/content_migrations
- description: List Migration Systems
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/content_migrations/migrators
- description: List migration issues
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/content_migrations/:content_migration_id/migration_issues
- description: Get a migration issue
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/content_migrations/:content_migration_id/migration_issues/:id
- description: Update a migration issue
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/content_migrations/:content_migration_id/migration_issues/:id
- description: Get a content migration
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/content_migrations/:id
- description: Update a content migration
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/content_migrations/:id
- description: List items for selective import
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/content_migrations/:id/selective_data
- description: List discussion topics
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/discussion_topics
- description: Create a new discussion topic
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/discussion_topics
- description: Mark all topic as read
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/discussion_topics/read_all
- description: Reorder pinned topics
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/discussion_topics/reorder
- description: Delete a topic
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id
- description: Get a single topic
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id
- description: Update a topic
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id
- description: Duplicate discussion topic
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/duplicate
- description: List topic entries
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries
- description: Post an entry
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries
- description: Rate entry
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/rating
- description: Mark entry as unread
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/read
- description: Mark entry as read
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/read
- description: List entry replies
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/replies
- description: Post a reply
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:entry_id/replies
- description: Delete an entry
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:id
- description: Update an entry
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/entries/:id
- description: List entries
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/entry_list
- description: Mark topic as unread
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/read
- description: Mark topic as read
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/read
- description: Mark all entries as unread
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/read_all
- description: Mark all entries as read
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/read_all
- description: Unsubscribe from a topic
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/discussion_topics/:topic_id/subscribed
- description: Subscribe to a topic
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/subscribed
- description: Find Last Summary
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/summaries
- description: Find or Create Summary
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/summaries
- description: Disable summary
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/discussion_topics/:topic_id/summaries/disable
- description: Summary Feedback
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/discussion_topics/:topic_id/summaries/:summary_id/feedback
- description: Get the full topic
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/discussion_topics/:topic_id/view
- description: List external feeds
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/external_feeds
- description: Create an external feed
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/external_feeds
- description: Delete an external feed
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/external_feeds/:external_feed_id
- description: List external tools
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/external_tools
- description: List files
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/files
- description: Upload a file
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/files
- description: Get quota information
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/files/quota
- description: Get file
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/files/:id
- description: List all folders
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/folders
- description: Create folder
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/folders
- description: Resolve path
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/folders/by_path
- description: Resolve path
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/folders/by_path/*full_path
- description: Get uploaded media folder for user
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/folders/media
- description: Get folder
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/folders/:id
- description: Show front page
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/front_page
- description: Update/create front page
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/front_page
- description: Invite others to a group
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/invite
- description: List Media Objects
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/media_attachments
- description: List Media Objects
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/media_objects
- description: List group memberships
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/memberships
- description: Create a membership
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/memberships
- description: Leave a group
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/memberships/:membership_id
- description: Get a single group membership
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/memberships/:membership_id
- description: Update a membership
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/memberships/:membership_id
- description: List pages
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/pages
- description: Create page
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/pages
- description: Delete page
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/pages/:url_or_id
- description: Show page
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/pages/:url_or_id
- description: Update/create page
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/pages/:url_or_id
- description: List revisions
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/pages/:url_or_id/revisions
- description: Show revision
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/pages/:url_or_id/revisions/latest
- description: Show revision
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/pages/:url_or_id/revisions/:revision_id
- description: Revert to revision
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/pages/:url_or_id/revisions/:revision_id
- description: Permissions
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/permissions
- description: List potential members
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/potential_collaborators
- description: Preview processed html
  flows: []
  scope: url:POST|/api/v1/groups/:group_id/preview_html
- description: List available tabs for a course or group
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/tabs
- description: Remove usage rights
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/usage_rights
- description: Set usage rights
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/usage_rights
- description: Bulk delete memberships Bulk deletes memberships by providing an array of user IDs, or, for differentiation tag groups, by providing `all_in_group_course` to remove every course student matching an optional role/tag filter.
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/users
- description: List group's users
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/users
- description: Leave a group
  flows: []
  scope: url:DELETE|/api/v1/groups/:group_id/users/:user_id
- description: Get a single group membership
  flows: []
  scope: url:GET|/api/v1/groups/:group_id/users/:user_id
- description: Update a membership
  flows: []
  scope: url:PUT|/api/v1/groups/:group_id/users/:user_id
- description: List horizon accounts
  flows: []
  scope: url:GET|/api/v1/horizon_accounts
- description: '[DEPRECATED] Create InstAccess token'
  flows: []
  scope: url:POST|/api/v1/inst_access_tokens
- description: Create JWT
  flows: []
  scope: url:POST|/api/v1/jwts
- description: Refresh JWT
  flows: []
  scope: url:POST|/api/v1/jwts/refresh
- description: Get accounts that admins can manage
  flows: []
  scope: url:GET|/api/v1/manageable_accounts
- description: Get the manually-created courses sub-account for the domain root account
  flows: []
  scope: url:GET|/api/v1/manually_created_courses_account
- description: List Media Objects
  flows: []
  scope: url:GET|/api/v1/media_attachments
- description: Update Media Object
  flows: []
  scope: url:PUT|/api/v1/media_attachments/:attachment_id
- description: List media tracks for a Media Object or Attachment
  flows: []
  scope: url:GET|/api/v1/media_attachments/:attachment_id/media_tracks
- description: Update Media Tracks
  flows: []
  scope: url:PUT|/api/v1/media_attachments/:attachment_id/media_tracks
- description: List Media Objects
  flows: []
  scope: url:GET|/api/v1/media_objects
- description: Update Media Object
  flows: []
  scope: url:PUT|/api/v1/media_objects/:media_object_id
- description: List media tracks for a Media Object or Attachment
  flows: []
  scope: url:GET|/api/v1/media_objects/:media_object_id/media_tracks
- description: Update Media Tracks
  flows: []
  scope: url:PUT|/api/v1/media_objects/:media_object_id/media_tracks
- description: Show an outcome
  flows: []
  scope: url:GET|/api/v1/outcomes/:id
- description: Update an outcome
  flows: []
  scope: url:PUT|/api/v1/outcomes/:id
- description: Retrieve permission groups
  flows: []
  scope: url:GET|/api/v1/permissions/groups
- description: Get help text for permissions
  flows: []
  scope: url:GET|/api/v1/permissions/:context_type/:permission/help
- description: List planner items
  flows: []
  scope: url:GET|/api/v1/planner/items
- description: List planner overrides
  flows: []
  scope: url:GET|/api/v1/planner/overrides
- description: Create a planner override
  flows: []
  scope: url:POST|/api/v1/planner/overrides
- description: Delete a planner override
  flows: []
  scope: url:DELETE|/api/v1/planner/overrides/:id
- description: Show a planner override
  flows: []
  scope: url:GET|/api/v1/planner/overrides/:id
- description: Update a planner override
  flows: []
  scope: url:PUT|/api/v1/planner/overrides/:id
- description: List planner notes
  flows: []
  scope: url:GET|/api/v1/planner_notes
- description: Create a planner note
  flows: []
  scope: url:POST|/api/v1/planner_notes
- description: Delete a planner note
  flows: []
  scope: url:DELETE|/api/v1/planner_notes/:id
- description: Show a planner note
  flows: []
  scope: url:GET|/api/v1/planner_notes/:id
- description: Update a planner note
  flows: []
  scope: url:PUT|/api/v1/planner_notes/:id
- description: List closed poll sessions
  flows: []
  scope: url:GET|/api/v1/poll_sessions/closed
- description: List opened poll sessions
  flows: []
  scope: url:GET|/api/v1/poll_sessions/opened
- description: List polls
  flows: []
  scope: url:GET|/api/v1/polls
- description: Create a single poll
  flows: []
  scope: url:POST|/api/v1/polls
- description: Delete a poll
  flows: []
  scope: url:DELETE|/api/v1/polls/:id
- description: Get a single poll
  flows: []
  scope: url:GET|/api/v1/polls/:id
- description: Update a single poll
  flows: []
  scope: url:PUT|/api/v1/polls/:id
- description: List poll choices in a poll
  flows: []
  scope: url:GET|/api/v1/polls/:poll_id/poll_choices
- description: Create a single poll choice
  flows: []
  scope: url:POST|/api/v1/polls/:poll_id/poll_choices
- description: Delete a poll choice
  flows: []
  scope: url:DELETE|/api/v1/polls/:poll_id/poll_choices/:id
- description: Get a single poll choice
  flows: []
  scope: url:GET|/api/v1/polls/:poll_id/poll_choices/:id
- description: Update a single poll choice
  flows: []
  scope: url:PUT|/api/v1/polls/:poll_id/poll_choices/:id
- description: List poll sessions for a poll
  flows: []
  scope: url:GET|/api/v1/polls/:poll_id/poll_sessions
- description: Create a single poll session
  flows: []
  scope: url:POST|/api/v1/polls/:poll_id/poll_sessions
- description: Delete a poll session
  flows: []
  scope: url:DELETE|/api/v1/polls/:poll_id/poll_sessions/:id
- description: Get the results for a single poll session
  flows: []
  scope: url:GET|/api/v1/polls/:poll_id/poll_sessions/:id
- description: Update a single poll session
  flows: []
  scope: url:PUT|/api/v1/polls/:poll_id/poll_sessions/:id
- description: Close an opened poll session
  flows: []
  scope: url:GET|/api/v1/polls/:poll_id/poll_sessions/:id/close
- description: Open a poll session
  flows: []
  scope: url:GET|/api/v1/polls/:poll_id/poll_sessions/:id/open
- description: Create a single poll submission
  flows: []
  scope: url:POST|/api/v1/polls/:poll_id/poll_sessions/:poll_session_id/poll_submissions
- description: Get a single poll submission
  flows: []
  scope: url:GET|/api/v1/polls/:poll_id/poll_sessions/:poll_session_id/poll_submissions/:id
- description: Query progress
  flows: []
  scope: url:GET|/api/v1/progress/:id
- description: Cancel progress
  flows: []
  scope: url:POST|/api/v1/progress/:id/cancel
- description: List question banks
  flows: []
  scope: url:GET|/api/v1/question_banks
- description: Get a single question bank
  flows: []
  scope: url:GET|/api/v1/question_banks/:id
- description: List assessment questions for a question bank
  flows: []
  scope: url:GET|/api/v1/question_banks/:id/questions
- description: Get all quiz submission questions.
  flows: []
  scope: url:GET|/api/v1/quiz_submissions/:quiz_submission_id/questions
- description: Answering questions
  flows: []
  scope: url:POST|/api/v1/quiz_submissions/:quiz_submission_id/questions
- description: Flagging a question.
  flows: []
  scope: url:PUT|/api/v1/quiz_submissions/:quiz_submission_id/questions/:id/flag
- description: Get a formatted student numerical answer.
  flows: []
  scope: url:GET|/api/v1/quiz_submissions/:quiz_submission_id/questions/:id/formatted_answer
- description: Unflagging a question.
  flows: []
  scope: url:PUT|/api/v1/quiz_submissions/:quiz_submission_id/questions/:id/unflag
- description: Templated file for importing a rubric
  flows: []
  scope: url:GET|/api/v1/rubrics/upload_template
- description: List all courses
  flows: []
  scope: url:GET|/api/v1/search/all_courses
- description: Find recipients
  flows: []
  scope: url:GET|/api/v1/search/recipients
- description: Redirect to the assignment override for a section
  flows: []
  scope: url:GET|/api/v1/sections/:course_section_id/assignments/:assignment_id/override
- description: Delete a section
  flows: []
  scope: url:DELETE|/api/v1/sections/:id
- description: Get section information
  flows: []
  scope: url:GET|/api/v1/sections/:id
- description: Edit a section
  flows: []
  scope: url:PUT|/api/v1/sections/:id
- description: De-cross-list a Section
  flows: []
  scope: url:DELETE|/api/v1/sections/:id/crosslist
- description: Cross-list a Section
  flows: []
  scope: url:POST|/api/v1/sections/:id/crosslist/:new_course_id
- description: List section's users
  flows: []
  scope: url:GET|/api/v1/sections/:id/users
- description: Get a single submission by anonymous id
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/anonymous_submissions/:anonymous_id
- description: Grade or comment on a submission by anonymous id
  flows: []
  scope: url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/anonymous_submissions/:anonymous_id
- description: Get all Peer Reviews
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/peer_reviews
- description: Submission Summary
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submission_summary
- description: List assignment submissions
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions
- description: Submit an assignment
  flows: []
  scope: url:POST|/api/v1/sections/:section_id/assignments/:assignment_id/submissions
- description: Grade or comment on multiple submissions
  flows: []
  scope: url:POST|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/update_grades
- description: Delete Peer Review
  flows: []
  scope: url:DELETE|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- description: Get all Peer Reviews
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- description: Create Peer Review
  flows: []
  scope: url:POST|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:submission_id/peer_reviews
- description: Get a single submission
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id
- description: Grade or comment on a submission
  flows: []
  scope: url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id
- description: Get document annotations read state
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/document_annotations/read
- description: Mark document annotations as read
  flows: []
  scope: url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/document_annotations/read
- description: Upload a file
  flows: []
  scope: url:POST|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/files
- description: Mark submission as unread
  flows: []
  scope: url:DELETE|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/read
- description: Mark submission as read
  flows: []
  scope: url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/read
- description: Mark submission item as read
  flows: []
  scope: url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/read/:item
- description: Get rubric assessments read state
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/rubric_assessments/read
- description: Mark rubric assessments as read
  flows: []
  scope: url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/rubric_assessments/read
- description: Get rubric assessments read state
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/rubric_comments/read
- description: Mark rubric assessments as read
  flows: []
  scope: url:PUT|/api/v1/sections/:section_id/assignments/:assignment_id/submissions/:user_id/rubric_comments/read
- description: List enrollments
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/enrollments
- description: Enroll a user
  flows: []
  scope: url:POST|/api/v1/sections/:section_id/enrollments
- description: List submissions for multiple assignments
  flows: []
  scope: url:GET|/api/v1/sections/:section_id/students/submissions
- description: Mark bulk submissions as read
  flows: []
  scope: url:PUT|/api/v1/sections/:section_id/submissions/bulk_mark_read
- description: Grade or comment on multiple submissions
  flows: []
  scope: url:POST|/api/v1/sections/:section_id/submissions/update_grades
- description: Clear unread status for all submissions.
  flows: []
  scope: url:PUT|/api/v1/sections/:section_id/submissions/:user_id/clear_unread
- description: Get Kaltura config
  flows: []
  scope: url:GET|/api/v1/services/kaltura
- description: Start Kaltura session
  flows: []
  scope: url:POST|/api/v1/services/kaltura_session
- description: List environment settings
  flows: []
  scope: url:GET|/api/v1/settings/environment
- description: Un-share a BrandConfig (Theme)
  flows: []
  scope: url:DELETE|/api/v1/shared_brand_configs/:id
- description: Update a submission's what-if score and calculate grades
  flows: []
  scope: url:PUT|/api/v1/submissions/:id/what_if_grades
- description: Bulk Temporary Enrollment Status
  flows: []
  scope: url:GET|/api/v1/temporary_enrollment_status
- description: List the activity stream
  flows: []
  scope: url:GET|/api/v1/users/activity_stream
- description: Log users out of all mobile apps
  flows: []
  scope: url:DELETE|/api/v1/users/mobile_sessions
- description: BETA - Initiate batch page views query
  flows: []
  scope: url:POST|/api/v1/users/page_views/query
- description: BETA - Poll batch query status
  flows: []
  scope: url:GET|/api/v1/users/page_views/query/:query_id
- description: BETA - Get batch query results
  flows: []
  scope: url:GET|/api/v1/users/page_views/query/:query_id/results
- description: Kickoff password recovery flow
  flows: []
  scope: url:POST|/api/v1/users/reset_password
- description: Hide all stream items
  flows: []
  scope: url:DELETE|/api/v1/users/self/activity_stream
- description: List the activity stream
  flows: []
  scope: url:GET|/api/v1/users/self/activity_stream
- description: Activity stream summary
  flows: []
  scope: url:GET|/api/v1/users/self/activity_stream/summary
- description: Hide a stream item
  flows: []
  scope: url:DELETE|/api/v1/users/self/activity_stream/:id
- description: List bookmarks
  flows: []
  scope: url:GET|/api/v1/users/self/bookmarks
- description: Create bookmark
  flows: []
  scope: url:POST|/api/v1/users/self/bookmarks
- description: Delete bookmark
  flows: []
  scope: url:DELETE|/api/v1/users/self/bookmarks/:id
- description: Get bookmark
  flows: []
  scope: url:GET|/api/v1/users/self/bookmarks/:id
- description: Update bookmark
  flows: []
  scope: url:PUT|/api/v1/users/self/bookmarks/:id
- description: Delete a push notification endpoint
  flows: []
  scope: url:DELETE|/api/v1/users/self/communication_channels/push
- description: Update preferences by category
  flows: []
  scope: url:PUT|/api/v1/users/self/communication_channels/:communication_channel_id/notification_preference_categories/:category
- description: Update multiple preferences
  flows: []
  scope: url:PUT|/api/v1/users/self/communication_channels/:communication_channel_id/notification_preferences
- description: Update a preference
  flows: []
  scope: url:PUT|/api/v1/users/self/communication_channels/:communication_channel_id/notification_preferences/:notification
- description: Update multiple preferences
  flows: []
  scope: url:PUT|/api/v1/users/self/communication_channels/:type/:address/notification_preferences
- description: Update a preference
  flows: []
  scope: url:PUT|/api/v1/users/self/communication_channels/:type/:address/notification_preferences/:notification
- description: Clear course nicknames
  flows: []
  scope: url:DELETE|/api/v1/users/self/course_nicknames
- description: List course nicknames
  flows: []
  scope: url:GET|/api/v1/users/self/course_nicknames
- description: Remove course nickname
  flows: []
  scope: url:DELETE|/api/v1/users/self/course_nicknames/:course_id
- description: Get course nickname
  flows: []
  scope: url:GET|/api/v1/users/self/course_nicknames/:course_id
- description: Set course nickname
  flows: []
  scope: url:PUT|/api/v1/users/self/course_nicknames/:course_id
- description: Reset course favorites
  flows: []
  scope: url:DELETE|/api/v1/users/self/favorites/courses
- description: List favorite courses
  flows: []
  scope: url:GET|/api/v1/users/self/favorites/courses
- description: Remove course from favorites
  flows: []
  scope: url:DELETE|/api/v1/users/self/favorites/courses/:id
- description: Add course to favorites
  flows: []
  scope: url:POST|/api/v1/users/self/favorites/courses/:id
- description: Reset group favorites
  flows: []
  scope: url:DELETE|/api/v1/users/self/favorites/groups
- description: List favorite groups
  flows: []
  scope: url:GET|/api/v1/users/self/favorites/groups
- description: Remove group from favorites
  flows: []
  scope: url:DELETE|/api/v1/users/self/favorites/groups/:id
- description: Add group to favorites
  flows: []
  scope: url:POST|/api/v1/users/self/favorites/groups/:id
- description: List your groups
  flows: []
  scope: url:GET|/api/v1/users/self/groups
- description: Get a Pandata Events jwt token and its expiration date
  flows: []
  scope: url:POST|/api/v1/users/self/pandata_events_token
- description: List the TODO items
  flows: []
  scope: url:GET|/api/v1/users/self/todo
- description: List counts for todo items
  flows: []
  scope: url:GET|/api/v1/users/self/todo_item_count
- description: List upcoming assignments, calendar events
  flows: []
  scope: url:GET|/api/v1/users/self/upcoming_events
- description: Show user details
  flows: []
  scope: url:GET|/api/v1/users/:id
- description: Edit a user
  flows: []
  scope: url:PUT|/api/v1/users/:id
- description: Get custom colors
  flows: []
  scope: url:GET|/api/v1/users/:id/colors
- description: Get custom color
  flows: []
  scope: url:GET|/api/v1/users/:id/colors/:asset_string
- description: Update custom color
  flows: []
  scope: url:PUT|/api/v1/users/:id/colors/:asset_string
- description: Get dashboard positions
  flows: []
  scope: url:GET|/api/v1/users/:id/dashboard_positions
- description: Update dashboard positions
  flows: []
  scope: url:PUT|/api/v1/users/:id/dashboard_positions
- description: Update files UI version preference
  flows: []
  scope: url:PUT|/api/v1/users/:id/files_ui_version_preference
- description: Get a users most recently graded submissions
  flows: []
  scope: url:GET|/api/v1/users/:id/graded_submissions
- description: Merge user into another user
  flows: []
  scope: url:PUT|/api/v1/users/:id/merge_into/accounts/:destination_account_id/users/:destination_user_id
- description: Merge user into another user
  flows: []
  scope: url:PUT|/api/v1/users/:id/merge_into/:destination_user_id
- description: Log users out of all mobile apps
  flows: []
  scope: url:DELETE|/api/v1/users/:id/mobile_sessions
- description: Terminate all user sessions
  flows: []
  scope: url:DELETE|/api/v1/users/:id/sessions
- description: Update user settings.
  flows: []
  scope: url:GET|/api/v1/users/:id/settings
- description: Split merged users into separate users
  flows: []
  scope: url:POST|/api/v1/users/:id/split
- description: Update text editor preference
  flows: []
  scope: url:PUT|/api/v1/users/:id/text_editor_preference
- description: List avatar options
  flows: []
  scope: url:GET|/api/v1/users/:user_id/avatars
- description: List calendar events for a user
  flows: []
  scope: url:GET|/api/v1/users/:user_id/calendar_events
- description: List user communication channels
  flows: []
  scope: url:GET|/api/v1/users/:user_id/communication_channels
- description: Create a communication channel
  flows: []
  scope: url:POST|/api/v1/users/:user_id/communication_channels
- description: List of preference categories
  flows: []
  scope: url:GET|/api/v1/users/:user_id/communication_channels/:communication_channel_id/notification_preference_categories
- description: List preferences
  flows: []
  scope: url:GET|/api/v1/users/:user_id/communication_channels/:communication_channel_id/notification_preferences
- description: Get a preference
  flows: []
  scope: url:GET|/api/v1/users/:user_id/communication_channels/:communication_channel_id/notification_preferences/:notification
- description: Delete a communication channel
  flows: []
  scope: url:DELETE|/api/v1/users/:user_id/communication_channels/:id
- description: Delete a communication channel
  flows: []
  scope: url:DELETE|/api/v1/users/:user_id/communication_channels/:type/:address
- description: List preferences
  flows: []
  scope: url:GET|/api/v1/users/:user_id/communication_channels/:type/:address/notification_preferences
- description: Get a preference
  flows: []
  scope: url:GET|/api/v1/users/:user_id/communication_channels/:type/:address/notification_preferences/:notification
- description: List content exports
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_exports
- description: Export content
  flows: []
  scope: url:POST|/api/v1/users/:user_id/content_exports
- description: Show content export
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_exports/:id
- description: List licenses
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_licenses
- description: List content migrations
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_migrations
- description: Create a content migration
  flows: []
  scope: url:POST|/api/v1/users/:user_id/content_migrations
- description: List Migration Systems
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_migrations/migrators
- description: List migration issues
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_migrations/:content_migration_id/migration_issues
- description: Get a migration issue
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_migrations/:content_migration_id/migration_issues/:id
- description: Update a migration issue
  flows: []
  scope: url:PUT|/api/v1/users/:user_id/content_migrations/:content_migration_id/migration_issues/:id
- description: Get a content migration
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_migrations/:id
- description: Update a content migration
  flows: []
  scope: url:PUT|/api/v1/users/:user_id/content_migrations/:id
- description: List items for selective import
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_migrations/:id/selective_data
- description: Create a content share
  flows: []
  scope: url:POST|/api/v1/users/:user_id/content_shares
- description: List content shares
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_shares/received
- description: List content shares
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_shares/sent
- description: Get unread shares count
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_shares/unread_count
- description: Remove content share
  flows: []
  scope: url:DELETE|/api/v1/users/:user_id/content_shares/:id
- description: Get content share
  flows: []
  scope: url:GET|/api/v1/users/:user_id/content_shares/:id
- description: Update a content share
  flows: []
  scope: url:PUT|/api/v1/users/:user_id/content_shares/:id
- description: Add users to content share
  flows: []
  scope: url:POST|/api/v1/users/:user_id/content_shares/:id/add_users
- description: List courses for a user
  flows: []
  scope: url:GET|/api/v1/users/:user_id/courses
- description: List assignments for user
  flows: []
  scope: url:GET|/api/v1/users/:user_id/courses/:course_id/assignments
- description: Delete custom data
  flows: []
  scope: url:DELETE|/api/v1/users/:user_id/custom_data
- description: Load custom data
  flows: []
  scope: url:GET|/api/v1/users/:user_id/custom_data
- description: Store custom data
  flows: []
  scope: url:PUT|/api/v1/users/:user_id/custom_data
- description: Trigger accessibility course scan
  flows: []
  scope: url:POST|/api/v1/users/:user_id/educator_accessibility_course_scan
- description: List accessibility course statistics
  flows: []
  scope: url:GET|/api/v1/users/:user_id/educator_accessibility_course_statistics
- description: List accessibility course statistic terms
  flows: []
  scope: url:GET|/api/v1/users/:user_id/educator_accessibility_course_terms
- description: List enrollments
  flows: []
  scope: url:GET|/api/v1/users/:user_id/enrollments
- description: Get all ePortfolios for a User
  flows: []
  scope: url:GET|/api/v1/users/:user_id/eportfolios
- description: Moderate all ePortfolios for a User
  flows: []
  scope: url:PUT|/api/v1/users/:user_id/eportfolios
- description: List features
  flows: []
  scope: url:GET|/api/v1/users/:user_id/features
- description: List enabled features
  flows: []
  scope: url:GET|/api/v1/users/:user_id/features/enabled
- description: Remove feature flag
  flows: []
  scope: url:DELETE|/api/v1/users/:user_id/features/flags/:feature
- description: Get feature flag
  flows: []
  scope: url:GET|/api/v1/users/:user_id/features/flags/:feature
- description: Set feature flag
  flows: []
  scope: url:PUT|/api/v1/users/:user_id/features/flags/:feature
- description: List files
  flows: []
  scope: url:GET|/api/v1/users/:user_id/files
- description: Upload a file
  flows: []
  scope: url:POST|/api/v1/users/:user_id/files
- description: Get quota information
  flows: []
  scope: url:GET|/api/v1/users/:user_id/files/quota
- description: Get file
  flows: []
  scope: url:GET|/api/v1/users/:user_id/files/:id
- description: List all folders
  flows: []
  scope: url:GET|/api/v1/users/:user_id/folders
- description: Create folder
  flows: []
  scope: url:POST|/api/v1/users/:user_id/folders
- description: Resolve path
  flows: []
  scope: url:GET|/api/v1/users/:user_id/folders/by_path
- description: Resolve path
  flows: []
  scope: url:GET|/api/v1/users/:user_id/folders/by_path/*full_path
- description: Get folder
  flows: []
  scope: url:GET|/api/v1/users/:user_id/folders/:id
- description: List recent history for a user
  flows: []
  scope: url:GET|/api/v1/users/:user_id/history
- description: List user logins
  flows: []
  scope: url:GET|/api/v1/users/:user_id/logins
- description: Delete a user login
  flows: []
  scope: url:DELETE|/api/v1/users/:user_id/logins/:id
- description: List Missing Submissions
  flows: []
  scope: url:GET|/api/v1/users/:user_id/missing_submissions
- description: List linked observees
  flows: []
  scope: url:GET|/api/v1/users/:user_id/observees
- description: Add an observee with credentials
  flows: []
  scope: url:POST|/api/v1/users/:user_id/observees
- description: Remove an observee
  flows: []
  scope: url:DELETE|/api/v1/users/:user_id/observees/:observee_id
- description: Show an observee
  flows: []
  scope: url:GET|/api/v1/users/:user_id/observees/:observee_id
- description: Add an observee
  flows: []
  scope: url:PUT|/api/v1/users/:user_id/observees/:observee_id
- description: Create observer pairing code
  flows: []
  scope: url:POST|/api/v1/users/:user_id/observer_pairing_codes
- description: List linked observers
  flows: []
  scope: url:GET|/api/v1/users/:user_id/observers
- description: Show an observer
  flows: []
  scope: url:GET|/api/v1/users/:user_id/observers/:observer_id
- description: List user page views
  flows: []
  scope: url:GET|/api/v1/users/:user_id/page_views
- description: BETA - Initiate page views query
  flows: []
  scope: url:POST|/api/v1/users/:user_id/page_views/query
- description: BETA - Poll query status
  flows: []
  scope: url:GET|/api/v1/users/:user_id/page_views/query/:query_id
- description: BETA - Get query results
  flows: []
  scope: url:GET|/api/v1/users/:user_id/page_views/query/:query_id/results
- description: List planner items
  flows: []
  scope: url:GET|/api/v1/users/:user_id/planner/items
- description: Create a portfolio notification
  flows: []
  scope: url:POST|/api/v1/users/:user_id/portfolio_notifications
- description: Get user profile
  flows: []
  scope: url:GET|/api/v1/users/:user_id/profile
- description: List available tabs for a course or group
  flows: []
  scope: url:GET|/api/v1/users/:user_id/tabs
- description: Show Temporary Enrollment recipient and provider status
  flows: []
  scope: url:GET|/api/v1/users/:user_id/temporary_enrollment_status
- description: Create an access token
  flows: []
  scope: url:POST|/api/v1/users/:user_id/tokens
- description: Delete an access token
  flows: []
  scope: url:DELETE|/api/v1/users/:user_id/tokens/:id
- description: Show an access token
  flows: []
  scope: url:GET|/api/v1/users/:user_id/tokens/:id
- description: Update an access token
  flows: []
  scope: url:PUT|/api/v1/users/:user_id/tokens/:id
- description: Remove usage rights
  flows: []
  scope: url:DELETE|/api/v1/users/:user_id/usage_rights
- description: Set usage rights
  flows: []
  scope: url:PUT|/api/v1/users/:user_id/usage_rights
- description: List access tokens for a user
  flows: []
  scope: url:GET|/api/v1/users/:user_id/user_generated_tokens
slug: canvas-scopes
source_filename: canvas-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/canvas-lms-openapi.yml (paths + verbs) rendered through the scope format Instructure publishes\ndocs: https://developerdocs.instructure.com/services/canvas/resources/api_token_scopes\nmodel: per-endpoint scopes\nformat:\n  template: url:<HTTP_VERB>|/api/v1/<path with :params>\n  example: url:GET|/api/v1/courses\n  published_at: https://developerdocs.instructure.com/services/canvas/resources/api_token_scopes\n  note: 'Canvas does not use named OAuth scopes. A scope IS an endpoint: one string per HTTP verb + route. Instructure\n    prints the exact scope string on every resource documentation page, and a live account can enumerate them from\n    GET /api/v1/accounts/:account_id/scopes. The list below is that same string built mechanically from the 1,117\n    operations Instructure publishes in its own Swagger 1.2 documents — the format is theirs, the operations are\n    theirs; nothing is invented.'\nenumeration_endpoint:\n\
  \  method: GET\n  path: /api/v1/accounts/:account_id/scopes\n  operationId: list_scopes\n  scope: url:GET|/api/v1/accounts/:account_id/scopes\n  params:\n    group_by: resource_name\n  status: BETA — Instructure flags this resource as not finalized\nenforcement:\n  where: Developer Keys\n  note: Scopes are enforced only when a developer key has \"Enforce Scopes\" turned on. A key without scope enforcement\n    grants everything the user can do.\n  docs: https://developerdocs.instructure.com/services/canvas/oauth2/file.developer_keys\nspecial_scopes:\n- scope: /auth/userinfo\n  description: Identity only. Returns the current user's name and id and does NOT return an API access token.\n  source: https://developerdocs.instructure.com/services/canvas/oauth2/file.oauth\nscope_count: 1117\nschemes:\n- name: oauth2\n  source: openapi/canvas-lms-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://canvas.instructure.com/login/oauth2/auth\n    tokenUrl: https://canvas.instructure.com/login/oauth2/token\n\
  scopes:\n- scope: url:GET|/api/lti/accounts/:account_id\n  description: Get account\n  resource: Accounts (Lti)\n  operationId: get_account\n- scope: url:PUT|/api/lti/asset_processor_eulas/:context_external_tool_id/deployment\n  description: Update Eula Deployment Configuration\n  resource: Asset Processor\n  operationId: update_eula_deployment_configuration\n- scope: url:DELETE|/api/lti/asset_processor_eulas/:context_external_tool_id/user\n  description: Delete Eula Acceptances for deployment\n  resource: Asset Processor\n  operationId: delete_eula_acceptances_for_deployment\n- scope: url:POST|/api/lti/asset_processor_eulas/:context_external_tool_id/user\n  description: Create an Eula Acceptance\n  resource: Asset Processor\n  operationId: create_eula_acceptance\n- scope: url:POST|/api/lti/asset_processors/:asset_processor_id/reports\n  description: Create an Asset Report\n  resource: Asset Processor\n  operationId: create_asset_report\n- scope: url:GET|/api/lti/assignments/:assignment_id\n\
  \  description: Get a single assignment (lti)\n  resource: Plagiarism Detection Platform Assignments\n  operationId: get_single_assignment_lti\n- scope: url:GET|/api/lti/assignments/:assignment_id/files/:file_id/originality_report\n  description: Show an Originality Report\n  resource: Originality Reports\n  operationId: show_originality_report_files\n- scope: url:PUT|/api/lti/assignments/:assignment_id/files/:file_id/originality_report\n  description: Edit an Originality Report\n  resource: Originality Reports\n  operationId: edit_originality_report_files\n- scope: url:GET|/api/lti/assignments/:assignment_id/submissions/:submission_id\n  description: Get a single submission\n  resource: Plagiarism Detection Submissions\n  operationId: get_single_submission\n- scope: url:GET|/api/lti/assignments/:assignment_id/submissions/:submission_id/history\n  description: Get the history of a single submission\n  resource: Plagiarism Detection Submissions\n  operationId: get_history_of_single_submission\n\
  - scope: url:POST|/api/lti/assignments/:assignment_id/submissions/:submission_id/originality_report\n  description: Create an Originality Report\n  resource: Originality Reports\n  operationId: create_originality_report\n- scope: url:GET|/api/lti/assignments/:assignment_id/submissions/:submission_id/originality_report/:id\n  description: Show an Originality Report\n  resource: Originality Reports\n  operationId: show_originality_report_submissions\n- scope: url:PUT|/api/lti/assignments/:assignment_id/submissions/:submission_id/originality_report/:id\n  description: Edit an Originality Report\n  resource: Originality Reports\n  operationId: edit_originality_report_submissions\n- scope: url:GET|/api/lti/courses/:course_id/line_items\n  description: List line Items\n  resource: Line Items\n  operationId: list_line_items\n- scope: url:POST|/api/lti/courses/:course_id/line_items\n  description: Create a Line Item\n  resource: Line Items\n  operationId: create_line_item\n- scope: url:DELETE|/api/lti/courses/:course_id/line_items/:id\n\
  \  description: Delete a Line Item\n  resource: Line Items\n  operationId: delete_line_item\n- scope: url:GET|/api/lti/courses/:course_id/line_items/:id\n  description: Show a Line Item\n  resource: Line Items\n  operationId: show_line_item\n- scope: url:PUT|/api/lti/courses/:course_id/line_items/:id\n  description: Update a Line Item\n  resource: Line Items\n  operationId: update_line_item\n- scope: url:GET|/api/lti/courses/:course_id/line_items/:line_item_id/results\n  description: Show a collection of Results\n  resource: Result\n  operationId: show_collection_of_results\n- scope: url:GET|/api/lti/courses/:course_id/line_items/:line_item_id/results/:id\n  description: Show a Result\n  resource: Result\n  operationId: show_result\n- scope: url:POST|/api/lti/courses/:course_id/line_items/:line_item_id/scores\n  description: Create a Score\n  resource: Score\n  operationId: create_score\n- scope: url:GET|/api/lti/courses/:course_id/names_and_roles\n  description: List Course Memberships\n\
  \  resource: Names And Role\n  operationId: list_course_memberships\n- scope: url:GET|/api/lti/courses/:course_id/progress/:id\n  description: Query progress\n  resource: Progress\n  operationId: query_progress_progress\n- scope: url:PUT|/api/lti/developer_key/update_public_jwk\n  description: Update Public JWK\n  resource: Public Jwk\n  operationId: update_public_jwk\n- scope: url:GET|/api/lti/groups/:group_id/names_and_roles\n  description: List Group Memberships\n  resource: Names And Role\n  operationId: list_group_memberships_names_and_role\n- scope: url:GET|/api/lti/groups/:group_id/users\n  description: Get all users in a group (lti)\n  resource: Plagiarism Detection Platform Users\n  operationId: get_all_users_in_group_lti\n- scope: url:GET|/api/lti/notice-handlers/:context_external_tool_id\n  description: Show notice handlers\n  resource: Notice Handlers\n  operationId: show_notice_handlers\n- scope: url:PUT|/api/lti/notice-handlers/:context_external_tool_id\n  description: Set\
  \ notice handler\n  resource: Notice Handlers\n  operationId: set_notice_handler\n- scope: url:GET|/api/lti/subscriptions\n  description: List all Webhook Subscription for a tool proxy\n  resource: Webhooks Subscriptions For Plagiarism Platform\n  operationId: list_all_webhook_subscription_for_tool_proxy\n- scope: url:POST|/api/lti/subscriptions\n  description: Create a Webhook Subscription\n  resource: Webhooks Subscriptions For Plagiarism Platform\n  operationId: create_webhook_subscription\n- scope: url:DELETE|/api/lti/subscriptions/:id\n  description: Delete a Webhook Subscription\n  resource: Webhooks Subscriptions For Plagiarism Platform\n  operationId: delete_webhook_subscription\n- scope: url:GET|/api/lti/subscriptions/:id\n  description: Show a single Webhook Subscription\n  resource: Webhooks Subscriptions For Plagiarism Platform\n  operationId: show_single_webhook_subscription\n- scope: url:PUT|/api/lti/subscriptions/:id\n  description: Update a Webhook Subscription\n  resource:\
  \ Webhooks Subscriptions For Plagiarism Platform\n  operationId: update_webhook_subscription\n- scope: url:GET|/api/lti/users/:id\n  description: Get a single user (lti)\n  resource: Plagiarism Detection Platform Users\n  operationId: get_single_user_lti\n- scope: url:GET|/api/lti/uuid_map\n  description: Download UUID Mapping for this Sandbox\n  resource: Sandboxes\n  operationId: download_uuid_mapping_for_this_sandbox\n- scope: url:POST|/api/quiz/v1/courses/:course_id/accommodations\n  description: Set Course-Level Accommodations\n  resource: New Quizzes Accommodations\n  operationId: set_course_level_accommodations\n- scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes\n  description: List new quizzes\n  resource: New Quizzes\n  operationId: list_new_quizzes\n- scope: url:POST|/api/quiz/v1/courses/:course_id/quizzes\n  description: Create a new quiz\n  resource: New Quizzes\n  operationId: create_new_quiz\n- scope: url:DELETE|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id\n\
  \  description: Delete a new quiz\n  resource: New Quizzes\n  operationId: delete_new_quiz\n- scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id\n  description: Get a new quiz\n  resource: New Quizzes\n  operationId: get_new_quiz\n- scope: url:PATCH|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id\n  description: Update a single quiz\n  resource: New Quizzes\n  operationId: update_single_quiz\n- scope: url:POST|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/accommodations\n  description: Set Quiz-Level Accommodations\n  resource: New Quizzes Accommodations\n  operationId: set_quiz_level_accommodations\n- scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items\n  description: List quiz items\n  resource: New Quiz Items\n  operationId: list_quiz_items\n- scope: url:POST|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items\n  description: Create a quiz item\n  resource: New Quiz Items\n  operationId: create_quiz_item\n- scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/media_upload_url\n\
  \  description: Get items media_upload_url\n  resource: New Quiz Items\n  operationId: get_items_media_upload_url\n- scope: url:DELETE|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/:item_id\n  description: Delete a quiz item\n  resource: New Quiz Items\n  operationId: delete_quiz_item\n- scope: url:GET|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/:item_id\n  description: Get a quiz item\n  resource: New Quiz Items\n  operationId: get_quiz_item\n- scope: url:PATCH|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/items/:item_id\n  description: Update a quiz item\n  resource: New Quiz Items\n  operationId: update_quiz_item\n- scope: url:POST|/api/quiz/v1/courses/:course_id/quizzes/:assignment_id/reports\n  description: Create a quiz report\n  resource: New Quizzes Reports\n  operationId: create_quiz_report\n- scope: url:GET|/api/sis/accounts/:account_id/assignments\n  description: Retrieve assignments enabled for grade export to SIS\n  resource: Sis Integration\n\
  \  operationId: retrieve_assignments_enabled_for_grade_export_to_sis_accounts\n- scope: url:GET|/api/sis/courses/:course_id/assignments\n  description: Retrieve assignments enabled for grade export to SIS\n  resource: Sis Integration\n  operationId: retrieve_assignments_enabled_for_grade_export_to_sis_courses\n- scope: url:PUT|/api/sis/courses/:course_id/disable_post_to_sis\n  description: Disable assignments currently enabled for grade export to SIS\n  resource: Sis Integration\n  operationId: disable_assignments_currently_enabled_for_grade_export_to_sis\n- scope: url:GET|/api/v1/account_calendars\n  description: List available account calendars\n  resource: Account Calendars\n  operationId: list_available_account_calendars\n- scope: url:GET|/api/v1/account_calendars/:account_id\n  description: Get a single account calendar\n  resource: Account Calendars\n  operationId: get_single_account_calendar\n- scope: url:PUT|/api/v1/account_calendars/:account_id\n  description: Update a calendar\n\
  \  resource: Account Calendars\n  operationId: update_calendar\n- scope: url:GET|/api/v1/accounts\n  description: List accounts\n  resource: Accounts\n  operationId: list_accounts\n- scope: url:GET|/api/v1/accounts/search\n  description: Search account domains\n  resource: Account Domain Lookups\n  operationId: search_account_domains\n- scope: url:GET|/api/v1/accounts/:account_id/account_calendars\n  description: List all account calendars\n  resource: Account Calendars\n  operationId: list_all_account_calendars\n- scope: url:PUT|/api/v1/accounts/:account_id/account_calendars\n  description: Update several calendars\n  resource: Account Calendars\n  operationId: update_several_calendars\n- scope: url:GET|/api/v1/accounts/:account_id/account_notifications\n  description: Index of active global notification for the user\n  resource: Account Notifications\n  operationId: index_of_active_global_notification_for_user\n- scope: url:POST|/api/v1/accounts/:account_id/account_notifications\n  description:\
  \ Create a global notification\n  resource: Account Notifications\n  operationId: create_global_notification\n- scope: url:DELETE|/api/v1/accounts/:account_id/account_notifications/:id\n  description: Close notification for user. Destroy notification for admin\n  resource: Account Notifications\n  operationId: close_notification_for_user_destroy_notification_for_admin\n- scope: url:GET|/api/v1/accounts/:account_id/account_notifications/:id\n  description: Show a global notification\n  resource: Account Notifications\n  operationId: show_global_notification\n- scope: url:PUT|/api/v1/accounts/:account_id/account_notifications/:id\n  description: Update a global notification\n  resource: Account Notifications\n  operationId: update_global_notification\n- scope: url:GET|/api/v1/accounts/:account_id/admins\n  description: List account admins\n  resource: Admins\n  operationId: list_account_admins\n- scope: url:POST|/api/v1/accounts/:account_id/admins\n  description: Make an account admin\n\
  \  resource: Admins\n  operationId: make_account_admin\n- scope: url:GET|/api/v1/accounts/:account_id/admins/self\n  description: List my admin roles\n  resource: Admins\n  operationId: list_my_admin_roles\n- scope: url:DELETE|/api/v1/accounts/:account_id/admins/:user_id\n  description: Remove account admin\n  resource: Admins\n  operationId: remove_account_admin\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/completed/activity\n  description: Get department-level participation data\n  resource: Analytics\n  operationId: get_department_level_participation_data_completed\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/completed/grades\n  description: Get department-level grade data\n  resource: Analytics\n  operationId: get_department_level_grade_data_completed\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/completed/statistics\n  description: Get department-level statistics\n  resource: Analytics\n  operationId: get_department_level_statistics_completed\n-\
  \ scope: url:GET|/api/v1/accounts/:account_id/analytics/completed/statistics_by_subaccount\n  description: Get department-level statistics, broken down by subaccount\n  resource: Analytics\n  operationId: get_department_level_statistics_broken_down_by_subaccount_completed\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/current/activity\n  description: Get department-level participation data\n  resource: Analytics\n  operationId: get_department_level_participation_data_current\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/current/grades\n  description: Get department-level grade data\n  resource: Analytics\n  operationId: get_department_level_grade_data_current\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/current/statistics\n  description: Get department-level statistics\n  resource: Analytics\n  operationId: get_department_level_statistics_current\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/current/statistics_by_subaccount\n  description: Get\
  \ department-level statistics, broken down by subaccount\n  resource: Analytics\n  operationId: get_department_level_statistics_broken_down_by_subaccount_current\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/activity\n  description: Get department-level participation data\n  resource: Analytics\n  operationId: get_department_level_participation_data_terms\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/grades\n  description: Get department-level grade data\n  resource: Analytics\n  operationId: get_department_level_grade_data_terms\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/statistics\n  description: Get department-level statistics\n  resource: Analytics\n  operationId: get_department_level_statistics_terms\n- scope: url:GET|/api/v1/accounts/:account_id/analytics/terms/:term_id/statistics_by_subaccount\n  description: Get department-level statistics, broken down by subaccount\n  resource: Analytics\n  operationId:\
  \ get_department_level_statistics_broken_down_by_subaccount_terms\n- scope: url:GET|/api/v1/accounts/:account_id/app_by_client_id/:client_id\n  description: Show an LTI Registration (via the client_id)\n  resource: Lti Registrations\n  operationId: show_lti_registration_via_client_id_app_by_client_id\n- scope: url:GET|/api/v1/accounts/:account_id/apps\n  description: List LTI Registrations in an account\n  resource: Lti Registrations\n  operationId: list_lti_registrations_in_account_apps\n- scope: url:POST|/api/v1/accounts/:account_id/apps\n  description: Create an LTI Registration\n  resource: Lti Registrations\n  operationId: create_lti_registration_apps\n- scope: url:GET|/api/v1/accounts/:account_id/apps/by_utid/:utid\n  description: Get LTI Registration by Unified Tool ID\n  resource: Lti Registrations\n  operationId: get_lti_registration_by_unified_tool_id_apps\n- scope: url:GET|/api/v1/accounts/:account_id/apps/install_status/:client_id\n  description: Check LTI Registration Install\
  \ Status\n  resource: Lti Registrations\n  operationId: check_lti_registration_install_status_apps\n- scope: url:DELETE|/api/v1/accounts/:account_id/apps/:id\n  description: Delete an LTI Registration\n  resource: Lti Registrations\n  operationId: delete_lti_registration_apps\n- scope: url:GET|/api/v1/accounts/:account_id/apps/:id\n  description: Show an LTI Registration\n  resource: Lti Registrations\n  operationId: show_lti_registration_apps\n- scope: url:PUT|/api/v1/accounts/:account_id/apps/:id\n  description: Update an LTI Registration\n  resource: Lti Registrations\n  operationId: update_lti_registration_apps\n- scope: url:DELETE|/api/v1/accounts/:account_id/apps/:id/bind\n  description: Remove an Inherited LTI Registration\n  resource: Lti Registrations\n  operationId: remove_inherited_lti_registration_apps\n- scope: url:POST|/api/v1/accounts/:account_id/apps/:id/bind\n  description: Bind an LTI Registration to a Root Account\n  resource: Lti Registrations\n  operationId: bind_lti_registration_to_root_account_apps\n\
  - scope: url:GET|/api/v1/accounts/:account_id/apps/:id/history\n  description: Get LTI Registration History\n  resource: Lti Registrations\n  operationId: get_lti_registration_history_apps\n- scope: url:POST|/api/v1/accounts/:account_id/apps/:id/install_from_template\n  description: Install an LTI Registration from a Template\n  resource: Lti Registrations\n  operationId: install_lti_registration_from_template_apps\n- scope: url:GET|/api/v1/accounts/:account_id/apps/:id/latest_update_request\n  description: Get Latest LTI Registration Update Request\n  resource: Lti Registrations\n  operationId: get_latest_lti_registration_update_request_apps\n- scope: url:GET|/api/v1/accounts/:account_id/apps/:id/overlay_history\n  description: Get LTI Registration Overlay History\n  resource: Lti Registrations\n  operationId: get_lti_registration_overlay_history_apps\n- scope: url:PUT|/api/v1/accounts/:account_id/apps/:id/reset\n  description: Reset an LTI Registration to Defaults\n  resource: Lti Registrations\n\
  \  operationId: reset_lti_registration_to_defaults_apps\n- scope: url:GET|/api/v1/accounts/:account_id/apps/:id/update_requests/:update_request_id\n  description: Get LTI Registration Update Request\n  resource: Lti Registrations\n  operationId: get_lti_registration_update_request_apps\n- scope: url:PUT|/api/v1/accounts/:account_id/apps/:id/update_requests/:update_request_id/apply\n  description: Apply LTI Registration Update Requst\n  resource: Lti Registrations\n  operationId: apply_lti_registration_update_requst_apps\n- scope: url:GET|/api/v1/accounts/:account_id/apps/:registration_id/deployments/:deployment_id/context_search\n  description: Search for Accounts and Courses\n  resource: Lti Registrations\n  operationId: search_for_accounts_and_courses_apps\n- scope: url:GET|/api/v1/accounts/:account_id/authentication_providers\n  description: List authentication providers\n  resource: Authentication Providers\n  operationId: list_authentication_providers\n- scope: url:POST|/api/v1/accounts/:account_id/authentication_providers\n\
  \  description: Add authentication provider\n  resource: Authentication Providers\n  operationId: add_authentication_provider\n- scope: url:POST|/api/v1/accounts/:account_id/authentication_providers/force_password_reset\n  description: Force password reset\n  resource: Authentication Providers\n  operationId: force_password_reset\n- scope: url:DELETE|/api/v1/accounts/:account_id/authentication_providers/:id\n  description: Delete authentication provider\n  resource: Authentication Providers\n  operationId: delete_authentication_provider\n- scope: url:GET|/api/v1/accounts/:account_id/authentication_providers/:id\n  description: Get authentication provider\n  resource: Authentication Providers\n  operationId: get_authentication_provider\n- scope: url:PUT|/api/v1/accounts/:account_id/authentication_providers/:id\n  description: Update authentication provider\n  resource: Authentication Providers\n  operationId: update_authentication_provider\n- scope: url:PUT|/api/v1/accounts/:account_id/authentication_providers/:id/restore\n\
  \  description: Restore a deleted authentication provider\n  resource: Authentication Providers\n  operationId: restore_deleted_authentication_provider\n- scope: url:GET|/api/v1/accounts/:account_id/blackout_dates\n  description: List blackout dates\n  resource: Blackout Dates\n  operationId: list_blackout_dates_accounts\n- scope: url:POST|/api/v1/accounts/:account_id/blackout_dates\n  description: Create Blackout Date\n  resource: Blackout Dates\n  operationId: create_blackout_date_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/blackout_dates/new\n  description: New Blackout Date\n  resource: Blackout Dates\n  operationId: new_blackout_date_accounts\n- scope: url:DELETE|/api/v1/accounts/:account_id/blackout_dates/:id\n  description: Delete Blackout Date\n  resource: Blackout Dates\n  operationId: delete_blackout_date_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/blackout_dates/:id\n  description: Get a single blackout date\n  resource: Blackout Dates\n  operationId:\
  \ get_single_blackout_date_accounts\n- scope: url:PUT|/api/v1/accounts/:account_id/blackout_dates/:id\n  description: Update Blackout Date\n  resource: Blackout Dates\n  operationId: update_blackout_date_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/brand_variables\n  description: Get the brand config variables for a sub-account or course\n  resource: Brand Configs\n  operationId: get_brand_config_variables_for_sub_account_or_course_accounts\n- scope: url:POST|/api/v1/accounts/:account_id/bulk_enrollment\n  description: Enroll multiple users to one or more courses\n  resource: Enrollments\n  operationId: enroll_multiple_users_to_one_or_more_courses\n- scope: url:GET|/api/v1/accounts/:account_id/content_migrations\n  description: List content migrations\n  resource: Content Migrations\n  operationId: list_content_migrations_accounts\n- scope: url:POST|/api/v1/accounts/:account_id/content_migrations\n  description: Create a content migration\n  resource: Content Migrations\n  operationId:\
  \ create_content_migration_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/content_migrations/migrators\n  description: List Migration Systems\n  resource: Content Migrations\n  operationId: list_migration_systems_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/content_migrations/:content_migration_id/migration_issues\n  description: List migration issues\n  resource: Content Migrations\n  operationId: list_migration_issues_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/content_migrations/:content_migration_id/migration_issues/:id\n  description: Get a migration issue\n  resource: Content Migrations\n  operationId: get_migration_issue_accounts\n- scope: url:PUT|/api/v1/accounts/:account_id/content_migrations/:content_migration_id/migration_issues/:id\n  description: Update a migration issue\n  resource: Content Migrations\n  operationId: update_migration_issue_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/content_migrations/:id\n  description: Get a content\
  \ migration\n  resource: Content Migrations\n  operationId: get_content_migration_accounts\n- scope: url:PUT|/api/v1/accounts/:account_id/content_migrations/:id\n  description: Update a content migration\n  resource: Content Migrations\n  operationId: update_content_migration_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/content_migrations/:id/selective_data\n  description: List items for selective import\n  resource: Content Migrations\n  operationId: list_items_for_selective_import_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/courses\n  description: List active courses in an account\n  resource: Accounts\n  operationId: list_active_courses_in_account\n- scope: url:POST|/api/v1/accounts/:account_id/courses\n  description: Create a new course\n  resource: Courses\n  operationId: create_new_course\n- scope: url:PUT|/api/v1/accounts/:account_id/courses\n  description: Update courses\n  resource: Courses\n  operationId: update_courses\n- scope: url:GET|/api/v1/accounts/:account_id/courses/:id\n\
  \  description: Get a single course\n  resource: Courses\n  operationId: get_single_course_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/csp_settings\n  description: Get current settings for account or course\n  resource: Content Security Policy Settings\n  operationId: get_current_settings_for_account_or_course_accounts\n- scope: url:PUT|/api/v1/accounts/:account_id/csp_settings\n  description: Enable, disable, or clear explicit CSP setting\n  resource: Content Security Policy Settings\n  operationId: enable_disable_or_clear_explicit_csp_setting_accounts\n- scope: url:DELETE|/api/v1/accounts/:account_id/csp_settings/domains\n  description: Remove a domain from account\n  resource: Content Security Policy Settings\n  operationId: remove_domain_from_account\n- scope: url:POST|/api/v1/accounts/:account_id/csp_settings/domains\n  description: Add an allowed domain to account\n  resource: Content Security Policy Settings\n  operationId: add_allowed_domain_to_account\n- scope: url:POST|/api/v1/accounts/:account_id/csp_settings/domains/batch_create\n\
  \  description: Add multiple allowed domains to an account\n  resource: Content Security Policy Settings\n  operationId: add_multiple_allowed_domains_to_account\n- scope: url:PUT|/api/v1/accounts/:account_id/csp_settings/lock\n  description: Lock or unlock current CSP settings for sub-accounts and courses\n  resource: Content Security Policy Settings\n  operationId: lock_or_unlock_current_csp_settings_for_sub_accounts_and_courses\n- scope: url:GET|/api/v1/accounts/:account_id/developer_keys\n  description: List Developer Keys\n  resource: Developer Keys\n  operationId: list_developer_keys\n- scope: url:POST|/api/v1/accounts/:account_id/developer_keys\n  description: Create a Developer Key\n  resource: Developer Keys\n  operationId: create_developer_key\n- scope: url:POST|/api/v1/accounts/:account_id/developer_keys/:developer_key_id/developer_key_account_bindings\n  description: Create a Developer Key Account Binding\n  resource: Developer Key Account Bindings\n  operationId: create_developer_key_account_binding\n\
  - scope: url:GET|/api/v1/accounts/:account_id/enrollments/:id\n  description: Enrollment by ID\n  resource: Enrollments\n  operationId: enrollment_by_id\n- scope: url:GET|/api/v1/accounts/:account_id/external_tools\n  description: List external tools\n  resource: External Tools\n  operationId: list_external_tools_accounts\n- scope: url:POST|/api/v1/accounts/:account_id/external_tools\n  description: Create an external tool\n  resource: External Tools\n  operationId: create_external_tool_accounts\n- scope: url:DELETE|/api/v1/accounts/:account_id/external_tools/rce_favorites/:id\n  description: Unmark tool as RCE Favorite\n  resource: External Tools\n  operationId: unmark_tool_as_rce_favorite\n- scope: url:POST|/api/v1/accounts/:account_id/external_tools/rce_favorites/:id\n  description: Mark tool as RCE Favorite\n  resource: External Tools\n  operationId: mark_tool_as_rce_favorite\n- scope: url:GET|/api/v1/accounts/:account_id/external_tools/sessionless_launch\n  description: Get a sessionless\
  \ launch url for an external tool.\n  resource: External Tools\n  operationId: get_sessionless_launch_url_for_external_tool_accounts\n- scope: url:DELETE|/api/v1/accounts/:account_id/external_tools/top_nav_favorites/:id\n  description: Remove tool from Top Navigation Favorites\n  resource: External Tools\n  operationId: remove_tool_from_top_navigation_favorites\n- scope: url:POST|/api/v1/accounts/:account_id/external_tools/top_nav_favorites/:id\n  description: Add tool to Top Navigation Favorites\n  resource: External Tools\n  operationId: add_tool_to_top_navigation_favorites\n- scope: url:DELETE|/api/v1/accounts/:account_id/external_tools/:external_tool_id\n  description: Delete an external tool\n  resource: External Tools\n  operationId: delete_external_tool_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/external_tools/:external_tool_id\n  description: Get a single external tool\n  resource: External Tools\n  operationId: get_single_external_tool_accounts\n- scope: url:PUT|/api/v1/accounts/:account_id/external_tools/:external_tool_id\n\
  \  description: Edit an external tool\n  resource: External Tools\n  operationId: edit_external_tool_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/features\n  description: List features\n  resource: Feature Flags\n  operationId: list_features_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/features/enabled\n  description: List enabled features\n  resource: Feature Flags\n  operationId: list_enabled_features_accounts\n- scope: url:DELETE|/api/v1/accounts/:account_id/features/flags/:feature\n  description: Remove feature flag\n  resource: Feature Flags\n  operationId: remove_feature_flag_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/features/flags/:feature\n  description: Get feature flag\n  resource: Feature Flags\n  operationId: get_feature_flag_accounts\n- scope: url:PUT|/api/v1/accounts/:account_id/features/flags/:feature\n  description: Set feature flag\n  resource: Feature Flags\n  operationId: set_feature_flag_accounts\n- scope: url:POST|/api/v1/accounts/:account_id/folders\n\
  \  description: Create folder\n  resource: Files\n  operationId: create_folder_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/grading_period_sets\n  description: List grading period sets\n  resource: Grading Period Sets\n  operationId: list_grading_period_sets\n- scope: url:POST|/api/v1/accounts/:account_id/grading_period_sets\n  description: Create a grading period set\n  resource: Grading Period Sets\n  operationId: create_grading_period_set\n- scope: url:DELETE|/api/v1/accounts/:account_id/grading_period_sets/:id\n  description: Delete a grading period set\n  resource: Grading Period Sets\n  operationId: delete_grading_period_set\n- scope: url:PATCH|/api/v1/accounts/:account_id/grading_period_sets/:id\n  description: Update a grading period set\n  resource: Grading Period Sets\n  operationId: update_grading_period_set\n- scope: url:GET|/api/v1/accounts/:account_id/grading_periods\n  description: List grading periods\n  resource: Grading Periods\n  operationId: list_grading_periods_accounts\n\
  - scope: url:DELETE|/api/v1/accounts/:account_id/grading_periods/:id\n  description: Delete a grading period\n  resource: Grading Periods\n  operationId: delete_grading_period_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/grading_standards\n  description: List the grading standards available in a context.\n  resource: Grading Standards\n  operationId: list_grading_standards_available_in_context_accounts\n- scope: url:POST|/api/v1/accounts/:account_id/grading_standards\n  description: Create a new grading standard\n  resource: Grading Standards\n  operationId: create_new_grading_standard_accounts\n- scope: url:DELETE|/api/v1/accounts/:account_id/grading_standards/:grading_standard_id\n  description: Delete a grading standard\n  resource: Grading Standards\n  operationId: delete_grading_standard_accounts\n- scope: url:GET|/api/v1/accounts/:account_id/\n\n# --- truncated at 32 KB (198 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/canvas/refs/heads/main/scopes/canvas-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas/refs/heads/main/scopes/canvas-scopes.yml
summary_line: 1117 scopes · authorizationCode
tags:
- Education
- EdTech
- GraphQL
- Learning Management System
- LMS
- LTI
- Open-Source
- REST
token_urls:
- https://canvas.instructure.com/login/oauth2/token
---
