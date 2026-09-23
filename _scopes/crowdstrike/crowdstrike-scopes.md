---
authorization_urls: []
description: 'The 187 named scopes a CrowdStrike Falcon API client can be granted, harvested from the provider''s own operation reference: every operation page states the scope it requires, in the form ''<Service collection>: READ'' or ''<Service collection>: WRITE''. Scopes are selected when the API client is created in the Falcon console. Counts are the number of documented operations that name each scope. NOT derived from an OpenAPI — CrowdStrike publishes none; derive-oauth-scopes.py has no spec to read in this repo.'
docs: https://developer.crowdstrike.com/falcon-mcp/getting-started/credentials/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Crowdstrike Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CrowdStrike publishes 187 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CrowdStrike API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CrowdStrike
provider_slug: crowdstrike
schemes:
- flow: clientCredentials
  name: FalconOAuth2
  token_url: https://api.crowdstrike.com/oauth2/token
scope_count: 187
scope_names:
- 'API integrations: READ'
- 'API integrations: WRITE'
- 'ASPM Admin: READ'
- 'ASPM Admin: WRITE'
- 'ASPM Analyst: WRITE'
- 'ASPM Falcon Admin: WRITE'
- 'ASPM Read-Only: READ'
- 'AWS accounts: READ'
- 'AWS accounts: WRITE'
- 'Access Scope: READ'
- 'Actors (Falcon Intelligence): READ'
- 'Alerts: READ'
- 'Alerts: WRITE'
- 'Api Client Mgmt: READ'
- 'Api Client Mgmt: WRITE'
- 'App Logs: READ'
- 'App Logs: WRITE'
- 'Apps: READ'
- 'Assets: READ'
- 'Assets: WRITE'
- 'Bulk uninstallation token: WRITE'
- 'CAO Hunting: READ'
- 'CAO Incidents: READ'
- 'CSPM registration: READ'
- 'CSPM registration: WRITE'
- 'Case Templates: READ'
- 'Case Templates: WRITE'
- 'Cases: READ'
- 'Cases: WRITE'
- 'Charlotte AI Agent Definition: READ'
- 'Charlotte AI Agent Definition: WRITE'
- 'Cloud Registration: WRITE'
- 'Cloud Security API Assets: READ'
- 'Cloud Security API Detections: READ'
- 'Cloud Security API Risks: READ'
- 'Cloud Security AWS Registration: READ'
- 'Cloud Security AWS Registration: WRITE'
- 'Cloud Security Azure Registration: READ'
- 'Cloud Security Azure Registration: WRITE'
- 'Cloud Security Google Cloud Registration: READ'
- 'Cloud Security Google Cloud Registration: WRITE'
- 'Cloud Security OCI Registration: READ'
- 'Cloud Security OCI Registration: WRITE'
- 'Cloud Security Policies: READ'
- 'Cloud Security Policies: WRITE'
- 'Cloud Security Tools Download: READ'
- 'Configuration Assessment: READ'
- 'Content Update Policy: READ'
- 'Content Update Policy: WRITE'
- 'Correlation Rules Admin: WRITE'
- 'Correlation Rules: READ'
- 'Correlation Rules: WRITE'
- 'Custom IOA rules: READ'
- 'Custom IOA rules: WRITE'
- 'Custom storage: READ'
- 'Custom storage: WRITE'
- 'D4C registration: READ'
- 'D4C registration: WRITE'
- 'Data Protection: READ'
- 'Data Protection: WRITE'
- 'Delete Managed Assets: WRITE'
- 'Delivery Settings: READ'
- 'Delivery Settings: WRITE'
- 'Deployment Coordinator: READ'
- 'Detections: READ'
- 'Detections: WRITE'
- 'Device Content: READ'
- 'Device control policies: READ'
- 'Device control policies: WRITE'
- 'Event streams: READ'
- 'Falcon Complete Dashboard: READ'
- 'Falcon Container CLI: READ'
- 'Falcon Container CLI: WRITE'
- 'Falcon Container Image: READ'
- 'Falcon Container Image: WRITE'
- 'Falcon Container Policies: READ'
- 'Falcon Container Policies: WRITE'
- 'Falcon Data Replicator: READ'
- 'Falcon Discover IoT: READ'
- 'Falcon FileVantage Content: READ'
- 'Falcon FileVantage: READ'
- 'Falcon FileVantage: WRITE'
- 'Falcon Id: READ'
- 'Falcon Id: WRITE'
- 'Falcon Indicator Graph: READ'
- 'Firewall management: READ'
- 'Firewall management: WRITE'
- 'Flight Control: READ'
- 'Flight Control: WRITE'
- 'Host Migration: READ'
- 'Host Migration: WRITE'
- 'Host groups: READ'
- 'Host groups: WRITE'
- 'Hosts: READ'
- 'Hosts: WRITE'
- 'IOA Exclusions: READ'
- 'IOA Exclusions: WRITE'
- 'IOC Management: READ'
- 'IOC Management: WRITE'
- 'IOCs (Indicators of Compromise): READ'
- 'IT Automation - Policies: READ'
- 'IT Automation - Policies: WRITE'
- 'IT Automation - Task Executions: READ'
- 'IT Automation - Task Executions: WRITE'
- 'IT Automation - Tasks: READ'
- 'IT Automation - Tasks: WRITE'
- 'IT Automation - User Groups: READ'
- 'IT Automation - User Groups: WRITE'
- 'Identity Protection Entities: READ'
- 'Identity Protection GraphQL: WRITE'
- 'Identity Protection Policy Rules: READ'
- 'Identity Protection Policy Rules: WRITE'
- 'Indicators (Falcon Intelligence): READ'
- 'Infrastructure as Code (IaC): READ'
- 'Installation Tokens Settings: WRITE'
- 'Installation Tokens: READ'
- 'Installation Tokens: WRITE'
- 'Kubernetes Protection: READ'
- 'Kubernetes Protection: WRITE'
- 'Machine Learning Exclusions: READ'
- 'Machine Learning Exclusions: WRITE'
- 'MalQuery: READ'
- 'MalQuery: WRITE'
- 'Malware Families (Falcon Intelligence): READ'
- 'Message Center: READ'
- 'Message Center: WRITE'
- 'Mobile Enrollment: WRITE'
- 'Monitoring rules (Falcon Intelligence Recon): READ'
- 'Monitoring rules (Falcon Intelligence Recon): WRITE'
- 'NGSIEM Dashboards: READ'
- 'NGSIEM Dashboards: WRITE'
- 'NGSIEM Data Connections API: READ'
- 'NGSIEM Data Connections API: WRITE'
- 'NGSIEM Lookup Files: READ'
- 'NGSIEM Lookup Files: WRITE'
- 'NGSIEM Parsers: READ'
- 'NGSIEM Parsers: WRITE'
- 'NGSIEM Saved Queries: READ'
- 'NGSIEM Saved Queries: WRITE'
- 'NGSIEM: READ'
- 'NGSIEM: WRITE'
- 'Network scanning: READ'
- 'Network scanning: WRITE'
- 'On-demand scans (ODS): READ'
- 'On-demand scans (ODS): WRITE'
- 'Prevention policies: READ'
- 'Prevention policies: WRITE'
- 'Quarantined Files: READ'
- 'Quarantined Files: WRITE'
- 'Quick Scan (Falcon Intelligence): READ'
- 'Quick Scan (Falcon Intelligence): WRITE'
- 'QuickScan Pro: READ'
- 'QuickScan Pro: WRITE'
- 'Real time response (admin): WRITE'
- 'Real time response audit: READ'
- 'Real time response: READ'
- 'Real time response: WRITE'
- 'Reports (Falcon Intelligence): READ'
- 'Response policies: READ'
- 'Response policies: WRITE'
- 'Risk Platform - Risk: READ'
- 'Rules (Falcon Intelligence): READ'
- 'SaaS Security (Falcon Shield): READ'
- 'SaaS Security (Falcon Shield): WRITE'
- 'Sample uploads: READ'
- 'Sample uploads: WRITE'
- 'Sandbox (Falcon Intelligence): READ'
- 'Sandbox (Falcon Intelligence): WRITE'
- 'Scheduled Reports: READ'
- 'Sensor Download: READ'
- 'Sensor Usage: READ'
- 'Sensor Visibility Exclusions: READ'
- 'Sensor Visibility Exclusions: WRITE'
- 'Sensor update policies: READ'
- 'Sensor update policies: WRITE'
- 'Snapshot Scanner Image Download: READ'
- 'Snapshot: READ'
- 'Snapshot: WRITE'
- 'Tailored Intelligence: READ'
- 'Threatgraph: READ'
- 'User management: READ'
- 'User management: WRITE'
- 'Vulnerabilities (Falcon Intelligence): READ'
- 'Vulnerabilities: READ'
- 'Workflow: READ'
- 'Workflow: WRITE'
- 'Zero Trust Assessment: READ'
scopes:
- description: ''
  flows: []
  scope: 'API integrations: READ'
