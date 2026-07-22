---
authorization_urls:
- https://id.planday.com/connect/authorize
description: ''
docs: https://openapi.planday.com/gettingstarted/authorization-flow/
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Planday Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Planday publishes 78 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Planday API on a user''s behalf.


  Tokens are issued from https://id.planday.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Planday
provider_slug: planday
schemes:
- flows:
  - authorizationUrl: https://id.planday.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://id.planday.com/connect/token
  - flow: clientCredentials
    tokenUrl: https://id.planday.com/connect/token
  - flow: refreshToken
    tokenUrl: https://id.planday.com/connect/token
  name: OAuth2
  source: https://id.planday.com/.well-known/openid-configuration
  type: oauth2
scope_count: 78
scope_names:
- openid
- plandayid
- email
- offline_access
- employee:read
- employee:create
- employee:update
- employee:deactivate
- employee:history
- employeetype:read
- employeegroup:read
- employeegroup:create
- employeegroup:update
- employeegroup:delete
- department:read
- department:create
- department:update
- department:delete
- skill:read
- skill:create
- skill:update
- skill:delete
- bankaccount:read
- bankaccount:create
- bankaccount:update
- birthdate:read
- birthdate:create
- birthdate:update
- ssn:read
- ssn:create
- ssn:update
- shift:read
- shift:create
- shift:update
- shift:delete
- shifttype:read
- shifttype:create
- shifttype:delete
- shiftposition:read
- shiftposition:create
- shiftposition:update
- shiftposition:delete
- timeandcost:read
- punchclockshift:read
- punchclockshift:create
- punchclockkioskdevice:read
- punchclockkioskdevice:create
- punchclockkioskdevice:delete
- punchclockkioskprofile:read
- punchclockkioskprofile:create
- absence:read
- absence:create
- absence:update
- absencesettings:read
- absencesettings:create
- absencesettings:update
- absencesettings:delete
- revenue:read
- revenue:set
- revenue:update
- revenue:delete
- payroll:read
- payrates:read
- payrates:update
- salaries:read
- salaries:update
- contractrules:read
- contractrules:update
- portal:create
- securitygroups:read
- securitygroupmembership:read
- securitygroupmembership:update
- securitygroupmembership:delete
- datacenter:read
- datacenter:create
- platform_access_token
- access_token
- impersonate
scopes:
- description: OpenID Connect authentication
  flows: []
  scope: openid
- description: Planday identity claim
  flows: []
  scope: plandayid
- description: Access the user email claim
  flows: []
  scope: email
- description: Issue a refresh token for long-lived access
  flows: []
  scope: offline_access
- description: Read employee details
  flows: []
  scope: employee:read
- description: Create employees
  flows: []
  scope: employee:create
- description: Update employee details
  flows: []
  scope: employee:update
- description: Deactivate employees
  flows: []
  scope: employee:deactivate
- description: Read employee history
  flows: []
  scope: employee:history
- description: Read employee types
  flows: []
  scope: employeetype:read
- description: Read employee groups
  flows: []
  scope: employeegroup:read
- description: Create employee groups
  flows: []
  scope: employeegroup:create
- description: Update employee groups
  flows: []
  scope: employeegroup:update
- description: Delete employee groups
  flows: []
  scope: employeegroup:delete
- description: Read departments
  flows: []
  scope: department:read
- description: Create departments
  flows: []
  scope: department:create
- description: Update departments
  flows: []
  scope: department:update
- description: Delete departments
  flows: []
  scope: department:delete
- description: Read skills
  flows: []
  scope: skill:read
- description: Create skills
  flows: []
  scope: skill:create
- description: Update skills
  flows: []
  scope: skill:update
- description: Delete skills
  flows: []
  scope: skill:delete
- description: Read employee bank account details
  flows: []
  scope: bankaccount:read
- description: Create employee bank account details
  flows: []
  scope: bankaccount:create
- description: Update employee bank account details
  flows: []
  scope: bankaccount:update
- description: Read employee birthdate
  flows: []
  scope: birthdate:read
- description: Set employee birthdate
  flows: []
  scope: birthdate:create
- description: Update employee birthdate
  flows: []
  scope: birthdate:update
- description: Read employee social security number
  flows: []
  scope: ssn:read
- description: Set employee social security number
  flows: []
  scope: ssn:create
- description: Update employee social security number
  flows: []
  scope: ssn:update
- description: Read scheduled shifts
  flows: []
  scope: shift:read
- description: Create shifts
  flows: []
  scope: shift:create
- description: Update shifts
  flows: []
  scope: shift:update
- description: Delete shifts
  flows: []
  scope: shift:delete
