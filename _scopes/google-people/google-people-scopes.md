---
api_specs:
- filename: google-people-people-api-openapi.yml
  format: yaml
  label: Google People API
  slug: google-people-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-people/openapi/google-people-people-api-openapi.yml
- filename: google-people-othercontacts-api-openapi.yml
  format: yaml
  label: Google People Other Contacts API
  slug: google-people-othercontacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-people/openapi/google-people-othercontacts-api-openapi.yml
- filename: google-people-contact-groups-api-openapi.yml
  format: yaml
  label: Google People Contact Groups API
  slug: google-people-contact-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-people/openapi/google-people-contact-groups-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google People Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google People publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google People API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google People
provider_slug: google-people
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-people-contact-groups-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-people-other-contacts-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-people-people-api-openapi.yml
scope_count: 12
scope_names:
- https://www.googleapis.com/auth/contacts
- https://www.googleapis.com/auth/contacts.other.readonly
- https://www.googleapis.com/auth/contacts.readonly
- https://www.googleapis.com/auth/directory.readonly
- https://www.googleapis.com/auth/user.addresses.read
- https://www.googleapis.com/auth/user.birthday.read
- https://www.googleapis.com/auth/user.emails.read
- https://www.googleapis.com/auth/user.gender.read
- https://www.googleapis.com/auth/user.organization.read
- https://www.googleapis.com/auth/user.phonenumbers.read
- https://www.googleapis.com/auth/userinfo.email
- https://www.googleapis.com/auth/userinfo.profile
scopes:
- description: See, edit, download, and permanently delete your contacts
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/contacts
- description: See and download contact info automatically saved in your "Other contacts"
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/contacts.other.readonly
- description: See and download your contacts
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/contacts.readonly
- description: See and download your organization's Google Workspace directory
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/directory.readonly
- description: View your street addresses
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/user.addresses.read
- description: See and download your exact date of birth
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/user.birthday.read
- description: See and download all of your Google Account email addresses
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/user.emails.read
- description: See your gender
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/user.gender.read
- description: See your education, work history and org info
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/user.organization.read
- description: See and download your personal phone numbers
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/user.phonenumbers.read
- description: See your primary Google Account email address
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/userinfo.email
- description: See your personal info, including any personal info you've made publicly available
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/userinfo.profile
slug: google-people-scopes
source_filename: google-people-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-people-contact-groups-api-openapi.yml, openapi/google-people-other-contacts-api-openapi.yml,\n  openapi/google-people-people-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-people-contact-groups-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-people-other-contacts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-people-people-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/contacts\n  description:\
  \ See, edit, download, and permanently delete your contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/contacts.other.readonly\n  description: See and download contact info automatically saved in your \"Other contacts\"\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/contacts.readonly\n  description: See and download your contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/directory.readonly\n\
  \  description: See and download your organization's Google Workspace directory\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/user.addresses.read\n  description: View your street addresses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/user.birthday.read\n  description: See and download your exact date of birth\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/user.emails.read\n  description:\
  \ See and download all of your Google Account email addresses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/user.gender.read\n  description: See your gender\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/user.organization.read\n  description: See your education, work history and org info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/user.phonenumbers.read\n  description: See and\
  \ download your personal phone numbers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/userinfo.email\n  description: See your primary Google Account email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n- scope: https://www.googleapis.com/auth/userinfo.profile\n  description: See your personal info, including any personal info you've made publicly available\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-people-contact-groups-api-openapi.yml\n  - openapi/google-people-other-contacts-api-openapi.yml\n  - openapi/google-people-people-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-people/scopes/google-people-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Address Book
- Contacts
- Google
- People
- Profiles
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
