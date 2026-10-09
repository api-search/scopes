---
api_specs:
- filename: weidmueller-variable-nats-asyncapi.yml
  format: yaml
  label: Weidmüller u-OS Data Hub Variable-NATS API
  slug: u-os-data-hub-variable-nats-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/asyncapi/weidmueller-variable-nats-asyncapi.yml
- filename: weidmueller-consumer-api-openapi.yml
  format: yaml
  label: Weidmüller Consumer API
  slug: weidmueller-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-consumer-api-openapi.yml
- filename: weidmueller-firewall-api-openapi.yml
  format: yaml
  label: Weidmüller Firewall API
  slug: weidmueller-firewall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-firewall-api-openapi.yml
- filename: weidmueller-logging-api-openapi.yml
  format: yaml
  label: Weidmüller Logging API
  slug: weidmueller-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-logging-api-openapi.yml
- filename: weidmueller-network-api-openapi.yml
  format: yaml
  label: Weidmüller Network API
  slug: weidmueller-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-network-api-openapi.yml
- filename: weidmueller-operations-api-openapi.yml
  format: yaml
  label: Weidmüller Operations API
  slug: weidmueller-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-operations-api-openapi.yml
- filename: weidmueller-ping-api-openapi.yml
  format: yaml
  label: Weidmüller Ping API
  slug: weidmueller-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-ping-api-openapi.yml
- filename: weidmueller-realtime-api-openapi.yml
  format: yaml
  label: Weidmüller Realtime API
  slug: weidmueller-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-realtime-api-openapi.yml
- filename: weidmueller-recovery-api-openapi.yml
  format: yaml
  label: Weidmüller Recovery API
  slug: weidmueller-recovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-recovery-api-openapi.yml
- filename: weidmueller-security-api-openapi.yml
  format: yaml
  label: Weidmüller Security API
  slug: weidmueller-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-security-api-openapi.yml
- filename: weidmueller-serial-interfaces-api-openapi.yml
  format: yaml
  label: Weidmüller Serial Interfaces API
  slug: weidmueller-serial-interfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-serial-interfaces-api-openapi.yml
- filename: weidmueller-syslog-api-openapi.yml
  format: yaml
  label: Weidmüller Syslog API
  slug: weidmueller-syslog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-syslog-api-openapi.yml
- filename: weidmueller-system-api-openapi.yml
  format: yaml
  label: Weidmüller System API
  slug: weidmueller-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-system-api-openapi.yml
- filename: weidmueller-time-api-openapi.yml
  format: yaml
  label: Weidmüller Time API
  slug: weidmueller-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-time-api-openapi.yml
- filename: weidmueller-update-api-openapi.yml
  format: yaml
  label: Weidmüller Update API
  slug: weidmueller-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-update-api-openapi.yml
- filename: weidmueller-open-api-api-openapi.yml
  format: yaml
  label: Weidmüller Open API
  slug: weidmueller-open-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-open-api-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Weidmueller Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Weidmüller publishes 22 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Weidmüller API on a user''s behalf.


  Tokens are issued from /oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Weidmüller
provider_slug: weidmueller
schemes:
- description: The HTTP API uses the OAuth2 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: OAuth2
  source: openapi/weidmueller-administration-openapi.yml
- description: The HTTP API uses the OAuth2 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: OAuth2
  source: openapi/weidmueller-variable-http-openapi.yml
scope_count: 22
scope_names:
- hub.variables.readonly
- hub.variables.readwrite
- u-os-adm.firewall.readonly
- u-os-adm.firewall.readwrite
- u-os-adm.logging.readonly
- u-os-adm.network.readonly
- u-os-adm.network.readwrite
- u-os-adm.realtime.readonly
- u-os-adm.realtime.readwrite
- u-os-adm.recovery.readwrite
- u-os-adm.security.readonly
- u-os-adm.security.readwrite
- u-os-adm.serial-interfaces.readonly
- u-os-adm.serial-interfaces.readwrite
- u-os-adm.syslog.readonly
- u-os-adm.syslog.readwrite
- u-os-adm.system.readonly
- u-os-adm.system.readwrite
- u-os-adm.time.readonly
- u-os-adm.time.readwrite
- u-os-adm.update.readonly
- u-os-adm.update.readwrite
scopes:
- description: Read-only access to Data Hub variables.
  flows:
  - clientCredentials
  scope: hub.variables.readonly
