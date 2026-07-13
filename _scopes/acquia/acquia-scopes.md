---
api_specs:
- filename: acquia-cloud-openapi.yml
  format: yaml
  label: Acquia Cloud API
  slug: acquia-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-cloud-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Acquia Scopes
name_suffix: OAuth Scopes
note: Acquia Cloud Platform API uses OAuth 2.0 client credentials tied to per-user API tokens, with access governed by Teams and Permissions roles rather than a scope catalog; the only documented scope is organization:{uuid}, required when the organization uses Federated Authentication (https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication).
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
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication\nnote: Acquia Cloud Platform API uses OAuth 2.0 client credentials tied to per-user API tokens, with access governed by Teams and Permissions roles rather than a scope catalog; the only documented scope is organization:{uuid}, required when the organization uses Federated Authentication (https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication).\nsource: openapi/acquia-cloud-account.yml, openapi/acquia-cloud-agreements.yml, openapi/acquia-cloud-application-performance-monitoring-services.yml,\n  openapi/acquia-cloud-applications.yml, openapi/acquia-cloud-cloud-ide.yml, openapi/acquia-cloud-codebases.yml,\n  openapi/acquia-cloud-current-system-health.yml, openapi/acquia-cloud-distributions.yml, openapi/acquia-cloud-email.yml,\n  openapi/acquia-cloud-environments.yml, openapi/acquia-cloud-identity-providers.yml, openapi/acquia-cloud-invite.yml,\n\
  \  openapi/acquia-cloud-messages.yml, openapi/acquia-cloud-notifications.yml, openapi/acquia-cloud-openapi-full.yml,\n  openapi/acquia-cloud-options.yml, openapi/acquia-cloud-organizations.yml, openapi/acquia-cloud-private-networks.yml,\n  openapi/acquia-cloud-subscriptions.yml, openapi/acquia-cloud-teams-and-permissions.yml\nschemes:\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-account.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click\
  \ **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-agreements.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click\
  \ **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-application-performance-monitoring-services.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n\
  \  source: openapi/acquia-cloud-applications.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-cloud-ide.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n\
  \  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-codebases.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can\
  \ generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-current-system-health.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/)\
  \ interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-distributions.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click\
  \ **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-email.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that\
  \ appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-environments.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key\
  \ and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-identity-providers.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-invite.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-messages.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls\
  \ need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-notifications.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\
  \n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-openapi-full.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address\
  \ and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-options.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the\
  \ Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-organizations.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label\
  \ so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-private-networks.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n\
  - name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-subscriptions.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  source: openapi/acquia-cloud-teams-and-permissions.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://accounts.acquia.com/api/token\n  description: |-\n    All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.\n\n    ### To generate a token:\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n    3. On the Profile page, click **API Tokens**.\n    4. Click **Create Token**.\n    5. In the pop-up that appears, give your token a label so that you can easily find it later. Then click **Create Token**.\n    6. Copy your API key and API secret. Click **OK**.\nscopes:\n- scope: organization:{uuid}\n  description: Grants the API token access to the resources of the organization identified\n    by the given UUID; required when generating an API token for an organization that\n    uses Federated Authentication.\n  sources:\n\
  \  - https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/scopes/acquia-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Content
- Experience
token_urls:
- https://accounts.acquia.com/api/token
---
