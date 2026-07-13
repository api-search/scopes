---
api_specs:
- filename: auth0-management-api-openapi.yml
  format: yaml
  label: Auth0 Management API
  slug: auth0-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-management-api-openapi.yml
- filename: auth0-authentication-api-openapi.yml
  format: yaml
  label: Auth0 Authentication API
  slug: auth0-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-authentication-api-openapi.yml
- filename: auth0-fga-openapi.yml
  format: yaml
  label: Auth0 FGA (Fine-Grained Authorization)
  slug: auth0-fga
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-fga-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Auth0 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Auth0 publishes 221 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Auth0 API on a user''s behalf.


  Tokens are issued from /oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Auth0
provider_slug: auth0
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token/
  name: oAuth2ClientCredentials
  source: openapi/auth0-management-api-openapi.yml
scope_count: 221
scope_names:
- create:actions
- create:authentication_methods
- create:client_credentials
- create:client_grants
- create:clients
- create:connection_profiles
- create:connections
- create:connections_keys
- create:current_user_device_credentials
- create:custom_domains
- create:custom_signing_keys
- create:directory_provisionings
- create:email_provider
- create:email_templates
- create:encryption_keys
- create:event_streams
- create:flows
- create:flows_vault_connections
- create:forms
- create:guardian_enrollment_tickets
- create:hooks
- create:log_streams
- create:network_acls
- create:organization_client_grants
- create:organization_connections
- create:organization_discovery_domains
- create:organization_invitations
- create:organization_member_roles
- create:organization_members
- create:organizations
- create:phone_providers
- create:phone_templates
- create:resource_servers
- create:role_members
- create:roles
- create:rules
- create:scim_config
- create:scim_token
- create:self_service_profiles
- create:signing_keys
- create:sso_access_tickets
- create:token_exchange_profiles
- create:user_attribute_profiles
- create:user_tickets
- create:users
- create:vdcs_templates
- delete:actions
- delete:anomaly_blocks
- delete:authentication_methods
- delete:branding
- delete:client_credentials
- delete:client_grants
- delete:clients
- delete:connection_profiles
- delete:connections
- delete:current_user
- delete:current_user_device_credentials
- delete:custom_domains
- delete:custom_signing_keys
- delete:device_credentials
- delete:directory_provisionings
- delete:email_provider
- delete:encryption_keys
- delete:event_streams
- delete:federated_connections_tokens
- delete:flows
- delete:flows_executions
- delete:flows_vault_connections
- delete:forms
- delete:grants
- delete:groups
- delete:guardian_enrollments
- delete:hooks
- delete:log_streams
- delete:network_acls
- delete:organization_client_grants
- delete:organization_connections
- delete:organization_discovery_domains
- delete:organization_invitations
- delete:organization_member_roles
- delete:organization_members
- delete:organizations
- delete:phone_providers
- delete:phone_templates
- delete:refresh_tokens
- delete:resource_servers
- delete:role_members
- delete:roles
- delete:rules
- delete:rules_configs
- delete:scim_config
- delete:scim_token
- delete:self_service_profiles
- delete:sessions
- delete:sso_access_tickets
- delete:token_exchange_profiles
- delete:user_attribute_profiles
- delete:users
- delete:vdcs_templates
- read:actions
- read:anomaly_blocks
- read:attack_protection
- read:authentication_methods
- read:branding
- read:client_credentials
- read:client_grants
- read:client_keys
- read:client_summary
- read:clients
- read:connection_profiles
- read:connections
- read:connections_keys
- read:current_user
- read:custom_domains
- read:custom_signing_keys
- read:device_credentials
- read:directory_provisionings
- read:email_provider
- read:email_templates
- read:encryption_keys
- read:event_deliveries
- read:event_streams
- read:events
- read:federated_connections_tokens
- read:flows
- read:flows_executions
- read:flows_vault_connections
- read:forms
- read:grants
- read:group_members
- read:groups
- read:guardian_enrollments
- read:guardian_factors
- read:hooks
- read:log_streams
- read:logs
- read:logs_users
- read:mfa_policies
- read:network_acls
- read:organization_client_grants
- read:organization_connections
- read:organization_discovery_domains
- read:organization_invitations
- read:organization_member_roles
- read:organization_members
- read:organizations
- read:organizations_summary
- read:phone_providers
- read:phone_templates
- read:prompts
- read:refresh_tokens
- read:resource_servers
- read:role_members
- read:roles
- read:rules
- read:rules_configs
- read:scim_config
- read:scim_token
- read:self_service_profile_custom_texts
- read:self_service_profiles
- read:sessions
- read:signing_keys
- read:stats
- read:tenant_settings
- read:token_exchange_profiles
- read:user_attribute_profiles
- read:user_idp_tokens
- read:users
- read:vdcs_templates
- update:actions
- update:attack_protection
- update:authentication_methods
- update:branding
- update:client_credentials
- update:client_grants
- update:client_keys
- update:client_token_vault_privileged_access
- update:clients
- update:connection_profiles
- update:connections
- update:connections_keys
- update:current_user_identities
- update:current_user_metadata
- update:custom_domains
- update:custom_signing_keys
- update:directory_provisionings
- update:email_provider
- update:email_templates
- update:encryption_keys
- update:event_deliveries
- update:event_streams
- update:flows
- update:flows_vault_connections
- update:forms
- update:guardian_factors
- update:hooks
- update:log_streams
- update:mfa_policies
- update:network_acls
- update:organization_connections
- update:organization_discovery_domains
- update:organizations
- update:phone_providers
- update:phone_templates
- update:prompts
- update:refresh_tokens
- update:resource_servers
- update:roles
- update:rules
- update:rules_configs
- update:scim_config
- update:self_service_profile_custom_texts
- update:self_service_profiles
- update:sessions
- update:signing_keys
- update:tenant_settings
- update:token_exchange_profiles
- update:user_attribute_profiles
- update:users
- update:users_app_metadata
- update:vdcs_templates
scopes:
- description: Create Actions
  flows:
  - clientCredentials
  scope: create:actions
