---
api_specs:
- filename: laravel-forge-openapi.json
  format: json
  label: Laravel Forge API
  slug: forge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laravel/refs/heads/main/openapi/laravel-forge-openapi.json
- filename: laravel-cloud-openapi.json
  format: json
  label: Laravel Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laravel/refs/heads/main/openapi/laravel-cloud-openapi.json
authorization_urls:
- https://forge.laravel.com/oauth/authorize
description: ''
docs: https://forge.laravel.com/docs/api
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Laravel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Laravel publishes 62 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Laravel API on a user''s behalf.


  Tokens are issued from https://forge.laravel.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Laravel
provider_slug: laravel
schemes:
- flows:
  - authorizationUrl: https://forge.laravel.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://forge.laravel.com/oauth/token
  name: oauth2
  source: openapi/laravel-forge-openapi.json
scope_count: 62
scope_names:
- billing:manage
- credential:manage
- credential:view
- integrations:manage
- organization:delete
- organization:manage
- organization:view
- recipe:manage
- recipe:view
- resources:create-buckets
- resources:create-databases
- resources:delete-buckets
- resources:delete-databases
- resources:manage-buckets
- resources:manage-databases
- resources:view
- server:archive
- server:create
- server:create-backups
- server:create-daemons
- server:create-databases
- server:create-keys
- server:create-monitors
- server:create-schedulers
- server:delete
- server:delete-backups
- server:delete-daemons
- server:delete-databases
- server:delete-keys
- server:delete-monitors
- server:delete-schedulers
- server:manage-logs
- server:manage-meta
- server:manage-network
- server:manage-nginx-templates
- server:manage-packages
- server:manage-password
- server:manage-php
- server:manage-services
- server:transfer
- server:view
- server:web-terminal
- site:create
- site:delete
- site:manage-commands
- site:manage-deploys
- site:manage-environment
- site:manage-heartbeats
- site:manage-integrations
- site:manage-nginx
- site:manage-notifications
- site:manage-project
- site:manage-queues
- site:manage-redirects
- site:manage-security
- site:manage-ssl
- site:meta
- storage:manage
- team:create
- team:delete
- team:view
- user:view
scopes:
- description: Allow members to manage the organization's subscription
  flows:
  - authorizationCode
  scope: billing:manage
- description: Allow members to manage credentials
  flows:
  - authorizationCode
  scope: credential:manage
- description: Allow members to view credentials
  flows:
  - authorizationCode
  scope: credential:view
- description: Allow members to manage the organization's integrations
  flows:
  - authorizationCode
  scope: integrations:manage
- description: Allow members to delete the organization
  flows:
  - authorizationCode
  scope: organization:delete
- description: Allow members to manage the organization
  flows:
  - authorizationCode
  scope: organization:manage
- description: Allow members to view the organization
  flows:
  - authorizationCode
  scope: organization:view
- description: Allow members to manage recipes
  flows:
  - authorizationCode
  scope: recipe:manage
- description: Allow members to view recipes
  flows:
  - authorizationCode
  scope: recipe:view
- description: Allow members to create object storage buckets
  flows:
  - authorizationCode
  scope: resources:create-buckets
- description: Allow members to create managed database & cache clusters
  flows:
  - authorizationCode
  scope: resources:create-databases
- description: Allow members to delete object storage buckets
  flows:
  - authorizationCode
  scope: resources:delete-buckets
- description: Allow members to delete managed database & cache clusters
  flows:
  - authorizationCode
  scope: resources:delete-databases
- description: Allow members to manage object storage buckets and their access keys
  flows:
  - authorizationCode
  scope: resources:manage-buckets
- description: Allow members to manage managed database & cache clusters settings
  flows:
  - authorizationCode
  scope: resources:manage-databases
- description: Allow members to view resources
  flows:
  - authorizationCode
  scope: resources:view
- description: Allow members to archive servers
  flows:
  - authorizationCode
  scope: server:archive
- description: Allow members to create servers
  flows:
  - authorizationCode
  scope: server:create
- description: Allow members to create database backup configurations
  flows:
  - authorizationCode
  scope: server:create-backups
- description: Allow members to create daemons
  flows:
  - authorizationCode
  scope: server:create-daemons
- description: Allow members to create databases and database users
  flows:
  - authorizationCode
  scope: server:create-databases
- description: Allow members to add SSH keys to servers
  flows:
  - authorizationCode
  scope: server:create-keys
- description: Allow members to create server monitors
  flows:
  - authorizationCode
  scope: server:create-monitors
- description: Allow members to create scheduled jobs
  flows:
  - authorizationCode
  scope: server:create-schedulers
- description: Allow members to delete servers
  flows:
  - authorizationCode
  scope: server:delete
- description: Allow members to delete database backup configurations
  flows:
  - authorizationCode
  scope: server:delete-backups
- description: Allow members to delete daemons
  flows:
  - authorizationCode
  scope: server:delete-daemons
- description: Allow members to delete databases and database users
  flows:
  - authorizationCode
  scope: server:delete-databases
