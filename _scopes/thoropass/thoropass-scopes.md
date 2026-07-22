---
authorization_urls:
- https://app.thoropass.com/partner-api
description: ''
docs: https://docs.thoropass.com/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Thoropass Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Thoropass publishes 24 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Thoropass API on a user''s behalf.


  Tokens are issued from https://api.thoropass.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Thoropass
provider_slug: thoropass
schemes:
- flows:
  - authorizationUrl: https://app.thoropass.com/partner-api
    flow: authorizationCode
    tokenUrl: https://api.thoropass.com/oauth/token/
  name: OAuth2
  source: https://api.thoropass.com/.well-known/oauth-authorization-server
scope_count: 24
scope_names:
- alertConfiguration:read
- alertConfiguration:write
- alertEvent:read
- alertEvent:write
- integrationUser:read
- integrationUser:write
- device:read
- device:write
- changeRequest:read
- changeRequest:write
- training:read
- training:write
- vulnerabilityScanConfiguration:read
- vulnerabilityScanConfiguration:write
- vulnerabilityScan:read
- vulnerabilityScan:write
- vulnerability:read
- vulnerability:write
- audit:read
- audit:write
- evidenceRequest:read
- evidenceRequest:write
- globalControl:read
- mcp:invoke
scopes:
- description: Read compliance monitoring alert configurations
  flows: []
  scope: alertConfiguration:read
- description: Manage compliance monitoring alert configurations
  flows: []
  scope: alertConfiguration:write
- description: Read triggered monitoring alert events
  flows: []
  scope: alertEvent:read
- description: Manage/acknowledge monitoring alert events
  flows: []
  scope: alertEvent:write
- description: Read integration (service) user records
  flows: []
  scope: integrationUser:read
- description: Manage integration (service) user records
  flows: []
  scope: integrationUser:write
- description: Read managed device / endpoint inventory
  flows: []
  scope: device:read
- description: Manage device / endpoint inventory records
  flows: []
  scope: device:write
- description: Read change requests
  flows: []
  scope: changeRequest:read
- description: Create or update change requests
  flows: []
  scope: changeRequest:write
- description: Read security-awareness training records
  flows: []
  scope: training:read
- description: Manage security-awareness training records
  flows: []
  scope: training:write
- description: Read vulnerability-scan configurations
  flows: []
  scope: vulnerabilityScanConfiguration:read
- description: Manage vulnerability-scan configurations
  flows: []
  scope: vulnerabilityScanConfiguration:write
- description: Read vulnerability scans
  flows: []
  scope: vulnerabilityScan:read
- description: Trigger or manage vulnerability scans
  flows: []
  scope: vulnerabilityScan:write
- description: Read discovered vulnerabilities
  flows: []
  scope: vulnerability:read
- description: Manage / triage discovered vulnerabilities
  flows: []
  scope: vulnerability:write
- description: Read audit records and audit lifecycle state
  flows: []
  scope: audit:read
- description: Manage audit records and audit lifecycle
  flows: []
  scope: audit:write
- description: Read auditor evidence requests
  flows: []
  scope: evidenceRequest:read
- description: Fulfill / respond to auditor evidence requests
  flows: []
  scope: evidenceRequest:write
- description: Read the global control library
  flows: []
  scope: globalControl:read
- description: Invoke tools on the Thoropass hosted MCP server
  flows: []
  scope: mcp:invoke
slug: thoropass-scopes
source_filename: thoropass-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.thoropass.com/.well-known/oauth-authorization-server\ndocs: https://docs.thoropass.com/mcp\nschemes:\n- name: OAuth2\n  source: https://api.thoropass.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.thoropass.com/partner-api\n    tokenUrl: https://api.thoropass.com/oauth/token/\nscopes:\n- {scope: 'alertConfiguration:read',  description: Read compliance monitoring alert configurations}\n- {scope: 'alertConfiguration:write', description: Manage compliance monitoring alert configurations}\n- {scope: 'alertEvent:read',          description: Read triggered monitoring alert events}\n- {scope: 'alertEvent:write',         description: Manage/acknowledge monitoring alert events}\n- {scope: 'integrationUser:read',     description: Read integration (service) user records}\n- {scope: 'integrationUser:write',    description: Manage integration (service) user\
  \ records}\n- {scope: 'device:read',              description: Read managed device / endpoint inventory}\n- {scope: 'device:write',             description: Manage device / endpoint inventory records}\n- {scope: 'changeRequest:read',       description: Read change requests}\n- {scope: 'changeRequest:write',      description: Create or update change requests}\n- {scope: 'training:read',            description: Read security-awareness training records}\n- {scope: 'training:write',           description: Manage security-awareness training records}\n- {scope: 'vulnerabilityScanConfiguration:read',  description: Read vulnerability-scan configurations}\n- {scope: 'vulnerabilityScanConfiguration:write', description: Manage vulnerability-scan configurations}\n- {scope: 'vulnerabilityScan:read',   description: Read vulnerability scans}\n- {scope: 'vulnerabilityScan:write',  description: Trigger or manage vulnerability scans}\n- {scope: 'vulnerability:read',        description: Read discovered vulnerabilities}\n\
  - {scope: 'vulnerability:write',       description: Manage / triage discovered vulnerabilities}\n- {scope: 'audit:read',                description: Read audit records and audit lifecycle state}\n- {scope: 'audit:write',               description: Manage audit records and audit lifecycle}\n- {scope: 'evidenceRequest:read',      description: Read auditor evidence requests}\n- {scope: 'evidenceRequest:write',     description: Fulfill / respond to auditor evidence requests}\n- {scope: 'globalControl:read',        description: Read the global control library}\n- {scope: 'mcp:invoke',                description: Invoke tools on the Thoropass hosted MCP server}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thoropass/refs/heads/main/scopes/thoropass-scopes.yml
summary_line: 24 scopes · authorizationCode
tags:
- Company
- Fintech
- Compliance
- Compliance Automation
- Audit
- Security
- Cybersecurity
- GRC
- SOC 2
- MCP
token_urls:
- https://api.thoropass.com/oauth/token/
---
