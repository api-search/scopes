---
api_specs:
- filename: sonde-health-authentication-api-openapi.yml
  format: yaml
  label: Sonde Health Authentication API
  slug: sonde-health-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonde-health/refs/heads/main/openapi/sonde-health-authentication-api-openapi.yml
- filename: sonde-health-platform-api-openapi.yml
  format: yaml
  label: Sonde Health Platform API
  slug: sonde-health-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonde-health/refs/heads/main/openapi/sonde-health-platform-api-openapi.yml
authorization_urls: []
description: ''
docs: https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706931713/Authentication+Scopes
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Sonde Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sonde Health publishes 17 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sonde Health API on a user''s behalf.


  Tokens are issued from https://api.sondeservices.com/platform/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sonde Health
provider_slug: sonde-health
schemes: []
scope_count: 17
scope_names:
- sonde-platform/users.write
- sonde-platform/storage.write
- sonde-platform/storage.read
- sonde-platform/scores.write
- sonde-platform/voice-feature-scores.write
- sonde-platform/voice-feature-scores.read
- sonde-platform/measures.read
- sonde-platform/measures.list
- sonde-platform/questionnaires.read
- sonde-platform/questionnaires.write
- sonde-platform/questionnaire.write
- sonde-platform/questionnaire-responses.write
- sonde-platform/questionnaire-responses.read
- sonde-platform/transcriptions.write
- sonde-platform/transcriptions.read
- sonde-platform/reports.read
- sonde-platform/screening-results.list
scopes:
- description: Permission to create subjects in UserService.
  flows: []
  scope: sonde-platform/users.write
- description: Permission to upload wav files to StorageService.
  flows: []
  scope: sonde-platform/storage.write
- description: Permission to download uploaded files.
  flows: []
  scope: sonde-platform/storage.read
- description: Permission to calculate a score from InferenceService.
  flows: []
  scope: sonde-platform/scores.write
- description: Permission to create a job to infer voice-feature scores for a measure.
  flows: []
  scope: sonde-platform/voice-feature-scores.write
- description: Permission to pull a voice-feature job and to get the voice-feature-scores.
  flows: []
  scope: sonde-platform/voice-feature-scores.read
- description: Permission to read the particular measures permitted to you from MeasureService.
  flows: []
  scope: sonde-platform/measures.read
- description: Permission to list the measures permitted to you from MeasureService.
  flows: []
  scope: sonde-platform/measures.list
- description: Permission to read questionnaire.
  flows: []
  scope: sonde-platform/questionnaires.read
- description: Permission to create a questionnaire.
  flows: []
  scope: sonde-platform/questionnaires.write
- description: Singular variant of the questionnaire-write scope observed in the questionnaire creation docs alongside the plural form.
  flows: []
  scope: sonde-platform/questionnaire.write
- description: Permission to submit responses of questionnaire.
  flows: []
  scope: sonde-platform/questionnaire-responses.write
- description: Permission to read submitted questionnaire responses.
  flows: []
  scope: sonde-platform/questionnaire-responses.read
- description: Permission to create a transcribe job.
  flows: []
  scope: sonde-platform/transcriptions.write
- description: Permission to poll (or read) a transcribe job (or transcript).
  flows: []
  scope: sonde-platform/transcriptions.read
- description: Read screening-result reports.
  flows: []
  scope: sonde-platform/reports.read
- description: List screening results.
  flows: []
  scope: sonde-platform/screening-results.list
slug: sonde-health-scopes
source_filename: sonde-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706931713/Authentication+Scopes\ndocs: https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706931713/Authentication+Scopes\nflow: clientCredentials\ntoken_url: https://api.sondeservices.com/platform/v1/oauth2/token\nallocation: >-\n  \"As per your contract, SondeHealth will allocate authentication scopes to you.\" Scopes\n  are granted at onboarding; a partner cannot self-grant.\nscope_count: 17\nscopes:\n- name: sonde-platform/users.write\n  description: Permission to create subjects in UserService.\n  service: UserService\n- name: sonde-platform/storage.write\n  description: Permission to upload wav files to StorageService.\n  service: StorageService\n- name: sonde-platform/storage.read\n  description: Permission to download uploaded files.\n  service: StorageService\n- name: sonde-platform/scores.write\n  description: Permission to calculate a score from InferenceService.\n\
  \  service: InferenceService\n- name: sonde-platform/voice-feature-scores.write\n  description: Permission to create a job to infer voice-feature scores for a measure.\n  service: InferenceService\n- name: sonde-platform/voice-feature-scores.read\n  description: Permission to pull a voice-feature job and to get the voice-feature-scores.\n  service: InferenceService\n- name: sonde-platform/measures.read\n  description: Permission to read the particular measures permitted to you from MeasureService.\n  service: MeasureService\n- name: sonde-platform/measures.list\n  description: Permission to list the measures permitted to you from MeasureService.\n  service: MeasureService\n- name: sonde-platform/questionnaires.read\n  description: Permission to read questionnaire.\n  service: QuestionnaireManager\n- name: sonde-platform/questionnaires.write\n  description: Permission to create a questionnaire.\n  service: QuestionnaireManager\n  note: Observed in the Partner Questionnaire Creation use\
  \ case.\n- name: sonde-platform/questionnaire.write\n  description: Singular variant of the questionnaire-write scope observed in the questionnaire\n    creation docs alongside the plural form.\n  service: QuestionnaireManager\n  note: Both spellings appear in Sonde's published curl examples; recorded verbatim\n    rather than normalised.\n- name: sonde-platform/questionnaire-responses.write\n  description: Permission to submit responses of questionnaire.\n  service: QuestionnaireManager\n- name: sonde-platform/questionnaire-responses.read\n  description: Permission to read submitted questionnaire responses.\n  service: QuestionnaireManager\n- name: sonde-platform/transcriptions.write\n  description: Permission to create a transcribe job.\n  service: TranscriptionService\n- name: sonde-platform/transcriptions.read\n  description: Permission to poll (or read) a transcribe job (or transcript).\n  service: TranscriptionService\n- name: sonde-platform/reports.read\n  description: Read screening-result\
  \ reports.\n  service: ScreeningReports\n  source: openapi/sonde-health-screening-api-openapi.yaml\n- name: sonde-platform/screening-results.list\n  description: List screening results.\n  service: ScreeningReports\n  source: openapi/sonde-health-screening-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonde-health/refs/heads/main/scopes/sonde-health-scopes.yml
summary_line: 17 scopes · clientCredentials
tags:
- Company
- Health
- Healthcare
- Digital Health
- Vocal Biomarkers
- Voice
- Audio
- Machine Learning
- Artificial Intelligence
- Mental Health
- Respiratory
- Remote Patient Monitoring
- Wellness
- HIPAA
token_bound: false
token_urls:
- https://api.sondeservices.com/platform/v1/oauth2/token
---
