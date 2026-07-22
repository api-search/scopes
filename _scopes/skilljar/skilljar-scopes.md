---
api_specs:
- filename: skilljar-openapi-original.yml
  format: yaml
  label: Skilljar API
  slug: skilljar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skilljar/refs/heads/main/openapi/skilljar-openapi-original.yml
authorization_urls:
- https://dashboard.skilljar.com/oauth/authorize
description: ''
docs: https://support.gainsight.com/Skilljar/Develop_and_Customize/API
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Skilljar Scopes
name_suffix: OAuth Scopes
note: Scopes harvested from the RFC 8414 OAuth 2.0 Authorization Server Metadata document. Applies to the Skilljar v2 OAuth API (authorization_code + refresh_token, PKCE S256). The v1 API uses HTTP Basic API-key auth and is not scope-gated.
overview: 'Skilljar publishes 89 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Skilljar API on a user''s behalf.


  Tokens are issued from https://api.skilljar.com/v2/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Skilljar
provider_slug: skilljar
schemes:
- flows:
  - authorizationUrl: https://dashboard.skilljar.com/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    refreshUrl: https://api.skilljar.com/v2/auth/token
    tokenUrl: https://api.skilljar.com/v2/auth/token
  jwks_uri: https://api.skilljar.com/.well-known/jwks.json
  name: OAuth2
  registration_endpoint: https://api.skilljar.com/v2/oauth/register
  revocation_endpoint: https://api.skilljar.com/v2/auth/revoke
  source: https://api.skilljar.com
scope_count: 89
scope_names:
- courses:read
- courses:write
- lessons:read
- lessons:write
- assets:read
- assets:write
- quizzes:read
- quizzes:write
- question-banks:read
- question-banks:write
- web-packages:read
- web-packages:write
- content-items:read
- content-items:write
- labels:read
- labels:write
- instructors:read
- instructors:write
- course-families:read
- course-families:write
- domains:read
- domains:write
- published-courses:read
- published-courses:write
- catalog-pages:read
- catalog-pages:write
- paths:read
- paths:write
- plans:read
- plans:write
- tags:read
- tags:write
- themes:read
- themes:write
- enrollments:read
- enrollments:write
- students:read
- students:write
- students:deactivate
- students:anonymize
- students:manage-password
- signup-fields:read
- student-groups:read
- student-groups:write
- certificates:read
- certificates:write
- email-templates:read
- email-templates:write
- language-packs:read
- language-packs:write
- admin-users:read
- admin-users:write
- roles:read
- roles:write
- analytics:read
- audit:read
- promo-codes:read
- promo-codes:write
- training-credits:read
- training-credits:write
- licensing:read
- licensing:write
- offers:read
- offers:write
- orders:read
- access-codes:read
- access-codes:write
- vilt-sessions:read
- vilt-sessions:write
- scheduled-reports:read
- scheduled-reports:write
- data-export:read
- data-export:write
- workflows:read
- workflows:write
- syndication:read
- syndication:write
- announcements:read
- announcements:write
- action-items:read
- action-items:write
- organization:read
- organization:write
- webhooks:read
- webhooks:write
- integrations:read
- integrations:write
- clients:read
- clients:write
scopes:
- description: Read access to courses
  flows:
  - authorizationCode
  scope: courses:read
- description: Write access to courses
  flows:
  - authorizationCode
  scope: courses:write
- description: Read access to lessons
  flows:
  - authorizationCode
  scope: lessons:read
- description: Write access to lessons
  flows:
  - authorizationCode
  scope: lessons:write
- description: Read access to assets
  flows:
  - authorizationCode
  scope: assets:read
- description: Write access to assets
  flows:
  - authorizationCode
  scope: assets:write
- description: Read access to quizzes
  flows:
  - authorizationCode
  scope: quizzes:read
- description: Write access to quizzes
  flows:
  - authorizationCode
  scope: quizzes:write
- description: Read access to question banks
  flows:
  - authorizationCode
  scope: question-banks:read
- description: Write access to question banks
  flows:
  - authorizationCode
  scope: question-banks:write
- description: Read access to web packages
  flows:
  - authorizationCode
  scope: web-packages:read
- description: Write access to web packages
  flows:
  - authorizationCode
  scope: web-packages:write