- description: Create Authentication Methods
  flows:
  - clientCredentials
  scope: create:authentication_methods
- description: Create Client Credentials
  flows:
  - clientCredentials
  scope: create:client_credentials
- description: Create Client Grants
  flows:
  - clientCredentials
  scope: create:client_grants
- description: Create Clients
  flows:
  - clientCredentials
  scope: create:clients
- description: Create Connection Profiles
  flows:
  - clientCredentials
  scope: create:connection_profiles
- description: Create Connections
  flows:
  - clientCredentials
  scope: create:connections
- description: Create Connections Keys
  flows:
  - clientCredentials
  scope: create:connections_keys
- description: Create Current User Device Credentials
  flows:
  - clientCredentials
  scope: create:current_user_device_credentials
- description: Create Custom Domains
  flows:
  - clientCredentials
  scope: create:custom_domains
- description: Create Custom Signing Keys
  flows:
  - clientCredentials
  scope: create:custom_signing_keys
- description: Create Directory Provisionings
  flows:
  - clientCredentials
  scope: create:directory_provisionings
- description: Create Email Provider
  flows:
  - clientCredentials
  scope: create:email_provider
- description: Create Email Templates
  flows:
  - clientCredentials
  scope: create:email_templates
- description: Create Encryption Keys
  flows:
  - clientCredentials
  scope: create:encryption_keys
- description: Create Event Streams
  flows:
  - clientCredentials
  scope: create:event_streams
- description: Create Flows
  flows:
  - clientCredentials
  scope: create:flows
- description: Create Flows Vault Connections
  flows:
  - clientCredentials
  scope: create:flows_vault_connections
- description: Create Forms
  flows:
  - clientCredentials
  scope: create:forms
- description: Create Guardian Enrollment Tickets
  flows:
  - clientCredentials
  scope: create:guardian_enrollment_tickets
- description: Create Hooks
  flows:
  - clientCredentials
  scope: create:hooks
- description: Create Log Streams
  flows:
  - clientCredentials
  scope: create:log_streams
- description: Create Network Acls
  flows:
  - clientCredentials
  scope: create:network_acls
- description: Create Organization Client Grants
  flows:
  - clientCredentials
  scope: create:organization_client_grants
- description: Create Organization Connections
  flows:
  - clientCredentials
  scope: create:organization_connections
- description: Create Organization Discovery Domains
  flows:
  - clientCredentials
  scope: create:organization_discovery_domains
- description: Create Organization Invitations
  flows:
  - clientCredentials
  scope: create:organization_invitations
- description: Create Organization Member Roles
  flows:
  - clientCredentials
  scope: create:organization_member_roles
- description: Create Organization Members
  flows:
  - clientCredentials
  scope: create:organization_members
- description: Create Organizations
  flows:
  - clientCredentials
  scope: create:organizations
- description: Create Phone Providers
  flows:
  - clientCredentials
  scope: create:phone_providers
- description: Create Phone Templates
  flows:
  - clientCredentials
  scope: create:phone_templates
- description: Create Resource Servers
  flows:
  - clientCredentials
  scope: create:resource_servers
- description: Create Role Members
  flows:
  - clientCredentials
  scope: create:role_members
- description: Create Roles
  flows:
  - clientCredentials
  scope: create:roles
- description: Create Rules
  flows:
  - clientCredentials
  scope: create:rules
- description: Create Scim Config
  flows:
  - clientCredentials
  scope: create:scim_config
- description: Create Scim Token
  flows:
  - clientCredentials
  scope: create:scim_token
- description: Create Self Service Profiles
  flows:
  - clientCredentials
  scope: create:self_service_profiles
- description: Create Signing Keys
  flows:
  - clientCredentials
  scope: create:signing_keys
