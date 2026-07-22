---
api_specs:
- filename: sign-in-enterprise-guest-api-openapi-original.yml
  format: yaml
  label: Sign In Solutions VMS API
  slug: sign-in-solutions-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sign-in-enterprise/refs/heads/main/openapi/sign-in-enterprise-guest-api-openapi-original.yml
authorization_urls:
- https://us.tractionguest.com/oauth/authorize
description: ''
docs: https://developers.signinenterprise.com/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sign In Enterprise Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sign In Enterprise publishes 48 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sign In Enterprise API on a user''s behalf.


  Tokens are issued from https://us.tractionguest.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sign In Enterprise
provider_slug: sign-in-enterprise
schemes:
- flows:
  - authorizationUrl: https://us.tractionguest.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://us.tractionguest.com/oauth/token
  name: TractionGuestAuth
  source: well-known/sign-in-enterprise-openid-configuration.json
  type: openIdConnect
scope_count: 48
scope_names:
- openid
- all
- admin:webhooks
- admin:workflow_triggers:*
- admin:workflow_triggers:read
- admin:workflow_triggers:write
- admin:workflow_emails:*
- admin:workflow_emails:read
- admin:workflow_emails:write
- audit_logs:*
- audit_logs:read
- batch_jobs:*
- batch_jobs:read
- batch_jobs:write
- custom_fields:*
- custom_fields:read
- custom_fields:write
- devices:*
- devices:read
- devices:write
- watchlists:*
- watchlists:read
- watchlists:write
- screening_providers:*
- screening_providers:read
- screening_providers:write
- users:*
- users:read
- users:write
- visitors:*
- visitors:read
- visitors:write
- parking:*
- parking:read
- parking:write
- locations:*
- locations:read
- locations:write
- hosts:*
- hosts:read
- hosts:write
- email_templates:*
- email_templates:read
- email_templates:write
- registrations:*
- registrations:read
- capacities:*
- capacities:read
scopes:
- description: OpenID Connect authentication
  flows: []
  scope: openid
- description: Full access to all authorized resources
  flows: []
  scope: all
- description: Manage webhook subscriptions
  flows: []
  scope: admin:webhooks
- description: Full access to workflow triggers
  flows: []
  scope: admin:workflow_triggers:*
- description: Read workflow triggers
  flows: []
  scope: admin:workflow_triggers:read
- description: Create and update workflow triggers
  flows: []
  scope: admin:workflow_triggers:write
- description: Full access to workflow emails
  flows: []
  scope: admin:workflow_emails:*
- description: Read workflow emails
  flows: []
  scope: admin:workflow_emails:read
- description: Create and update workflow emails
  flows: []
  scope: admin:workflow_emails:write
- description: Full access to audit logs
  flows: []
  scope: audit_logs:*
- description: Read audit logs
  flows: []
  scope: audit_logs:read
- description: Full access to batch jobs
  flows: []
  scope: batch_jobs:*
- description: Read batch jobs
  flows: []
  scope: batch_jobs:read
- description: Create batch jobs
  flows: []
  scope: batch_jobs:write
- description: Full access to custom fields
  flows: []
  scope: custom_fields:*
- description: Read custom fields
  flows: []
  scope: custom_fields:read
- description: Create and update custom fields
  flows: []
  scope: custom_fields:write
- description: Full access to devices
  flows: []
  scope: devices:*
- description: Read devices
  flows: []
  scope: devices:read
- description: Create and update devices
  flows: []
  scope: devices:write
- description: Full access to watchlists
  flows: []
  scope: watchlists:*
- description: Read watchlists
  flows: []
  scope: watchlists:read
- description: Create and update watchlists
  flows: []
  scope: watchlists:write
- description: Full access to screening providers
  flows: []
  scope: screening_providers:*
- description: Read screening providers
  flows: []
  scope: screening_providers:read
- description: Configure screening providers
  flows: []
  scope: screening_providers:write
- description: Full access to users
  flows: []
  scope: users:*
- description: Read users
  flows: []
  scope: users:read
- description: Create and update users
  flows: []
  scope: users:write
- description: Full access to visitors
  flows: []
  scope: visitors:*
- description: Read visitors and sign-ins
  flows: []
  scope: visitors:read
- description: Create and update visitors and sign-ins
  flows: []
  scope: visitors:write
- description: Full access to parking
  flows: []
  scope: parking:*
- description: Read parking lots and stalls
  flows: []
  scope: parking:read
- description: Manage parking allocations
  flows: []
  scope: parking:write
- description: Full access to locations
  flows: []
  scope: locations:*
- description: Read locations
  flows: []
  scope: locations:read
- description: Create and update locations
  flows: []
  scope: locations:write
- description: Full access to hosts
  flows: []
  scope: hosts:*
