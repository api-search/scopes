---
api_specs:
- filename: vidocu-ai-ai-recorder-api-openapi.yml
  format: yaml
  label: vidocu-ai AI Recorder API
  slug: vidocu-ai-ai-recorder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-ai-recorder-api-openapi.yml
- filename: vidocu-ai-brand-kit-api-openapi.yml
  format: yaml
  label: vidocu-ai Brand Kit API
  slug: vidocu-ai-brand-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-brand-kit-api-openapi.yml
- filename: vidocu-ai-courses-api-openapi.yml
  format: yaml
  label: vidocu-ai Courses API
  slug: vidocu-ai-courses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-courses-api-openapi.yml
- filename: vidocu-ai-governance-api-openapi.yml
  format: yaml
  label: vidocu-ai Governance API
  slug: vidocu-ai-governance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-governance-api-openapi.yml
- filename: vidocu-ai-jobs-api-openapi.yml
  format: yaml
  label: vidocu-ai Jobs API
  slug: vidocu-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-jobs-api-openapi.yml
- filename: vidocu-ai-knowledge-center-api-openapi.yml
  format: yaml
  label: vidocu-ai Knowledge Center API
  slug: vidocu-ai-knowledge-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-knowledge-center-api-openapi.yml
- filename: vidocu-ai-operations-api-openapi.yml
  format: yaml
  label: vidocu-ai Operations API
  slug: vidocu-ai-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-operations-api-openapi.yml
- filename: vidocu-ai-projects-api-openapi.yml
  format: yaml
  label: vidocu-ai Projects API
  slug: vidocu-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-projects-api-openapi.yml
- filename: vidocu-ai-reference-api-openapi.yml
  format: yaml
  label: vidocu-ai Reference API
  slug: vidocu-ai-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-reference-api-openapi.yml
- filename: vidocu-ai-remix-api-openapi.yml
  format: yaml
  label: vidocu-ai Remix API
  slug: vidocu-ai-remix-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-remix-api-openapi.yml
- filename: vidocu-ai-studio-api-openapi.yml
  format: yaml
  label: vidocu-ai Studio API
  slug: vidocu-ai-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-studio-api-openapi.yml
- filename: vidocu-ai-tools-api-openapi.yml
  format: yaml
  label: vidocu-ai Tools API
  slug: vidocu-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-tools-api-openapi.yml
- filename: vidocu-ai-training-modules-api-openapi.yml
  format: yaml
  label: vidocu-ai Training Modules API
  slug: vidocu-ai-training-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-training-modules-api-openapi.yml
- filename: vidocu-ai-usage-api-openapi.yml
  format: yaml
  label: vidocu-ai Usage API
  slug: vidocu-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-usage-api-openapi.yml
- filename: vidocu-ai-videos-api-openapi.yml
  format: yaml
  label: vidocu-ai Videos API
  slug: vidocu-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-videos-api-openapi.yml
- filename: vidocu-ai-webhooks-api-openapi.yml
  format: yaml
  label: vidocu-ai Webhooks API
  slug: vidocu-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-webhooks-api-openapi.yml
authorization_urls:
- https://vidocu.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Vidocu Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'vidocu-ai publishes 42 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the vidocu-ai API on a user''s behalf.


  Tokens are issued from https://api.vidocu.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: vidocu-ai
provider_slug: vidocu-ai
schemes:
- flows:
  - authorizationUrl: https://vidocu.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.vidocu.ai/oauth/token
  name: oauth2
  source: openapi/support-vidocu-openapi.json
- flows:
  - authorizationUrl: https://vidocu.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.vidocu.ai/oauth/token
  name: oauth2
  source: openapi/vidocu-ai-openapi.json
