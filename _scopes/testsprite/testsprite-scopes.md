---
authorization_urls: []
description: TestSprite API keys are scoped. These are API-key permission scopes (not OAuth2 flows — TestSprite issues no OAuth authorization/token endpoints). New and grandfathered keys both default to the five scopes the CLI needs. Scope enforcement surfaces as the AUTH_FORBIDDEN error / exit code 3 (see errors/testsprite-error-codes.yml).
docs: https://docs.testsprite.com/cli/core/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Testsprite Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TestSprite publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the TestSprite API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TestSprite
provider_slug: testsprite
schemes: []
scope_count: 5
scope_names:
- read:me
- read:projects
- read:tests
- write:tests
- run:tests
scopes:
- description: Identity and usage — `auth status`, `usage`.
  flows: []
  scope: read:me
- description: Read projects — `project list`, `project get`.
  flows: []
  scope: read:projects
- description: Read tests, execution steps, results, and failure artifacts.
  flows: []
  scope: read:tests
- description: Create/update/delete tests and projects — test create, test create-batch, test update, test delete, test delete-batch, test code put, test plan put, project create, project update.
  flows: []
  scope: write:tests
- description: Execute tests — test run, test wait, test rerun.
  flows: []
  scope: run:tests
slug: testsprite-scopes
source_filename: testsprite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.testsprite.com/cli/core/authentication\ndocs: https://docs.testsprite.com/cli/core/authentication\ndescription: >-\n  TestSprite API keys are scoped. These are API-key permission scopes (not OAuth2\n  flows — TestSprite issues no OAuth authorization/token endpoints). New and\n  grandfathered keys both default to the five scopes the CLI needs. Scope\n  enforcement surfaces as the AUTH_FORBIDDEN error / exit code 3 (see\n  errors/testsprite-error-codes.yml).\nscheme:\n  type: apiKey\n  binding: TestSprite API key\nscopes:\n  - scope: read:me\n    description: Identity and usage — `auth status`, `usage`.\n  - scope: read:projects\n    description: Read projects — `project list`, `project get`.\n  - scope: read:tests\n    description: Read tests, execution steps, results, and failure artifacts.\n  - scope: write:tests\n    description: >-\n      Create/update/delete tests and projects — test create, test create-batch,\n\
  \      test update, test delete, test delete-batch, test code put, test plan put,\n      project create, project update.\n  - scope: run:tests\n    description: Execute tests — test run, test wait, test rerun.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testsprite/refs/heads/main/scopes/testsprite-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Software Testing
- API Testing
- Test Automation
- AI
- Developer Tools
- Model Context Protocol
- Quality Assurance
- CI/CD
- Agentic
token_urls: []
---
