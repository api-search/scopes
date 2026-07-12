---
authorization_urls: []
description: ''
docs: https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/using-communications/oauth-api-authetication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Adobe Experience Manager Scopes
name_suffix: OAuth Scopes
note: AEM as a Cloud Service uses Adobe IMS OAuth Server-to-Server (client_credentials) tokens; Adobe documents a fixed set of IMS scopes for AEM API access rather than granular per-endpoint scopes, with the scopes available to a credential shown in the Adobe Developer Console project.
overview: 'Adobe Experience Manager publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adobe Experience Manager API on a user''s behalf.


  Tokens are issued from https://ims-na1.adobelogin.com/ims/token/v3.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adobe Experience Manager
provider_slug: adobe-experience-manager
schemes:
- description: Adobe IMS OAuth 2.0 with Server-to-Server credentials issued from the Adobe Developer Console for an AEM as a Cloud Service project.
  flows:
  - flow: clientCredentials
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: adobeIMS
  source: openapi/adobe-experience-manager-openapi.yml
scope_count: 6
scope_names:
- openid
- AdobeID
- read_organizations
- additional_info.projectedProductContext
- read_pc.dma_aem_cloud
- aem.document
scopes:
- description: Standard OpenID Connect scope required by Adobe IMS when requesting an access token for AEM as a Cloud Service APIs.
  flows: []
  scope: openid
- description: Adobe IMS identity scope required for authenticating a Developer Console credential against AEM as a Cloud Service APIs.
  flows: []
  scope: AdobeID
- description: Allows the credential to read the Adobe organization information associated with the Developer Console project.
  flows: []
  scope: read_organizations
- description: Includes the projected product context in the IMS access token, used by AEM as a Cloud Service to authorize API calls.
  flows: []
  scope: additional_info.projectedProductContext
- description: Grants read access to the AEM as a Cloud Service (dma_aem_cloud) product context for the authenticated credential.
  flows: []
  scope: read_pc.dma_aem_cloud
- description: Scope required for invoking the AEM Forms Communications (document generation) APIs on AEM as a Cloud Service.
  flows: []
  scope: aem.document
slug: adobe-experience-manager-scopes
source_filename: adobe-experience-manager-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/using-communications/oauth-api-authetication\nsource: openapi/adobe-experience-manager-openapi.yml\nschemes:\n- name: adobeIMS\n  source: openapi/adobe-experience-manager-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n  description: Adobe IMS OAuth 2.0 with Server-to-Server credentials issued from the Adobe Developer\n    Console for an AEM as a Cloud Service project.\nnote: AEM as a Cloud Service uses Adobe IMS OAuth Server-to-Server (client_credentials) tokens;\n  Adobe documents a fixed set of IMS scopes for AEM API access rather than granular per-endpoint\n  scopes, with the scopes available to a credential shown in the Adobe Developer Console project.\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope required by Adobe IMS when requesting an access\n    token\
  \ for AEM as a Cloud Service APIs.\n  sources:\n  - https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/using-communications/oauth-api-authetication\n- scope: AdobeID\n  description: Adobe IMS identity scope required for authenticating a Developer Console credential\n    against AEM as a Cloud Service APIs.\n  sources:\n  - https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/using-communications/oauth-api-authetication\n- scope: read_organizations\n  description: Allows the credential to read the Adobe organization information associated with\n    the Developer Console project.\n  sources:\n  - https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/using-communications/oauth-api-authetication\n- scope: additional_info.projectedProductContext\n  description: Includes the projected product context in the IMS access token, used by AEM as\n    a Cloud Service to authorize API calls.\n  sources:\n \
  \ - https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/using-communications/oauth-api-authetication\n- scope: read_pc.dma_aem_cloud\n  description: Grants read access to the AEM as a Cloud Service (dma_aem_cloud) product context\n    for the authenticated credential.\n  sources:\n  - https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/using-communications/oauth-api-authetication\n- scope: aem.document\n  description: Scope required for invoking the AEM Forms Communications (document generation)\n    APIs on AEM as a Cloud Service.\n  sources:\n  - https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/using-communications/oauth-api-authetication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-manager/refs/heads/main/scopes/adobe-experience-manager-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Content Management
- Enterprise CMS
- Digital Asset Management
- Headless CMS
- Content Fragments
- Adaptive Forms
token_urls:
- https://ims-na1.adobelogin.com/ims/token/v3
---
