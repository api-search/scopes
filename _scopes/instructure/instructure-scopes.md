---
api_specs:
- filename: canvas.openapi.yaml
  format: yaml
  label: Canvas LMS REST API
  slug: canvas-lms-rest-api
  spec_type: OpenAPI
  url: https://github.com/instructure/canvas-lms/blob/master/public/doc/openapi/canvas.openapi.yaml
- filename: instructure-canvas-lti-openapi.yml
  format: yaml
  label: Canvas LTI 1.3 API
  slug: canvas-lti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-canvas-lti-openapi.yml
authorization_urls:
- https://{canvas_domain}/login/oauth2/auth
description: ''
docs: https://developerdocs.instructure.com/services/canvas/oauth2/file.developer_keys
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Instructure Scopes
name_suffix: OAuth Scopes
note: In addition to the named scopes below, every Canvas REST API endpoint has an auto-generated granular token scope of the form "url:<HTTP verb>|<endpoint path>" (e.g. url:GET|/api/v1/courses); the full list is enumerable via GET /api/v1/accounts/:account_id/scopes and is documented per endpoint at https://developerdocs.instructure.com/services/canvas/resources/api_token_scopes.
overview: 'Instructure publishes 17 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Instructure API on a user''s behalf.


  Tokens are issued from https://{canvas_domain}/login/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Instructure
provider_slug: instructure
schemes:
- description: OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://{canvas_domain}/login/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://{canvas_domain}/login/oauth2/token
  name: oauth2
  source: openapi/instructure-canvas-lti-openapi.yml
scope_count: 17
scope_names:
- /auth/userinfo
- https://purl.imsglobal.org/spec/lti-reg/scope/registration.readonly
- https://purl.imsglobal.org/spec/lti-reg/scope/registration
- https://purl.imsglobal.org/spec/lti-ags/scope/lineitem
- https://purl.imsglobal.org/spec/lti-ags/scope/lineitem.readonly
- https://purl.imsglobal.org/spec/lti-ags/scope/result.readonly
- https://purl.imsglobal.org/spec/lti-ags/scope/score
- https://purl.imsglobal.org/spec/lti-nrps/scope/contextmembership.readonly
- https://purl.imsglobal.org/spec/lti/scope/noticehandlers
- https://purl.imsglobal.org/spec/lti/scope/asset.readonly
- https://purl.imsglobal.org/spec/lti/scope/report
- https://purl.imsglobal.org/spec/lti/scope/eula/user
- https://purl.imsglobal.org/spec/lti/scope/eula/deployment
- https://canvas.instructure.com/lti/public_jwk/scope/update
- https://canvas.instructure.com/lti/account_lookup/scope/show
- https://canvas.instructure.com/lti-ags/progress/scope/show
- https://canvas.instructure.com/lti/page_content/show
scopes:
- description: Allows an application to rely on Canvas for user identity; Canvas returns only the current user's name and id and does not issue an API access token for this scope.
  flows: []
  scope: /auth/userinfo
- description: Can view LTI registrations associated with the tool.
  flows: []
  scope: https://purl.imsglobal.org/spec/lti-reg/scope/registration.readonly
- description: Can send automatic updates to be approved by an Administrator.
  flows: []
  scope: https://purl.imsglobal.org/spec/lti-reg/scope/registration
- description: Can create and view assignment data in the gradebook associated with the tool (LTI Assignment and Grade Services).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti-ags/scope/lineitem
- description: Can view assignment data in the gradebook associated with the tool (LTI Assignment and Grade Services).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti-ags/scope/lineitem.readonly
- description: Can view submission data for assignments associated with the tool (LTI Assignment and Grade Services).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti-ags/scope/result.readonly
- description: Can create and update submission results for assignments associated with the tool (LTI Assignment and Grade Services).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti-ags/scope/score
- description: Can retrieve user data associated with the context the tool is installed in (LTI Names and Role Provisioning Services).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti-nrps/scope/contextmembership.readonly
- description: Can register to receive asynchronous notifications from Canvas (LTI Platform Notification Service).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti/scope/noticehandlers
- description: Can retrieve submissions from Document Processor Assignments (LTI Asset Processor).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti/scope/asset.readonly
- description: Can send reports for Document Processor Assignments (LTI Asset Processor).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti/scope/report
- description: Can track if EULA has been accepted (LTI Asset Processor).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti/scope/eula/user
- description: Can reset EULA acceptance status (LTI Asset Processor).
  flows: []
  scope: https://purl.imsglobal.org/spec/lti/scope/eula/deployment