- description: Read hosts
  flows: []
  scope: hosts:read
- description: Create and update hosts
  flows: []
  scope: hosts:write
- description: Full access to email templates
  flows: []
  scope: email_templates:*
- description: Read email templates
  flows: []
  scope: email_templates:read
- description: Create and update email templates
  flows: []
  scope: email_templates:write
- description: Full access to registrations
  flows: []
  scope: registrations:*
- description: Read registrations
  flows: []
  scope: registrations:read
- description: Full access to capacity data
  flows: []
  scope: capacities:*
- description: Read location capacities and forecasts
  flows: []
  scope: capacities:read
slug: sign-in-enterprise-scopes
source_filename: sign-in-enterprise-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sign-in-enterprise-guest-api-openapi-original.yml\ndocs: https://developers.signinenterprise.com/\nreference: well-known/sign-in-enterprise-openid-configuration.json\nschemes:\n- name: TractionGuestAuth\n  type: openIdConnect\n  source: well-known/sign-in-enterprise-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us.tractionguest.com/oauth/authorize\n    tokenUrl: https://us.tractionguest.com/oauth/token\n# scopes_supported harvested verbatim from the live OpenID Connect discovery document\nscopes:\n- {scope: openid, description: OpenID Connect authentication}\n- {scope: all, description: Full access to all authorized resources}\n- {scope: 'admin:webhooks', description: Manage webhook subscriptions}\n- {scope: 'admin:workflow_triggers:*', description: Full access to workflow triggers}\n- {scope: 'admin:workflow_triggers:read', description: Read workflow triggers}\n- {scope:\
  \ 'admin:workflow_triggers:write', description: Create and update workflow triggers}\n- {scope: 'admin:workflow_emails:*', description: Full access to workflow emails}\n- {scope: 'admin:workflow_emails:read', description: Read workflow emails}\n- {scope: 'admin:workflow_emails:write', description: Create and update workflow emails}\n- {scope: 'audit_logs:*', description: Full access to audit logs}\n- {scope: 'audit_logs:read', description: Read audit logs}\n- {scope: 'batch_jobs:*', description: Full access to batch jobs}\n- {scope: 'batch_jobs:read', description: Read batch jobs}\n- {scope: 'batch_jobs:write', description: Create batch jobs}\n- {scope: 'custom_fields:*', description: Full access to custom fields}\n- {scope: 'custom_fields:read', description: Read custom fields}\n- {scope: 'custom_fields:write', description: Create and update custom fields}\n- {scope: 'devices:*', description: Full access to devices}\n- {scope: 'devices:read', description: Read devices}\n- {scope: 'devices:write',\
  \ description: Create and update devices}\n- {scope: 'watchlists:*', description: Full access to watchlists}\n- {scope: 'watchlists:read', description: Read watchlists}\n- {scope: 'watchlists:write', description: Create and update watchlists}\n- {scope: 'screening_providers:*', description: Full access to screening providers}\n- {scope: 'screening_providers:read', description: Read screening providers}\n- {scope: 'screening_providers:write', description: Configure screening providers}\n- {scope: 'users:*', description: Full access to users}\n- {scope: 'users:read', description: Read users}\n- {scope: 'users:write', description: Create and update users}\n- {scope: 'visitors:*', description: Full access to visitors}\n- {scope: 'visitors:read', description: Read visitors and sign-ins}\n- {scope: 'visitors:write', description: Create and update visitors and sign-ins}\n- {scope: 'parking:*', description: Full access to parking}\n- {scope: 'parking:read', description: Read parking lots and stalls}\n\
  - {scope: 'parking:write', description: Manage parking allocations}\n- {scope: 'locations:*', description: Full access to locations}\n- {scope: 'locations:read', description: Read locations}\n- {scope: 'locations:write', description: Create and update locations}\n- {scope: 'hosts:*', description: Full access to hosts}\n- {scope: 'hosts:read', description: Read hosts}\n- {scope: 'hosts:write', description: Create and update hosts}\n- {scope: 'email_templates:*', description: Full access to email templates}\n- {scope: 'email_templates:read', description: Read email templates}\n- {scope: 'email_templates:write', description: Create and update email templates}\n- {scope: 'registrations:*', description: Full access to registrations}\n- {scope: 'registrations:read', description: Read registrations}\n- {scope: 'capacities:*', description: Full access to capacity data}\n- {scope: 'capacities:read', description: Read location capacities and forecasts}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sign-in-enterprise/refs/heads/main/scopes/sign-in-enterprise-scopes.yml
summary_line: 48 scopes · authorizationCode
tags:
- Company
- Vertical Software
- Visitor Management
- Physical Security
- Workplace Experience
- Identity
- Compliance
- Access Control
token_urls:
- https://us.tractionguest.com/oauth/token
---
