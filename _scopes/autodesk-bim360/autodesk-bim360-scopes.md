---
authorization_urls: []
description: ''
docs: https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/
flows:
- clientCredentials
- implicit
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Autodesk Bim360 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Autodesk BIM 360 publishes 17 OAuth 2.0 scopes via the clientCredentials, implicit, and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Autodesk BIM 360 API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Autodesk BIM 360
provider_slug: autodesk-bim360
schemes:
- flows:
  - flow: clientCredentials
  name: 2-legged
  source: openapi/autodesk-bim360-account-admin-openapi.yml
- flows:
  - flow: implicit
  name: 3-legged-implicit
  source: openapi/autodesk-bim360-account-admin-openapi.yml
- flows:
  - flow: authorizationCode
  name: 3-legged
  source: openapi/autodesk-bim360-account-admin-openapi.yml
- flows:
  - flow: clientCredentials
  name: 2-legged
  source: openapi/autodesk-bim360-issues-openapi.yml
- flows:
  - flow: authorizationCode
  name: 3-legged
  source: openapi/autodesk-bim360-issues-openapi.yml
- flows:
  - flow: implicit
  name: 3-legged-implicit
  source: openapi/autodesk-bim360-issues-openapi.yml
scope_count: 17
scope_names:
- user-profile:read
- user:read
- user:write
- viewables:read
- data:read
- data:write
- data:create
- data:search
- bucket:create
- bucket:read
- bucket:update
- bucket:delete
- code:all
- account:read
- account:write
- openid
- data:read:<URN_OF_RESOURCE>
scopes:
- description: The application will be able to read the end user's profile data (not including associated products and services).
  flows: []
  scope: user-profile:read
- description: The application will be able to read the end user's profile data, including associated products and services.
  flows: []
  scope: user:read
- description: The application will be able to create, update, and delete the end user's profile data, including associated products and services.
  flows: []
  scope: user:write
- description: The application will only be able to read the end user's viewable data (e.g., PNG and SVF files) within the Autodesk ecosystem.
  flows: []
  scope: viewables:read
- description: The application will be able to read all the end user's data (viewable and non-viewable) within the Autodesk ecosystem.
  flows: []
  scope: data:read
- description: The application will be able to create, update, and delete data on behalf of the end user within the Autodesk ecosystem.
  flows: []
  scope: data:write
- description: The application will be able to create data on behalf of the end user within the Autodesk ecosystem.
  flows: []
  scope: data:create
- description: The application will be able to search the end user's data within the Autodesk ecosystem.
  flows: []
  scope: data:search
- description: The application will be able to create an OSS bucket it will own.
  flows: []
  scope: bucket:create
- description: The application will be able to read the metadata and list contents for OSS buckets that it has access to.
  flows: []
  scope: bucket:read
- description: The application will be able to set permissions and entitlements for OSS buckets that it has permission to modify.
  flows: []
  scope: bucket:update
- description: The application will be able to delete a bucket that it has permission to delete.
  flows: []
  scope: bucket:delete
- description: The application will be able to author and execute code on behalf of the end user (e.g., scripts processed by the Design Automation API).
  flows: []
  scope: code:all
- description: For Product APIs, the application will be able to read the account data the end user has entitlements to.
  flows: []
  scope: account:read
- description: For Product APIs, the application will be able to update the account data the end user has entitlements to.
  flows: []
  scope: account:write
- description: The application requires this scope to generate an id_token.
  flows: []
  scope: openid
- description: Dynamic scope that allows the client to access only the specific resource with the URN/Object ID specified by <URN_OF_RESOURCE> (a raw urn:adsk.* URN, not Base64 encoded).
  flows: []
  scope: data:read:<URN_OF_RESOURCE>
slug: autodesk-bim360-scopes
source_filename: autodesk-bim360-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\nsource: openapi/autodesk-bim360-account-admin-openapi.yml, openapi/autodesk-bim360-issues-openapi.yml\nschemes:\n- name: 2-legged\n  source: openapi/autodesk-bim360-account-admin-openapi.yml\n  flows:\n  - flow: clientCredentials\n- name: 3-legged-implicit\n  source: openapi/autodesk-bim360-account-admin-openapi.yml\n  flows:\n  - flow: implicit\n- name: 3-legged\n  source: openapi/autodesk-bim360-account-admin-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: 2-legged\n  source: openapi/autodesk-bim360-issues-openapi.yml\n  flows:\n  - flow: clientCredentials\n- name: 3-legged\n  source: openapi/autodesk-bim360-issues-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: 3-legged-implicit\n  source: openapi/autodesk-bim360-issues-openapi.yml\n  flows:\n  - flow: implicit\nscopes:\n- scope: user-profile:read\n  description: The application will\
  \ be able to read the end user's profile data\n    (not including associated products and services).\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: user:read\n  description: The application will be able to read the end user's profile data,\n    including associated products and services.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: user:write\n  description: The application will be able to create, update, and delete the end\n    user's profile data, including associated products and services.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: viewables:read\n  description: The application will only be able to read the end user's viewable\n    data (e.g., PNG and SVF files) within the Autodesk ecosystem.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: data:read\n  description: The application will be able\
  \ to read all the end user's data (viewable\n    and non-viewable) within the Autodesk ecosystem.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: data:write\n  description: The application will be able to create, update, and delete data on\n    behalf of the end user within the Autodesk ecosystem.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: data:create\n  description: The application will be able to create data on behalf of the end user\n    within the Autodesk ecosystem.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: data:search\n  description: The application will be able to search the end user's data within\n    the Autodesk ecosystem.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: bucket:create\n  description: The application will be able to create an OSS bucket it will own.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n\
  - scope: bucket:read\n  description: The application will be able to read the metadata and list contents\n    for OSS buckets that it has access to.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: bucket:update\n  description: The application will be able to set permissions and entitlements for\n    OSS buckets that it has permission to modify.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: bucket:delete\n  description: The application will be able to delete a bucket that it has permission\n    to delete.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: code:all\n  description: The application will be able to author and execute code on behalf\n    of the end user (e.g., scripts processed by the Design Automation API).\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: account:read\n  description: For Product\
  \ APIs, the application will be able to read the account\n    data the end user has entitlements to.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: account:write\n  description: For Product APIs, the application will be able to update the account\n    data the end user has entitlements to.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: openid\n  description: The application requires this scope to generate an id_token.\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n- scope: data:read:<URN_OF_RESOURCE>\n  description: Dynamic scope that allows the client to access only the specific resource\n    with the URN/Object ID specified by <URN_OF_RESOURCE> (a raw urn:adsk.* URN, not\n    Base64 encoded).\n  sources:\n  - https://aps.autodesk.com/en/docs/oauth/v2/developers_guide/scopes/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-bim360/refs/heads/main/scopes/autodesk-bim360-scopes.yml
summary_line: 17 scopes · clientCredentials/implicit/authorizationCode
tags:
- Construction
- Project Management
- BIM
- Document Management
- Field Management
- Issues Tracking
- Cost Management
- Model Coordination
- RFIs
- Checklists
token_urls: []
---
