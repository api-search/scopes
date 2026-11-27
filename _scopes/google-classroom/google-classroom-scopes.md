---
api_specs:
- filename: google-classroom-courses-api-openapi.yml
  format: yaml
  label: Google Classroom Courses API
  slug: google-classroom-courses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-classroom/openapi/google-classroom-courses-api-openapi.yml
- filename: google-classroom-invitations-api-openapi.yml
  format: yaml
  label: Google Classroom Invitations API
  slug: google-classroom-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-classroom/openapi/google-classroom-invitations-api-openapi.yml
- filename: google-classroom-registrations-api-openapi.yml
  format: yaml
  label: Google Classroom Registrations API
  slug: google-classroom-registrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-classroom/openapi/google-classroom-registrations-api-openapi.yml
- filename: google-classroom-user-profiles-api-openapi.yml
  format: yaml
  label: Google Classroom User Profiles API
  slug: google-classroom-user-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-classroom/openapi/google-classroom-user-profiles-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: https://developers.google.com/workspace/classroom/guides/auth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Classroom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Classroom publishes 24 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Classroom API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Classroom
provider_slug: google-classroom
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-classroom-registrations-api-openapi.yml
scope_count: 24
scope_names:
- https://www.googleapis.com/auth/classroom.addons.student
- https://www.googleapis.com/auth/classroom.addons.teacher
- https://www.googleapis.com/auth/classroom.announcements
- https://www.googleapis.com/auth/classroom.announcements.readonly
- https://www.googleapis.com/auth/classroom.courses
- https://www.googleapis.com/auth/classroom.courses.readonly
- https://www.googleapis.com/auth/classroom.coursework.me
- https://www.googleapis.com/auth/classroom.coursework.me.readonly
- https://www.googleapis.com/auth/classroom.coursework.students
- https://www.googleapis.com/auth/classroom.coursework.students.readonly
- https://www.googleapis.com/auth/classroom.courseworkmaterials
- https://www.googleapis.com/auth/classroom.courseworkmaterials.readonly
- https://www.googleapis.com/auth/classroom.guardianlinks.me.readonly
- https://www.googleapis.com/auth/classroom.guardianlinks.students
- https://www.googleapis.com/auth/classroom.guardianlinks.students.readonly
- https://www.googleapis.com/auth/classroom.profile.emails
- https://www.googleapis.com/auth/classroom.profile.photos
- https://www.googleapis.com/auth/classroom.push-notifications
- https://www.googleapis.com/auth/classroom.rosters
- https://www.googleapis.com/auth/classroom.rosters.readonly
- https://www.googleapis.com/auth/classroom.student-submissions.me.readonly
- https://www.googleapis.com/auth/classroom.student-submissions.students.readonly
- https://www.googleapis.com/auth/classroom.topics
- https://www.googleapis.com/auth/classroom.topics.readonly
scopes:
- description: See and update its own attachments to posts in Google Classroom
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.addons.student
- description: See, create, and update its own attachments to posts in classes you teach in Google Classroom
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.addons.teacher
- description: View and manage announcements in Google Classroom
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.announcements
- description: View announcements in Google Classroom
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.announcements.readonly
- description: See, edit, create, and permanently delete your Google Classroom classes
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.courses
- description: View your Google Classroom classes
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.courses.readonly
- description: See, create and edit coursework items including assignments, questions, and grades
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.coursework.me
- description: View your course work and grades in Google Classroom
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.coursework.me.readonly
- description: Manage course work and grades for students in the Google Classroom classes you teach and view the course work and grades for classes you administer
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.coursework.students
- description: View course work and grades for students in the Google Classroom classes you teach or administer
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.coursework.students.readonly
- description: See, edit, and create classwork materials in Google Classroom
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.courseworkmaterials
- description: See all classwork materials for your Google Classroom classes
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.courseworkmaterials.readonly
- description: View your Google Classroom guardians
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.guardianlinks.me.readonly
- description: View and manage guardians for students in your Google Classroom classes
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.guardianlinks.students
- description: View guardians for students in your Google Classroom classes
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.guardianlinks.students.readonly
- description: View the email addresses of people in your classes
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.profile.emails
- description: View the profile photos of people in your classes
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.profile.photos
- description: Receive notifications about your Google Classroom data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.push-notifications
- description: Manage your Google Classroom class rosters
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.rosters
- description: View your Google Classroom class rosters
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.rosters.readonly
- description: View your course work and grades in Google Classroom
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.student-submissions.me.readonly
- description: View course work and grades for students in the Google Classroom classes you teach or administer
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.student-submissions.students.readonly
- description: See, create, and edit topics in Google Classroom
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.topics
- description: View topics in Google Classroom
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/classroom.topics.readonly
slug: google-classroom-scopes
source_filename: google-classroom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-classroom-registrations-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-classroom-registrations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/classroom.addons.student\n  description: See and update its own attachments to posts in Google Classroom\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.addons.teacher\n  description: See, create, and update its own attachments to posts in classes you\n    teach in Google Classroom\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.announcements\n  description: View and\
  \ manage announcements in Google Classroom\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.announcements.readonly\n  description: View announcements in Google Classroom\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.courses\n  description: See, edit, create, and permanently delete your Google Classroom classes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.courses.readonly\n  description: View your Google Classroom classes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.coursework.me\n  description: See, create and edit coursework items including assignments,\
  \ questions,\n    and grades\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.coursework.me.readonly\n  description: View your course work and grades in Google Classroom\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.coursework.students\n  description: Manage course work and grades for students in the Google Classroom\n    classes you teach and view the course work and grades for classes you administer\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.coursework.students.readonly\n  description: View course work and grades for students in the Google Classroom classes\n    you teach or administer\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/classroom.courseworkmaterials\n  description: See, edit, and create classwork materials in Google Classroom\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.courseworkmaterials.readonly\n  description: See all classwork materials for your Google Classroom classes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.guardianlinks.me.readonly\n  description: View your Google Classroom guardians\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.guardianlinks.students\n  description: View and manage guardians for students in your Google Classroom classes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/classroom.guardianlinks.students.readonly\n  description: View guardians for students in your Google Classroom classes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.profile.emails\n  description: View the email addresses of people in your classes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.profile.photos\n  description: View the profile photos of people in your classes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.push-notifications\n  description: Receive notifications about your Google Classroom data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.rosters\n\
  \  description: Manage your Google Classroom class rosters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.rosters.readonly\n  description: View your Google Classroom class rosters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.student-submissions.me.readonly\n  description: View your course work and grades in Google Classroom\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.student-submissions.students.readonly\n  description: View course work and grades for students in the Google Classroom classes\n    you teach or administer\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.topics\n\
  \  description: See, create, and edit topics in Google Classroom\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\n- scope: https://www.googleapis.com/auth/classroom.topics.readonly\n  description: View topics in Google Classroom\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-classroom-registrations-api-openapi.yml\ndocs: https://developers.google.com/workspace/classroom/guides/auth\n"
source_yaml_url: https://artifacts.apis.io/google-classroom/scopes/google-classroom-scopes.yml
summary_line: 24 scopes · authorizationCode
tags:
- Assignments
- Classroom
- Courses
- Education
- Google
- Google Workspace
- Students
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
