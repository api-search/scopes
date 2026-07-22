---
api_specs:
- filename: synack-monolith-v1-openapi.yaml
  format: yaml
  label: Synack Enterprise API (Monolith v1)
  slug: synack-enterprise-api-monolith-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-monolith-v1-openapi.yaml
- filename: synack-monolith-v2-openapi.yaml
  format: yaml
  label: Synack Client API (Monolith v2)
  slug: synack-client-api-monolith-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-monolith-v2-openapi.yaml
- filename: synack-assessment-v1-openapi.yaml
  format: yaml
  label: Synack Assessment Service
  slug: synack-assessment-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-assessment-v1-openapi.yaml
- filename: synack-asset-v2-openapi.yaml
  format: yaml
  label: Synack Asset Service
  slug: synack-asset-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-asset-v2-openapi.yaml
- filename: synack-asset-discovery-openapi.yaml
  format: yaml
  label: Synack Asset Discovery Service
  slug: synack-asset-discovery-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-asset-discovery-openapi.yaml
- filename: synack-mission-v2-openapi.yaml
  format: yaml
  label: Synack Mission Service v2
  slug: synack-mission-service-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-mission-v2-openapi.yaml
- filename: synack-vulns-openapi.yaml
  format: yaml
  label: Synack Vulnerability Service
  slug: synack-vulnerability-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-vulns-openapi.yaml
- filename: synack-tagging-openapi.yaml
  format: yaml
  label: Synack Tagging Service
  slug: synack-tagging-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-tagging-openapi.yaml
- filename: synack-streaming-openapi.yaml
  format: yaml
  label: Synack Streaming Service
  slug: synack-streaming-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-streaming-openapi.yaml
authorization_urls:
- login.synack.com
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Synack Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Synack publishes 21 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Synack API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Synack
provider_slug: synack
schemes:
- flows:
  - authorizationUrl: login.synack.com
    flow: implicit
  name: OAuth2
  source: openapi/synack-asset-discovery-openapi.yaml
- flows:
  - authorizationUrl: login.synack.com
    flow: implicit
  name: OAuth2
  source: openapi/synack-asset-v2-openapi.yaml
- flows:
  - authorizationUrl: login.synack.com
    flow: implicit
  name: OAuth2
  source: openapi/synack-tagging-openapi.yaml
- flows:
  - authorizationUrl: login.synack.com
    flow: implicit
  name: OAuth2
  source: openapi/synack-vulns-openapi.yaml
scope_count: 21
scope_names:
- asset_boss_lw
- asset_boss_ow
- asset_client_lw
- asset_client_ow
- asset_gr
- asset_gw
- asset_lr
- asset_or
- asset_scan_gr
- asset_srt_lr
- asset_user_or
- assetdiscovery_gr
- assetdiscovery_lr
- assetdiscovery_or
- assetdiscovery_ow
- tag_gr
- tag_gw
- tag_lr
- tag_lw
- tag_or
- tag_ow
scopes:
- description: Grants per-listing write access to assets that may be modified by BOSS users.
  flows:
  - implicit
  scope: asset_boss_lw
- description: Grants organization-level access to assets owned by a particular organization that may be modified by BOSS users.
  flows:
  - implicit
  scope: asset_boss_ow
- description: Grants listing-level to write seed groups and seeds.
  flows:
  - implicit
  scope: asset_client_lw
- description: Grants organization-level access to assets owned by a particular organization that may be modified by Client users.
  flows:
  - implicit
  scope: asset_client_ow
- description: Grants unrestricted read access to all assets. Except for credential data of cloud accout assets.
  flows:
  - implicit
  scope: asset_gr
- description: Grants unrestricted write access to all assets.
  flows:
  - implicit
  scope: asset_gw
- description: Grants per-listing read access for all types of assets.
  flows:
  - implicit
  scope: asset_lr
- description: Grants organization-level read access for all types of assets owned by a particular organization.
  flows:
  - implicit
  scope: asset_or
- description: Grants unrestricted read access to all assets. Including credential data of cloud account assets.
  flows:
  - implicit
  scope: asset_scan_gr
- description: Grants per-listing read access to assets that may be read by SRTs.
  flows:
  - implicit
  scope: asset_srt_lr
- description: Grants user-level read access to asset stats that owned by a particular organization.
  flows:
  - implicit
  scope: asset_user_or
- description: Grants global-level to read seed groups and seeds.
  flows:
  - implicit
  scope: assetdiscovery_gr
