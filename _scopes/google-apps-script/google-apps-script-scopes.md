---
api_specs:
- filename: google-apps-script-processes-api-openapi.yml
  format: yaml
  label: Google Apps Script Processes API
  slug: google-apps-script-processes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-apps-script/openapi/google-apps-script-processes-api-openapi.yml
- filename: google-apps-script-projects-api-openapi.yml
  format: yaml
  label: Google Apps Script Projects API
  slug: google-apps-script-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-apps-script/openapi/google-apps-script-projects-api-openapi.yml
- filename: google-apps-script-scripts-api-openapi.yml
  format: yaml
  label: Google Apps Script Scripts API
  slug: google-apps-script-scripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-apps-script/openapi/google-apps-script-scripts-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.google.com/apps-script/concepts/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Apps Script Scopes
name_suffix: OAuth Scopes
note: scripts.run requires an OAuth token covering all scopes used by the script (https://developers.google.com/apps-script/api/how-tos/execute).
overview: 'Google Apps Script publishes 18 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Apps Script API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Apps Script
provider_slug: google-apps-script
schemes: []
scope_count: 18
scope_names:
- https://www.google.com/m8/feeds
- https://www.googleapis.com/auth/script.processes
- https://www.googleapis.com/auth/forms.currentonly
- https://www.googleapis.com/auth/forms
- https://www.googleapis.com/auth/documents
- https://www.googleapis.com/auth/drive
- https://mail.google.com/
- https://www.googleapis.com/auth/admin.directory.user
- https://www.googleapis.com/auth/userinfo.email
- https://www.googleapis.com/auth/spreadsheets
- https://www.google.com/calendar/feeds
- https://www.googleapis.com/auth/script.metrics
- https://www.googleapis.com/auth/script.projects
- https://www.googleapis.com/auth/groups
- https://www.googleapis.com/auth/script.deployments.readonly
- https://www.googleapis.com/auth/admin.directory.group
- https://www.googleapis.com/auth/script.projects.readonly
- https://www.googleapis.com/auth/script.deployments
scopes:
- description: See, edit, download, and permanently delete your contacts
  flows: []
  scope: https://www.google.com/m8/feeds
- description: View Google Apps Script processes
  flows: []
  scope: https://www.googleapis.com/auth/script.processes
- description: View and manage forms that this application has been installed in
  flows: []
  scope: https://www.googleapis.com/auth/forms.currentonly
- description: View and manage your forms in Google Drive
  flows: []
  scope: https://www.googleapis.com/auth/forms
- description: See, edit, create, and delete all your Google Docs documents
  flows: []
  scope: https://www.googleapis.com/auth/documents
- description: See, edit, create, and delete all of your Google Drive files
  flows: []
  scope: https://www.googleapis.com/auth/drive
- description: Read, compose, send, and permanently delete all your email from Gmail
  flows: []
  scope: https://mail.google.com/
- description: View and manage the provisioning of users on your domain
  flows: []
  scope: https://www.googleapis.com/auth/admin.directory.user
- description: See your primary Google Account email address
  flows: []
  scope: https://www.googleapis.com/auth/userinfo.email
- description: See, edit, create, and delete all your Google Sheets spreadsheets
  flows: []
  scope: https://www.googleapis.com/auth/spreadsheets
- description: See, edit, share, and permanently delete all the calendars you can access using Google Calendar
  flows: []
  scope: https://www.google.com/calendar/feeds
- description: View Google Apps Script project's metrics
  flows: []
  scope: https://www.googleapis.com/auth/script.metrics
- description: Create and update Google Apps Script projects
  flows: []
  scope: https://www.googleapis.com/auth/script.projects
- description: View and manage your Google Groups
  flows: []
  scope: https://www.googleapis.com/auth/groups
- description: View Google Apps Script deployments
  flows: []
  scope: https://www.googleapis.com/auth/script.deployments.readonly
- description: View and manage the provisioning of groups on your domain
  flows: []
  scope: https://www.googleapis.com/auth/admin.directory.group
- description: View Google Apps Script projects
  flows: []
  scope: https://www.googleapis.com/auth/script.projects.readonly
- description: Create and update Google Apps Script deployments
  flows: []
  scope: https://www.googleapis.com/auth/script.deployments
slug: google-apps-script-scopes
source_filename: google-apps-script-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Google Apps Script OAuth scopes\ngenerated: '2026-11-11'\nmethod: searched\nsource: discovery/script-v1.json (Google Discovery document auth.oauth2.scopes)\ndocs: https://developers.google.com/apps-script/concepts/scopes\nscopes:\n- name: https://www.google.com/m8/feeds\n  description: See, edit, download, and permanently delete your contacts\n- name: https://www.googleapis.com/auth/script.processes\n  description: View Google Apps Script processes\n- name: https://www.googleapis.com/auth/forms.currentonly\n  description: View and manage forms that this application has been installed in\n- name: https://www.googleapis.com/auth/forms\n  description: View and manage your forms in Google Drive\n- name: https://www.googleapis.com/auth/documents\n  description: See, edit, create, and delete all your Google Docs documents\n- name: https://www.googleapis.com/auth/drive\n  description: See, edit, create, and delete all of your Google Drive files\n- name: https://mail.google.com/\n\
  \  description: Read, compose, send, and permanently delete all your email from Gmail\n- name: https://www.googleapis.com/auth/admin.directory.user\n  description: View and manage the provisioning of users on your domain\n- name: https://www.googleapis.com/auth/userinfo.email\n  description: See your primary Google Account email address\n- name: https://www.googleapis.com/auth/spreadsheets\n  description: See, edit, create, and delete all your Google Sheets spreadsheets\n- name: https://www.google.com/calendar/feeds\n  description: See, edit, share, and permanently delete all the calendars you can access using Google Calendar\n- name: https://www.googleapis.com/auth/script.metrics\n  description: View Google Apps Script project's metrics\n- name: https://www.googleapis.com/auth/script.projects\n  description: Create and update Google Apps Script projects\n- name: https://www.googleapis.com/auth/groups\n  description: View and manage your Google Groups\n- name: https://www.googleapis.com/auth/script.deployments.readonly\n\
  \  description: View Google Apps Script deployments\n- name: https://www.googleapis.com/auth/admin.directory.group\n  description: View and manage the provisioning of groups on your domain\n- name: https://www.googleapis.com/auth/script.projects.readonly\n  description: View Google Apps Script projects\n- name: https://www.googleapis.com/auth/script.deployments\n  description: Create and update Google Apps Script deployments\nnote: scripts.run requires an OAuth token covering all scopes used by the script (https://developers.google.com/apps-script/api/how-tos/execute).\n"
source_yaml_url: https://artifacts.apis.io/google-apps-script/scopes/google-apps-script-scopes.yml
summary_line: 18 scopes
tags:
- Apps Script
- Automation
- Deployment
- Google
- Google Workspace
- Scripting
token_bound: false
token_urls: []
---