- description: Create Sso Access Tickets
  flows:
  - clientCredentials
  scope: create:sso_access_tickets
- description: Create Token Exchange Profiles
  flows:
  - clientCredentials
  scope: create:token_exchange_profiles
- description: Create User Attribute Profiles
  flows:
  - clientCredentials
  scope: create:user_attribute_profiles
- description: Create User Tickets
  flows:
  - clientCredentials
  scope: create:user_tickets
- description: Create Users
  flows:
  - clientCredentials
  scope: create:users
- description: Create Vdcs Templates
  flows:
  - clientCredentials
  scope: create:vdcs_templates
- description: Delete Actions
  flows:
  - clientCredentials
  scope: delete:actions
- description: Delete Anomaly Blocks
  flows:
  - clientCredentials
  scope: delete:anomaly_blocks
- description: Delete Authentication Methods
  flows:
  - clientCredentials
  scope: delete:authentication_methods
- description: Delete Branding
  flows:
  - clientCredentials
  scope: delete:branding
- description: Delete Client Credentials
  flows:
  - clientCredentials
  scope: delete:client_credentials
- description: Delete Client Grants
  flows:
  - clientCredentials
  scope: delete:client_grants
- description: Delete Clients
  flows:
  - clientCredentials
  scope: delete:clients
- description: Delete Connection Profiles
  flows:
  - clientCredentials
  scope: delete:connection_profiles
- description: Delete Connections
  flows:
  - clientCredentials
  scope: delete:connections
- description: Delete Current User
  flows:
  - clientCredentials
  scope: delete:current_user
- description: Delete Current User Device Credentials
  flows:
  - clientCredentials
  scope: delete:current_user_device_credentials
- description: Delete Custom Domains
  flows:
  - clientCredentials
  scope: delete:custom_domains
- description: Delete Custom Signing Keys
  flows:
  - clientCredentials
  scope: delete:custom_signing_keys
- description: Delete Device Credentials
  flows:
  - clientCredentials
  scope: delete:device_credentials
- description: Delete Directory Provisionings
  flows:
  - clientCredentials
  scope: delete:directory_provisionings
- description: Delete Email Provider
  flows:
  - clientCredentials
  scope: delete:email_provider
- description: Delete Encryption Keys
  flows:
  - clientCredentials
  scope: delete:encryption_keys
- description: Delete Event Streams
  flows:
  - clientCredentials
  scope: delete:event_streams
- description: Delete Federated Connections Tokens
  flows:
  - clientCredentials
  scope: delete:federated_connections_tokens
- description: Delete Flows
  flows:
  - clientCredentials
  scope: delete:flows
- description: Delete Flows Executions
  flows:
  - clientCredentials
  scope: delete:flows_executions
- description: Delete Flows Vault Connections
  flows:
  - clientCredentials
  scope: delete:flows_vault_connections
- description: Delete Forms
  flows:
  - clientCredentials
  scope: delete:forms
- description: Delete Grants
  flows:
  - clientCredentials
  scope: delete:grants
- description: Delete Groups
  flows:
  - clientCredentials
  scope: delete:groups
- description: Delete Guardian Enrollments
  flows:
  - clientCredentials
  scope: delete:guardian_enrollments
- description: Delete Hooks
  flows:
  - clientCredentials
  scope: delete:hooks
- description: Delete Log Streams
  flows:
  - clientCredentials
  scope: delete:log_streams
- description: Delete Network Acls
  flows:
  - clientCredentials
  scope: delete:network_acls
- description: Delete Organization Client Grants
  flows:
  - clientCredentials
  scope: delete:organization_client_grants
- description: Delete Organization Connections
  flows:
  - clientCredentials
  scope: delete:organization_connections
- description: Delete Organization Discovery Domains
  flows:
  - clientCredentials
  scope: delete:organization_discovery_domains
- description: Delete Organization Invitations
  flows:
  - clientCredentials
  scope: delete:organization_invitations
- description: Delete Organization Member Roles
  flows:
  - clientCredentials
  scope: delete:organization_member_roles
- description: Delete Organization Members
  flows:
  - clientCredentials
  scope: delete:organization_members
- description: Delete Organizations
  flows:
  - clientCredentials
  scope: delete:organizations
- description: Delete Phone Providers
  flows:
  - clientCredentials
  scope: delete:phone_providers
- description: Delete Phone Templates
  flows:
  - clientCredentials
  scope: delete:phone_templates
- description: Delete Refresh Tokens
  flows:
  - clientCredentials
  scope: delete:refresh_tokens
- description: Delete Resource Servers
  flows:
  - clientCredentials
  scope: delete:resource_servers
- description: Delete Role Members
  flows:
  - clientCredentials
  scope: delete:role_members
- description: Delete Roles
  flows:
  - clientCredentials
  scope: delete:roles
