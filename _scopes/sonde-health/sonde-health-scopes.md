---
api_specs:
- filename: sonde-health-screening-api-openapi.yaml
  format: yaml
  label: Sonde Screening API
  slug: sonde-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonde-health/refs/heads/main/openapi/sonde-health-screening-api-openapi.yaml
authorization_urls: []
description: ''
docs: https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706931713/Authentication+Scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Sonde Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sonde Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sonde Health
provider_slug: sonde-health
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: sonde-health-scopes
source_filename: sonde-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706931713/Authentication+Scopes\ndocs: https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706931713/Authentication+Scopes\nflow: clientCredentials\ntoken_url: https://api.sondeservices.com/platform/v1/oauth2/token\nallocation: >-\n  \"As per your contract, SondeHealth will allocate authentication scopes to you.\" Scopes\n  are granted at onboarding; a partner cannot self-grant.\nscope_count: 17\nscopes:\n- name: sonde-platform/users.write\n  description: Permission to create subjects in UserService.\n  service: UserService\n- name: sonde-platform/storage.write\n  description: Permission to upload wav files to StorageService.\n  service: StorageService\n- name: sonde-platform/storage.read\n  description: Permission to download uploaded files.\n  service: StorageService\n- name: sonde-platform/scores.write\n  description: Permission to calculate a score from InferenceService.\n\
  \  service: InferenceService\n- name: sonde-platform/voice-feature-scores.write\n  description: Permission to create a job to infer voice-feature scores for a measure.\n  service: InferenceService\n- name: sonde-platform/voice-feature-scores.read\n  description: Permission to pull a voice-feature job and to get the voice-feature-scores.\n  service: InferenceService\n- name: sonde-platform/measures.read\n  description: Permission to read the particular measures permitted to you from MeasureService.\n  service: MeasureService\n- name: sonde-platform/measures.list\n  description: Permission to list the measures permitted to you from MeasureService.\n  service: MeasureService\n- name: sonde-platform/questionnaires.read\n  description: Permission to read questionnaire.\n  service: QuestionnaireManager\n- name: sonde-platform/questionnaires.write\n  description: Permission to create a questionnaire.\n  service: QuestionnaireManager\n  note: Observed in the Partner Questionnaire Creation use\
  \ case.\n- name: sonde-platform/questionnaire.write\n  description: Singular variant of the questionnaire-write scope observed in the questionnaire\n    creation docs alongside the plural form.\n  service: QuestionnaireManager\n  note: Both spellings appear in Sonde's published curl examples; recorded verbatim\n    rather than normalised.\n- name: sonde-platform/questionnaire-responses.write\n  description: Permission to submit responses of questionnaire.\n  service: QuestionnaireManager\n- name: sonde-platform/questionnaire-responses.read\n  description: Permission to read submitted questionnaire responses.\n  service: QuestionnaireManager\n- name: sonde-platform/transcriptions.write\n  description: Permission to create a transcribe job.\n  service: TranscriptionService\n- name: sonde-platform/transcriptions.read\n  description: Permission to poll (or read) a transcribe job (or transcript).\n  service: TranscriptionService\n- name: sonde-platform/reports.read\n  description: Read screening-result\
  \ reports.\n  service: ScreeningReports\n  source: openapi/sonde-health-screening-api-openapi.yaml\n- name: sonde-platform/screening-results.list\n  description: List screening results.\n  service: ScreeningReports\n  source: openapi/sonde-health-screening-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonde-health/refs/heads/main/scopes/sonde-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health
- Healthcare
- Digital Health
- Vocal Biomarkers
- Voice
- Audio
- Machine-Learning
- Artificial Intelligence
- Mental Health
- Respiratory
- Remote Patient Monitoring
- Wellness
- HIPAA
token_urls: []
---
