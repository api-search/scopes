---
api_specs:
- filename: microsoft-azure-maps-search-api-openapi.yml
  format: yaml
  label: Azure Maps Search API
  slug: microsoft-azure-maps-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-search-api-openapi.yml
- filename: microsoft-azure-maps-geocode-api-openapi.yml
  format: yaml
  label: Azure Maps Geocode API
  slug: microsoft-azure-maps-geocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geocode-api-openapi.yml
- filename: microsoft-azure-maps-geocode-autocomplete-api-openapi.yml
  format: yaml
  label: Azure Maps Geocode:autocomplete API
  slug: microsoft-azure-maps-geocode-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geocode-autocomplete-api-openapi.yml
- filename: microsoft-azure-maps-geocode-batch-api-openapi.yml
  format: yaml
  label: Azure Maps Geocode:batch API
  slug: microsoft-azure-maps-geocode-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geocode-batch-api-openapi.yml
- filename: microsoft-azure-maps-geolocation-api-openapi.yml
  format: yaml
  label: Azure Maps Geolocation API
  slug: microsoft-azure-maps-geolocation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geolocation-api-openapi.yml
- filename: microsoft-azure-maps-map-api-openapi.yml
  format: yaml
  label: Azure Maps Map API
  slug: microsoft-azure-maps-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-map-api-openapi.yml
- filename: microsoft-azure-maps-reversegeocode-api-openapi.yml
  format: yaml
  label: Azure Maps Reverse Geocode API
  slug: microsoft-azure-maps-reversegeocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-reversegeocode-api-openapi.yml
- filename: microsoft-azure-maps-reversegeocode-batch-api-openapi.yml
  format: yaml
  label: Azure Maps Reverse Geocode:batch API
  slug: microsoft-azure-maps-reversegeocode-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-reversegeocode-batch-api-openapi.yml
- filename: microsoft-azure-maps-route-api-openapi.yml
  format: yaml
  label: Azure Maps Route API
  slug: microsoft-azure-maps-route-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-route-api-openapi.yml
- filename: microsoft-azure-maps-timezone-api-openapi.yml
  format: yaml
  label: Azure Maps Timezone API
  slug: microsoft-azure-maps-timezone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-timezone-api-openapi.yml
- filename: microsoft-azure-maps-traffic-api-openapi.yml
  format: yaml
  label: Azure Maps Traffic API
  slug: microsoft-azure-maps-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-traffic-api-openapi.yml
- filename: microsoft-azure-maps-weather-api-openapi.yml
  format: yaml
  label: Azure Maps Weather API
  slug: microsoft-azure-maps-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-weather-api-openapi.yml
- filename: microsoft-azure-maps-accounts-api-openapi.yml
  format: yaml
  label: Azure Maps Accounts API
  slug: microsoft-azure-maps-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-accounts-api-openapi.yml
- filename: microsoft-azure-maps-creators-api-openapi.yml
  format: yaml
  label: Azure Maps Creators API
  slug: microsoft-azure-maps-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-creators-api-openapi.yml
- filename: microsoft-azure-maps-operations-api-openapi.yml
  format: yaml
  label: Azure Maps Operations API
  slug: microsoft-azure-maps-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-operations-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Maps Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Maps publishes 2 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Maps API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Maps
provider_slug: microsoft-azure-maps
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/microsoft-azure-maps-geocoding-api-openapi.yml
- description: 'These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.


    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.


    > [!NOTE]

    >

    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).

    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.

    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.

    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.

    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: AadToken
  source: openapi/microsoft-azure-maps-geolocation-openapi.yml
- description: 'These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.


    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.


    > [!NOTE]

    >

    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).

    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.

    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.

    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.

    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: AadToken
  source: openapi/microsoft-azure-maps-render-openapi.yml
- description: 'These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.


    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.


    > [!NOTE]

    >

    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).

    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.

    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.

    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.

    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: AadToken
  source: openapi/microsoft-azure-maps-route-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/_superseded/microsoft-azure-maps-search-api-openapi.yml
- description: 'These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.


    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.


    > [!NOTE]

    >

    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).

    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.

    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.

    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.

    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: AadToken
  source: openapi/microsoft-azure-maps-search-openapi.yml
- description: 'These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.


    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.


    > [!NOTE]

    >

    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).

    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.

    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.

    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.

    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: AadToken
  source: openapi/microsoft-azure-maps-timezone-openapi.yml
- description: 'These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.


    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.


    > [!NOTE]

    >

    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).

    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.

    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.

    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.

    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: AadToken
  source: openapi/microsoft-azure-maps-traffic-openapi.yml
- description: 'These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.


    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.


    > [!NOTE]

    >

    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).

    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.

    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.

    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.

    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: AadToken
  source: openapi/microsoft-azure-maps-weather-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-maps-openapi.yml
scope_count: 2
scope_names:
- https://atlas.microsoft.com/.default
- user_impersonation
scopes:
- description: ''
  flows:
  - implicit
  scope: https://atlas.microsoft.com/.default