- description: Delete Rules
  flows:
  - clientCredentials
  scope: delete:rules
- description: Delete Rules Configs
  flows:
  - clientCredentials
  scope: delete:rules_configs
- description: Delete Scim Config
  flows:
  - clientCredentials
  scope: delete:scim_config
- description: Delete Scim Token
  flows:
  - clientCredentials
  scope: delete:scim_token
- description: Delete Self Service Profiles
  flows:
  - clientCredentials
  scope: delete:self_service_profiles
- description: Delete Sessions
  flows:
  - clientCredentials
  scope: delete:sessions
- description: Delete Sso Access Tickets
  flows:
  - clientCredentials
  scope: delete:sso_access_tickets
- description: Delete Token Exchange Profiles
  flows:
  - clientCredentials
  scope: delete:token_exchange_profiles
- description: Delete User Attribute Profiles
  flows:
  - clientCredentials
  scope: delete:user_attribute_profiles
- description: Delete Users
  flows:
  - clientCredentials
  scope: delete:users
- description: Delete Vdcs Templates
  flows:
  - clientCredentials
  scope: delete:vdcs_templates
- description: Read Actions
  flows:
  - clientCredentials
  scope: read:actions
- description: Read Anomaly Blocks
  flows:
  - clientCredentials
  scope: read:anomaly_blocks
- description: Read Attack Protection
  flows:
  - clientCredentials
  scope: read:attack_protection
- description: Read Authentication Methods
  flows:
  - clientCredentials
  scope: read:authentication_methods
- description: Read Branding
  flows:
  - clientCredentials
  scope: read:branding
- description: Read Client Credentials
  flows:
  - clientCredentials
  scope: read:client_credentials
- description: Read Client Grants
  flows:
  - clientCredentials
  scope: read:client_grants
- description: Read Client Keys
  flows:
  - clientCredentials
  scope: read:client_keys
- description: Read Client Summary
  flows:
  - clientCredentials
  scope: read:client_summary
- description: Read Clients
  flows:
  - clientCredentials
  scope: read:clients
- description: Read Connection Profiles
  flows:
  - clientCredentials
  scope: read:connection_profiles
- description: Read Connections
  flows:
  - clientCredentials
  scope: read:connections
- description: Read Connections Keys
  flows:
  - clientCredentials
  scope: read:connections_keys
- description: Read Current User
  flows:
  - clientCredentials
  scope: read:current_user
- description: Read Custom Domains
  flows:
  - clientCredentials
  scope: read:custom_domains
- description: Read Custom Signing Keys
  flows:
  - clientCredentials
  scope: read:custom_signing_keys
- description: Read Device Credentials
  flows:
  - clientCredentials
  scope: read:device_credentials
- description: Read Directory Provisionings
  flows:
  - clientCredentials
  scope: read:directory_provisionings
- description: Read Email Provider
  flows:
  - clientCredentials
  scope: read:email_provider
- description: Read Email Templates
  flows:
  - clientCredentials
  scope: read:email_templates
- description: Read Encryption Keys
  flows:
  - clientCredentials
  scope: read:encryption_keys
- description: Read Event Deliveries
  flows:
  - clientCredentials
  scope: read:event_deliveries
- description: Read Event Streams
  flows:
  - clientCredentials
  scope: read:event_streams
- description: Read Events
  flows:
  - clientCredentials
  scope: read:events
- description: Read Federated Connections Tokens
  flows:
  - clientCredentials
  scope: read:federated_connections_tokens
- description: Read Flows
  flows:
  - clientCredentials
  scope: read:flows
- description: Read Flows Executions
  flows:
  - clientCredentials
  scope: read:flows_executions
- description: Read Flows Vault Connections
  flows:
  - clientCredentials
  scope: read:flows_vault_connections
- description: Read Forms
  flows:
  - clientCredentials
  scope: read:forms
- description: Read Grants
  flows:
  - clientCredentials
  scope: read:grants
- description: Read Group Members
  flows:
  - clientCredentials
  scope: read:group_members
- description: Read Groups
  flows:
  - clientCredentials
  scope: read:groups
- description: Read Guardian Enrollments
  flows:
  - clientCredentials
  scope: read:guardian_enrollments
- description: Read Guardian Factors
  flows:
  - clientCredentials
  scope: read:guardian_factors
- description: Read Hooks
  flows:
  - clientCredentials
  scope: read:hooks
- description: Read Log Streams
  flows:
  - clientCredentials
  scope: read:log_streams
- description: Read Logs
  flows:
  - clientCredentials
  scope: read:logs
- description: Read Logs Users
  flows:
  - clientCredentials
  scope: read:logs_users
- description: Read Mfa Policies
  flows:
  - clientCredentials
  scope: read:mfa_policies
- description: Read Network Acls
  flows:
  - clientCredentials
  scope: read:network_acls
- description: Read Organization Client Grants
  flows:
  - clientCredentials
  scope: read:organization_client_grants