scope_count: 42
scope_names:
- analyze:write
- approvals:read
- approvals:write
- article:read
- article:write
- avatars:read
- avatars:write
- brand_kit:read
- brand_kit:write
- comments:read
- comments:write
- courses:read
- courses:write
- export:write
- jobs:read
- knowledge_base:read
- knowledge_base:write
- locks:write
- modules:read
- modules:write
- process:write
- projects:read
- projects:write
- recordings:read
- recordings:write
- remixes:read
- remixes:write
- studio:read
- studio:write
- subtitles:read
- subtitles:write
- tools:read
- tools:write
- translate:write
- usage:read
- videos:read
- videos:write
- voiceover:write
- voices:read
- voices:write
- webhooks:read
- webhooks:write
scopes:
- description: Analyze videos
  flows:
  - authorizationCode
  scope: analyze:write
- description: View approval rounds and requests
  flows:
  - authorizationCode
  scope: approvals:read
- description: Request, decide and withdraw approvals
  flows:
  - authorizationCode
  scope: approvals:write
- description: View help articles
  flows:
  - authorizationCode
  scope: article:read
- description: Generate help articles
  flows:
  - authorizationCode
  scope: article:write
- description: List available AI avatars
  flows:
  - authorizationCode
  scope: avatars:read
- description: Create custom AI avatars
  flows:
  - authorizationCode
  scope: avatars:write
- description: View Brand Kit settings, skills and glossary
  flows:
  - authorizationCode
  scope: brand_kit:read
- description: Change Brand Kit settings, skills and glossary
  flows:
  - authorizationCode
  scope: brand_kit:write
- description: View comments on videos
  flows:
  - authorizationCode
  scope: comments:read
- description: Add and delete comments
  flows:
  - authorizationCode
  scope: comments:write
- description: View courses and their storyboards
  flows:
  - authorizationCode
  scope: courses:read
- description: Create courses and run planning, storyboarding and generation
  flows:
  - authorizationCode
  scope: courses:write
- description: Export videos
  flows:
  - authorizationCode
  scope: export:write
- description: View job status
  flows:
  - authorizationCode
  scope: jobs:read
- description: View the knowledge base, its articles and analytics
  flows:
  - authorizationCode
  scope: knowledge_base:read
- description: Create and edit knowledge base content
  flows:
  - authorizationCode
  scope: knowledge_base:write
- description: Lock and unlock videos and modules
  flows:
  - authorizationCode
  scope: locks:write
- description: View training modules, results and qualifications
  flows:
  - authorizationCode
  scope: modules:read
- description: Create, edit and translate training modules; record attempts and sign-offs
  flows:
  - authorizationCode
  scope: modules:write
- description: Use one-shot process endpoint
  flows:
  - authorizationCode
  scope: process:write
- description: View project folders
  flows:
  - authorizationCode
  scope: projects:read
- description: Create, update, and delete project folders
  flows:
  - authorizationCode
  scope: projects:write
- description: View AI Recorder jobs and saved logins
  flows:
  - authorizationCode
  scope: recordings:read
- description: Start recordings and manage saved logins
  flows:
  - authorizationCode
  scope: recordings:write
- description: View remixes and their analysis
  flows:
  - authorizationCode
  scope: remixes:read
- description: Create remixes and run analysis
  flows:
  - authorizationCode
  scope: remixes:write
- description: View Studio projects and templates
  flows:
  - authorizationCode
  scope: studio:read
- description: Create, edit and share Studio projects
  flows:
  - authorizationCode
  scope: studio:write
- description: View subtitles
  flows:
  - authorizationCode
  scope: subtitles:read
- description: Generate and edit subtitles
  flows:
  - authorizationCode
  scope: subtitles:write
- description: List and view tools
  flows:
  - authorizationCode
  scope: tools:read
- description: Execute tools
  flows:
  - authorizationCode
  scope: tools:write
- description: Translate videos
  flows:
  - authorizationCode
  scope: translate:write
- description: View usage statistics
  flows:
  - authorizationCode
  scope: usage:read