- description: Read shift types
  flows: []
  scope: shifttype:read
- description: Create shift types
  flows: []
  scope: shifttype:create
- description: Delete shift types
  flows: []
  scope: shifttype:delete
- description: Read shift positions
  flows: []
  scope: shiftposition:read
- description: Create shift positions
  flows: []
  scope: shiftposition:create
- description: Update shift positions
  flows: []
  scope: shiftposition:update
- description: Delete shift positions
  flows: []
  scope: shiftposition:delete
- description: Read time and cost data for shifts
  flows: []
  scope: timeandcost:read
- description: Read punch clock shift entries
  flows: []
  scope: punchclockshift:read
- description: Create punch clock shift entries
  flows: []
  scope: punchclockshift:create
- description: Read punch clock kiosk devices
  flows: []
  scope: punchclockkioskdevice:read
- description: Create punch clock kiosk devices
  flows: []
  scope: punchclockkioskdevice:create
- description: Delete punch clock kiosk devices
  flows: []
  scope: punchclockkioskdevice:delete
- description: Read punch clock kiosk profiles
  flows: []
  scope: punchclockkioskprofile:read
- description: Create punch clock kiosk profiles
  flows: []
  scope: punchclockkioskprofile:create
- description: Read absence records
  flows: []
  scope: absence:read
- description: Create absence records
  flows: []
  scope: absence:create
- description: Update absence records
  flows: []
  scope: absence:update
- description: Read absence settings
  flows: []
  scope: absencesettings:read
- description: Create absence settings
  flows: []
  scope: absencesettings:create
- description: Update absence settings
  flows: []
  scope: absencesettings:update
- description: Delete absence settings
  flows: []
  scope: absencesettings:delete
- description: Read revenue data
  flows: []
  scope: revenue:read
- description: Set revenue data
  flows: []
  scope: revenue:set
- description: Update revenue data
  flows: []
  scope: revenue:update
- description: Delete revenue data
  flows: []
  scope: revenue:delete
- description: Read payroll reporting data
  flows: []
  scope: payroll:read
- description: Read employee pay rates
  flows: []
  scope: payrates:read
- description: Update employee pay rates
  flows: []
  scope: payrates:update
- description: Read employee salaries
  flows: []
  scope: salaries:read
- description: Update employee salaries
  flows: []
  scope: salaries:update
- description: Read employee contract rules
  flows: []
  scope: contractrules:read
- description: Update employee contract rules
  flows: []
  scope: contractrules:update
- description: Create portal connection details
  flows: []
  scope: portal:create
- description: Read security groups
  flows: []
  scope: securitygroups:read
- description: Read security group membership
  flows: []
  scope: securitygroupmembership:read
- description: Update security group membership
  flows: []
  scope: securitygroupmembership:update
- description: Delete security group membership
  flows: []
  scope: securitygroupmembership:delete
- description: Read data center details
  flows: []
  scope: datacenter:read
- description: Create data center details
  flows: []
  scope: datacenter:create
- description: Issue a platform access token
  flows: []
  scope: platform_access_token
- description: Issue an access token
  flows: []
  scope: access_token
- description: Impersonate a user (privileged)
  flows: []
  scope: impersonate
