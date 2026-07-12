---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sentinel Hub Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sentinel Hub publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sentinel Hub API on a user''s behalf.


  Tokens are issued from https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sentinel Hub
provider_slug: sentinel-hub
schemes:
- description: "### Authentication\n\nMore about the authentication <a href=\"https://docs.planet.com/develop/authentication/\" target=\"_blank\">here</a>.\n\nTo get an access token using curl:\n\n```\ncurl --request POST \\\n  --url https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token \\\n  --header \"content-type: application/x-www-form-urlencoded\" \\\n  --data \"grant_type=client_credentials&client_id=<your client id>&client_secret=<your client secret>\"\n```"
  flows:
  - flow: clientCredentials
    tokenUrl: https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token
  name: OAuth2
  source: openapi/sentinel-hub-openapi.yaml
scope_count: 1
scope_names:
- SH
scopes:
- description: Sentinel Hub
  flows:
  - clientCredentials
  scope: SH
slug: sentinel-hub-scopes
source_filename: sentinel-hub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sentinel-hub-openapi.yaml\nschemes:\n- name: OAuth2\n  source: openapi/sentinel-hub-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token\n  description: |-\n    ### Authentication\n\n    More about the authentication <a href=\"https://docs.planet.com/develop/authentication/\" target=\"_blank\">here</a>.\n\n    To get an access token using curl:\n\n    ```\n    curl --request POST \\\n      --url https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token \\\n      --header \"content-type: application/x-www-form-urlencoded\" \\\n      --data \"grant_type=client_credentials&client_id=<your client id>&client_secret=<your client secret>\"\n    ```\nscopes:\n- scope: SH\n  description: Sentinel Hub\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sentinel-hub-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentinel-hub/refs/heads/main/scopes/sentinel-hub-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Satellite Imagery
- Geospatial
- Remote Sensing
- Earth Observation
- NDVI
- Sentinel
- Landsat
- MODIS
- OGC
- STAC
token_urls:
- https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token
---
