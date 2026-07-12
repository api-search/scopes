---
authorization_urls: []
description: ''
docs: https://pan.dev/sase/docs/scope/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Palo Alto Networks Scopes
name_suffix: OAuth Scopes
note: Prisma SASE OAuth 2.0 (client_credentials) uses the scope field solely to name the target Tenant Service Group (tsg_id:<TSG_ID>); there is no catalog of named permission scopes, and API permissions are instead governed by IAM roles assigned to the service account (https://pan.dev/sase/docs/scope/).
overview: 'Palo Alto Networks publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Palo Alto Networks API on a user''s behalf.


  Tokens are issued from https://auth.apps.paloaltonetworks.com/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schemes:
- description: OAuth 2.0 client credentials flow for obtaining an access token. Requires a client ID and client secret from the Palo Alto Networks SASE identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.apps.paloaltonetworks.com/oauth2/access_token
  name: oauth2
  source: openapi/palo-alto-autonomous-dem-api-openapi-original.yml
- description: OAuth 2.0 client credentials flow for obtaining an access token. Requires a client ID and client secret from the Palo Alto Networks SASE identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.apps.paloaltonetworks.com/oauth2/access_token
  name: oauth2
  source: openapi/palo-alto-prisma-access-api-openapi-original.yml
- description: OAuth 2.0 client credentials flow for obtaining an access token. Requires a client ID and client secret from the Palo Alto Networks SASE identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.apps.paloaltonetworks.com/oauth2/access_token
  name: oauth2
  source: openapi/palo-alto-prisma-sd-wan-api-openapi-original.yml
scope_count: 1
scope_names:
- tsg_id:<TSG_ID>
scopes:
- description: Scopes the access token to a single Tenant Service Group (TSG), identified by its 10-digit TSG ID (e.g. scope=tsg_id:1838006364). The service account used to authenticate must belong to the named TSG or an ancestor of it; all API requests made with the token are routed to that tenant. This is the only scope form the Prisma SASE Authentication Service documents.
  flows: []
  scope: tsg_id:<TSG_ID>
slug: palo-alto-networks-scopes
source_filename: palo-alto-networks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://pan.dev/sase/docs/scope/\nsource: openapi/palo-alto-autonomous-dem-api-openapi-original.yml, openapi/palo-alto-prisma-access-api-openapi-original.yml,\n  openapi/palo-alto-prisma-sd-wan-api-openapi-original.yml\nschemes:\n- name: oauth2\n  source: openapi/palo-alto-autonomous-dem-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.apps.paloaltonetworks.com/oauth2/access_token\n  description: OAuth 2.0 client credentials flow for obtaining an access token. Requires a client\n    ID and client secret from the Palo Alto Networks SASE identity provider.\n- name: oauth2\n  source: openapi/palo-alto-prisma-access-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.apps.paloaltonetworks.com/oauth2/access_token\n  description: OAuth 2.0 client credentials flow for obtaining an access token. Requires a client\n    ID and client secret from the Palo\
  \ Alto Networks SASE identity provider.\n- name: oauth2\n  source: openapi/palo-alto-prisma-sd-wan-api-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.apps.paloaltonetworks.com/oauth2/access_token\n  description: OAuth 2.0 client credentials flow for obtaining an access token. Requires a client\n    ID and client secret from the Palo Alto Networks SASE identity provider.\nscopes:\n- scope: tsg_id:<TSG_ID>\n  description: Scopes the access token to a single Tenant Service Group (TSG), identified by its\n    10-digit TSG ID (e.g. scope=tsg_id:1838006364). The service account used to authenticate must\n    belong to the named TSG or an ancestor of it; all API requests made with the token are routed\n    to that tenant. This is the only scope form the Prisma SASE Authentication Service documents.\n  sources:\n  - https://pan.dev/sase/docs/scope/\n  - https://pan.dev/sase/docs/access-tokens/\nnote: Prisma SASE OAuth 2.0 (client_credentials) uses the scope\
  \ field solely to name the target\n  Tenant Service Group (tsg_id:<TSG_ID>); there is no catalog of named permission scopes, and API\n  permissions are instead governed by IAM roles assigned to the service account\n  (https://pan.dev/sase/docs/scope/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/scopes/palo-alto-networks-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
token_urls:
- https://auth.apps.paloaltonetworks.com/oauth2/access_token
---