- description: ''
  flows: []
  scope: 'API integrations: WRITE'
- description: ''
  flows: []
  scope: 'ASPM Admin: READ'
- description: ''
  flows: []
  scope: 'ASPM Admin: WRITE'
- description: ''
  flows: []
  scope: 'ASPM Analyst: WRITE'
- description: ''
  flows: []
  scope: 'ASPM Falcon Admin: WRITE'
- description: ''
  flows: []
  scope: 'ASPM Read-Only: READ'
- description: ''
  flows: []
  scope: 'AWS accounts: READ'
- description: ''
  flows: []
  scope: 'AWS accounts: WRITE'
- description: ''
  flows: []
  scope: 'Access Scope: READ'
- description: ''
  flows: []
  scope: 'Actors (Falcon Intelligence): READ'
- description: ''
  flows: []
  scope: 'Alerts: READ'
- description: ''
  flows: []
  scope: 'Alerts: WRITE'
- description: ''
  flows: []
  scope: 'Api Client Mgmt: READ'
- description: ''
  flows: []
  scope: 'Api Client Mgmt: WRITE'
- description: ''
  flows: []
  scope: 'App Logs: READ'
- description: ''
  flows: []
  scope: 'App Logs: WRITE'
- description: ''
  flows: []
  scope: 'Apps: READ'
- description: ''
  flows: []
  scope: 'Assets: READ'
- description: ''
  flows: []
  scope: 'Assets: WRITE'
- description: ''
  flows: []
  scope: 'Bulk uninstallation token: WRITE'
- description: ''
  flows: []
  scope: 'CAO Hunting: READ'
- description: ''
  flows: []
  scope: 'CAO Incidents: READ'
- description: ''
  flows: []
  scope: 'CSPM registration: READ'
- description: ''
  flows: []
  scope: 'CSPM registration: WRITE'
- description: ''
  flows: []
  scope: 'Case Templates: READ'
- description: ''
  flows: []
  scope: 'Case Templates: WRITE'
- description: ''
  flows: []
  scope: 'Cases: READ'
- description: ''
  flows: []
  scope: 'Cases: WRITE'
- description: ''
  flows: []
  scope: 'Charlotte AI Agent Definition: READ'
- description: ''
  flows: []
  scope: 'Charlotte AI Agent Definition: WRITE'
- description: ''
  flows: []
  scope: 'Cloud Registration: WRITE'
- description: ''
  flows: []
  scope: 'Cloud Security API Assets: READ'
- description: ''
  flows: []
  scope: 'Cloud Security API Detections: READ'
- description: ''
  flows: []
  scope: 'Cloud Security API Risks: READ'
- description: ''
  flows: []
  scope: 'Cloud Security AWS Registration: READ'
- description: ''
  flows: []
  scope: 'Cloud Security AWS Registration: WRITE'
- description: ''
  flows: []
  scope: 'Cloud Security Azure Registration: READ'
- description: ''
  flows: []
  scope: 'Cloud Security Azure Registration: WRITE'
- description: ''
  flows: []
  scope: 'Cloud Security Google Cloud Registration: READ'
- description: ''
  flows: []
  scope: 'Cloud Security Google Cloud Registration: WRITE'
- description: ''
  flows: []
  scope: 'Cloud Security OCI Registration: READ'
- description: ''
  flows: []
  scope: 'Cloud Security OCI Registration: WRITE'
- description: ''
  flows: []
  scope: 'Cloud Security Policies: READ'
- description: ''
  flows: []
  scope: 'Cloud Security Policies: WRITE'
- description: ''
  flows: []
  scope: 'Cloud Security Tools Download: READ'
- description: ''
  flows: []
  scope: 'Configuration Assessment: READ'
- description: ''
  flows: []
  scope: 'Content Update Policy: READ'
- description: ''
  flows: []
  scope: 'Content Update Policy: WRITE'
- description: ''
  flows: []
  scope: 'Correlation Rules Admin: WRITE'
- description: ''
  flows: []
  scope: 'Correlation Rules: READ'
- description: ''
  flows: []
  scope: 'Correlation Rules: WRITE'
- description: ''
  flows: []
  scope: 'Custom IOA rules: READ'
- description: ''
  flows: []
  scope: 'Custom IOA rules: WRITE'
- description: ''
  flows: []
  scope: 'Custom storage: READ'
- description: ''
  flows: []
  scope: 'Custom storage: WRITE'
- description: ''
  flows: []
  scope: 'D4C registration: READ'
- description: ''
  flows: []
  scope: 'D4C registration: WRITE'
- description: ''
  flows: []
  scope: 'Data Protection: READ'
- description: ''
  flows: []
  scope: 'Data Protection: WRITE'
- description: ''
  flows: []
  scope: 'Delete Managed Assets: WRITE'
- description: ''
  flows: []
  scope: 'Delivery Settings: READ'
- description: ''
  flows: []
  scope: 'Delivery Settings: WRITE'
- description: ''
  flows: []
  scope: 'Deployment Coordinator: READ'
- description: ''
  flows: []
  scope: 'Detections: READ'
- description: ''
  flows: []
  scope: 'Detections: WRITE'
- description: ''
  flows: []
  scope: 'Device Content: READ'
- description: ''
  flows: []
  scope: 'Device control policies: READ'
- description: ''
  flows: []
  scope: 'Device control policies: WRITE'
- description: ''
  flows: []
  scope: 'Event streams: READ'
- description: ''
  flows: []
  scope: 'Falcon Complete Dashboard: READ'
- description: ''
  flows: []
  scope: 'Falcon Container CLI: READ'
- description: ''
  flows: []
  scope: 'Falcon Container CLI: WRITE'
- description: ''
  flows: []
  scope: 'Falcon Container Image: READ'
- description: ''
  flows: []
  scope: 'Falcon Container Image: WRITE'
- description: ''
  flows: []
  scope: 'Falcon Container Policies: READ'
- description: ''
  flows: []
  scope: 'Falcon Container Policies: WRITE'
- description: ''
  flows: []
  scope: 'Falcon Data Replicator: READ'
- description: ''
  flows: []
  scope: 'Falcon Discover IoT: READ'
- description: ''
  flows: []
  scope: 'Falcon FileVantage Content: READ'
- description: ''
  flows: []
  scope: 'Falcon FileVantage: READ'
- description: ''
  flows: []
  scope: 'Falcon FileVantage: WRITE'
- description: ''
  flows: []
  scope: 'Falcon Id: READ'
- description: ''
  flows: []
  scope: 'Falcon Id: WRITE'
- description: ''
  flows: []
  scope: 'Falcon Indicator Graph: READ'
- description: ''
  flows: []
  scope: 'Firewall management: READ'
- description: ''
  flows: []
  scope: 'Firewall management: WRITE'
- description: ''
  flows: []
  scope: 'Flight Control: READ'
- description: ''
  flows: []
  scope: 'Flight Control: WRITE'
- description: ''
  flows: []
  scope: 'Host Migration: READ'
- description: ''
  flows: []
  scope: 'Host Migration: WRITE'
- description: ''
  flows: []
  scope: 'Host groups: READ'
- description: ''
  flows: []
  scope: 'Host groups: WRITE'
- description: ''
  flows: []
  scope: 'Hosts: READ'
- description: ''
  flows: []
  scope: 'Hosts: WRITE'
