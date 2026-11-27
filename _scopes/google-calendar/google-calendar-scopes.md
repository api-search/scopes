---
api_specs:
- filename: google-calendar-calendars-api-openapi.yml
  format: yaml
  label: Google Calendar Calendars API
  slug: google-calendar-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-calendars-api-openapi.yml
- filename: google-calendar-colors-api-openapi.yml
  format: yaml
  label: Google Calendar Colors API
  slug: google-calendar-colors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-colors-api-openapi.yml
- filename: google-calendar-acl-api-openapi.yml
  format: yaml
  label: Google Calendar Acl API
  slug: google-calendar-acl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-acl-api-openapi.yml
- filename: google-calendar-channels-api-openapi.yml
  format: yaml
  label: Google Calendar Channels API
  slug: google-calendar-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-channels-api-openapi.yml
- filename: google-calendar-events-api-openapi.yml
  format: yaml
  label: Google Calendar Events API
  slug: google-calendar-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-events-api-openapi.yml
- filename: google-calendar-settings-api-openapi.yml
  format: yaml
  label: Google Calendar Settings API
  slug: google-calendar-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-settings-api-openapi.yml
- filename: google-calendar-calendar-list-api-openapi.yml
  format: yaml
  label: Google Calendar Calendar Calendar List API
  slug: google-calendar-calendar-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-calendar-list-api-openapi.yml
- filename: google-calendar-freebusy-api-openapi.yml
  format: yaml
  label: Google Calendar Calendar Freebusy API
  slug: google-calendar-freebusy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-calendar/openapi/google-calendar-freebusy-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Calendar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Calendar publishes 18 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Calendar API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Calendar
provider_slug: google-calendar
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-calendar-acl-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-calendar-calendar-list-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-calendar-channels-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-calendar-events-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-calendar-freebusy-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-calendar-settings-api-openapi.yml
scope_count: 18
scope_names:
- https://www.googleapis.com/auth/calendar
- https://www.googleapis.com/auth/calendar.acls
- https://www.googleapis.com/auth/calendar.acls.readonly
- https://www.googleapis.com/auth/calendar.app.created
- https://www.googleapis.com/auth/calendar.calendarlist
- https://www.googleapis.com/auth/calendar.calendarlist.readonly
- https://www.googleapis.com/auth/calendar.calendars
- https://www.googleapis.com/auth/calendar.calendars.readonly
- https://www.googleapis.com/auth/calendar.events
- https://www.googleapis.com/auth/calendar.events.freebusy
- https://www.googleapis.com/auth/calendar.events.owned
- https://www.googleapis.com/auth/calendar.events.owned.readonly
- https://www.googleapis.com/auth/calendar.events.public.readonly
- https://www.googleapis.com/auth/calendar.events.readonly
- https://www.googleapis.com/auth/calendar.freebusy
- https://www.googleapis.com/auth/calendar.readonly
- https://www.googleapis.com/auth/calendar.settings
- https://www.googleapis.com/auth/calendar.settings.readonly
scopes:
- description: See, edit, share, and permanently delete all the calendars you can access using Google Calendar
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar
- description: See and change the sharing permissions of Google calendars you own
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.acls
- description: See the sharing permissions of Google calendars you own
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.acls.readonly
- description: Make secondary Google calendars, and see, create, change, and delete events on them
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.app.created
- description: See, add, and remove Google calendars you’re subscribed to
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.calendarlist
- description: See the list of Google calendars you’re subscribed to
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.calendarlist.readonly
- description: See and change the properties of Google calendars you have access to, and create secondary calendars
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.calendars
- description: See the title, description, default time zone, and other properties of Google calendars you have access to
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.calendars.readonly
- description: View and edit events on all your calendars
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.events
- description: See the availability on Google calendars you have access to
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.events.freebusy
- description: See, create, change, and delete events on Google calendars you own
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.events.owned
- description: See the events on Google calendars you own
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.events.owned.readonly
- description: See the events on public calendars
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.events.public.readonly
- description: View events on all your calendars
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.events.readonly
- description: View your availability in your calendars
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.freebusy
- description: See and download any calendar you can access using your Google Calendar
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.readonly
- description: View and edit your Calendar settings
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.settings
- description: View your Calendar settings
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/calendar.settings.readonly
slug: google-calendar-scopes
source_filename: google-calendar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-calendar-acl-api-openapi.yml, openapi/google-calendar-calendar-list-api-openapi.yml,\n  openapi/google-calendar-channels-api-openapi.yml, openapi/google-calendar-events-api-openapi.yml,\n  openapi/google-calendar-freebusy-api-openapi.yml, openapi/google-calendar-settings-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-calendar-acl-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-calendar-calendar-list-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-calendar-channels-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n\
  \    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-calendar-events-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-calendar-freebusy-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-calendar-settings-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/calendar\n  description: See, edit, share, and permanently delete all the calendars you can access using\n    Google Calendar\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n\
  \  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.acls\n  description: See and change the sharing permissions of Google calendars you own\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.acls.readonly\n  description: See the sharing permissions of Google calendars you own\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n\
  \  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.app.created\n  description: Make secondary Google calendars, and see, create, change, and delete events on\n    them\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.calendarlist\n  description: See, add, and remove Google calendars you’re subscribed to\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n\
  \  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.calendarlist.readonly\n  description: See the list of Google calendars you’re subscribed to\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.calendars\n  description: See and change the properties of Google calendars you have access to, and create\n    secondary calendars\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.calendars.readonly\n  description: See the title, description, default time zone, and other properties of Google\n    calendars you have access to\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.events\n  description: View and edit events on all\
  \ your calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.events.freebusy\n  description: See the availability on Google calendars you have access to\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.events.owned\n  description: See, create, change, and delete\
  \ events on Google calendars you own\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.events.owned.readonly\n  description: See the events on Google calendars you own\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.events.public.readonly\n  description: See the\
  \ events on public calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.events.readonly\n  description: View events on all your calendars\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.freebusy\n  description: View your availability in your calendars\n \
  \ flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.readonly\n  description: See and download any calendar you can access using your Google Calendar\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.settings\n  description: View and edit your Calendar settings\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n- scope: https://www.googleapis.com/auth/calendar.settings.readonly\n  description: View your Calendar settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-calendar-acl-api-openapi.yml\n  - openapi/google-calendar-calendar-list-api-openapi.yml\n  - openapi/google-calendar-channels-api-openapi.yml\n  - openapi/google-calendar-events-api-openapi.yml\n  - openapi/google-calendar-freebusy-api-openapi.yml\n  - openapi/google-calendar-settings-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-calendar/scopes/google-calendar-scopes.yml
summary_line: 18 scopes · authorizationCode
tags:
- Availability
- Calendar
- Event
- Google
- Google Workspace
- Scheduling
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