- description: Read Organization Connections
  flows:
  - clientCredentials
  scope: read:organization_connections
- description: Read Organization Discovery Domains
  flows:
  - clientCredentials
  scope: read:organization_discovery_domains
- description: Read Organization Invitations
  flows:
  - clientCredentials
  scope: read:organization_invitations
- description: Read Organization Member Roles
  flows:
  - clientCredentials
  scope: read:organization_member_roles
- description: Read Organization Members
  flows:
  - clientCredentials
  scope: read:organization_members
- description: Read Organizations
  flows:
  - clientCredentials
  scope: read:organizations
- description: Read Organizations Summary
  flows:
  - clientCredentials
  scope: read:organizations_summary
- description: Read Phone Providers
  flows:
  - clientCredentials
  scope: read:phone_providers
- description: Read Phone Templates
  flows:
  - clientCredentials
  scope: read:phone_templates
- description: Read Prompts
  flows:
  - clientCredentials
  scope: read:prompts
- description: Read Refresh Tokens
  flows:
  - clientCredentials
  scope: read:refresh_tokens
- description: Read Resource Servers
  flows:
  - clientCredentials
  scope: read:resource_servers
- description: Read Role Members
  flows:
  - clientCredentials
  scope: read:role_members
- description: Read Roles
  flows:
  - clientCredentials
  scope: read:roles
- description: Read Rules
  flows:
  - clientCredentials
  scope: read:rules
- description: Read Rules Configs
  flows:
  - clientCredentials
  scope: read:rules_configs
- description: Read Scim Config
  flows:
  - clientCredentials
  scope: read:scim_config
- description: Read Scim Token
  flows:
  - clientCredentials
  scope: read:scim_token
- description: Read Self Service Profile Custom Texts
  flows:
  - clientCredentials
  scope: read:self_service_profile_custom_texts
- description: Read Self Service Profiles
  flows:
  - clientCredentials
  scope: read:self_service_profiles
- description: Read Sessions
  flows:
  - clientCredentials
  scope: read:sessions
- description: Read Signing Keys
  flows:
  - clientCredentials
  scope: read:signing_keys
- description: Read Stats
  flows:
  - clientCredentials
  scope: read:stats
- description: Read Tenant Settings
  flows:
  - clientCredentials
  scope: read:tenant_settings
- description: Read Token Exchange Profiles
  flows:
  - clientCredentials
  scope: read:token_exchange_profiles
- description: Read User Attribute Profiles
  flows:
  - clientCredentials
  scope: read:user_attribute_profiles
- description: Read User Idp Tokens
  flows:
  - clientCredentials
  scope: read:user_idp_tokens
- description: Read Users
  flows:
  - clientCredentials
  scope: read:users
- description: Read Vdcs Templates
  flows:
  - clientCredentials
  scope: read:vdcs_templates
- description: Update Actions
  flows:
  - clientCredentials
  scope: update:actions
- description: Update Attack Protection
  flows:
  - clientCredentials
  scope: update:attack_protection
- description: Update Authentication Methods
  flows:
  - clientCredentials
  scope: update:authentication_methods
- description: Update Branding
  flows:
  - clientCredentials
  scope: update:branding
- description: Update Client Credentials
  flows:
  - clientCredentials
  scope: update:client_credentials
- description: Update Client Grants
  flows:
  - clientCredentials
  scope: update:client_grants
- description: Update Client Keys
  flows:
  - clientCredentials
  scope: update:client_keys
- description: Update Client Token Vault Privileged Access
  flows:
  - clientCredentials
  scope: update:client_token_vault_privileged_access
- description: Update Clients
  flows:
  - clientCredentials
  scope: update:clients
- description: Update Connection Profiles
  flows:
  - clientCredentials
  scope: update:connection_profiles
- description: Update Connections
  flows:
  - clientCredentials
  scope: update:connections
- description: Update Connections Keys
  flows:
  - clientCredentials
  scope: update:connections_keys
- description: Update Current User Identities
  flows:
  - clientCredentials
  scope: update:current_user_identities
- description: Update Current User Metadata
  flows:
  - clientCredentials
  scope: update:current_user_metadata
- description: Update Custom Domains
  flows:
  - clientCredentials
  scope: update:custom_domains
- description: Update Custom Signing Keys
  flows:
  - clientCredentials
  scope: update:custom_signing_keys
- description: Update Directory Provisionings
  flows:
  - clientCredentials
  scope: update:directory_provisionings
- description: Update Email Provider
  flows:
  - clientCredentials
  scope: update:email_provider
- description: Update Email Templates
  flows:
  - clientCredentials
  scope: update:email_templates
- description: Update Encryption Keys
  flows:
  - clientCredentials
  scope: update:encryption_keys
- description: Update Event Deliveries
  flows:
  - clientCredentials
  scope: update:event_deliveries
