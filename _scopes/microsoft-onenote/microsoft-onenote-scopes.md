---
api_specs:
- filename: microsoft-onenote-notebooks-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Notebooks API
  slug: microsoft-onenote-notebooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-notebooks-api-openapi.yml
- filename: microsoft-onenote-pages-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Pages API
  slug: microsoft-onenote-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-pages-api-openapi.yml
- filename: microsoft-onenote-sectiongroups-api-openapi.yml
  format: yaml
  label: Microsoft OneNote SectionGroups API
  slug: microsoft-onenote-sectiongroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-sectiongroups-api-openapi.yml
- filename: microsoft-onenote-sections-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Sections API
  slug: microsoft-onenote-sections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-sections-api-openapi.yml
- filename: microsoft-onenote-groups-onenote-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Groups.onenote API
  slug: microsoft-onenote-groups-onenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-groups-onenote-api-openapi.yml
- filename: microsoft-onenote-sites-onenote-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Sites.onenote API
  slug: microsoft-onenote-sites-onenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-sites-onenote-api-openapi.yml
- filename: microsoft-onenote-users-onenote-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Users.onenote API
  slug: microsoft-onenote-users-onenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-users-onenote-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: https://learn.microsoft.com/en-us/graph/permissions-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Onenote Scopes
name_suffix: OAuth Scopes
note: The Notes OpenAPI declares the azureaadv2 OAuth2 scheme with an empty scopes map; the permissions below are the Notes.* permissions documented in the Microsoft Graph permissions reference.
overview: 'Microsoft OneNote publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft OneNote API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft OneNote
provider_slug: microsoft-onenote
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: azureaadv2
scope_count: 6
scope_names:
- Notes.Create
- Notes.Read
- Notes.Read.All
- Notes.ReadWrite
- Notes.ReadWrite.All
- Notes.ReadWrite.CreatedByApp
scopes:
- description: Allows the app to read the titles of OneNote notebooks and sections and to create new pages, notebooks, and sections on behalf of the signed-in user.
  flows: []
  scope: Notes.Create
- description: Allows the app to read OneNote notebooks on behalf of the signed-in user.
  flows: []
  scope: Notes.Read
- description: Read all OneNote notebooks (application) / Read all OneNote notebooks that user can access (delegated).
  flows: []
  scope: Notes.Read.All
- description: Allows the app to read, share, and modify OneNote notebooks on behalf of the signed-in user.
  flows: []
  scope: Notes.ReadWrite
- description: Read and write all OneNote notebooks (application) / that the user can access (delegated).
  flows: []
  scope: Notes.ReadWrite.All
- description: Limited notebook access (deprecated). This permission no longer has any effect.
  flows: []
  scope: Notes.ReadWrite.CreatedByApp
slug: microsoft-onenote-scopes
source_filename: microsoft-onenote-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Microsoft OneNote OAuth scopes\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/graph/permissions-reference\ndocs: https://learn.microsoft.com/en-us/graph/permissions-reference\nnote: The Notes OpenAPI declares the azureaadv2 OAuth2 scheme with an empty scopes map; the permissions below are the Notes.* permissions documented in the Microsoft Graph permissions reference.\nschemes:\n- name: azureaadv2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\nscopes:\n- name: Notes.Create\n  description: Allows the app to read the titles of OneNote notebooks and sections and to create new pages, notebooks, and sections on behalf of the signed-in user.\n  type: delegated\n- name: Notes.Read\n  description: Allows the app to read OneNote notebooks on behalf of the signed-in user.\n  type: delegated\n\
  - name: Notes.Read.All\n  description: Read all OneNote notebooks (application) / Read all OneNote notebooks that user can access (delegated).\n  type: delegated, application\n- name: Notes.ReadWrite\n  description: Allows the app to read, share, and modify OneNote notebooks on behalf of the signed-in user.\n  type: delegated\n- name: Notes.ReadWrite.All\n  description: Read and write all OneNote notebooks (application) / that the user can access (delegated).\n  type: delegated, application\n- name: Notes.ReadWrite.CreatedByApp\n  description: Limited notebook access (deprecated). This permission no longer has any effect.\n  type: delegated\n  deprecated: true\n"
source_yaml_url: https://artifacts.apis.io/microsoft-onenote/scopes/microsoft-onenote-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Microsoft
- Microsoft 365
- Notebooks
- Notes
- Productivity
token_bound: false
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