- description: ''
  flows: []
  scope: 'IOA Exclusions: READ'
- description: ''
  flows: []
  scope: 'IOA Exclusions: WRITE'
- description: ''
  flows: []
  scope: 'IOC Management: READ'
- description: ''
  flows: []
  scope: 'IOC Management: WRITE'
- description: ''
  flows: []
  scope: 'IOCs (Indicators of Compromise): READ'
- description: ''
  flows: []
  scope: 'IT Automation - Policies: READ'
- description: ''
  flows: []
  scope: 'IT Automation - Policies: WRITE'
- description: ''
  flows: []
  scope: 'IT Automation - Task Executions: READ'
- description: ''
  flows: []
  scope: 'IT Automation - Task Executions: WRITE'
- description: ''
  flows: []
  scope: 'IT Automation - Tasks: READ'
- description: ''
  flows: []
  scope: 'IT Automation - Tasks: WRITE'
- description: ''
  flows: []
  scope: 'IT Automation - User Groups: READ'
- description: ''
  flows: []
  scope: 'IT Automation - User Groups: WRITE'
- description: ''
  flows: []
  scope: 'Identity Protection Entities: READ'
- description: ''
  flows: []
  scope: 'Identity Protection GraphQL: WRITE'
- description: ''
  flows: []
  scope: 'Identity Protection Policy Rules: READ'
- description: ''
  flows: []
  scope: 'Identity Protection Policy Rules: WRITE'
- description: ''
  flows: []
  scope: 'Indicators (Falcon Intelligence): READ'
- description: ''
  flows: []
  scope: 'Infrastructure as Code (IaC): READ'
- description: ''
  flows: []
  scope: 'Installation Tokens Settings: WRITE'
- description: ''
  flows: []
  scope: 'Installation Tokens: READ'
- description: ''
  flows: []
  scope: 'Installation Tokens: WRITE'
- description: ''
  flows: []
  scope: 'Kubernetes Protection: READ'
- description: ''
  flows: []
  scope: 'Kubernetes Protection: WRITE'
- description: ''
  flows: []
  scope: 'Machine Learning Exclusions: READ'
- description: ''
  flows: []
  scope: 'Machine Learning Exclusions: WRITE'
- description: ''
  flows: []
  scope: 'MalQuery: READ'
- description: ''
  flows: []
  scope: 'MalQuery: WRITE'
- description: ''
  flows: []
  scope: 'Malware Families (Falcon Intelligence): READ'
- description: ''
  flows: []
  scope: 'Message Center: READ'
- description: ''
  flows: []
  scope: 'Message Center: WRITE'
- description: ''
  flows: []
  scope: 'Mobile Enrollment: WRITE'
- description: ''
  flows: []
  scope: 'Monitoring rules (Falcon Intelligence Recon): READ'
- description: ''
  flows: []
  scope: 'Monitoring rules (Falcon Intelligence Recon): WRITE'
- description: ''
  flows: []
  scope: 'NGSIEM Dashboards: READ'
- description: ''
  flows: []
  scope: 'NGSIEM Dashboards: WRITE'
- description: ''
  flows: []
  scope: 'NGSIEM Data Connections API: READ'
- description: ''
  flows: []
  scope: 'NGSIEM Data Connections API: WRITE'
- description: ''
  flows: []
  scope: 'NGSIEM Lookup Files: READ'
- description: ''
  flows: []
  scope: 'NGSIEM Lookup Files: WRITE'
- description: ''
  flows: []
  scope: 'NGSIEM Parsers: READ'
- description: ''
  flows: []
  scope: 'NGSIEM Parsers: WRITE'
- description: ''
  flows: []
  scope: 'NGSIEM Saved Queries: READ'
- description: ''
  flows: []
  scope: 'NGSIEM Saved Queries: WRITE'
- description: ''
  flows: []
  scope: 'NGSIEM: READ'
- description: ''
  flows: []
  scope: 'NGSIEM: WRITE'
- description: ''
  flows: []
  scope: 'Network scanning: READ'
- description: ''
  flows: []
  scope: 'Network scanning: WRITE'
- description: ''
  flows: []
  scope: 'On-demand scans (ODS): READ'
- description: ''
  flows: []
  scope: 'On-demand scans (ODS): WRITE'
- description: ''
  flows: []
  scope: 'Prevention policies: READ'
- description: ''
  flows: []
  scope: 'Prevention policies: WRITE'
- description: ''
  flows: []
  scope: 'Quarantined Files: READ'
- description: ''
  flows: []
  scope: 'Quarantined Files: WRITE'
- description: ''
  flows: []
  scope: 'Quick Scan (Falcon Intelligence): READ'
- description: ''
  flows: []
  scope: 'Quick Scan (Falcon Intelligence): WRITE'
- description: ''
  flows: []
  scope: 'QuickScan Pro: READ'
- description: ''
  flows: []
  scope: 'QuickScan Pro: WRITE'
- description: ''
  flows: []
  scope: 'Real time response (admin): WRITE'
- description: ''
  flows: []
  scope: 'Real time response audit: READ'
- description: ''
  flows: []
  scope: 'Real time response: READ'
- description: ''
  flows: []
  scope: 'Real time response: WRITE'
- description: ''
  flows: []
  scope: 'Reports (Falcon Intelligence): READ'
- description: ''
  flows: []
  scope: 'Response policies: READ'
- description: ''
  flows: []
  scope: 'Response policies: WRITE'
- description: ''
  flows: []
  scope: 'Risk Platform - Risk: READ'
- description: ''
  flows: []
  scope: 'Rules (Falcon Intelligence): READ'
- description: ''
  flows: []
  scope: 'SaaS Security (Falcon Shield): READ'
- description: ''
  flows: []
  scope: 'SaaS Security (Falcon Shield): WRITE'
- description: ''
  flows: []
  scope: 'Sample uploads: READ'
- description: ''
  flows: []
  scope: 'Sample uploads: WRITE'
- description: ''
  flows: []
  scope: 'Sandbox (Falcon Intelligence): READ'
- description: ''
  flows: []
  scope: 'Sandbox (Falcon Intelligence): WRITE'
- description: ''
  flows: []
  scope: 'Scheduled Reports: READ'
- description: ''
  flows: []
  scope: 'Sensor Download: READ'
- description: ''
  flows: []
  scope: 'Sensor Usage: READ'
- description: ''
  flows: []
  scope: 'Sensor Visibility Exclusions: READ'
- description: ''
  flows: []
  scope: 'Sensor Visibility Exclusions: WRITE'
- description: ''
  flows: []
  scope: 'Sensor update policies: READ'
- description: ''
  flows: []
  scope: 'Sensor update policies: WRITE'
- description: ''
  flows: []
  scope: 'Snapshot Scanner Image Download: READ'
- description: ''
  flows: []
  scope: 'Snapshot: READ'
- description: ''
  flows: []
  scope: 'Snapshot: WRITE'
- description: ''
  flows: []
  scope: 'Tailored Intelligence: READ'
- description: ''
  flows: []
  scope: 'Threatgraph: READ'
- description: ''
  flows: []
  scope: 'User management: READ'
- description: ''
  flows: []
  scope: 'User management: WRITE'
- description: ''
  flows: []
  scope: 'Vulnerabilities (Falcon Intelligence): READ'
- description: ''
  flows: []
  scope: 'Vulnerabilities: READ'
- description: ''
  flows: []
  scope: 'Workflow: READ'
- description: ''
  flows: []
  scope: 'Workflow: WRITE'
- description: ''
  flows: []
  scope: 'Zero Trust Assessment: READ'
