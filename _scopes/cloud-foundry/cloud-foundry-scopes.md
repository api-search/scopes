---
api_specs:
- filename: cloud-foundry-capi-v3-openapi.yaml
  format: yaml
  label: Cloud Foundry Cloud Controller API v3
  slug: capi-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-capi-v3-openapi.yaml
- filename: cloud-foundry-open-service-broker-api-openapi.yaml
  format: yaml
  label: Open Service Broker API
  slug: open-service-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-open-service-broker-api-openapi.yaml
- filename: cloud-foundry-apps-api-openapi.yml
  format: yaml
  label: Cloud Foundry Apps API
  slug: cloud-foundry-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-apps-api-openapi.yml
- filename: cloud-foundry-builds-api-openapi.yml
  format: yaml
  label: Cloud Foundry Builds API
  slug: cloud-foundry-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-builds-api-openapi.yml
- filename: cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml
  format: yaml
  label: Cloud Foundry Cloud Foundry Cloud Controller API V3 API
  slug: cloud-foundry-cloud-foundry-cloud-controller-api-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml
- filename: cloud-foundry-deployments-api-openapi.yml
  format: yaml
  label: Cloud Foundry Deployments API
  slug: cloud-foundry-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-deployments-api-openapi.yml
- filename: cloud-foundry-jobs-api-openapi.yml
  format: yaml
  label: Cloud Foundry Jobs API
  slug: cloud-foundry-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-jobs-api-openapi.yml
- filename: cloud-foundry-organizations-api-openapi.yml
  format: yaml
  label: Cloud Foundry Organizations API
  slug: cloud-foundry-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-organizations-api-openapi.yml
- filename: cloud-foundry-service-instances-api-openapi.yml
  format: yaml
  label: Cloud Foundry Service Instances API
  slug: cloud-foundry-service-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-service-instances-api-openapi.yml
- filename: cloud-foundry-spaces-api-openapi.yml
  format: yaml
  label: Cloud Foundry Spaces API
  slug: cloud-foundry-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-spaces-api-openapi.yml
- filename: cloud-foundry-app-autoscaler-policy-api-openapi.yaml
  format: yaml
  label: Cloud Foundry App Autoscaler API
  slug: app-autoscaler
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-app-autoscaler-policy-api-openapi.yaml
authorization_urls:
- https://uaa.cloudfoundry.local/api-oauth/dialog
description: ''
docs:
- https://docs.cloudfoundry.org/uaa/
- https://docs.cloudfoundry.org/concepts/roles.html
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Cloud Foundry Scopes
name_suffix: OAuth Scopes
note: 'Scopes are issued by the target foundation''s UAA and are read verbatim from the Cloud Foundry Foundation''s own CAPI OpenAPI. THE SCOPE IS ONLY HALF THE AUTHORIZATION. Cloud Foundry authorizes on two axes: a UAA scope gates the VERB, and a Cloud Foundry ROLE on the target organization or space gates the OBJECT. A token carrying cloud_controller.write still gets 403 on a space where the user has no role. The roles (org manager, org auditor, org billing manager, space developer, space manager, space auditor, space supporter) are Cloud Controller data, not UAA scopes, and appear nowhere in the securitySchemes block — which is why a client built purely from the spec''s scope list will misdiagnose its own 403s. The authorizationUrl above (uaa.cloudfoundry.local) is a placeholder: the real value is uaa.<system-domain> for the foundation you are calling.'
overview: 'Cloud Foundry publishes 7 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cloud Foundry API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cloud Foundry
provider_slug: cloud-foundry
schemes:
- flows:
  - authorizationUrl: https://uaa.cloudfoundry.local/api-oauth/dialog
    flow: implicit
  name: oauth
  source: openapi/cloud-foundry-capi-v3-openapi.yaml
scope_count: 7
scope_names:
- cloud_controller.admin
- cloud_controller.admin_read_only
- cloud_controller.global_auditor
- cloud_controller.read
- cloud_controller.update_build_state
- cloud_controller.write
- cloud_controller_service_permissions.read
scopes:
- description: This scope provides read and write access to all resources
  flows:
  - implicit
  scope: cloud_controller.admin
- description: This scope provides read only access to all resources
  flows:
  - implicit
  scope: cloud_controller.admin_read_only
- description: This scope provides read access to all resources
  flows:
  - implicit
  scope: cloud_controller.global_auditor