- description: Update Event Streams
  flows:
  - clientCredentials
  scope: update:event_streams
- description: Update Flows
  flows:
  - clientCredentials
  scope: update:flows
- description: Update Flows Vault Connections
  flows:
  - clientCredentials
  scope: update:flows_vault_connections
- description: Update Forms
  flows:
  - clientCredentials
  scope: update:forms
- description: Update Guardian Factors
  flows:
  - clientCredentials
  scope: update:guardian_factors
- description: Update Hooks
  flows:
  - clientCredentials
  scope: update:hooks
- description: Update Log Streams
  flows:
  - clientCredentials
  scope: update:log_streams
- description: Update Mfa Policies
  flows:
  - clientCredentials
  scope: update:mfa_policies
- description: Update Network Acls
  flows:
  - clientCredentials
  scope: update:network_acls
- description: Update Organization Connections
  flows:
  - clientCredentials
  scope: update:organization_connections
- description: Update Organization Discovery Domains
  flows:
  - clientCredentials
  scope: update:organization_discovery_domains
- description: Update Organizations
  flows:
  - clientCredentials
  scope: update:organizations
- description: Update Phone Providers
  flows:
  - clientCredentials
  scope: update:phone_providers
- description: Update Phone Templates
  flows:
  - clientCredentials
  scope: update:phone_templates
- description: Update Prompts
  flows:
  - clientCredentials
  scope: update:prompts
- description: Update Refresh Tokens
  flows:
  - clientCredentials
  scope: update:refresh_tokens
- description: Update Resource Servers
  flows:
  - clientCredentials
  scope: update:resource_servers
- description: Update Roles
  flows:
  - clientCredentials
  scope: update:roles
- description: Update Rules
  flows:
  - clientCredentials
  scope: update:rules
- description: Update Rules Configs
  flows:
  - clientCredentials
  scope: update:rules_configs
- description: Update Scim Config
  flows:
  - clientCredentials
  scope: update:scim_config
- description: Update Self Service Profile Custom Texts
  flows:
  - clientCredentials
  scope: update:self_service_profile_custom_texts
- description: Update Self Service Profiles
  flows:
  - clientCredentials
  scope: update:self_service_profiles
- description: Update Sessions
  flows:
  - clientCredentials
  scope: update:sessions
- description: Update Signing Keys
  flows:
  - clientCredentials
  scope: update:signing_keys
- description: Update Tenant Settings
  flows:
  - clientCredentials
  scope: update:tenant_settings
- description: Update Token Exchange Profiles
  flows:
  - clientCredentials
  scope: update:token_exchange_profiles
- description: Update User Attribute Profiles
  flows:
  - clientCredentials
  scope: update:user_attribute_profiles
- description: Update Users
  flows:
  - clientCredentials
  scope: update:users
- description: Update Users App Metadata
  flows:
  - clientCredentials
  scope: update:users_app_metadata
- description: Update Vdcs Templates
  flows:
  - clientCredentials
  scope: update:vdcs_templates