- description: Grants listing-level to read seed groups and seeds.
  flows:
  - implicit
  scope: assetdiscovery_lr
- description: Grants organization-level to read seed groups and seeds.
  flows:
  - implicit
  scope: assetdiscovery_or
- description: Grants organization-level to create or modify seed groups and seeds.
  flows:
  - implicit
  scope: assetdiscovery_ow
- description: Grants global-level to read tags.
  flows:
  - implicit
  scope: tag_gr
- description: Grants global-level to create or modify tags.
  flows:
  - implicit
  scope: tag_gw
- description: ''
  flows: []
  scope: tag_lr
- description: ''
  flows: []
  scope: tag_lw
- description: Grants organization-level to read tags.
  flows:
  - implicit
  scope: tag_or
- description: Grants organization-level to create or modify tags.
  flows:
  - implicit
  scope: tag_ow
slug: synack-scopes
source_filename: synack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/synack-asset-discovery-openapi.yaml, openapi/synack-asset-v2-openapi.yaml, openapi/synack-tagging-openapi.yaml,\n  openapi/synack-vulns-openapi.yaml\nschemes:\n- name: OAuth2\n  source: openapi/synack-asset-discovery-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: login.synack.com\n- name: OAuth2\n  source: openapi/synack-asset-v2-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: login.synack.com\n- name: OAuth2\n  source: openapi/synack-tagging-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: login.synack.com\n- name: OAuth2\n  source: openapi/synack-vulns-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: login.synack.com\nscopes:\n- scope: asset_boss_lw\n  description: Grants per-listing write access to assets that may be modified by BOSS users.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-tagging-openapi.yaml\n\
  \  - openapi/synack-vulns-openapi.yaml\n- scope: asset_boss_ow\n  description: Grants organization-level access to assets owned by a particular organization\n    that may be modified by BOSS users.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-tagging-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- scope: asset_client_lw\n  description: Grants listing-level to write seed groups and seeds.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-discovery-openapi.yaml\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-tagging-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- scope: asset_client_ow\n  description: Grants organization-level access to assets owned by a particular organization\n    that may be modified by Client users.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-tagging-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- scope: asset_gr\n\
  \  description: Grants unrestricted read access to all assets. Except for credential data of\n    cloud accout assets.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-tagging-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- scope: asset_gw\n  description: Grants unrestricted write access to all assets.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-tagging-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- scope: asset_lr\n  description: Grants per-listing read access for all types of assets.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-tagging-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- scope: asset_or\n  description: Grants organization-level read access for all types of assets owned by a particular\n    organization.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-tagging-openapi.yaml\n\
  \  - openapi/synack-vulns-openapi.yaml\n- scope: asset_scan_gr\n  description: Grants unrestricted read access to all assets. Including credential data of cloud\n    account assets.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- scope: asset_srt_lr\n  description: Grants per-listing read access to assets that may be read by SRTs.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- scope: asset_user_or\n  description: Grants user-level read access to asset stats that owned by a particular organization.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- scope: assetdiscovery_gr\n  description: Grants global-level to read seed groups and seeds.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-discovery-openapi.yaml\n- scope: assetdiscovery_lr\n  description: Grants listing-level\
  \ to read seed groups and seeds.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-discovery-openapi.yaml\n- scope: assetdiscovery_or\n  description: Grants organization-level to read seed groups and seeds.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-discovery-openapi.yaml\n- scope: assetdiscovery_ow\n  description: Grants organization-level to create or modify seed groups and seeds.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-asset-discovery-openapi.yaml\n- scope: tag_gr\n  description: Grants global-level to read tags.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-tagging-openapi.yaml\n- scope: tag_gw\n  description: Grants global-level to create or modify tags.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-tagging-openapi.yaml\n- scope: tag_lr\n  sources:\n  - openapi/synack-tagging-openapi.yaml\n- scope: tag_lw\n  sources:\n  - openapi/synack-tagging-openapi.yaml\n- scope: tag_or\n  description: Grants organization-level\
  \ to read tags.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-tagging-openapi.yaml\n- scope: tag_ow\n  description: Grants organization-level to create or modify tags.\n  flows:\n  - implicit\n  sources:\n  - openapi/synack-tagging-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/scopes/synack-scopes.yml
summary_line: 21 scopes · implicit
tags:
- Company
- Security
- Penetration Testing
- Vulnerability Management
- Attack Surface Management
- Crowdsourced Security
- Compliance
- API
token_urls: []
---