- description: Read access to content items
  flows:
  - authorizationCode
  scope: content-items:read
- description: Write access to content items
  flows:
  - authorizationCode
  scope: content-items:write
- description: Read access to labels
  flows:
  - authorizationCode
  scope: labels:read
- description: Write access to labels
  flows:
  - authorizationCode
  scope: labels:write
- description: Read access to instructors
  flows:
  - authorizationCode
  scope: instructors:read
- description: Write access to instructors
  flows:
  - authorizationCode
  scope: instructors:write
- description: Read access to course families
  flows:
  - authorizationCode
  scope: course-families:read
- description: Write access to course families
  flows:
  - authorizationCode
  scope: course-families:write
- description: Read access to domains
  flows:
  - authorizationCode
  scope: domains:read
- description: Write access to domains
  flows:
  - authorizationCode
  scope: domains:write
- description: Read access to published courses
  flows:
  - authorizationCode
  scope: published-courses:read
- description: Write access to published courses
  flows:
  - authorizationCode
  scope: published-courses:write
- description: Read access to catalog pages
  flows:
  - authorizationCode
  scope: catalog-pages:read
- description: Write access to catalog pages
  flows:
  - authorizationCode
  scope: catalog-pages:write
- description: Read access to paths
  flows:
  - authorizationCode
  scope: paths:read
- description: Write access to paths
  flows:
  - authorizationCode
  scope: paths:write
- description: Read access to plans
  flows:
  - authorizationCode
  scope: plans:read
- description: Write access to plans
  flows:
  - authorizationCode
  scope: plans:write
- description: Read access to tags
  flows:
  - authorizationCode
  scope: tags:read
- description: Write access to tags
  flows:
  - authorizationCode
  scope: tags:write
- description: Read access to themes
  flows:
  - authorizationCode
  scope: themes:read
- description: Write access to themes
  flows:
  - authorizationCode
  scope: themes:write
- description: Read access to enrollments
  flows:
  - authorizationCode
  scope: enrollments:read
- description: Write access to enrollments
  flows:
  - authorizationCode
  scope: enrollments:write
- description: Read access to students
  flows:
  - authorizationCode
  scope: students:read
- description: Write access to students
  flows:
  - authorizationCode
  scope: students:write
- description: Deactivate students
  flows:
  - authorizationCode
  scope: students:deactivate
- description: Anonymize students
  flows:
  - authorizationCode
  scope: students:anonymize
- description: Manage students passwords
  flows:
  - authorizationCode
  scope: students:manage-password
- description: Read access to signup fields
  flows:
  - authorizationCode
  scope: signup-fields:read
- description: Read access to student groups
  flows:
  - authorizationCode
  scope: student-groups:read
- description: Write access to student groups
  flows:
  - authorizationCode
  scope: student-groups:write
- description: Read access to certificates
  flows:
  - authorizationCode
  scope: certificates:read
- description: Write access to certificates
  flows:
  - authorizationCode
  scope: certificates:write
- description: Read access to email templates
  flows:
  - authorizationCode
  scope: email-templates:read
- description: Write access to email templates
  flows:
  - authorizationCode
  scope: email-templates:write
- description: Read access to language packs
  flows:
  - authorizationCode
  scope: language-packs:read
- description: Write access to language packs
  flows:
  - authorizationCode
  scope: language-packs:write
- description: Read access to admin users
  flows:
  - authorizationCode
  scope: admin-users:read
- description: Write access to admin users
  flows:
  - authorizationCode
  scope: admin-users:write
- description: Read access to roles
  flows:
  - authorizationCode
  scope: roles:read
- description: Write access to roles
  flows:
  - authorizationCode
  scope: roles:write
- description: Read access to analytics
  flows:
  - authorizationCode
  scope: analytics:read
- description: Read access to audit
  flows:
  - authorizationCode
  scope: audit:read
- description: Read access to promo codes
  flows:
  - authorizationCode
  scope: promo-codes:read
- description: Write access to promo codes
  flows:
  - authorizationCode
  scope: promo-codes:write
- description: Read access to training credits
  flows:
  - authorizationCode
  scope: training-credits:read
- description: Write access to training credits
  flows:
  - authorizationCode
  scope: training-credits:write
- description: Read access to licensing
  flows:
  - authorizationCode
  scope: licensing:read