- description: Allow members to remove SSH keys from servers
  flows:
  - authorizationCode
  scope: server:delete-keys
- description: Allow members to delete server monitors
  flows:
  - authorizationCode
  scope: server:delete-monitors
- description: Allow members to delete scheduled jobs
  flows:
  - authorizationCode
  scope: server:delete-schedulers
- description: Allow members to clear server and site logs
  flows:
  - authorizationCode
  scope: server:manage-logs
- description: Allow members to change server settings such as name and IP address
  flows:
  - authorizationCode
  scope: server:manage-meta
- description: Allow members to change the server‘s firewall
  flows:
  - authorizationCode
  scope: server:manage-network
- description: Allow members to manage Nginx templates
  flows:
  - authorizationCode
  scope: server:manage-nginx-templates
- description: Allow members to configure and remove server and site package authentication
  flows:
  - authorizationCode
  scope: server:manage-packages
- description: Allow members to reset the sudo password
  flows:
  - authorizationCode
  scope: server:manage-password
- description: Allow members to install and change PHP installations
  flows:
  - authorizationCode
  scope: server:manage-php
- description: Allow members to start, stop and restart services
  flows:
  - authorizationCode
  scope: server:manage-services
- description: Allow members to transfer servers to another Forge account
  flows:
  - authorizationCode
  scope: server:transfer
- description: Allow members to view servers
  flows:
  - authorizationCode
  scope: server:view
- description: Allow members to start web terminal sessions
  flows:
  - authorizationCode
  scope: server:web-terminal
- description: Allow members to create sites
  flows:
  - authorizationCode
  scope: site:create
- description: Allow members to delete sites
  flows:
  - authorizationCode
  scope: site:delete
- description: Allow members to run arbitrary commands from the site‘s root directory
  flows:
  - authorizationCode
  scope: site:manage-commands
- description: Allow members to deploy the site and update the deployment script
  flows:
  - authorizationCode
  scope: site:manage-deploys
- description: Allow members to update the site‘s environment file
  flows:
  - authorizationCode
  scope: site:manage-environment
- description: Allow members to manage heartbeats
  flows:
  - authorizationCode
  scope: site:manage-heartbeats
- description: Allow members to manage site integrations
  flows:
  - authorizationCode
  scope: site:manage-integrations
- description: Allow members to manage the site‘s Nginx configuration file
  flows:
  - authorizationCode
  scope: site:manage-nginx
- description: Allow members to configure deployment notifications
  flows:
  - authorizationCode
  scope: site:manage-notifications
- description: Allow members to install Git repositories, phpMyAdmin and WordPress applications
  flows:
  - authorizationCode
  scope: site:manage-project
- description: Allow members to configure queue workers
  flows:
  - authorizationCode
  scope: site:manage-queues
- description: Allow members to configure URL redirects
  flows:
  - authorizationCode
  scope: site:manage-redirects
- description: Allow members to configure HTTP Basic Authentication
  flows:
  - authorizationCode
  scope: site:manage-security
- description: Allow members to configure SSL and Let‘s Encrypt certificates
  flows:
  - authorizationCode
  scope: site:manage-ssl
- description: Allow members to update site meta data such as domain name and aliases
  flows:
  - authorizationCode
  scope: site:meta
- description: Allow members to manage the organization's storage providers.
  flows:
  - authorizationCode
  scope: storage:manage
- description: Allow members to create teams
  flows:
  - authorizationCode
  scope: team:create
- description: Allow members to delete teams and team members
  flows:
  - authorizationCode
  scope: team:delete
- description: Allow members to view teams
  flows:
  - authorizationCode
  scope: team:view
- description: Allow members to view user details
  flows:
  - authorizationCode
  scope: user:view