- description: Read and write access to Data Hub variables.
  flows:
  - clientCredentials
  scope: hub.variables.readwrite
- description: Read access for firewall endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.firewall.readonly
- description: Read and write access for firewall endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.firewall.readwrite
- description: Read access for logging endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.logging.readonly
- description: Read access for network endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.network.readonly
- description: Read and write access for network endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.network.readwrite
- description: Read access for realtime endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.realtime.readonly
- description: Read and write access for realtime endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.realtime.readwrite
- description: Read and write access for recovery endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.recovery.readwrite
- description: Read access for security endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.security.readonly
- description: Read and write access for security endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.security.readwrite
- description: Read access for serial interface configuration endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.serial-interfaces.readonly
- description: Read and write access for serial interface configuration endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.serial-interfaces.readwrite
- description: Read access for syslog endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.syslog.readonly
- description: Read and write access for syslog endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.syslog.readwrite
- description: Read access for system endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.system.readonly
- description: Read and write access for system endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.system.readwrite
- description: Read access for time settings endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.time.readonly
- description: Read and write access for time settings endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.time.readwrite
- description: Read access for update endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.update.readonly
- description: Read and write access for update endpoints
  flows:
  - clientCredentials
  scope: u-os-adm.update.readwrite
slug: weidmueller-scopes
source_filename: weidmueller-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/weidmueller-administration-openapi.yml, openapi/weidmueller-variable-http-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/weidmueller-administration-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n  description: The HTTP API uses the OAuth2 client credentials flow.\n- name: OAuth2\n  source: openapi/weidmueller-variable-http-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n  description: The HTTP API uses the OAuth2 client credentials flow.\nscopes:\n- scope: hub.variables.readonly\n  description: Read-only access to Data Hub variables.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-variable-http-openapi.yml\n- scope: hub.variables.readwrite\n  description: Read and write access to Data Hub variables.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-variable-http-openapi.yml\n- scope: u-os-adm.firewall.readonly\n\
  \  description: Read access for firewall endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.firewall.readwrite\n  description: Read and write access for firewall endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.logging.readonly\n  description: Read access for logging endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.network.readonly\n  description: Read access for network endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.network.readwrite\n  description: Read and write access for network endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.realtime.readonly\n  description: Read access for realtime endpoints\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.realtime.readwrite\n  description: Read and write access for realtime endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.recovery.readwrite\n  description: Read and write access for recovery endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.security.readonly\n  description: Read access for security endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.security.readwrite\n  description: Read and write access for security endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.serial-interfaces.readonly\n  description: Read access for serial interface configuration endpoints\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.serial-interfaces.readwrite\n  description: Read and write access for serial interface configuration endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.syslog.readonly\n  description: Read access for syslog endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.syslog.readwrite\n  description: Read and write access for syslog endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.system.readonly\n  description: Read access for system endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.system.readwrite\n  description: Read and write access for system endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n\
  - scope: u-os-adm.time.readonly\n  description: Read access for time settings endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.time.readwrite\n  description: Read and write access for time settings endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.update.readonly\n  description: Read access for update endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n- scope: u-os-adm.update.readwrite\n  description: Read and write access for update endpoints\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/weidmueller-administration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/scopes/weidmueller-scopes.yml
summary_line: 22 scopes · clientCredentials
tags:
- Company
- Industrial Automation
- Industrial Connectivity
- Edge Computing
- IIoT
- u-OS
- Manufacturing
token_bound: false
token_urls:
- /oauth2/token
---
