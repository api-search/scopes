---
api_specs:
- filename: acquia-account-api-openapi.yml
  format: yaml
  label: Acquia Account API
  slug: acquia-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-account-api-openapi.yml
- filename: acquia-agreements-api-openapi.yml
  format: yaml
  label: Acquia Agreements API
  slug: acquia-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-agreements-api-openapi.yml
- filename: acquia-application-performance-monitoring-services-api-openapi.yml
  format: yaml
  label: Acquia Application Performance Monitoring Services API
  slug: acquia-application-performance-monitoring-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-application-performance-monitoring-services-api-openapi.yml
- filename: acquia-applications-api-openapi.yml
  format: yaml
  label: Acquia Applications API
  slug: acquia-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-applications-api-openapi.yml
- filename: acquia-cloud-ide-api-openapi.yml
  format: yaml
  label: Acquia Cloud IDE API
  slug: acquia-cloud-ide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-cloud-ide-api-openapi.yml
- filename: acquia-codebases-api-openapi.yml
  format: yaml
  label: Acquia Codebases API
  slug: acquia-codebases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-codebases-api-openapi.yml
- filename: acquia-current-system-health-api-openapi.yml
  format: yaml
  label: Acquia Current system health API
  slug: acquia-current-system-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-current-system-health-api-openapi.yml
- filename: acquia-distributions-api-openapi.yml
  format: yaml
  label: Acquia Distributions API
  slug: acquia-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-distributions-api-openapi.yml
- filename: acquia-email-api-openapi.yml
  format: yaml
  label: Acquia Email API
  slug: acquia-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-email-api-openapi.yml
- filename: acquia-environments-api-openapi.yml
  format: yaml
  label: Acquia Environments API
  slug: acquia-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-environments-api-openapi.yml
- filename: acquia-identity-providers-api-openapi.yml
  format: yaml
  label: Acquia Identity Providers API
  slug: acquia-identity-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-identity-providers-api-openapi.yml
- filename: acquia-invite-api-openapi.yml
  format: yaml
  label: Acquia Invite API
  slug: acquia-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-invite-api-openapi.yml
- filename: acquia-messages-api-openapi.yml
  format: yaml
  label: Acquia Messages API
  slug: acquia-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-messages-api-openapi.yml
- filename: acquia-notifications-api-openapi.yml
  format: yaml
  label: Acquia Notifications API
  slug: acquia-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-notifications-api-openapi.yml
- filename: acquia-options-api-openapi.yml
  format: yaml
  label: Acquia Options API
  slug: acquia-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-options-api-openapi.yml
- filename: acquia-organizations-api-openapi.yml
  format: yaml
  label: Acquia Organizations API
  slug: acquia-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-organizations-api-openapi.yml
- filename: acquia-private-networks-api-openapi.yml
  format: yaml
  label: Acquia Private Networks API
  slug: acquia-private-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-private-networks-api-openapi.yml
- filename: acquia-subscriptions-api-openapi.yml
  format: yaml
  label: Acquia Subscriptions API
  slug: acquia-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-subscriptions-api-openapi.yml
- filename: acquia-teams-and-permissions-api-openapi.yml
  format: yaml
  label: Acquia Teams and Permissions API
  slug: acquia-teams-and-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-teams-and-permissions-api-openapi.yml
- filename: acquia-content-api-openapi.yaml
  format: yaml
  label: Acquia Content API
  slug: acquia-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-content-api-openapi.yaml
authorization_urls: []
description: ''
docs:
- https://dev.acquia.com/source-cms/reference/authentication.md
- https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Acquia Scopes
name_suffix: OAuth Scopes
note: 'Acquia runs two OAuth surfaces with completely different scope models. (1) Cloud Platform API: OAuth 2.0 client_credentials tied to per-user API tokens, with access governed by Teams and Permissions ROLES rather than a scope catalog; the only documented scope is organization:{uuid}, required when the organization uses Federated Authentication. That is why the OpenAPI declares 19 oauth2 securitySchemes carrying ZERO scopes. (2) Source CMS Content API and MCP server: a real 22-scope vocabulary, selected as checkboxes on each API client, published in full at dev.acquia.com. The Source CMS vocabulary is recorded below and was NOT present in earlier rounds.'
overview: 'Acquia publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Acquia API on a user''s behalf.


  Tokens are issued from https://accounts.acquia.com/api/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Acquia
provider_slug: acquia
schemes:
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-account.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-agreements.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-application-performance-monitoring-services.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-applications.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-cloud-ide.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-codebases.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-current-system-health.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-distributions.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-email.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-environments.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-identity-providers.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-invite.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-messages.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-notifications.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-openapi-full.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-options.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-organizations.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-private-networks.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-subscriptions.yml
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page, click **API Tokens**.

    4. Click **Create Token**.

    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.

    6. Copy your API key and API secret. Click **OK**.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  source: openapi/acquia-cloud-teams-and-permissions.yml
scope_count: 1
scope_names:
- organization:{uuid}
scopes:
- description: Grants the API token access to the resources of the organization identified by the given UUID; required when generating an API token for an organization that uses Federated Authentication.
  flows: []
  scope: organization:{uuid}