slug: laravel-scopes
source_filename: laravel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/laravel-forge-openapi.json\napi: laravel:forge-api\ndocs: https://forge.laravel.com/docs/api\nscope_count: 62\nnotes: The 62 scopes below are declared in the Forge OpenAPI oauth2 authorizationCode flow, each with a\n  provider-authored description. Laravel publishes no standalone scopes-reference page; the token\n  documentation (forge.laravel.com/docs/api) only instructs users to \"select the scopes you wish to\n  assign\" when creating a token in the API dashboard, so the OpenAPI remains the authoritative scope\n  registry. Scopes are namespaced by domain (organization, server, site, team, billing, credential,\n  integrations) with view/create/delete/manage verbs.\nother_oauth_surfaces:\n- issuer: https://id.laravel.com\n  role: end-user SSO identity provider (Laravel Cloud sign-in), distinct from the Forge resource API\n  scopes_supported:\n  - email\n  - offline_access\n  - openid\n  - profile\n  source: well-known/laravel-oauth-authorization-server.json\n\
  - api: laravel:cloud-api\n  model: bearer token only; no OAuth 2.0 scheme and no scope model is declared in the Cloud OpenAPI\n  source: openapi/laravel-cloud-openapi.json\n- api: laravel:envoyer-api\n  model: 'API-key bearer token with a coarse scope model documented in prose: all GET endpoints are\n    freely accessible with any API token, and *:create scopes govern creating and updating resources.'\n  source: https://envoyer.io/api-documentation\nschemes:\n- name: oauth2\n  source: openapi/laravel-forge-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://forge.laravel.com/oauth/authorize\n    tokenUrl: https://forge.laravel.com/oauth/token\nscopes:\n- scope: billing:manage\n  description: Allow members to manage the organization's subscription\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: credential:manage\n  description: Allow members to manage credentials\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/laravel-forge-openapi.json\n- scope: credential:view\n  description: Allow members to view credentials\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: integrations:manage\n  description: Allow members to manage the organization's integrations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: organization:delete\n  description: Allow members to delete the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: organization:manage\n  description: Allow members to manage the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: organization:view\n  description: Allow members to view the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: recipe:manage\n  description: Allow members to manage recipes\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: recipe:view\n  description: Allow members to view recipes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: resources:create-buckets\n  description: Allow members to create object storage buckets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: resources:create-databases\n  description: Allow members to create managed database & cache clusters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: resources:delete-buckets\n  description: Allow members to delete object storage buckets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: resources:delete-databases\n  description: Allow members to delete managed database & cache clusters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: resources:manage-buckets\n\
  \  description: Allow members to manage object storage buckets and their access keys\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: resources:manage-databases\n  description: Allow members to manage managed database & cache clusters settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: resources:view\n  description: Allow members to view resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:archive\n  description: Allow members to archive servers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:create\n  description: Allow members to create servers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:create-backups\n  description: Allow members to create database backup configurations\n  flows:\n  - authorizationCode\n  sources:\n \
  \ - openapi/laravel-forge-openapi.json\n- scope: server:create-daemons\n  description: Allow members to create daemons\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:create-databases\n  description: Allow members to create databases and database users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:create-keys\n  description: Allow members to add SSH keys to servers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:create-monitors\n  description: Allow members to create server monitors\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:create-schedulers\n  description: Allow members to create scheduled jobs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:delete\n  description: Allow members to delete servers\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:delete-backups\n  description: Allow members to delete database backup configurations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:delete-daemons\n  description: Allow members to delete daemons\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:delete-databases\n  description: Allow members to delete databases and database users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:delete-keys\n  description: Allow members to remove SSH keys from servers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:delete-monitors\n  description: Allow members to delete server monitors\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:delete-schedulers\n  description: Allow\
  \ members to delete scheduled jobs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:manage-logs\n  description: Allow members to clear server and site logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:manage-meta\n  description: Allow members to change server settings such as name and IP address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:manage-network\n  description: Allow members to change the server‘s firewall\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:manage-nginx-templates\n  description: Allow members to manage Nginx templates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:manage-packages\n  description: Allow members to configure and remove server and site package authentication\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:manage-password\n  description: Allow members to reset the sudo password\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:manage-php\n  description: Allow members to install and change PHP installations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:manage-services\n  description: Allow members to start, stop and restart services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:transfer\n  description: Allow members to transfer servers to another Forge account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:view\n  description: Allow members to view servers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: server:web-terminal\n  description: Allow members to start\
  \ web terminal sessions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:create\n  description: Allow members to create sites\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:delete\n  description: Allow members to delete sites\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-commands\n  description: Allow members to run arbitrary commands from the site‘s root directory\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-deploys\n  description: Allow members to deploy the site and update the deployment script\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-environment\n  description: Allow members to update the site‘s environment file\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n\
  - scope: site:manage-heartbeats\n  description: Allow members to manage heartbeats\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-integrations\n  description: Allow members to manage site integrations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-nginx\n  description: Allow members to manage the site‘s Nginx configuration file\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-notifications\n  description: Allow members to configure deployment notifications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-project\n  description: Allow members to install Git repositories, phpMyAdmin and WordPress applications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-queues\n  description: Allow members to configure\
  \ queue workers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-redirects\n  description: Allow members to configure URL redirects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-security\n  description: Allow members to configure HTTP Basic Authentication\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:manage-ssl\n  description: Allow members to configure SSL and Let‘s Encrypt certificates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: site:meta\n  description: Allow members to update site meta data such as domain name and aliases\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: storage:manage\n  description: Allow members to manage the organization's storage providers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n\
  - scope: team:create\n  description: Allow members to create teams\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: team:delete\n  description: Allow members to delete teams and team members\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: team:view\n  description: Allow members to view teams\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n- scope: user:view\n  description: Allow members to view user details\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/laravel-forge-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laravel/refs/heads/main/scopes/laravel-scopes.yml
summary_line: 62 scopes · authorizationCode
tags:
- Company
- Cloud Saas
- PHP
- Developer Tools
- Platform as a Service
- Deployment
- Server Management
- Application Hosting
- Infrastructure
- Frameworks
- Monitoring
token_urls:
- https://forge.laravel.com/oauth/token
---