slug: crowdstrike-scopes
source_filename: crowdstrike-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: CrowdStrike\nproviderId: crowdstrike\ngenerated: '2026-09-19'\nmethod: searched\nsource: https://developer.crowdstrike.com/api-reference/all-operations/\ndocs: https://developer.crowdstrike.com/falcon-mcp/getting-started/credentials/\ndescription: 'The 187 named scopes a CrowdStrike Falcon API client can be granted, harvested from the provider''s\n  own operation reference: every operation page states the scope it requires, in the form ''<Service collection>:\n  READ'' or ''<Service collection>: WRITE''. Scopes are selected when the API client is created in the Falcon console.\n  Counts are the number of documented operations that name each scope. NOT derived from an OpenAPI — CrowdStrike\n  publishes none; derive-oauth-scopes.py has no spec to read in this repo.'\nschemes:\n- name: FalconOAuth2\n  flow: clientCredentials\n  token_url: https://api.crowdstrike.com/oauth2/token\nscope_count: 187\n\
  operations_covered: 1444\noperations_without_a_documented_scope: 19\nscopes:\n- scope: 'API integrations: READ'\n  service: API integrations\n  access: READ\n  operation_count: 1\n  example_operations:\n  - GetCombinedPluginConfigs\n- scope: 'API integrations: WRITE'\n  service: API integrations\n  access: WRITE\n  operation_count: 2\n  example_operations:\n  - ExecuteCommand\n  - ExecuteCommandProxy\n- scope: 'ASPM Admin: READ'\n  service: ASPM Admin\n  access: READ\n  operation_count: 10\n  example_operations:\n  - GetCloudSecurityIntegrationState\n  - GetExecutorNodes\n  - GetGroupHierarchy\n  - GetGroupV2\n  - GetIntegrationsV2\n- scope: 'ASPM Admin: WRITE'\n  service: ASPM Admin\n  access: WRITE\n  operation_count: 12\n  example_operations:\n  - CreateExecutorNode\n  - CreateIntegration\n  - CreateIntegrationTask\n  - DeleteExecutorNode\n  - DeleteIntegration\n- scope: 'ASPM Analyst: WRITE'\n  service: ASPM Analyst\n  access: WRITE\n  operation_count: 4\n  example_operations:\n  -\
  \ DeleteTags\n  - RunIntegrationTask\n  - UpsertBusinessApplications\n  - UpsertTags\n- scope: 'ASPM Falcon Admin: WRITE'\n  service: ASPM Falcon Admin\n  access: WRITE\n  operation_count: 3\n  example_operations:\n  - PostGroupV2\n  - UpdateDefaultGroup\n  - UpdateGroup\n- scope: 'ASPM Read-Only: READ'\n  service: ASPM Read-Only\n  access: READ\n  operation_count: 18\n  example_operations:\n  - ExecuteFunctionData\n  - ExecuteFunctionDataCount\n  - ExecuteFunctionDataQuery\n  - ExecuteFunctionDataQueryCount\n  - ExecuteFunctions\n- scope: 'AWS accounts: READ'\n  service: AWS accounts\n  access: READ\n  operation_count: 4\n  example_operations:\n  - GetAWSAccounts\n  - GetAWSSettings\n  - QueryAWSAccounts\n  - QueryAWSAccountsForIDs\n- scope: 'AWS accounts: WRITE'\n  service: AWS accounts\n  access: WRITE\n  operation_count: 5\n  example_operations:\n  - CreateOrUpdateAWSSettings\n  - DeleteAWSAccounts\n  - ProvisionAWSAccounts\n  - UpdateAWSAccounts\n  - VerifyAWSAccountAccess\n- scope:\
  \ 'Access Scope: READ'\n  service: Access Scope\n  access: READ\n  operation_count: 2\n  example_operations:\n  - ListAccessScopesExternal\n  - QueryAccessScopesExternal\n- scope: 'Actors (Falcon Intelligence): READ'\n  service: Actors (Falcon Intelligence)\n  access: READ\n  operation_count: 6\n  example_operations:\n  - GetIntelActorEntities\n  - GetMitreReport\n  - PostMitreAttacks\n  - QueryIntelActorEntities\n  - QueryIntelActorIds\n- scope: 'Alerts: READ'\n  service: Alerts\n  access: READ\n  operation_count: 7\n  example_operations:\n  - GetQueriesAlertsV1\n  - GetQueriesAlertsV2\n  - PostAggregatesAlertsV1\n  - PostAggregatesAlertsV2\n  - PostCombinedAlertsV1\n- scope: 'Alerts: WRITE'\n  service: Alerts\n  access: WRITE\n  operation_count: 2\n  example_operations:\n  - PatchEntitiesAlertsV2\n  - PatchEntitiesAlertsV3\n- scope: 'Api Client Mgmt: READ'\n  service: Api Client Mgmt\n  access: READ\n  operation_count: 3\n  example_operations:\n  - GetAccessibleScopes\n  - GetAllAPIClientIdsForCustomer\n\
  \  - GetAPIClients\n- scope: 'Api Client Mgmt: WRITE'\n  service: Api Client Mgmt\n  access: WRITE\n  operation_count: 4\n  example_operations:\n  - CreateAPIClient\n  - DeleteAPIClients\n  - ResetAPIClientSecret\n  - UpdateAPIClient\n- scope: 'App Logs: READ'\n  service: App Logs\n  access: READ\n  operation_count: 4\n  example_operations:\n  - GetSavedSearchesExecuteV1\n  - GetSavedSearchesJobResultsDownloadV1\n  - ListReposV1\n  - ListViewV1\n- scope: 'App Logs: WRITE'\n  service: App Logs\n  access: WRITE\n  operation_count: 5\n  example_operations:\n  - CreateSavedSearchesDynamicExecuteV1\n  - CreateSavedSearchesExecuteV1\n  - CreateSavedSearchesIngestV1\n  - IngestDataAsyncV1\n  - IngestDataV1\n- scope: 'Apps: READ'\n  service: Apps\n  access: READ\n  operation_count: 1\n  example_operations:\n  - ReadRequestBody\n- scope: 'Assets: READ'\n  service: Assets\n  access: READ\n  operation_count: 22\n  example_operations:\n  - ListCloudGroupIDsExternal\n  - ListCloudGroupsByIDExternal\n\
  \  - ListCloudGroupsExternal\n  - combined-applications\n  - combined-hosts\n- scope: 'Assets: WRITE'\n  service: Assets\n  access: WRITE\n  operation_count: 6\n  example_operations:\n  - CreateCloudGroupExternal\n  - DeleteCloudGroupsExternal\n  - UpdateCloudGroupExternal\n  - delete-external-assets\n  - patch-external-assets\n- scope: 'Bulk uninstallation token: WRITE'\n  service: Bulk uninstallation token\n  access: WRITE\n  operation_count: 1\n  example_operations:\n  - incrementUninstallToken\n- scope: 'CAO Hunting: READ'\n  service: CAO Hunting\n  access: READ\n  operation_count: 7\n  example_operations:\n  - AggregateHuntingGuides\n  - AggregateIntelligenceQueries\n  - GetArchiveExport\n  - GetHuntingGuides\n  - GetIntelligenceQueries\n- scope: 'CAO Incidents: READ'\n  service: CAO Incidents\n  access: READ\n  operation_count: 3\n  example_operations:\n  - cao_incidents_aggregates_v1\n  - cao_incidents_entities_v1\n  - cao_incidents_queries_v1\n- scope: 'CSPM registration: READ'\n\
  \  service: CSPM registration\n  access: READ\n  operation_count: 18\n  example_operations:\n  - DiscoverCloudAzureDownloadCertificate\n  - GetBehaviorDetections\n  - getCloudEventIDs\n  - GetConfigurationDetectionEntities\n  - GetConfigurationDetectionIDsV2\n- scope: 'CSPM registration: WRITE'\n  service: CSPM registration\n  access: WRITE\n  operation_count: 20\n  example_operations:\n  - AzureRefreshCertificate\n  - ConnectCSPMGCPAccount\n  - CreateCSPMAwsAccount\n  - CreateCSPMAzureAccount\n  - CreateCSPMAzureManagementGroup\n- scope: 'Case Templates: READ'\n  service: Case Templates\n  access: READ\n  operation_count: 20\n  example_operations:\n  - aggregates.access-tags.post.v1\n  - aggregates.notification-groups.post.v1\n  - aggregates.notification-groups.post.v2\n  - aggregates.slas.post.v1\n  - aggregates.templates.post.v1\n- scope: 'Case Templates: WRITE'\n  service: Case Templates\n  access: WRITE\n  operation_count: 13\n  example_operations:\n  - entities.notification-groups.delete.v1\n\
  \  - entities.notification-groups.delete.v2\n  - entities.notification-groups.patch.v1\n  - entities.notification-groups.patch.v2\n  - entities.notification-groups.post.v1\n- scope: 'Cases: READ'\n  service: Cases\n  access: READ\n  operation_count: 9\n  example_operations:\n  - aggregates.file-details.post.v1\n  - combined.file-details.get.v1\n  - entities.cases.post.v2\n  - entities.file-details.get.v1\n  - entities.files_bulk-download.post.v1\n- scope: 'Cases: WRITE'\n  service: Cases\n  access: WRITE\n  operation_count: 13\n  example_operations:\n  - entities.alert-evidence.post.v1\n  - entities.case-tags.delete.v1\n  - entities.case-tags.post.v1\n  - entities.cases.patch.v2\n  - entities.cases.put.v2\n- scope: 'Charlotte AI Agent Definition: READ'\n  service: Charlotte AI Agent Definition\n  access: READ\n  operation_count: 19\n  example_operations:\n  - EntitiesAgentTemplatesV1\n  - QueriesAgentTemplatesV1\n  - GetAgentVersionsV1\n  - QueryAgentVersionsV1\n  - CombinedKnowledgeBaseAuditEventsV1\n\
  - scope: 'Charlotte AI Agent Definition: WRITE'\n  service: Charlotte AI Agent Definition\n  access: WRITE\n  operation_count: 5\n  example_operations:\n  - EntitiesKnowledgeBaseFilesCreateV1\n  - EntitiesKnowledgeBaseFilesDeleteV1\n  - EntitiesKnowledgeBaseFilesUpdateV1\n  - EntitiesKnowledgeBasesCreateV1\n  - EntitiesKnowledgeBasesUpdateV1\n- scope: 'Cloud Registration: WRITE'\n  service: Cloud Registration\n  access: WRITE\n  operation_count: 1\n  example_operations:\n  - cloud-registration-cross-provider-get-account-aggregates\n- scope: 'Cloud Security API Assets: READ'\n  service: Cloud Security API Assets\n  access: READ\n  operation_count: 7\n  example_operations:\n  - cloud-security-assets-combined-application-findings\n  - cloud-security-assets-combined-compliance-by-account\n  - cloud-security-assets-entities-get\n  - cloud-security-assets-entities-post\n  - cloud-security-assets-queries\n- scope: 'Cloud Security API Detections: READ'\n  service: Cloud Security API Detections\n\
  \  access: READ\n  operation_count: 4\n  example_operations:\n  - cspm-evaluations-combined-iom-by-rule\n  - cspm-evaluations-iom-entities\n  - cspm-evaluations-iom-entities-post\n  - cspm-evaluations-iom-queries\n- scope: 'Cloud Security API Risks: READ'\n  service: Cloud Security API Risks\n  access: READ\n  operation_count: 2\n  example_operations:\n  - combined-cloud-risks\n  - cloud-security-timeline-risks-enriched\n- scope: 'Cloud Security AWS Registration: READ'\n  service: Cloud Security AWS Registration\n  access: READ\n  operation_count: 4\n  example_operations:\n  - cloud-registration-aws-get-accounts\n  - cloud-registration-aws-query-accounts\n  - cloud-registration-aws-trigger-health-check\n  - cloud-registration-aws-validate-accounts\n- scope: 'Cloud Security AWS Registration: WRITE'\n  service: Cloud Security AWS Registration\n  access: WRITE\n  operation_count: 3\n  example_operations:\n  - cloud-registration-aws-create-account\n  - cloud-registration-aws-delete-account\n\
  \  - cloud-registration-aws-update-account\n- scope: 'Cloud Security Azure Registration: READ'\n  service: Cloud Security Azure Registration\n  access: READ\n  operation_count: 9\n  example_operations:\n  - cloud-registration-azure-get-issue-suppression-values-by-field\n  - cloud-registration-azure-get-issue-values-by-field\n  - cloud-registration-azure-get-issues\n  - cloud-registration-azure-get-registration\n  - cloud-registration-azure-get-script\n- scope: 'Cloud Security Azure Registration: WRITE'\n  service: Cloud Security Azure Registration\n  access: WRITE\n  operation_count: 8\n  example_operations:\n  - cloud-registration-azure-create-registration\n  - cloud-registration-azure-create-suppressions\n  - cloud-registration-azure-delete-legacy-subscription\n  - cloud-registration-azure-delete-registration\n  - cloud-registration-azure-delete-suppressions\n- scope: 'Cloud Security Google Cloud Registration: READ'\n  service: Cloud Security Google Cloud Registration\n  access: READ\n\
  \  operation_count: 2\n  example_operations:\n  - cloud-registration-gcp-get-entities\n  - cloud-registration-gcp-get-registration\n- scope: 'Cloud Security Google Cloud Registration: WRITE'\n  service: Cloud Security Google Cloud Registration\n  access: WRITE\n  operation_count: 6\n  example_operations:\n  - cloud-registration-gcp-create-registration\n  - cloud-registration-gcp-delete-registration\n  - cloud-registration-gcp-post-terraform-script\n  - cloud-registration-gcp-put-registration\n  - cloud-registration-gcp-trigger-health-check\n- scope: 'Cloud Security OCI Registration: READ'\n  service: Cloud Security OCI Registration\n  access: READ\n  operation_count: 2\n  example_operations:\n  - cloud-security-registration-oci-download-script\n  - cloud-security-registration-oci-get-account\n- scope: 'Cloud Security OCI Registration: WRITE'\n  service: Cloud Security OCI Registration\n  access: WRITE\n  operation_count: 5\n  example_operations:\n  - cloud-security-registration-oci-create-account\n\
  \  - cloud-security-registration-oci-delete-account\n  - cloud-security-registration-oci-rotate-key\n  - cloud-security-registration-oci-update-account\n  - cloud-security-registration-oci-validate-tenancy\n- scope: 'Cloud Security Policies: READ'\n  service: Cloud Security Policies\n  access: READ\n  operation_count: 11\n  example_operations:\n  - GetComplianceControls\n  - GetComplianceFrameworks\n  - GetEnrichedAsset\n  - GetRule\n  - GetRuleInputSchema\n- scope: 'Cloud Security Policies: WRITE'\n  service: Cloud Security Policies\n  access: WRITE\n  operation_count: 19\n  example_operations:\n  - CloneComplianceFramework\n  - CreateComplianceControl\n  - CreateComplianceFramework\n  - CreateRuleMixin0\n  - CreateRuleOverride\n- scope: 'Cloud Security Tools Download: READ'\n  service: Cloud Security Tools Download\n  access: READ\n  operation_count: 1\n  example_operations:\n  - FetchFilesDownloadInfoV2\n- scope: 'Configuration Assessment: READ'\n  service: Configuration Assessment\n\
  \  access: READ\n  operation_count: 3\n  example_operations:\n  - getCombinedAssessmentsQuery\n  - getRuleDetails\n  - getEvaluationLogicMixin0\n- scope: 'Content Update Policy: READ'\n  service: Content Update Policy\n  access: READ\n  operation_count: 6\n  example_operations:\n  - getContentUpdatePolicies\n  - queryCombinedContentUpdatePolicies\n  - queryCombinedContentUpdatePolicyMembers\n  - queryContentUpdatePolicies\n  - queryContentUpdatePolicyMembers\n- scope: 'Content Update Policy: WRITE'\n  service: Content Update Policy\n  access: WRITE\n  operation_count: 5\n  example_operations:\n  - createContentUpdatePolicies\n  - deleteContentUpdatePolicies\n  - performContentUpdatePoliciesAction\n  - setContentUpdatePoliciesPrecedence\n  - updateContentUpdatePolicies\n- scope: 'Correlation Rules Admin: WRITE'\n  service: Correlation Rules Admin\n  access: WRITE\n  operation_count: 2\n  example_operations:\n  - entities.rules_ownership.put.v1\n  - entities.rules_ownership.put.v2\n- scope:\
  \ 'Correlation Rules: READ'\n  service: Correlation Rules\n  access: READ\n  operation_count: 9\n  example_operations:\n  - combined.rules.get.v1\n  - combined.rules.get.v2\n  - entities.latest-rules.get.v1\n  - entities.rules.get.v1\n  - entities.rules.get.v2\n- scope: 'Correlation Rules: WRITE'\n  service: Correlation Rules\n  access: WRITE\n  operation_count: 9\n  example_operations:\n  - aggregates.rule-versions.post.v1\n  - entities.rule-versions.delete.v1\n  - entities.rule-versions_export.post.v1\n  - entities.rule-versions_import.post.v1\n  - entities.rule-versions_publish.patch.v1\n- scope: 'Custom IOA rules: READ'\n  service: Custom IOA rules\n  access: READ\n  operation_count: 12\n  example_operations:\n  - get-patterns\n  - get-platformsMixin0\n  - get-rule-groupsMixin0\n  - get-rule-types\n  - get-rules-get\n- scope: 'Custom IOA rules: WRITE'\n  service: Custom IOA rules\n  access: WRITE\n  operation_count: 8\n  example_operations:\n  - create-rule\n  - create-rule-groupMixin0\n\
  \  - delete-rule-groupsMixin0\n  - delete-rules\n  - update-rule-groupMixin0\n- scope: 'Custom storage: READ'\n  service: Custom storage\n  access: READ\n  operation_count: 14\n  example_operations:\n  - DescribeCollection\n  - DescribeCollections\n  - GetObject\n  - GetObjectMetadata\n  - GetSchema\n- scope: 'Custom storage: WRITE'\n  service: Custom storage\n  access: WRITE\n  operation_count: 4\n  example_operations:\n  - DeleteObject\n  - DeleteVersionedObject\n  - PutObject\n  - PutObjectByVersion\n- scope: 'D4C registration: READ'\n  service: D4C registration\n  access: READ\n  operation_count: 12\n  example_operations:\n  - GetD4CAwsAccount\n  - GetD4CAWSAccountScriptsAttachment\n  - GetD4CAwsConsoleSetupURLs\n  - GetD4CCGPAccount\n  - GetD4CGCPServiceAccountsExt\n- scope: 'D4C registration: WRITE'\n  service: D4C registration\n  access: WRITE\n  operation_count: 8\n  example_operations:\n  - ConnectD4CGCPAccount\n  - CreateD4CAwsAccount\n  - CreateD4CGCPAccount\n  - CreateDiscoverCloudAzureAccount\n\
  \  - DeleteD4CAwsAccount\n- scope: 'Data Protection: READ'\n  service: Data Protection\n  access: READ\n  operation_count: 22\n  example_operations:\n  - entities.classification.get.v2\n  - entities.cloud-application.get\n  - entities.content-pattern.get\n  - entities.enterprise-account.get\n  - entities.file-type.get\n- scope: 'Data Protection: WRITE'\n  service: Data Protection\n  access: WRITE\n  operation_count: 30\n  example_operations:\n  - entities.classification.delete.v2\n  - entities.classification.patch.v2\n  - entities.classification.post.v2\n  - entities.cloud-application.create\n  - entities.cloud-application.delete\n- scope: 'Delete Managed Assets: WRITE'\n  service: Delete Managed Assets\n  access: WRITE\n  operation_count: 1\n  example_operations:\n  - DevicesActionsDeleteV1\n- scope: 'Delivery Settings: READ'\n  service: Delivery Settings\n  access: READ\n  operation_count: 1\n  example_operations:\n  - GetDeliverySettings\n- scope: 'Delivery Settings: WRITE'\n  service:\
  \ Delivery Settings\n  access: WRITE\n  operation_count: 1\n  example_operations:\n  - PostDeliverySettings\n- scope: 'Deployment Coordinator: READ'\n  service: Deployment Coordinator\n  access: READ\n  operation_count: 6\n  example_operations:\n  - CombinedReleaseNotesV1\n  - CombinedReleasesV1Mixin0\n  - GetDeploymentsExternalV1\n  - GetEntityIDsByQueryPOST\n  - GetEntityIDsByQueryPOSTV2\n- scope: 'Detections: READ'\n  service: Detections\n  access: READ\n  operation_count: 3\n  example_operations:\n  - GetAggregateDetects\n  - GetDetectSummaries\n  - QueryDetects\n- scope: 'Detections: WRITE'\n  service: Detections\n  access: WRITE\n  operation_count: 1\n  example_operations:\n  - UpdateDetectsByIdsV2\n- scope: 'Device Content: READ'\n  service: Device Content\n  access: READ\n  operation_count: 2\n  example_operations:\n  - entities.states.v1\n  - queries.states.v1\n- scope: 'Device control policies: READ'\n  service: Device control policies\n  access: READ\n  operation_count: 8\n\
  \  example_operations:\n  - getDefaultDeviceControlPolicies\n  - getDefaultDeviceControlSettings\n  - getDeviceControlPolicies\n  - getDeviceControlPoliciesV2\n  - queryCombinedDeviceControlPolicies\n- scope: 'Device control policies: WRITE'\n  service: Device control policies\n  access: WRITE\n  operation_count: 10\n  example_operations:\n  - createDeviceControlPolicies\n  - deleteDeviceControlPolicies\n  - patchDeviceControlPoliciesClassesV1\n  - patchDeviceControlPoliciesV2\n  - performDeviceControlPoliciesAction\n- scope: 'Event streams: READ'\n  service: Event streams\n  access: READ\n  operation_count: 2\n  example_operations:\n  - listAvailableStreamsOAuth2\n  - refreshActiveStreamSession\n- scope: 'Falcon Complete Dashboard: READ'\n  service: Falcon Complete Dashboard\n  access: READ\n  operation_count: 17\n  example_operations:\n  - AggregateAlerts\n  - AggregateAllowList\n  - AggregateBlockList\n  - AggregateDeviceCountCollection\n  - AggregateEscalations\n- scope: 'Falcon Container\
  \ CLI: READ'\n  service: Falcon Container CLI\n  access: READ\n  operation_count: 2\n  example_operations:\n  - GetCredentials\n  - HeadImageScanInventory\n- scope: 'Falcon Container CLI: WRITE'\n  service: Falcon Container CLI\n  access: WRITE\n  operation_count: 2\n  example_operations:\n  - PostImageScanInventory\n  - ReadImageVulnerabilities\n- scope: 'Falcon Container Image: READ'\n  service: Falcon Container Image\n  access: READ\n  operation_count: 128\n  example_operations:\n  - ReadContainerAlertsCount\n  - ReadContainerAlertsCountBySeverity\n  - SearchAndReadContainerAlerts\n  - GetRuntimeDetectionsCombinedV2\n  - ReadCombinedDetections\n- scope: 'Falcon Container Image: WRITE'\n  service: Falcon Container Image\n  access: WRITE\n  operation_count: 15\n  example_operations:\n  - CreateBaseImagesEntities\n  - DeleteBaseImages\n  - CreateRegistryEntities\n  - DeleteRegistryEntities\n  - UpdateRegistryEntities\n- scope: 'Falcon Container Policies: READ'\n  service: Falcon Container\
  \ Policies\n  access: READ\n  operation_count: 2\n  example_operations:\n  - admission-control-get-policies\n  - admission-control-query-policies\n- scope: 'Falcon Container Policies: WRITE'\n  service: Falcon Container Policies\n  access: WRITE\n  operation_count: 13\n  example_operations:\n  - admission-control-add-host-groups\n  - admission-control-add-rule-group-custom-rule\n  - admission-control-create-policy\n  - admission-control-create-rule-groups\n  - admission-control-delete-policies\n- scope: 'Falcon Data Replicator: READ'\n  service: Falcon Data Replicator\n  access: READ\n  operation_count: 5\n  example_operations:\n  - fdrschema.combined.event.get\n  - fdrschema.entities.event.get\n  - fdrschema.entities.field.get\n  - fdrschema.queries.event.get\n  - fdrschema.queries.field.get\n- scope: 'Falcon Discover IoT: READ'\n  service: Falcon Discover IoT\n  access: READ\n  operation_count: 3\n  example_operations:\n  - get-iot-hosts\n  - query-iot-hosts\n  - query-iot-hostsV2\n\
  - scope: 'Falcon FileVantage Content: READ'\n  service: Falcon FileVantage Content\n  access: READ\n  operation_count: 1\n  example_operations:\n  - getContents\n- scope: 'Falcon FileVantage: READ'\n  service: Falcon FileVantage\n  access: READ\n  operation_count: 12\n  example_operations:\n  - getActionsMixin0\n  - getChanges\n  - getPolicies\n  - getRuleGroups\n  - getRules\n- scope: 'Falcon FileVantage: WRITE'\n  service: Falcon FileVantage\n  access: WRITE\n  operation_count: 18\n  example_operations:\n  - createPolicies\n  - createRuleGroups\n  - createRules\n  - createScheduledExclusions\n  - deletePolicies\n- scope: 'Falcon Id: READ'\n  service: Falcon Id\n  access: READ\n  operation_count: 2\n  example_operations:\n  - GetThirdPartyPasskeyRegistry\n  - QueryThirdPartyPasskeyRegistry\n- scope: 'Falcon Id: WRITE'\n  service: Falcon Id\n  access: WRITE\n  operation_count: 2\n  example_operations:\n  - DeleteThirdPartyPasskeyRegistry\n  - UpdateThirdPartyPasskeyRegistry\n- scope: 'Falcon\
  \ Indicator Graph: READ'\n  service: Falcon Indicator Graph\n  access: READ\n  operation_count: 5\n  example_operations:\n  - DownloadFeedArchive\n  - ListFeedTypes\n  - QueryFeedArchives\n  - LookupIndicators\n  - SearchIndicators\n- scope: 'Firewall management: READ'\n  service: Firewall management\n  access: READ\n  operation_count: 20\n  example_operations:\n  - get-events\n  - get-firewall-fields\n  - get-network-locations\n  - get-network-locations-details\n  - get-platforms\n- scope: 'Firewall management: WRITE'\n  service: Firewall management\n  access: WRITE\n  operation_count: 23\n  example_operations:\n  - aggregate-events\n  - aggregate-policy-rules\n  - aggregate-rule-groups\n  - aggregate-rules\n  - create-network-locations\n- scope: 'Flight Control: READ'\n  service: Flight Control\n  access: READ\n  operation_count: 17\n  example_operations:\n  - getChildren\n  - getChildrenV2\n  - getCIDGroupByIdV1\n  - getCIDGroupByIdV2\n  - getCIDGroupMembersByV1\n- scope: 'Flight Control:\
  \ WRITE'\n  service: Flight Control\n  access: WRITE\n  operation_count: 13\n  example_operations:\n  - addCIDGroupMembers\n  - addRole\n  - addUserGroupMembers\n  - createCIDGroups\n  - createUserGroups\n- scope: 'Host Migration: READ'\n  service: Host Migration\n  access: READ\n  operation_count: 5\n  example_operations:\n  - GetHostMigrationIDsV1\n  - GetHostMigrationsV1\n  - GetMigrationDestinationsV1\n  - GetMigrationIDsV1\n  - GetMigrationsV1\n- scope: 'Host Migration: WRITE'\n  service: Host Migration\n  access: WRITE\n  operation_count: 5\n  example_operations:\n  - CreateMigrationV1\n  - HostMigrationAggregatesV1\n  - HostMigrationsActionsV1\n  - MigrationAggregatesV1\n  - MigrationsActionsV1\n- scope: 'Host groups: READ'\n  service: Host groups\n  access: READ\n  operation_count: 5\n  example_operations:\n  - getHostGroups\n  - queryCombinedGroupMembers\n  - queryCombinedHostGroups\n  - queryGroupMembers\n  - queryHostGroups\n- scope: 'Host groups: WRITE'\n  service: Host groups\n\
  \  access: WRITE\n  operation_count: 5\n  example_operations:\n  - createHostGroups\n  - deleteHostGroups\n  - performGroupAction\n  - updateHostGroups\n  - entities.perform_action\n- scope: 'Hosts: READ'\n  service: Hosts\n  access: READ\n  operation_count: 12\n  example_operations:\n  - CombinedDevicesByFilter\n  - CombinedHiddenDevicesByFilter\n  - GetDeviceDetails\n  - GetDeviceDetailsV2\n  - GetOnlineState.V1\n- scope: 'Hosts: WRITE'\n  service: Hosts\n  access: WRITE\n  operation_count: 2\n  example_operations:\n  - PerformActionV2\n  - UpdateDeviceTags\n- scope: 'IOA Exclusions: READ'\n  service: IOA Exclusions\n  access: READ\n  operation_count: 4\n  example_operations:\n  - getIOAExclusionsV1\n  - queryIOAExclusionsV1\n  - ss-ioa-exclusions.get.v2\n  - ss-ioa-exclusions.search.v2\n- scope: 'IOA Exclusions: WRITE'\n  service: IOA Exclusions\n  access: WRITE\n  operation_count: 10\n  example_operations:\n  - createIOAExclusionsV1\n  - deleteIOAExclusionsV1\n  - ss-ioa-exclusions.aggregates.v2\n\
  \  - ss-ioa-exclusions.create.v2\n  - ss-ioa-exclusions.delete.v2\n- scope: 'IOC Management: READ'\n  service: IOC Management\n  access: READ\n  operation_count: 13\n  example_operations:\n  - action.get.v1\n  - action.query.v1\n  - GetIndicatorsReport\n  - indicator.aggregate.v1\n  - indicator.combined.v1\n- scope: 'IOC Management: WRITE'\n  service: IOC Management\n  access: WRITE\n  operation_count: 4\n  example_operations:\n  - indicator.create.v1\n  - indicator.delete.v1\n  - indicator.sdmf-query.v1\n  - indicator.update.v1\n- scope: 'IOCs (Indicators of Compromise): READ'\n  service: IOCs (Indicators of Compromise)\n  access: READ\n  operation_count: 4\n  example_operations:\n  - DevicesCount\n  - DevicesRanOn\n  - entities.processes\n  - ProcessesRanOn\n- scope: 'IT Automation - Policies: READ'\n  service: IT Automation - Policies\n  access: READ\n  operation_count: 2\n  example_operations:\n  - ITAutomationGetPolicies\n  - ITAutomationQueryPolicies\n- scope: 'IT Automation - Policies:\
  \ WRITE'\n  service: IT Automation - Policies\n  access: WRITE\n  operation_count: 5\n  example_operations:\n  - ITAutomationCreatePolicy\n  - ITAutomationDeletePolicy\n  - ITAutomationUpdatePolicies\n  - ITAutomationUpdatePoliciesPrecedence\n  - ITAutomationUpdatePolicyHostGroups\n- scope: 'IT Automation - Task Executions: READ'\n  service: IT Automation - Task Executions\n  access: READ\n  operation_count: 10\n  example_operations:\n  - ITAutomationCombinedScheduledTasks\n  - ITAutomationGetExecutionResults\n  - ITAutomationGetExecutionResultsSearchStatus\n  - ITAutomationGetScheduledTasks\n  - ITAutomationGetTaskExecution\n- scope: 'IT Automation - Task Executions: WRITE'\n  service: IT Automation - Task Executions\n  access: WRITE\n  operation_count: 7\n  example_operations:\n  - ITAutomationCancelTaskExecution\n  - ITAutomationCreateScheduledTask\n  - ITAutomationDeleteScheduledTasks\n  - ITAutomationRerunTaskExecution\n  - ITAutomationRunLiveQuery\n- scope: 'IT Automation - Tasks:\
  \ READ'\n  service: IT Automation - Tasks\n  access: READ\n  operation_count: 7\n  example_operations:\n  - ITAutomationGetAssociatedTasks\n  - ITAutomationGetTaskGroups\n  - ITAutomationGetTaskGroupsByQuery\n  - ITAutomationGetTasks\n  - ITAutomationGetTasksByQuery\n- scope: 'IT Automation - Tasks: WRITE'\n  service: IT Automation - Tasks\n  access: WRITE\n  operation_count: 6\n  example_operations:\n  - ITAutomationCreateTask\n  - ITAutomationCreateTaskGroup\n  - ITAutomationDeleteTask\n  - ITAutomationDeleteTaskGroups\n  - ITAutomationUpdateTask\n- scope: 'IT Automation - User Groups: READ'\n  service: IT Automation - User Groups\n  access: READ\n  operation_count: 2\n  example_operations:\n  - ITAutomationGetUserGroup\n  - ITAutomationSearchUserGroup\n- scope: 'IT Automation - User Groups: WRITE'\n  service: IT Automation - User Groups\n  access: WRITE\n  operation_count: 3\n  example_operations:\n  - ITAutomationCreateUserGroup\n  - ITAutomationDeleteUserGroup\n  - ITAutomationUpdateUserGroup\n\
  - scope: 'Identity Protection Entities: READ'\n  service: Identity Protection Entities\n  access: READ\n  operation_count: 3\n  example_operations:\n  - GetSensorAggregates\n  - GetSensorDetails\n  - QuerySensorsByFilter\n- scope: 'Identity Protection GraphQL: WRITE'\n  service: Identity Protection GraphQL\n  access: WRITE\n  operation_count: 1\n  example_operations:\n  - api_preempt_proxy_post_graphql\n- scope: 'Identity Protection Policy Rules: READ'\n  service: Identity Protection Policy Rules\n  access: READ\n  operation_count: 4\n  example_operations:\n  - get_policy_rules\n  - get_policy_rules\n  - get_policy_rules_query\n  - get_policy_rules_query\n- scope: 'Identity Protection Policy Rules: WRITE'\n  service: Identity Protection Policy Rules\n  access: WRITE\n  operation_count: 4\n  example_operations:\n  - delete_policy_rules\n  - delete_policy_rules\n  - post_policy_rules\n  - post_policy_rules\n- scope: 'Indicators (Falcon Intelligence): READ'\n  service: Indicators (Falcon\
  \ Intelligence)\n  access: READ\n  operation_count: 3\n  example_operations:\n  - GetIntelIndicatorEntities\n  - QueryIntelIndicatorEntities\n  - QueryIntelIndicatorIds\n- scope: 'Infrastructure as Code (IaC): READ'\n  service: Infrastructure as Code (IaC)\n  access: READ\n  operation_count: 5\n  example_operations:\n  - CombinedDetections\n  - GetCredentialsIAC\n  - DownloadFile\n  - EnumerateFile\n  - FetchFilesDownloadInfo\n- scope: 'Installation Tokens Settings: WRITE'\n  service: Installation Tokens Settings\n  access: WRITE\n  operation_count: 1\n  example_operations:\n  - customer-settings-update\n- scope: 'Installation Tokens: READ'\n  service: Installation Tokens\n  access: READ\n  operation_count: 5\n  example_operations:\n  - audit-events-query\n  - audit-events-read\n  - customer-settings-read\n  - tokens-query\n  - tokens-read\n- scope: 'Installation Tokens: WRITE'\n  service: Installation Tokens\n  access: WRITE\n  operation_count: 3\n  example_operations:\n  - tokens-create\n\
  \  - tokens-delete\n  - tokens-update\n- scope: 'Kubernetes Protection: READ'\n  service: Kubernetes Protection\n  access: READ\n  operation_count: 10\n  example_operations:\n  - GetAWSAccountsMixin0\n  - GetAzureInstallScript\n  - GetAzureTenantConfig\n  - GetAzureTenantIDs\n  - GetClusters\n- scope: 'Kubernetes Protection: WRITE'\n  service: Kubernetes Protection\n  access: WRITE\n  operation_count: 8\n  example_operations:\n  - CreateAWSAccount\n  - CreateAzureSubscription\n  - DeleteAWSAccountsMixin0\n  - DeleteAzureSubscription\n  - PatchAzureServicePrincipal\n- scope: 'Machine Learning Exclusions: READ'\n  service: Machine Learning Exclusions\n  access: READ\n  operation_count: 8\n  example_operations:\n  - cb-exclusions.get.v1\n  - cb-exclusions.query.v1\n  - certificates.get.v1\n  - exclusions.get-all.v2\n  - exclusions.get.v2\n- scope: 'Machine Learning Exclusions: WRITE'\n  service: Machine Learning Exclusions\n  access: WRITE\n  operation_count: 13\n  example_operations:\n \
  \ - cb-exclusions.create.v1\n  - cb-exclusions.delete.v1\n  - cb-exclusions.update.v1\n  - createMLExclusionsV1\n  - deleteMLExclusionsV1\n- scope: 'MalQuery: READ'\n  service: MalQuery\n  access: READ\n  operation_count: 5\n  example_operations:\n  - GetMalQueryDownloadV1\n  - GetMalQueryEntitiesSamplesFetchV1\n  - GetMalQueryMetadataV1\n  - GetMalQueryQuotasV1\n  - GetMalQueryRequestV1\n- scope: 'MalQuery: WRITE'\n  service: MalQuery\n  access: WRITE\n  operation_count: 4\n  example_operations:\n  - PostMalQueryEntitiesSamplesMultidownloadV1\n  - PostMalQueryExactSearchV1\n  - PostMalQueryFuzzySearchV1\n  - PostMalQueryHuntV1\n- scope: 'Malware Families (Falcon Intelligence): READ'\n  service: Malware Families (Falcon Intelligence)\n  access: READ\n  operation_count: 5\n  example_operations:\n  - GetMalwareEntities\n  - GetMalwareMitreReport\n  - QueryMalware\n  - QueryMalwareEntities\n  - QueryMitreAttacksForMalware\n- scope: 'Message Center: READ'\n  service: Message Center\n  access:\
  \ READ\n  operation_count: 6\n  example_operations:\n  - AggregateCases\n  - CaseDownloadAttachment\n  - GetCaseActivityByIds\n  - GetCaseEntitiesByIDs\n  - QueryActivityByCaseID\n- scope: 'Message Center: WRITE'\n  service: Message Center\n  access: WRITE\n  operation_count: 3\n  example_operations:\n  - CaseAddActivity\n  - CaseAddAttachment\n  - CreateCaseV2\n- scope: 'Mobile Enrollment: WRITE'\n  service: Mobile Enrollment\n  access: WRITE\n  operation_count: 2\n  example_operations:\n  - RequestDeviceEnrollmentV3\n  - RequestDeviceEnrollmentV4\n- scope: 'Monitoring rules (Falcon Intelligence Recon): READ'\n  service: Monitoring rules (Falcon Intelligence Recon)\n  access: READ\n  operation_count: 16\n  example_operations:\n  - AggregateNotificationsExposedDataRecordsV1\n  - AggregateNotificationsV1\n  - GetActionsV1\n  - GetExportJobsV1\n  - GetFileContentForExportJobsV1\n- scope: 'Monitoring rules (Falcon Intelligence Recon): WRITE'\n  service: Monitoring rules (Falcon Intelligence\
  \ Recon)\n  access: WRITE\n  operation_count: 10\n  example_operations:\n  - CreateActionsV1\n  - CreateExportJobsV1\n  - CreateRulesV1\n  - DeleteActionV1\n  - DeleteExportJobsV1\n- scope: 'NGSIEM Dashboards: READ'\n  service: NGSIEM Dashboards\n  access: READ\n  operation_count: 2\n  example_operations:\n  - GetDashboardTemplate\n  - ListDashboards\n- scope: 'NGSIEM Dashboards: WRITE'\n  service: NGSIEM Dashboards\n  access: WRITE\n  operation_count: 11\n  example_operations:\n  - addDashboardLabels\n  - bulkAddDashboardLabels\n  - BulkCreateDashboardsFromTemplate\n  - bulkRemoveDashboardLabels\n  - bulkUpdateDashboardLabels\n- scope: 'NGSIEM Data Connections API: READ'\n  service: NGSIEM Data Connections API\n  access: READ\n  operation_count: 6\n  example_operations:\n\n\n# --- truncated at 32 KB (44 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/crowdstrike/refs/heads/main/scopes/crowdstrike-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdstrike/refs/heads/main/scopes/crowdstrike-scopes.yml
summary_line: 187 scopes
tags:
- Cybersecurity
- Endpoint Security
- EDR
- Threat Intelligence
- Cloud Security
- Identity Protection
- Vulnerability Management
- SIEM
- Security Operations
- MCP
token_urls: []
---