slug: auth0-scopes
source_filename: auth0-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/auth0-management-api-openapi.yml\nschemes:\n- name: oAuth2ClientCredentials\n  source: openapi/auth0-management-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token/\nscopes:\n- scope: create:actions\n  description: Create Actions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:authentication_methods\n  description: Create Authentication Methods\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:client_credentials\n  description: Create Client Credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:client_grants\n  description: Create Client Grants\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:clients\n  description: Create Clients\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:connection_profiles\n  description: Create Connection Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:connections\n  description: Create Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:connections_keys\n  description: Create Connections Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:current_user_device_credentials\n  description: Create Current User Device Credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:custom_domains\n  description: Create Custom Domains\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:custom_signing_keys\n  description: Create Custom Signing Keys\n  flows:\n  -\
  \ clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:directory_provisionings\n  description: Create Directory Provisionings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:email_provider\n  description: Create Email Provider\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:email_templates\n  description: Create Email Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:encryption_keys\n  description: Create Encryption Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:event_streams\n  description: Create Event Streams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:flows\n  description: Create Flows\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/auth0-management-api-openapi.yml\n- scope: create:flows_vault_connections\n  description: Create Flows Vault Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:forms\n  description: Create Forms\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:guardian_enrollment_tickets\n  description: Create Guardian Enrollment Tickets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:hooks\n  description: Create Hooks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:log_streams\n  description: Create Log Streams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:network_acls\n  description: Create Network Acls\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n\
  - scope: create:organization_client_grants\n  description: Create Organization Client Grants\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:organization_connections\n  description: Create Organization Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:organization_discovery_domains\n  description: Create Organization Discovery Domains\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:organization_invitations\n  description: Create Organization Invitations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:organization_member_roles\n  description: Create Organization Member Roles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:organization_members\n  description: Create Organization Members\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:organizations\n  description: Create Organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:phone_providers\n  description: Create Phone Providers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:phone_templates\n  description: Create Phone Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:resource_servers\n  description: Create Resource Servers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:role_members\n  description: Create Role Members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:roles\n  description: Create Roles\n  flows:\n  - clientCredentials\n  sources:\n  -\
  \ openapi/auth0-management-api-openapi.yml\n- scope: create:rules\n  description: Create Rules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:scim_config\n  description: Create Scim Config\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:scim_token\n  description: Create Scim Token\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:self_service_profiles\n  description: Create Self Service Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:signing_keys\n  description: Create Signing Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:sso_access_tickets\n  description: Create Sso Access Tickets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope:\
  \ create:token_exchange_profiles\n  description: Create Token Exchange Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:user_attribute_profiles\n  description: Create User Attribute Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:user_tickets\n  description: Create User Tickets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:users\n  description: Create Users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: create:vdcs_templates\n  description: Create Vdcs Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:actions\n  description: Delete Actions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:anomaly_blocks\n  description:\
  \ Delete Anomaly Blocks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:authentication_methods\n  description: Delete Authentication Methods\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:branding\n  description: Delete Branding\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:client_credentials\n  description: Delete Client Credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:client_grants\n  description: Delete Client Grants\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:clients\n  description: Delete Clients\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:connection_profiles\n  description: Delete Connection Profiles\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:connections\n  description: Delete Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:current_user\n  description: Delete Current User\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:current_user_device_credentials\n  description: Delete Current User Device Credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:custom_domains\n  description: Delete Custom Domains\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:custom_signing_keys\n  description: Delete Custom Signing Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:device_credentials\n  description: Delete Device Credentials\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:directory_provisionings\n  description: Delete Directory Provisionings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:email_provider\n  description: Delete Email Provider\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:encryption_keys\n  description: Delete Encryption Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:event_streams\n  description: Delete Event Streams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:federated_connections_tokens\n  description: Delete Federated Connections Tokens\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:flows\n  description: Delete Flows\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:flows_executions\n  description: Delete Flows Executions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:flows_vault_connections\n  description: Delete Flows Vault Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:forms\n  description: Delete Forms\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:grants\n  description: Delete Grants\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:groups\n  description: Delete Groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:guardian_enrollments\n  description: Delete Guardian Enrollments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n\
  - scope: delete:hooks\n  description: Delete Hooks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:log_streams\n  description: Delete Log Streams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:network_acls\n  description: Delete Network Acls\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:organization_client_grants\n  description: Delete Organization Client Grants\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:organization_connections\n  description: Delete Organization Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:organization_discovery_domains\n  description: Delete Organization Discovery Domains\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n\
  - scope: delete:organization_invitations\n  description: Delete Organization Invitations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:organization_member_roles\n  description: Delete Organization Member Roles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:organization_members\n  description: Delete Organization Members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:organizations\n  description: Delete Organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:phone_providers\n  description: Delete Phone Providers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:phone_templates\n  description: Delete Phone Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n\
  - scope: delete:refresh_tokens\n  description: Delete Refresh Tokens\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:resource_servers\n  description: Delete Resource Servers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:role_members\n  description: Delete Role Members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:roles\n  description: Delete Roles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:rules\n  description: Delete Rules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:rules_configs\n  description: Delete Rules Configs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:scim_config\n  description: Delete Scim Config\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:scim_token\n  description: Delete Scim Token\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:self_service_profiles\n  description: Delete Self Service Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:sessions\n  description: Delete Sessions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:sso_access_tickets\n  description: Delete Sso Access Tickets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:token_exchange_profiles\n  description: Delete Token Exchange Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:user_attribute_profiles\n  description: Delete User Attribute Profiles\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:users\n  description: Delete Users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: delete:vdcs_templates\n  description: Delete Vdcs Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:actions\n  description: Read Actions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:anomaly_blocks\n  description: Read Anomaly Blocks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:attack_protection\n  description: Read Attack Protection\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:authentication_methods\n  description: Read Authentication Methods\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n\
  - scope: read:branding\n  description: Read Branding\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:client_credentials\n  description: Read Client Credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:client_grants\n  description: Read Client Grants\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:client_keys\n  description: Read Client Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:client_summary\n  description: Read Client Summary\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:clients\n  description: Read Clients\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:connection_profiles\n  description: Read Connection Profiles\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:connections\n  description: Read Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:connections_keys\n  description: Read Connections Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:current_user\n  description: Read Current User\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:custom_domains\n  description: Read Custom Domains\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:custom_signing_keys\n  description: Read Custom Signing Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:device_credentials\n  description: Read Device Credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n\
  - scope: read:directory_provisionings\n  description: Read Directory Provisionings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:email_provider\n  description: Read Email Provider\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:email_templates\n  description: Read Email Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:encryption_keys\n  description: Read Encryption Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:event_deliveries\n  description: Read Event Deliveries\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:event_streams\n  description: Read Event Streams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:events\n  description:\
  \ Read Events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:federated_connections_tokens\n  description: Read Federated Connections Tokens\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:flows\n  description: Read Flows\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:flows_executions\n  description: Read Flows Executions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:flows_vault_connections\n  description: Read Flows Vault Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:forms\n  description: Read Forms\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:grants\n  description: Read Grants\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/auth0-management-api-openapi.yml\n- scope: read:group_members\n  description: Read Group Members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:groups\n  description: Read Groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:guardian_enrollments\n  description: Read Guardian Enrollments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:guardian_factors\n  description: Read Guardian Factors\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:hooks\n  description: Read Hooks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:log_streams\n  description: Read Log Streams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:logs\n  description: Read\
  \ Logs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:logs_users\n  description: Read Logs Users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:mfa_policies\n  description: Read Mfa Policies\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:network_acls\n  description: Read Network Acls\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:organization_client_grants\n  description: Read Organization Client Grants\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:organization_connections\n  description: Read Organization Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:organization_discovery_domains\n  description: Read Organization Discovery\
  \ Domains\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:organization_invitations\n  description: Read Organization Invitations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:organization_member_roles\n  description: Read Organization Member Roles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:organization_members\n  description: Read Organization Members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:organizations\n  description: Read Organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:organizations_summary\n  description: Read Organizations Summary\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:phone_providers\n  description: Read\
  \ Phone Providers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:phone_templates\n  description: Read Phone Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:prompts\n  description: Read Prompts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:refresh_tokens\n  description: Read Refresh Tokens\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:resource_servers\n  description: Read Resource Servers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:role_members\n  description: Read Role Members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:roles\n  description: Read Roles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n\
  - scope: read:rules\n  description: Read Rules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:rules_configs\n  description: Read Rules Configs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:scim_config\n  description: Read Scim Config\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:scim_token\n  description: Read Scim Token\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:self_service_profile_custom_texts\n  description: Read Self Service Profile Custom Texts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:self_service_profiles\n  description: Read Self Service Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:sessions\n  description: Read\
  \ Sessions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:signing_keys\n  description: Read Signing Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:stats\n  description: Read Stats\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:tenant_settings\n  description: Read Tenant Settings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:token_exchange_profiles\n  description: Read Token Exchange Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:user_attribute_profiles\n  description: Read User Attribute Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:user_idp_tokens\n  description: Read User Idp Tokens\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:users\n  description: Read Users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: read:vdcs_templates\n  description: Read Vdcs Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:actions\n  description: Update Actions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:attack_protection\n  description: Update Attack Protection\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:authentication_methods\n  description: Update Authentication Methods\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:branding\n  description: Update Branding\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope:\
  \ update:client_credentials\n  description: Update Client Credentials\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:client_grants\n  description: Update Client Grants\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:client_keys\n  description: Update Client Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:client_token_vault_privileged_access\n  description: Update Client Token Vault Privileged Access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:clients\n  description: Update Clients\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:connection_profiles\n  description: Update Connection Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n\
  - scope: update:connections\n  description: Update Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:connections_keys\n  description: Update Connections Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:current_user_identities\n  description: Update Current User Identities\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:current_user_metadata\n  description: Update Current User Metadata\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:custom_domains\n  description: Update Custom Domains\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:custom_signing_keys\n  description: Update Custom Signing Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n\
  - scope: update:directory_provisionings\n  description: Update Directory Provisionings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:email_provider\n  description: Update Email Provider\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:email_templates\n  description: Update Email Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:encryption_keys\n  description: Update Encryption Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:event_deliveries\n  description: Update Event Deliveries\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:event_streams\n  description: Update Event Streams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:flows\n\
  \  description: Update Flows\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:flows_vault_connections\n  description: Update Flows Vault Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:forms\n  description: Update Forms\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:guardian_factors\n  description: Update Guardian Factors\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:hooks\n  description: Update Hooks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:log_streams\n  description: Update Log Streams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:mfa_policies\n  description: Update Mfa Policies\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:network_acls\n  description: Update Network Acls\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:organization_connections\n  description: Update Organization Connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:organization_discovery_domains\n  description: Update Organization Discovery Domains\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:organizations\n  description: Update Organizations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:phone_providers\n  description: Update Phone Providers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:phone_templates\n  description: Update Phone Templates\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:prompts\n  description: Update Prompts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:refresh_tokens\n  description: Update Refresh Tokens\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:resource_servers\n  description: Update Resource Servers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:roles\n  description: Update Roles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- scope: update:rules\n  description: Update Rules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/auth0-management\n\n# --- truncated at 32 KB (33 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/scopes/auth0-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/scopes/auth0-scopes.yml
summary_line: 221 scopes · clientCredentials
tags:
- AI Agents
- Authentication
- Authorization
- FGA
- Identity Management
- MCP
- OAuth
- Okta
- OpenID Connect
- SAML
- Security
- SCIM
token_urls:
- /oauth/token/
---