- description: View videos in the workspace
  flows:
  - authorizationCode
  scope: videos:read
- description: Upload and modify videos
  flows:
  - authorizationCode
  scope: videos:write
- description: Generate voiceovers
  flows:
  - authorizationCode
  scope: voiceover:write
- description: List available voices
  flows:
  - authorizationCode
  scope: voices:read
- description: Delete cloned voices
  flows:
  - authorizationCode
  scope: voices:write
- description: View webhook subscriptions
  flows:
  - authorizationCode
  scope: webhooks:read
- description: Create, update, and delete webhooks
  flows:
  - authorizationCode
  scope: webhooks:write
slug: vidocu-ai-scopes
source_filename: vidocu-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/support-vidocu-openapi.json, openapi/vidocu-ai-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/support-vidocu-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vidocu.ai/oauth/authorize\n    tokenUrl: https://api.vidocu.ai/oauth/token\n- name: oauth2\n  source: openapi/vidocu-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vidocu.ai/oauth/authorize\n    tokenUrl: https://api.vidocu.ai/oauth/token\nscopes:\n- scope: analyze:write\n  description: Analyze videos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: approvals:read\n  description: View approval rounds and requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: approvals:write\n  description: Request, decide and withdraw\
  \ approvals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: article:read\n  description: View help articles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: article:write\n  description: Generate help articles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: avatars:read\n  description: List available AI avatars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: avatars:write\n  description: Create custom AI avatars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: brand_kit:read\n  description: View Brand Kit settings, skills and glossary\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: brand_kit:write\n  description: Change Brand Kit settings, skills and glossary\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: comments:read\n  description: View comments on videos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: comments:write\n  description: Add and delete comments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: courses:read\n  description: View courses and their storyboards\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: courses:write\n  description: Create courses and run planning, storyboarding and generation\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: export:write\n  description: Export videos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: jobs:read\n  description: View job status\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: knowledge_base:read\n  description: View the knowledge base, its articles and analytics\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: knowledge_base:write\n  description: Create and edit knowledge base content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: locks:write\n  description: Lock and unlock videos and modules\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n\
  \  - openapi/vidocu-ai-openapi.json\n- scope: modules:read\n  description: View training modules, results and qualifications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: modules:write\n  description: Create, edit and translate training modules; record attempts and sign-offs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: process:write\n  description: Use one-shot process endpoint\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: projects:read\n  description: View project folders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: projects:write\n  description: Create, update, and delete project folders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n\
  \  - openapi/vidocu-ai-openapi.json\n- scope: recordings:read\n  description: View AI Recorder jobs and saved logins\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: recordings:write\n  description: Start recordings and manage saved logins\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: remixes:read\n  description: View remixes and their analysis\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: remixes:write\n  description: Create remixes and run analysis\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: studio:read\n  description: View Studio projects and templates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n\
  - scope: studio:write\n  description: Create, edit and share Studio projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: subtitles:read\n  description: View subtitles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: subtitles:write\n  description: Generate and edit subtitles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: tools:read\n  description: List and view tools\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: tools:write\n  description: Execute tools\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: translate:write\n  description: Translate videos\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: usage:read\n  description: View usage statistics\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: videos:read\n  description: View videos in the workspace\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: videos:write\n  description: Upload and modify videos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: voiceover:write\n  description: Generate voiceovers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: voices:read\n  description: List available voices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n\
  - scope: voices:write\n  description: Delete cloned voices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: webhooks:read\n  description: View webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n- scope: webhooks:write\n  description: Create, update, and delete webhooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/support-vidocu-openapi.json\n  - openapi/vidocu-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/vidocu-ai/scopes/vidocu-ai-scopes.yml
summary_line: 42 scopes · authorizationCode
tags:
- Artificial Intelligence
- Video
- Documentation
- SOP
- Training
- Knowledge Base
token_bound: false
token_urls:
- https://api.vidocu.ai/oauth/token
---