- description: Write access to licensing
  flows:
  - authorizationCode
  scope: licensing:write
- description: Read access to offers
  flows:
  - authorizationCode
  scope: offers:read
- description: Write access to offers
  flows:
  - authorizationCode
  scope: offers:write
- description: Read access to orders
  flows:
  - authorizationCode
  scope: orders:read
- description: Read access to access codes
  flows:
  - authorizationCode
  scope: access-codes:read
- description: Write access to access codes
  flows:
  - authorizationCode
  scope: access-codes:write
- description: Read access to vilt sessions
  flows:
  - authorizationCode
  scope: vilt-sessions:read
- description: Write access to vilt sessions
  flows:
  - authorizationCode
  scope: vilt-sessions:write
- description: Read access to scheduled reports
  flows:
  - authorizationCode
  scope: scheduled-reports:read
- description: Write access to scheduled reports
  flows:
  - authorizationCode
  scope: scheduled-reports:write
- description: Read access to data export
  flows:
  - authorizationCode
  scope: data-export:read
- description: Write access to data export
  flows:
  - authorizationCode
  scope: data-export:write
- description: Read access to workflows
  flows:
  - authorizationCode
  scope: workflows:read
- description: Write access to workflows
  flows:
  - authorizationCode
  scope: workflows:write
- description: Read access to syndication
  flows:
  - authorizationCode
  scope: syndication:read
- description: Write access to syndication
  flows:
  - authorizationCode
  scope: syndication:write
- description: Read access to announcements
  flows:
  - authorizationCode
  scope: announcements:read
- description: Write access to announcements
  flows:
  - authorizationCode
  scope: announcements:write
- description: Read access to action items
  flows:
  - authorizationCode
  scope: action-items:read
- description: Write access to action items
  flows:
  - authorizationCode
  scope: action-items:write
- description: Read access to organization
  flows:
  - authorizationCode
  scope: organization:read
- description: Write access to organization
  flows:
  - authorizationCode
  scope: organization:write
- description: Read access to webhooks
  flows:
  - authorizationCode
  scope: webhooks:read
- description: Write access to webhooks
  flows:
  - authorizationCode
  scope: webhooks:write
- description: Read access to integrations
  flows:
  - authorizationCode
  scope: integrations:read
- description: Write access to integrations
  flows:
  - authorizationCode
  scope: integrations:write
- description: Read access to clients
  flows:
  - authorizationCode
  scope: clients:read
- description: Write access to clients
  flows:
  - authorizationCode
  scope: clients:write