slug: acquia-scopes
source_filename: acquia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\ndocs:\n- https://dev.acquia.com/source-cms/reference/authentication.md\n- https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication\nnote: 'Acquia runs two OAuth surfaces with completely different scope models. (1) Cloud Platform API:\n  OAuth 2.0 client_credentials tied to per-user API tokens, with access governed by Teams and Permissions\n  ROLES rather than a scope catalog; the only documented scope is organization:{uuid}, required when the\n  organization uses Federated Authentication. That is why the OpenAPI declares 19 oauth2 securitySchemes\n  carrying ZERO scopes. (2) Source CMS Content API and MCP server: a real 22-scope vocabulary, selected\n  as checkboxes on each API client, published in full at dev.acquia.com. The Source CMS vocabulary is\n  recorded below and was NOT present in earlier rounds.'\nsource: openapi/acquia-cloud-account.yml, openapi/acquia-cloud-agreements.yml, openapi/acquia-cloud-application-performance-monitoring-services.yml,\n\
  \  openapi/acquia-cloud-applications.yml, openapi/acquia-cloud-cloud-ide.yml, openapi/acquia-cloud-codebases.yml,\n  openapi/acquia-cloud-current-system-health.yml, openapi/acquia-cloud-distributions.yml, openapi/acquia-cloud-email.yml,\n  openapi/acquia-cloud-environments.yml, openapi/acquia-cloud-identity-providers.yml, openapi/acquia-cloud-invite.yml,\n  openapi/acquia-cloud-messages.yml, openapi/acquia-cloud-notifications.yml, openapi/acquia-cloud-openapi-full.yml,\n  openapi/acquia-cloud-options.yml, openapi/acquia-cloud-organizations.yml, openapi/acquia-cloud-private-networks.yml,\n  openapi/acquia-cloud-subscriptions.yml, openapi/acquia-cloud-teams-and-permissions.yml\nschemes:\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-account.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you\
  \ can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-agreements.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia\
  \ Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-application-performance-monitoring-services.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n\
  \    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-applications.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account\
  \ Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-cloud-ide.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n  \
  \  5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-codebases.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click\
  \ **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-current-system-health.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n\
  \  source: openapi/acquia-cloud-distributions.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-email.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n\
  \  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-environments.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n\
  \    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-identity-providers.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\
  \n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-invite.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n \
  \   Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-messages.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\
  \n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-notifications.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the\
  \ pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-openapi-full.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create\
  \ Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-options.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n\
  \  source: openapi/acquia-cloud-organizations.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-private-networks.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-subscriptions.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in\
  \ order to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-teams-and-permissions.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using\n    a token that you can generate on your Acquia Profile\
  \ page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page, click **API Tokens**.\n\n    4. Click **Create Token**.\n\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then\n    click **Create Token**.\n\n    6. Copy your API key and API secret. Click **OK**.'\nscopes:\n- scope: organization:{uuid}\n  description: Grants the API token access to the resources of the organization identified by the given\n    UUID; required when generating an API token for an organization that uses Federated Authentication.\n  sources:\n  - https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication\nsurfaces:\n- name: Cloud Platform API\n  scope_model: role-based (Teams and Permissions), not scope-based\n\
  \  scope_count: 1\n  tokenUrl: https://accounts.acquia.com/api/token\n  scopes:\n  - name: organization:{uuid}\n    description: Required when the organization uses Federated Authentication.\n    source: https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication\n- name: Source CMS (Content API + MCP server)\n  scope_model: scope-based, selected per API client at API > API clients\n  scope_count: 22\n  tokenUrl: '{DRUPAL_SITE_URL}/oauth/token'\n  source: https://dev.acquia.com/source-cms/reference/authentication.md\n  defaulting: A token request with NO scope parameter carries every scope selected on the client. A scope\n    parameter may only narrow to a subset; naming an unknown or unselected scope returns a 400 invalid_scope\n    whose hint names the offending scope.\n  gating_note: 'Scopes gate writes and admin surfaces, not published-content reads: a GET for published\n    content succeeds with any valid token regardless of scope, and with no token at all when\
  \ the site''s\n    Public access setting is Yes. Reading UNPUBLISHED content requires content:administer.'\n  mcp_note: 'Acquia''s MCP reference reports 16 scopes_supported in the MCP resource-metadata document\n    - a subset of the 22 below - and records that scope gating was NOT observable in its own verification:\n    a client_credentials token issued without a scope parameter called every tool successfully.'\n  scopes:\n  - name: content:administer\n    description: 'Content CRUD over JSON:API: create, update and delete entries. There is no read-only\n      content scope.'\n  - name: content_type:administer\n    description: Content types (bundles).\n  - name: content_type:administer_fields\n    description: Fields on content types.\n  - name: page_template:administer\n    description: Page templates.\n  - name: media:administer\n    description: Media entries.\n  - name: media_type:administer\n    description: Media types.\n  - name: taxonomy:administer\n    description: Taxonomy\
  \ vocabularies and terms.\n  - name: taxonomy:administer_fields\n    description: Fields on taxonomy terms.\n  - name: menu:administer\n    description: Menus.\n  - name: site_settings:administer\n    description: Site settings.\n  - name: canvas:page:read\n    description: Read Canvas pages.\n  - name: canvas:page:create\n    description: Create Canvas pages.\n  - name: canvas:page:edit\n    description: Edit Canvas pages.\n  - name: canvas:page:delete\n    description: Delete Canvas pages.\n  - name: canvas:page_region\n    description: Canvas page regions.\n  - name: canvas:content_template\n    description: Canvas content templates.\n  - name: canvas:asset_library\n    description: 'Drupal Canvas CLI: asset library access for downloading and uploading components.'\n  - name: canvas:js_component\n    description: 'Drupal Canvas CLI: JS component access for downloading and uploading components.'\n  - name: canvas:brand_kit\n    description: Canvas brand kits.\n  - name: canvas:media:view\n\
  \    description: View media from Canvas.\n  - name: canvas:media:image:create\n    description: Create images from Canvas.\n  - name: member\n    description: Basic member access.\nscope_count: 23\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/scopes/acquia-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Content
- Experience
- Drupal
- DXP
- CMS
- Digital Asset Management
- Cloud Hosting
- Headless
token_urls:
- https://accounts.acquia.com/api/token
---