- description: Read access to the Cloud Controller
  flows:
  - implicit
  scope: cloud_controller.read
- description: This scope allows its bearer to update the state of a build; currently only used when updating builds
  flows:
  - implicit
  scope: cloud_controller.update_build_state
- description: Write access to the Cloud Controller
  flows:
  - implicit
  scope: cloud_controller.write
- description: This scope provides read only access for service instance permissions
  flows:
  - implicit
  scope: cloud_controller_service_permissions.read
slug: cloud-foundry-scopes
source_filename: cloud-foundry-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/cloud-foundry-capi-v3-openapi.yaml components.securitySchemes.oauth, enriched from https://docs.cloudfoundry.org/concepts/architecture/uaa.html\n  and https://docs.cloudfoundry.org/uaa/\nschemes:\n- name: oauth\n  source: openapi/cloud-foundry-capi-v3-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://uaa.cloudfoundry.local/api-oauth/dialog\nscopes:\n- scope: cloud_controller.admin\n  description: This scope provides read and write access to all resources\n  flows:\n  - implicit\n  sources:\n  - openapi/cloud-foundry-capi-v3-openapi.yaml\n- scope: cloud_controller.admin_read_only\n  description: This scope provides read only access to all resources\n  flows:\n  - implicit\n  sources:\n  - openapi/cloud-foundry-capi-v3-openapi.yaml\n- scope: cloud_controller.global_auditor\n  description: This scope provides read access to all resources\n  flows:\n  - implicit\n  sources:\n  - openapi/cloud-foundry-capi-v3-openapi.yaml\n\
  - scope: cloud_controller.read\n  description: Read access to the Cloud Controller\n  flows:\n  - implicit\n  sources:\n  - openapi/cloud-foundry-capi-v3-openapi.yaml\n- scope: cloud_controller.update_build_state\n  description: This scope allows its bearer to update the state of a build; currently only used when updating builds\n  flows:\n  - implicit\n  sources:\n  - openapi/cloud-foundry-capi-v3-openapi.yaml\n- scope: cloud_controller.write\n  description: Write access to the Cloud Controller\n  flows:\n  - implicit\n  sources:\n  - openapi/cloud-foundry-capi-v3-openapi.yaml\n- scope: cloud_controller_service_permissions.read\n  description: This scope provides read only access for service instance permissions\n  flows:\n  - implicit\n  sources:\n  - openapi/cloud-foundry-capi-v3-openapi.yaml\ndocs:\n- https://docs.cloudfoundry.org/uaa/\n- https://docs.cloudfoundry.org/concepts/roles.html\nnote: 'Scopes are issued by the target foundation''s UAA and are read verbatim from the Cloud\
  \ Foundry Foundation''s\n  own CAPI OpenAPI. THE SCOPE IS ONLY HALF THE AUTHORIZATION. Cloud Foundry authorizes on two axes: a UAA scope\n  gates the VERB, and a Cloud Foundry ROLE on the target organization or space gates the OBJECT. A token carrying\n  cloud_controller.write still gets 403 on a space where the user has no role. The roles (org manager, org auditor,\n  org billing manager, space developer, space manager, space auditor, space supporter) are Cloud Controller data,\n  not UAA scopes, and appear nowhere in the securitySchemes block — which is why a client built purely from the\n  spec''s scope list will misdiagnose its own 403s. The authorizationUrl above (uaa.cloudfoundry.local) is a placeholder:\n  the real value is uaa.<system-domain> for the foundation you are calling.'\nauthorization_model:\n  axes:\n  - UAA OAuth 2.0 scope (verb)\n  - Cloud Foundry role on org/space (object)\n  roles:\n  - organization_manager\n  - organization_auditor\n  - organization_billing_manager\n\
  \  - organization_user\n  - space_developer\n  - space_manager\n  - space_auditor\n  - space_supporter\n  roles_api: listRoles / createRole (GET,POST /v3/roles) in openapi/cloud-foundry-capi-v3-openapi.yaml\n  note: Role assignment is itself an API surface — the Roles tag carries 4 operations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/scopes/cloud-foundry-scopes.yml
summary_line: 7 scopes · implicit
tags:
- Cloud Foundry Foundation
- Containers
- Multi-Cloud
- Open-Source
- Platform-as-a-Service
- Platform
token_urls: []
---