slug: skilljar-scopes
source_filename: skilljar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.skilljar.com/.well-known/oauth-authorization-server\ndocs: https://support.gainsight.com/Skilljar/Develop_and_Customize/API\nnote: Scopes harvested from the RFC 8414 OAuth 2.0 Authorization Server Metadata document. Applies to\n  the Skilljar v2 OAuth API (authorization_code + refresh_token, PKCE S256). The v1 API uses HTTP Basic\n  API-key auth and is not scope-gated.\nschemes:\n- name: OAuth2\n  source: https://api.skilljar.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dashboard.skilljar.com/oauth/authorize\n    tokenUrl: https://api.skilljar.com/v2/auth/token\n    refreshUrl: https://api.skilljar.com/v2/auth/token\n    pkce: S256\n    grant_types:\n    - authorization_code\n    - refresh_token\n  registration_endpoint: https://api.skilljar.com/v2/oauth/register\n  revocation_endpoint: https://api.skilljar.com/v2/auth/revoke\n  jwks_uri: https://api.skilljar.com/.well-known/jwks.json\n\
  scopes:\n- scope: courses:read\n  description: Read access to courses\n  flows:\n  - authorizationCode\n- scope: courses:write\n  description: Write access to courses\n  flows:\n  - authorizationCode\n- scope: lessons:read\n  description: Read access to lessons\n  flows:\n  - authorizationCode\n- scope: lessons:write\n  description: Write access to lessons\n  flows:\n  - authorizationCode\n- scope: assets:read\n  description: Read access to assets\n  flows:\n  - authorizationCode\n- scope: assets:write\n  description: Write access to assets\n  flows:\n  - authorizationCode\n- scope: quizzes:read\n  description: Read access to quizzes\n  flows:\n  - authorizationCode\n- scope: quizzes:write\n  description: Write access to quizzes\n  flows:\n  - authorizationCode\n- scope: question-banks:read\n  description: Read access to question banks\n  flows:\n  - authorizationCode\n- scope: question-banks:write\n  description: Write access to question banks\n  flows:\n  - authorizationCode\n- scope:\
  \ web-packages:read\n  description: Read access to web packages\n  flows:\n  - authorizationCode\n- scope: web-packages:write\n  description: Write access to web packages\n  flows:\n  - authorizationCode\n- scope: content-items:read\n  description: Read access to content items\n  flows:\n  - authorizationCode\n- scope: content-items:write\n  description: Write access to content items\n  flows:\n  - authorizationCode\n- scope: labels:read\n  description: Read access to labels\n  flows:\n  - authorizationCode\n- scope: labels:write\n  description: Write access to labels\n  flows:\n  - authorizationCode\n- scope: instructors:read\n  description: Read access to instructors\n  flows:\n  - authorizationCode\n- scope: instructors:write\n  description: Write access to instructors\n  flows:\n  - authorizationCode\n- scope: course-families:read\n  description: Read access to course families\n  flows:\n  - authorizationCode\n- scope: course-families:write\n  description: Write access to course families\n\
  \  flows:\n  - authorizationCode\n- scope: domains:read\n  description: Read access to domains\n  flows:\n  - authorizationCode\n- scope: domains:write\n  description: Write access to domains\n  flows:\n  - authorizationCode\n- scope: published-courses:read\n  description: Read access to published courses\n  flows:\n  - authorizationCode\n- scope: published-courses:write\n  description: Write access to published courses\n  flows:\n  - authorizationCode\n- scope: catalog-pages:read\n  description: Read access to catalog pages\n  flows:\n  - authorizationCode\n- scope: catalog-pages:write\n  description: Write access to catalog pages\n  flows:\n  - authorizationCode\n- scope: paths:read\n  description: Read access to paths\n  flows:\n  - authorizationCode\n- scope: paths:write\n  description: Write access to paths\n  flows:\n  - authorizationCode\n- scope: plans:read\n  description: Read access to plans\n  flows:\n  - authorizationCode\n- scope: plans:write\n  description: Write access to\
  \ plans\n  flows:\n  - authorizationCode\n- scope: tags:read\n  description: Read access to tags\n  flows:\n  - authorizationCode\n- scope: tags:write\n  description: Write access to tags\n  flows:\n  - authorizationCode\n- scope: themes:read\n  description: Read access to themes\n  flows:\n  - authorizationCode\n- scope: themes:write\n  description: Write access to themes\n  flows:\n  - authorizationCode\n- scope: enrollments:read\n  description: Read access to enrollments\n  flows:\n  - authorizationCode\n- scope: enrollments:write\n  description: Write access to enrollments\n  flows:\n  - authorizationCode\n- scope: students:read\n  description: Read access to students\n  flows:\n  - authorizationCode\n- scope: students:write\n  description: Write access to students\n  flows:\n  - authorizationCode\n- scope: students:deactivate\n  description: Deactivate students\n  flows:\n  - authorizationCode\n- scope: students:anonymize\n  description: Anonymize students\n  flows:\n  - authorizationCode\n\
  - scope: students:manage-password\n  description: Manage students passwords\n  flows:\n  - authorizationCode\n- scope: signup-fields:read\n  description: Read access to signup fields\n  flows:\n  - authorizationCode\n- scope: student-groups:read\n  description: Read access to student groups\n  flows:\n  - authorizationCode\n- scope: student-groups:write\n  description: Write access to student groups\n  flows:\n  - authorizationCode\n- scope: certificates:read\n  description: Read access to certificates\n  flows:\n  - authorizationCode\n- scope: certificates:write\n  description: Write access to certificates\n  flows:\n  - authorizationCode\n- scope: email-templates:read\n  description: Read access to email templates\n  flows:\n  - authorizationCode\n- scope: email-templates:write\n  description: Write access to email templates\n  flows:\n  - authorizationCode\n- scope: language-packs:read\n  description: Read access to language packs\n  flows:\n  - authorizationCode\n- scope: language-packs:write\n\
  \  description: Write access to language packs\n  flows:\n  - authorizationCode\n- scope: admin-users:read\n  description: Read access to admin users\n  flows:\n  - authorizationCode\n- scope: admin-users:write\n  description: Write access to admin users\n  flows:\n  - authorizationCode\n- scope: roles:read\n  description: Read access to roles\n  flows:\n  - authorizationCode\n- scope: roles:write\n  description: Write access to roles\n  flows:\n  - authorizationCode\n- scope: analytics:read\n  description: Read access to analytics\n  flows:\n  - authorizationCode\n- scope: audit:read\n  description: Read access to audit\n  flows:\n  - authorizationCode\n- scope: promo-codes:read\n  description: Read access to promo codes\n  flows:\n  - authorizationCode\n- scope: promo-codes:write\n  description: Write access to promo codes\n  flows:\n  - authorizationCode\n- scope: training-credits:read\n  description: Read access to training credits\n  flows:\n  - authorizationCode\n- scope: training-credits:write\n\
  \  description: Write access to training credits\n  flows:\n  - authorizationCode\n- scope: licensing:read\n  description: Read access to licensing\n  flows:\n  - authorizationCode\n- scope: licensing:write\n  description: Write access to licensing\n  flows:\n  - authorizationCode\n- scope: offers:read\n  description: Read access to offers\n  flows:\n  - authorizationCode\n- scope: offers:write\n  description: Write access to offers\n  flows:\n  - authorizationCode\n- scope: orders:read\n  description: Read access to orders\n  flows:\n  - authorizationCode\n- scope: access-codes:read\n  description: Read access to access codes\n  flows:\n  - authorizationCode\n- scope: access-codes:write\n  description: Write access to access codes\n  flows:\n  - authorizationCode\n- scope: vilt-sessions:read\n  description: Read access to vilt sessions\n  flows:\n  - authorizationCode\n- scope: vilt-sessions:write\n  description: Write access to vilt sessions\n  flows:\n  - authorizationCode\n- scope:\
  \ scheduled-reports:read\n  description: Read access to scheduled reports\n  flows:\n  - authorizationCode\n- scope: scheduled-reports:write\n  description: Write access to scheduled reports\n  flows:\n  - authorizationCode\n- scope: data-export:read\n  description: Read access to data export\n  flows:\n  - authorizationCode\n- scope: data-export:write\n  description: Write access to data export\n  flows:\n  - authorizationCode\n- scope: workflows:read\n  description: Read access to workflows\n  flows:\n  - authorizationCode\n- scope: workflows:write\n  description: Write access to workflows\n  flows:\n  - authorizationCode\n- scope: syndication:read\n  description: Read access to syndication\n  flows:\n  - authorizationCode\n- scope: syndication:write\n  description: Write access to syndication\n  flows:\n  - authorizationCode\n- scope: announcements:read\n  description: Read access to announcements\n  flows:\n  - authorizationCode\n- scope: announcements:write\n  description: Write access\
  \ to announcements\n  flows:\n  - authorizationCode\n- scope: action-items:read\n  description: Read access to action items\n  flows:\n  - authorizationCode\n- scope: action-items:write\n  description: Write access to action items\n  flows:\n  - authorizationCode\n- scope: organization:read\n  description: Read access to organization\n  flows:\n  - authorizationCode\n- scope: organization:write\n  description: Write access to organization\n  flows:\n  - authorizationCode\n- scope: webhooks:read\n  description: Read access to webhooks\n  flows:\n  - authorizationCode\n- scope: webhooks:write\n  description: Write access to webhooks\n  flows:\n  - authorizationCode\n- scope: integrations:read\n  description: Read access to integrations\n  flows:\n  - authorizationCode\n- scope: integrations:write\n  description: Write access to integrations\n  flows:\n  - authorizationCode\n- scope: clients:read\n  description: Read access to clients\n  flows:\n  - authorizationCode\n- scope: clients:write\n\
  \  description: Write access to clients\n  flows:\n  - authorizationCode\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skilljar/refs/heads/main/scopes/skilljar-scopes.yml
summary_line: 89 scopes · authorizationCode
tags:
- Company
- Education
- Learning Management System
- Customer Education
- Training
- Online Courses
- Certification
- Webhooks
- Enrollment
token_urls:
- https://api.skilljar.com/v2/auth/token
---