- description: Can update public jwk for LTI services.
  flows: []
  scope: https://canvas.instructure.com/lti/public_jwk/scope/update
- description: Can lookup Account information.
  flows: []
  scope: https://canvas.instructure.com/lti/account_lookup/scope/show
- description: Can view Progress records associated with the context the tool is installed in.
  flows: []
  scope: https://canvas.instructure.com/lti-ags/progress/scope/show
- description: Can view the content of a page the tool is launched from.
  flows: []
  scope: https://canvas.instructure.com/lti/page_content/show
slug: instructure-scopes
source_filename: instructure-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://developerdocs.instructure.com/services/canvas/oauth2/file.developer_keys\nnote: In addition to the named scopes below, every Canvas REST API endpoint has an\n  auto-generated granular token scope of the form \"url:<HTTP verb>|<endpoint path>\"\n  (e.g. url:GET|/api/v1/courses); the full list is enumerable via GET\n  /api/v1/accounts/:account_id/scopes and is documented per endpoint at\n  https://developerdocs.instructure.com/services/canvas/resources/api_token_scopes.\nsource: openapi/instructure-canvas-lti-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/instructure-canvas-lti-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{canvas_domain}/login/oauth2/auth\n    tokenUrl: https://{canvas_domain}/login/oauth2/token\n  description: OAuth 2.0 authentication\nscopes:\n- scope: /auth/userinfo\n  description: Allows an application to rely on Canvas for user identity; Canvas\n    returns\
  \ only the current user's name and id and does not issue an API access\n    token for this scope.\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/oauth2/file.oauth\n- scope: https://purl.imsglobal.org/spec/lti-reg/scope/registration.readonly\n  description: Can view LTI registrations associated with the tool.\n  sources:\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti-reg/scope/registration\n  description: Can send automatic updates to be approved by an Administrator.\n  sources:\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti-ags/scope/lineitem\n  description: Can create and view assignment data in the gradebook associated with\n    the tool (LTI Assignment and Grade Services).\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.lti_dev_key_config\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n\
  - scope: https://purl.imsglobal.org/spec/lti-ags/scope/lineitem.readonly\n  description: Can view assignment data in the gradebook associated with the tool\n    (LTI Assignment and Grade Services).\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.lti_dev_key_config\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti-ags/scope/result.readonly\n  description: Can view submission data for assignments associated with the tool\n    (LTI Assignment and Grade Services).\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.lti_dev_key_config\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti-ags/scope/score\n  description: Can create and update submission results for assignments associated\n    with the tool (LTI Assignment and Grade Services).\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.lti_dev_key_config\n\
  \  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti-nrps/scope/contextmembership.readonly\n  description: Can retrieve user data associated with the context the tool is installed\n    in (LTI Names and Role Provisioning Services).\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.lti_dev_key_config\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti/scope/noticehandlers\n  description: Can register to receive asynchronous notifications from Canvas (LTI\n    Platform Notification Service).\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.lti_dev_key_config\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti/scope/asset.readonly\n  description: Can retrieve submissions from Document\
  \ Processor Assignments (LTI\n    Asset Processor).\n  sources:\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti/scope/report\n  description: Can send reports for Document Processor Assignments (LTI Asset Processor).\n  sources:\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti/scope/eula/user\n  description: Can track if EULA has been accepted (LTI Asset Processor).\n  sources:\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://purl.imsglobal.org/spec/lti/scope/eula/deployment\n  description: Can reset EULA acceptance status (LTI Asset Processor).\n  sources:\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://canvas.instructure.com/lti/public_jwk/scope/update\n  description: Can update public jwk for LTI services.\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.lti_dev_key_config\n\
  \  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://canvas.instructure.com/lti/account_lookup/scope/show\n  description: Can lookup Account information.\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.registration\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://canvas.instructure.com/lti-ags/progress/scope/show\n  description: Can view Progress records associated with the context the tool is\n    installed in.\n  sources:\n  - https://developerdocs.instructure.com/services/canvas/external-tools/lti/file.registration\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n- scope: https://canvas.instructure.com/lti/page_content/show\n  description: Can view the content of a page the tool is launched from.\n  sources:\n  - https://github.com/instructure/canvas-lms/blob/master/lib/token_scopes.rb\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/scopes/instructure-scopes.yml
summary_line: 17 scopes · authorizationCode
tags:
- EdTech
- Education
- LMS
- Canvas
- Courses
- Enrollments
- Assignments
- Grades
- Discussions
- GraphQL
- LTI
- Learning Management
token_urls:
- https://{canvas_domain}/login/oauth2/token
---