slug: planday-scopes
source_filename: planday-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://id.planday.com/.well-known/openid-configuration\ndocs: https://openapi.planday.com/gettingstarted/authorization-flow/\nnotes: 'Scopes captured verbatim from the OpenID Connect discovery document''s\n  scopes_supported array. Scopes must be selected when an app is created in Planday\n  (Settings -> API access -> Create app); new scopes cannot be added after creation.\n  Descriptions are derived from the resource:action scope naming convention.'\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://id.planday.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.planday.com/connect/authorize\n    tokenUrl: https://id.planday.com/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://id.planday.com/connect/token\n  - flow: refreshToken\n    tokenUrl: https://id.planday.com/connect/token\nscopes:\n- {scope: openid, description: OpenID Connect authentication}\n\
  - {scope: plandayid, description: Planday identity claim}\n- {scope: email, description: Access the user email claim}\n- {scope: offline_access, description: Issue a refresh token for long-lived access}\n- {scope: 'employee:read', description: Read employee details}\n- {scope: 'employee:create', description: Create employees}\n- {scope: 'employee:update', description: Update employee details}\n- {scope: 'employee:deactivate', description: Deactivate employees}\n- {scope: 'employee:history', description: Read employee history}\n- {scope: 'employeetype:read', description: Read employee types}\n- {scope: 'employeegroup:read', description: Read employee groups}\n- {scope: 'employeegroup:create', description: Create employee groups}\n- {scope: 'employeegroup:update', description: Update employee groups}\n- {scope: 'employeegroup:delete', description: Delete employee groups}\n- {scope: 'department:read', description: Read departments}\n- {scope: 'department:create', description: Create departments}\n\
  - {scope: 'department:update', description: Update departments}\n- {scope: 'department:delete', description: Delete departments}\n- {scope: 'skill:read', description: Read skills}\n- {scope: 'skill:create', description: Create skills}\n- {scope: 'skill:update', description: Update skills}\n- {scope: 'skill:delete', description: Delete skills}\n- {scope: 'bankaccount:read', description: Read employee bank account details}\n- {scope: 'bankaccount:create', description: Create employee bank account details}\n- {scope: 'bankaccount:update', description: Update employee bank account details}\n- {scope: 'birthdate:read', description: Read employee birthdate}\n- {scope: 'birthdate:create', description: Set employee birthdate}\n- {scope: 'birthdate:update', description: Update employee birthdate}\n- {scope: 'ssn:read', description: Read employee social security number}\n- {scope: 'ssn:create', description: Set employee social security number}\n- {scope: 'ssn:update', description: Update employee\
  \ social security number}\n- {scope: 'shift:read', description: Read scheduled shifts}\n- {scope: 'shift:create', description: Create shifts}\n- {scope: 'shift:update', description: Update shifts}\n- {scope: 'shift:delete', description: Delete shifts}\n- {scope: 'shifttype:read', description: Read shift types}\n- {scope: 'shifttype:create', description: Create shift types}\n- {scope: 'shifttype:delete', description: Delete shift types}\n- {scope: 'shiftposition:read', description: Read shift positions}\n- {scope: 'shiftposition:create', description: Create shift positions}\n- {scope: 'shiftposition:update', description: Update shift positions}\n- {scope: 'shiftposition:delete', description: Delete shift positions}\n- {scope: 'timeandcost:read', description: Read time and cost data for shifts}\n- {scope: 'punchclockshift:read', description: Read punch clock shift entries}\n- {scope: 'punchclockshift:create', description: Create punch clock shift entries}\n- {scope: 'punchclockkioskdevice:read',\
  \ description: Read punch clock kiosk devices}\n- {scope: 'punchclockkioskdevice:create', description: Create punch clock kiosk devices}\n- {scope: 'punchclockkioskdevice:delete', description: Delete punch clock kiosk devices}\n- {scope: 'punchclockkioskprofile:read', description: Read punch clock kiosk profiles}\n- {scope: 'punchclockkioskprofile:create', description: Create punch clock kiosk profiles}\n- {scope: 'absence:read', description: Read absence records}\n- {scope: 'absence:create', description: Create absence records}\n- {scope: 'absence:update', description: Update absence records}\n- {scope: 'absencesettings:read', description: Read absence settings}\n- {scope: 'absencesettings:create', description: Create absence settings}\n- {scope: 'absencesettings:update', description: Update absence settings}\n- {scope: 'absencesettings:delete', description: Delete absence settings}\n- {scope: 'revenue:read', description: Read revenue data}\n- {scope: 'revenue:set', description: Set revenue\
  \ data}\n- {scope: 'revenue:update', description: Update revenue data}\n- {scope: 'revenue:delete', description: Delete revenue data}\n- {scope: 'payroll:read', description: Read payroll reporting data}\n- {scope: 'payrates:read', description: Read employee pay rates}\n- {scope: 'payrates:update', description: Update employee pay rates}\n- {scope: 'salaries:read', description: Read employee salaries}\n- {scope: 'salaries:update', description: Update employee salaries}\n- {scope: 'contractrules:read', description: Read employee contract rules}\n- {scope: 'contractrules:update', description: Update employee contract rules}\n- {scope: 'portal:create', description: Create portal connection details}\n- {scope: 'securitygroups:read', description: Read security groups}\n- {scope: 'securitygroupmembership:read', description: Read security group membership}\n- {scope: 'securitygroupmembership:update', description: Update security group membership}\n- {scope: 'securitygroupmembership:delete', description:\
  \ Delete security group membership}\n- {scope: 'datacenter:read', description: Read data center details}\n- {scope: 'datacenter:create', description: Create data center details}\n- {scope: platform_access_token, description: Issue a platform access token}\n- {scope: access_token, description: Issue an access token}\n- {scope: impersonate, description: Impersonate a user (privileged)}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planday/refs/heads/main/scopes/planday-scopes.yml
summary_line: 78 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Company
- SaaS
- Workforce Management
- Scheduling
- Time Tracking
- Payroll
- Human Resources
- Hospitality
- Retail
- REST
- OAuth2
token_urls:
- https://id.planday.com/connect/token
---