- description: Impersonate user
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-maps-scopes
source_filename: microsoft-azure-maps-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-maps-geocoding-api-openapi.yml, openapi/microsoft-azure-maps-geolocation-openapi.yml,\n  openapi/microsoft-azure-maps-openapi.yml, openapi/microsoft-azure-maps-render-openapi.yml,\n  openapi/microsoft-azure-maps-route-openapi.yml, openapi/_superseded/microsoft-azure-maps-search-api-openapi.yml,\n  openapi/microsoft-azure-maps-search-openapi.yml, openapi/microsoft-azure-maps-timezone-openapi.yml,\n  openapi/microsoft-azure-maps-traffic-openapi.yml, openapi/microsoft-azure-maps-weather-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/_superseded/microsoft-azure-maps-geocoding-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: AadToken\n  source: openapi/microsoft-azure-maps-geolocation-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n\
  \  description: |-\n    These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.\n\n    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.\n\n    > [!NOTE]\n    >\n    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource\
  \ the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).\n    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.\n    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.\n    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.\n    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).\n- name: AadToken\n  source: openapi/microsoft-azure-maps-render-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: |-\n   \
  \ These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.\n\n    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.\n\n    > [!NOTE]\n    >\n    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application\
  \ is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).\n    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.\n    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.\n    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.\n    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).\n- name: AadToken\n  source: openapi/microsoft-azure-maps-route-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: |-\n    These are the [Microsoft\
  \ Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.\n\n    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.\n\n    > [!NOTE]\n    >\n    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to.\
  \ This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).\n    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.\n    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.\n    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.\n    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).\n- name: azure_auth\n  source: openapi/_superseded/microsoft-azure-maps-search-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: AadToken\n  source: openapi/microsoft-azure-maps-search-openapi.yml\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: |-\n    These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.\n\n    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.\n\n    > [!NOTE]\n    >\n    >\
  \ * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).\n    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.\n    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.\n    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.\n    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).\n- name: AadToken\n  source: openapi/microsoft-azure-maps-timezone-openapi.yml\n  flows:\n  - flow:\
  \ implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: |-\n    These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.\n\n    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.\n\n    > [!NOTE]\n    >\n    > * This security definition\
  \ **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).\n    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.\n    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.\n    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.\n    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).\n- name: AadToken\n  source: openapi/microsoft-azure-maps-traffic-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl:\
  \ https://login.microsoftonline.com/common/oauth2/authorize\n  description: |-\n    These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.\n\n    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.\n\n    > [!NOTE]\n    >\n    > * This security definition **requires** the use of\
  \ the `x-ms-client-id` header to indicate which Azure Maps resource the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).\n    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.\n    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.\n    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.\n    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).\n- name: AadToken\n  source: openapi/microsoft-azure-maps-weather-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n\
  \  description: |-\n    These are the [Microsoft Entra OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v1-overview) Flows. When paired with [Azure role-based access](https://docs.microsoft.com/azure/role-based-access-control/overview) control it can be used to control access to Azure Maps REST APIs. Azure role-based access controls are used to designate access to one or more Azure Maps resource account or sub-resources. Any user, group, or service principal can be granted access via a  built-in role or a custom role composed of one or more permissions to Azure Maps REST APIs.\n\n    To implement scenarios, we recommend viewing [authentication concepts](https://aka.ms/amauth). In summary, this security definition provides a solution for modeling application(s) via objects capable of access control on specific APIs and scopes.\n\n    > [!NOTE]\n    >\n    > * This security definition **requires** the use of the `x-ms-client-id` header to indicate which Azure Maps resource\
  \ the application is requesting access to. This can be acquired from the [Maps management API](https://aka.ms/amauthdetails).\n    > * The `Authorization URL` is specific to the Azure public cloud instance. Sovereign clouds have unique Authorization URLs and Microsoft Entra ID configurations.\n    > * The Azure role-based access control is configured from the [Azure management plane](https://aka.ms/amrbac) via Azure portal, PowerShell, CLI, Azure SDKs, or REST APIs.\n    > * Usage of the [Azure Maps Web SDK](https://aka.ms/amaadmc) allows for configuration based setup of an application for multiple use cases.\n    > * For more information on Microsoft identity platform, see [Microsoft identity platform overview](https://learn.microsoft.com/entra/identity-platform/v2-overview).\n- name: azure_auth\n  source: openapi/microsoft-azure-maps-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\nscopes:\n- scope: https://atlas.microsoft.com/.default\n\
  \  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-maps-geolocation-openapi.yml\n  - openapi/microsoft-azure-maps-render-openapi.yml\n  - openapi/microsoft-azure-maps-route-openapi.yml\n  - openapi/microsoft-azure-maps-search-openapi.yml\n  - openapi/microsoft-azure-maps-timezone-openapi.yml\n  - openapi/microsoft-azure-maps-traffic-openapi.yml\n  - openapi/microsoft-azure-maps-weather-openapi.yml\n- scope: user_impersonation\n  description: Impersonate user\n  flows:\n  - implicit\n  sources:\n  - openapi/_superseded/microsoft-azure-maps-geocoding-api-openapi.yml\n  - openapi/microsoft-azure-maps-openapi.yml\n  - openapi/_superseded/microsoft-azure-maps-search-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-maps/scopes/microsoft-azure-maps-scopes.yml
summary_line: 2 scopes · implicit
tags:
- Geocoding
- Geospatial
- Location
- Maps
- Mobility
- Routing
- Traffic
- Weather
token_bound: false
token_urls: []
---
