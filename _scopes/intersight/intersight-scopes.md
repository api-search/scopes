---
api_specs:
- filename: intersight-fabric-openapi.json
  format: json
  label: Cisco Intersight Fabric API
  slug: fabric
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-fabric-openapi.json
- filename: intersight-hyperflex-openapi.json
  format: json
  label: Cisco Intersight HyperFlex API
  slug: hyperflex
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-hyperflex-openapi.json
- filename: intersight-kubernetes-openapi.json
  format: json
  label: Cisco Intersight Kubernetes API
  slug: kubernetes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-kubernetes-openapi.json
- filename: intersight-nexus-insight-advisor-openapi.json
  format: json
  label: Cisco Intersight Nexus Insight Advisor API
  slug: nexus-insight-advisor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-nexus-insight-advisor-openapi.json
- filename: intersight-orchestrator-openapi.json
  format: json
  label: Cisco Intersight Orchestrator API
  slug: orchestrator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-orchestrator-openapi.json
- filename: intersight-server-openapi.json
  format: json
  label: Cisco Intersight Server API
  slug: server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-server-openapi.json
- filename: intersight-storage-openapi.json
  format: json
  label: Cisco Intersight Storage API
  slug: storage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-storage-openapi.json
- filename: intersight-system-openapi.json
  format: json
  label: Cisco Intersight System API
  slug: system
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-system-openapi.json
- filename: intersight-telemetry-openapi.json
  format: json
  label: Cisco Intersight Telemetry API
  slug: telemetry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-telemetry-openapi.json
- filename: intersight-virtualization-openapi.json
  format: json
  label: Cisco Intersight Virtualization API
  slug: virtualization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-virtualization-openapi.json
- filename: intersight-workflows-openapi.json
  format: json
  label: Cisco Intersight Workflows API
  slug: workflows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-workflows-openapi.json
authorization_urls:
- /iam/app-authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Intersight Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cisco Intersight publishes 3317 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cisco Intersight API on a user''s behalf.


  Tokens are issued from /iam/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cisco Intersight
provider_slug: intersight
schemes:
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-fabric-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-hyperflex-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-kubernetes-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-nexus-insight-advisor-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-orchestrator-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-server-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-storage-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-system-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-telemetry-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-virtualization-openapi.json
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorization code flow, the client sends a list of requested scopes to

    the authorization URL (/iam/app-authorize). The scope in the authorization request

    must be one of the scopes that have been configured in the corresponding

    iam.AppRegistration resource.

    **Client Credentials**

    In the client credentials flow, the scope is selected when the AppRegistration

    is created. The client cannot select a specific scope in the token request.'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    tokenUrl: /iam/token
  - flow: clientCredentials
    tokenUrl: /iam/token
  name: oAuth2
  source: openapi/intersight-workflows-openapi.json
scope_count: 3317
scope_names:
- CREATE.aaa.RetentionPolicy
- CREATE.access.Policy
- CREATE.adapter.ConfigPolicy
- CREATE.appliance.Backup
- CREATE.appliance.BackupPolicy
- CREATE.appliance.ClusterInfo
- CREATE.appliance.ClusterReplaceNode
- CREATE.appliance.ClusterWorkerNode
- CREATE.appliance.ClusterWorkerNodeReplace
- CREATE.appliance.ClusterWorkerNodeReuse
- CREATE.appliance.DataExportPolicy
- CREATE.appliance.DeviceClaim
- CREATE.appliance.DiagSetting
- CREATE.appliance.ExternalSyslogSetting
- CREATE.appliance.FqdnUpdate
- CREATE.appliance.RemoteFileImport
- CREATE.appliance.Restore
- CREATE.asset.ClaimToken
- CREATE.asset.DeviceClaim
- CREATE.asset.DeviceContractNotification
- CREATE.asset.GeoLocation
- CREATE.asset.PreClaim
- CREATE.asset.Target
- CREATE.auditd.Policy
- CREATE.bios.Policy
- CREATE.boot.PrecisionPolicy
- CREATE.bulk.Export
- CREATE.bulk.MoCloner
- CREATE.bulk.MoDeepCloner
- CREATE.bulk.MoMerger
- CREATE.bulk.Request
- CREATE.certificatemanagement.Policy
- CREATE.chassis.ConfigImport
- CREATE.chassis.Profile
- CREATE.chassis.ProfileTemplate
- CREATE.cli.CliPolicy
- CREATE.cloud.CollectInventory
- CREATE.comm.HttpProxyPolicy
- CREATE.comm.TagDefinition
- CREATE.compute.HostUtilityOperation
- CREATE.compute.PcieConnectivityPolicy
- CREATE.compute.ScrubPolicy
- CREATE.cond.AlarmRule
- CREATE.cond.AlarmSuppression
- CREATE.cond.AlarmSuppressionDryRun
- CREATE.cond.CustomHclBaseline
- CREATE.cond.CustomHclStatus
- CREATE.cond.HclStatusJob
- CREATE.cond.ThresholdDefinition
- CREATE.connectorpack.ConnectorPackUpgrade
- CREATE.crd.CustomResource
- CREATE.deviceconnector.Policy
- CREATE.energy.DailyMetrics
- CREATE.energy.Metrics
- CREATE.externalsite.Authorization
- CREATE.fabric.AppliancePcRole
- CREATE.fabric.ApplianceRole
- CREATE.fabric.EstimateImpact
- CREATE.fabric.EthNetworkControlPolicy
- CREATE.fabric.EthNetworkGroupPolicy
- CREATE.fabric.EthNetworkPolicy
- CREATE.fabric.FcNetworkPolicy
- CREATE.fabric.FcStorageRole
- CREATE.fabric.FcUplinkPcRole
- CREATE.fabric.FcUplinkRole
- CREATE.fabric.FcZonePolicy
- CREATE.fabric.FcoeUplinkPcRole
- CREATE.fabric.FcoeUplinkRole
- CREATE.fabric.FlowControlPolicy
- CREATE.fabric.LanPinGroup
- CREATE.fabric.LinkAggregationPolicy
- CREATE.fabric.LinkControlPolicy
- CREATE.fabric.MacSecPolicy
- CREATE.fabric.MulticastPolicy
- CREATE.fabric.NetFlowExporter
- CREATE.fabric.NetFlowMonitor
- CREATE.fabric.NetFlowPolicy
- CREATE.fabric.NetFlowRecord
- CREATE.fabric.PcOperation
- CREATE.fabric.PortMode
- CREATE.fabric.PortOperation
- CREATE.fabric.PortPolicy
- CREATE.fabric.SanPinGroup
- CREATE.fabric.SecureRouterRole
- CREATE.fabric.ServerRole
- CREATE.fabric.SpanDestEthPort
- CREATE.fabric.SpanSession
- CREATE.fabric.SpanSourceEthPort
- CREATE.fabric.SpanSourceEthPortChannel
- CREATE.fabric.SpanSourceVlan
- CREATE.fabric.SpanSourceVnicEthIf
- CREATE.fabric.SwitchClusterProfile
- CREATE.fabric.SwitchClusterProfileTemplate
- CREATE.fabric.SwitchControlPolicy
- CREATE.fabric.SwitchProfile
- CREATE.fabric.SwitchProfileTemplate
- CREATE.fabric.SystemQosPolicy
- CREATE.fabric.UplinkPcRole
- CREATE.fabric.UplinkRole
- CREATE.fabric.Vlan
- CREATE.fabric.Vsan
- CREATE.fcpool.Pool
- CREATE.fcpool.Reservation
- CREATE.feedback.FeedbackPost
- CREATE.firmware.ChassisUpgrade
- CREATE.firmware.Distributable
- CREATE.firmware.DriverDistributable
- CREATE.firmware.Eula
- CREATE.firmware.PciNodeUpgrade
- CREATE.firmware.Policy
- CREATE.firmware.SecureRouterUpgrade
- CREATE.firmware.ServerConfigurationUtilityDistributable
- CREATE.firmware.SwitchUpgrade
- CREATE.firmware.UnsupportedVersionUpgrade
- CREATE.firmware.Upgrade
- CREATE.firmware.UpgradeImpact
- CREATE.firmware.UpgradeValidity
- CREATE.hcl.CompatibilityStatus
- CREATE.hcl.SupportedDriverName
- CREATE.hyperflex.AutoSupportPolicy
- CREATE.hyperflex.CapabilityInfo
- CREATE.hyperflex.ClusterBackupPolicy
- CREATE.hyperflex.ClusterBackupPolicyDeployment
- CREATE.hyperflex.ClusterNetworkPolicy
- CREATE.hyperflex.ClusterProfile
- CREATE.hyperflex.ClusterReplicationNetworkPolicy
- CREATE.hyperflex.ClusterReplicationNetworkPolicyDeployment
- CREATE.hyperflex.ClusterStoragePolicy
- CREATE.hyperflex.ExtFcStoragePolicy
- CREATE.hyperflex.ExtIscsiStoragePolicy
- CREATE.hyperflex.KeyEncryptionKey
- CREATE.hyperflex.LocalCredentialPolicy
- CREATE.hyperflex.NodeConfigPolicy
- CREATE.hyperflex.NodeProfile
- CREATE.hyperflex.ProxySettingPolicy
- CREATE.hyperflex.ReduceReSync
- CREATE.hyperflex.ServiceAuthToken
- CREATE.hyperflex.SoftwareVersionPolicy
- CREATE.hyperflex.StartReduceReSync
- CREATE.hyperflex.SysConfigPolicy
- CREATE.hyperflex.UcsmConfigPolicy
- CREATE.hyperflex.VcenterConfigPolicy
- CREATE.hyperflex.VmImportOperation
- CREATE.hyperflex.VmRestoreOperation
- CREATE.iam.Account
- CREATE.iam.ApiKey
- CREATE.iam.AppRegistration
- CREATE.iam.Certificate
- CREATE.iam.CertificateRequest
- CREATE.iam.CuiIntegration
- CREATE.iam.DomainNameInfo
- CREATE.iam.EndPointUser
- CREATE.iam.EndPointUserPolicy
- CREATE.iam.EndPointUserRole
- CREATE.iam.GuestAccessSettings
- CREATE.iam.Idp
- CREATE.iam.IpAccessManagement
- CREATE.iam.IpAddress
- CREATE.iam.LdapGroup
- CREATE.iam.LdapPolicy
- CREATE.iam.LdapProvider
- CREATE.iam.LocalUserPassword
- CREATE.iam.Permission
- CREATE.iam.PrivateKeySpec
- CREATE.iam.PrivilegeSet
- CREATE.iam.PrivilegeSetMetaInfo
- CREATE.iam.Qualifier
- CREATE.iam.ResourceRoles
- CREATE.iam.SessionLimits
- CREATE.iam.SharingRule
- CREATE.iam.TrustPoint
- CREATE.iam.User
- CREATE.iam.UserGroup
- CREATE.iam.UserQualifier
- CREATE.iam.UserSetting
- CREATE.inventory.Request
- CREATE.ipmioverlan.Policy
- CREATE.ippool.Pool
- CREATE.ippool.Reservation
- CREATE.iqnpool.Pool
- CREATE.iqnpool.Reservation
- CREATE.iwotenant.Migrate
- CREATE.iwotenant.TenantCustomization
- CREATE.kvm.Policy
- CREATE.kvm.Session
- CREATE.kvm.Tunnel
- CREATE.kvm.TunneledKvmPolicy
- CREATE.license.ErpLicenseCount
- CREATE.license.IksLicenseCount
- CREATE.license.IncLicenseCount
- CREATE.license.IwoLicenseCount
- CREATE.license.LicenseInfo
- CREATE.license.LicenseReservationOp
- CREATE.macpool.Pool
- CREATE.macpool.Reservation
- CREATE.memory.PersistentMemoryPolicy
- CREATE.memory.Policy
- CREATE.metrics.MetricsExploration
- CREATE.metrics.ResourceConfiguration
- CREATE.mgmt.ConfigBackupFile
- CREATE.mgmt.ConfigBackupOperation
- CREATE.mgmt.ConfigOperationSetting
- CREATE.mgmt.ConfigRestoreOperation
- CREATE.networkconfig.Policy
- CREATE.notification.AccountSubscription
- CREATE.ntp.Policy
- CREATE.oauth.Authorization
- CREATE.openapi.OpenApiSpecification
- CREATE.openapi.ProcessFile
- CREATE.openapi.TaskGenerationRequest
- CREATE.oprs.Deployment
- CREATE.oprs.SyncTargetListMessage
- CREATE.organization.Organization
- CREATE.os.BulkInstallInfo
- CREATE.os.ConfigurationFile
- CREATE.os.Install
- CREATE.os.OsSupport
- CREATE.os.TemplateFile
- CREATE.os.ValidInstallTarget
- CREATE.partnerintegration.DeviceConnector
- CREATE.partnerintegration.Etl
- CREATE.partnerintegration.File
- CREATE.partnerintegration.Inventory
- CREATE.partnerintegration.Metrics
- CREATE.partnerintegration.Model
- CREATE.pool.IdMappingPolicy
- CREATE.power.Policy
- CREATE.power.PowerGroup
- CREATE.recommendation.HardwareExpansionRequest
- CREATE.recommendation.HardwareExpansionRequestItem
- CREATE.recommendation.PurchaseOrderEstimate
- CREATE.recovery.BackupConfigPolicy
- CREATE.recovery.BackupProfile
- CREATE.recovery.OnDemandBackup
- CREATE.recovery.Restore
- CREATE.recovery.ScheduleConfigPolicy
- CREATE.resource.Group
- CREATE.resource.Reservation
- CREATE.resource.SelectionCriteria
- CREATE.resourcepool.Pool
- CREATE.resourcepool.QualificationPolicy
- CREATE.resourcepool.Reservation
- CREATE.rproxy.ReverseProxy
- CREATE.scheduler.SchedulePolicy
- CREATE.scheduler.TaskSchedule
- CREATE.sdaaci.Connection
- CREATE.sdaaci.ConnectionDetail
- CREATE.sdcard.Policy
- CREATE.search.SuggestItem
- CREATE.server.ConfigImport
- CREATE.server.DiagnosticStatus
- CREATE.server.Diagnostics
- CREATE.server.Profile
- CREATE.server.ProfileTemplate
- CREATE.smtp.Policy
- CREATE.smtp.PolicyTest
- CREATE.snmp.Policy
- CREATE.software.ApplianceDistributable
- CREATE.software.HciBundleDistributable
- CREATE.software.HciDistributable
- CREATE.software.HyperflexBundleDistributable
- CREATE.software.HyperflexDistributable
- CREATE.software.IksBundleDistributable
- CREATE.software.ReleaseMeta
- CREATE.software.SolutionDistributable
- CREATE.software.UcsdBundleDistributable
- CREATE.software.UcsdDistributable
- CREATE.softwarerepository.Authorization
- CREATE.softwarerepository.OperatingSystemFile
- CREATE.sol.Policy
- CREATE.ssh.Policy
- CREATE.storage.DriveGroup
- CREATE.storage.DriveSecurityPolicy
- CREATE.storage.StoragePolicy
- CREATE.syslog.Policy
- CREATE.tam.AdvisoryInfo
- CREATE.task.CatalystSdwanScopedInventory
- CREATE.task.FabricMosScopedInventory
- CREATE.task.HciScopedInventory
- CREATE.task.HitachiScopedInventory
- CREATE.task.HyperFlexManagementScopedInventory
- CREATE.task.HyperflexScopedInventory
- CREATE.task.MdsScopedInventory
- CREATE.task.MdsSystemScopedInventory
- CREATE.task.MerakiScopedInventory
- CREATE.task.NetAppScopedInventory
- CREATE.task.NexusScopedInventory
- CREATE.task.NexusSystemScopedInventory
- CREATE.task.NexusVlanScopedInventory
- CREATE.task.PureFlashBladeScopedInventory
- CREATE.task.PureScopedInventory
- CREATE.task.ServerScopedInventory
- CREATE.techsupportmanagement.CollectionControlPolicy
- CREATE.techsupportmanagement.TechSupportBundle
- CREATE.telemetry.TimeSeries
- CREATE.thermal.Policy
- CREATE.uuidpool.Pool
- CREATE.uuidpool.Reservation
- CREATE.virtualization.EsxiConsole
- CREATE.virtualization.VirtualMachine
- CREATE.vmedia.Policy
- CREATE.vmrc.Console
- CREATE.vnic.EthAdapterPolicy
- CREATE.vnic.EthIf
- CREATE.vnic.EthNetworkPolicy
- CREATE.vnic.EthQosPolicy
- CREATE.vnic.FcAdapterPolicy
- CREATE.vnic.FcIf
- CREATE.vnic.FcNetworkPolicy
- CREATE.vnic.FcQosPolicy
- CREATE.vnic.IscsiAdapterPolicy
- CREATE.vnic.IscsiBootPolicy
- CREATE.vnic.IscsiStaticTargetPolicy
- CREATE.vnic.LanConnectivityPolicy
- CREATE.vnic.SanConnectivityPolicy
- CREATE.vnic.VhbaTemplate
- CREATE.vnic.VnicTemplate
- CREATE.vrf.Vrf
- CREATE.webhook.Endpoint
- CREATE.webhook.Schema
- CREATE.workflow.AnsibleBatchExecutor
- CREATE.workflow.BatchApiExecutor
- CREATE.workflow.CatalogItemDefinition
- CREATE.workflow.CatalogServiceRequest
- CREATE.workflow.CustomDataTypeDefinition
- CREATE.workflow.ErrorResponseHandler
- CREATE.workflow.PowerShellBatchApiExecutor
- CREATE.workflow.RollbackWorkflow
- CREATE.workflow.ServiceItemActionDefinition
- CREATE.workflow.ServiceItemActionInstance
- CREATE.workflow.ServiceItemDefinition
- CREATE.workflow.ServiceItemInstance
- CREATE.workflow.ServiceItemOutput
- CREATE.workflow.SshBatchExecutor
- CREATE.workflow.TaskDefinition
- CREATE.workflow.TemplateEvaluation
- CREATE.workflow.TemplateParser
- CREATE.workflow.UiDisplayMetadata
- CREATE.workflow.Variable
- CREATE.workflow.WorkflowDefinition
- CREATE.workflow.WorkflowInfo
- CREATE.workload.Blueprint
- CREATE.workload.ClearWorkloadTag
- CREATE.workload.WorkloadDefinition
- CREATE.workload.WorkloadDeployment
- DELETE.access.Policy
- DELETE.adapter.ConfigPolicy
- DELETE.appliance.Backup
- DELETE.appliance.ClusterInfo
- DELETE.appliance.ExternalSyslogSetting
- DELETE.appliance.Restore
- DELETE.appliance.Upgrade
- DELETE.asset.ClaimToken
- DELETE.asset.DeviceClaim
- DELETE.asset.GeoLocation
- DELETE.asset.Target
- DELETE.auditd.Policy
- DELETE.bios.Policy
- DELETE.boot.PrecisionPolicy
- DELETE.bulk.Export
- DELETE.certificatemanagement.Policy
- DELETE.chassis.Profile
- DELETE.chassis.ProfileTemplate
- DELETE.cli.CliPolicy
- DELETE.comm.HttpProxyPolicy
- DELETE.comm.TagDefinition
- DELETE.compute.PcieConnectivityPolicy
- DELETE.compute.RackUnit
- DELETE.compute.RackUnitIdentity
- DELETE.compute.ScrubPolicy
- DELETE.compute.ServerPowerPolicy
- DELETE.cond.AlarmRule
- DELETE.cond.AlarmSuppression
- DELETE.cond.CustomHclBaseline
- DELETE.cond.ThresholdDefinition
- DELETE.connectorpack.ConnectorPackUpgrade
- DELETE.coremanagement.CoreFile
- DELETE.crd.CustomResource
- DELETE.deviceconnector.Policy
- DELETE.fabric.AppliancePcRole
- DELETE.fabric.ApplianceRole
- DELETE.fabric.EthNetworkControlPolicy
- DELETE.fabric.EthNetworkGroupPolicy
- DELETE.fabric.EthNetworkPolicy
- DELETE.fabric.FcNetworkPolicy
- DELETE.fabric.FcStorageRole
- DELETE.fabric.FcUplinkPcRole
- DELETE.fabric.FcUplinkRole
- DELETE.fabric.FcZonePolicy
- DELETE.fabric.FcoeUplinkPcRole
- DELETE.fabric.FcoeUplinkRole
- DELETE.fabric.FlowControlPolicy
- DELETE.fabric.LanPinGroup
- DELETE.fabric.LinkAggregationPolicy
- DELETE.fabric.LinkControlPolicy
- DELETE.fabric.MacSecPolicy
- DELETE.fabric.MulticastPolicy
- DELETE.fabric.NetFlowExporter
- DELETE.fabric.NetFlowMonitor
- DELETE.fabric.NetFlowPolicy
- DELETE.fabric.NetFlowRecord
- DELETE.fabric.PcOperation
- DELETE.fabric.PortMode
- DELETE.fabric.PortOperation
- DELETE.fabric.PortPolicy
- DELETE.fabric.SanPinGroup
- DELETE.fabric.SecureRouterRole
- DELETE.fabric.ServerRole
- DELETE.fabric.SpanDestEthPort
- DELETE.fabric.SpanSession
- DELETE.fabric.SpanSourceEthPort
- DELETE.fabric.SpanSourceEthPortChannel
- DELETE.fabric.SpanSourceVlan
- DELETE.fabric.SpanSourceVnicEthIf
- DELETE.fabric.SwitchClusterProfile
- DELETE.fabric.SwitchClusterProfileTemplate
- DELETE.fabric.SwitchControlPolicy
- DELETE.fabric.SwitchProfile
- DELETE.fabric.SwitchProfileTemplate
- DELETE.fabric.SystemQosPolicy
- DELETE.fabric.UplinkPcRole
- DELETE.fabric.UplinkRole
- DELETE.fabric.Vlan
- DELETE.fabric.Vsan
- DELETE.fcpool.Lease
- DELETE.fcpool.Pool
- DELETE.fcpool.Reservation
- DELETE.firmware.ChassisUpgrade
- DELETE.firmware.Distributable
- DELETE.firmware.DriverDistributable
- DELETE.firmware.PciNodeUpgrade
- DELETE.firmware.Policy
- DELETE.firmware.SecureRouterUpgrade
- DELETE.firmware.ServerConfigurationUtilityDistributable
- DELETE.firmware.SwitchUpgrade
- DELETE.firmware.UnsupportedVersionUpgrade
- DELETE.firmware.Upgrade
- DELETE.hyperflex.AutoSupportPolicy
- DELETE.hyperflex.BackupCluster
- DELETE.hyperflex.ClusterBackupPolicy
- DELETE.hyperflex.ClusterBackupPolicyDeployment
- DELETE.hyperflex.ClusterBackupPolicyInventory
- DELETE.hyperflex.ClusterNetworkPolicy
- DELETE.hyperflex.ClusterProfile
- DELETE.hyperflex.ClusterReplicationNetworkPolicy
- DELETE.hyperflex.ClusterReplicationNetworkPolicyDeployment
- DELETE.hyperflex.ClusterStoragePolicy
- DELETE.hyperflex.ExtFcStoragePolicy
- DELETE.hyperflex.ExtIscsiStoragePolicy
- DELETE.hyperflex.KeyEncryptionKey
- DELETE.hyperflex.LocalCredentialPolicy
- DELETE.hyperflex.NodeConfigPolicy
- DELETE.hyperflex.NodeProfile
- DELETE.hyperflex.ProxySettingPolicy
- DELETE.hyperflex.ServiceAuthToken
- DELETE.hyperflex.SoftwareVersionPolicy
- DELETE.hyperflex.SysConfigPolicy
- DELETE.hyperflex.UcsmConfigPolicy
- DELETE.hyperflex.VcenterConfigPolicy
- DELETE.hyperflex.VmBackupInfo
- DELETE.hyperflex.VmImportOperation
- DELETE.hyperflex.VmRestoreOperation
- DELETE.hyperflex.VmSnapshotInfo
- DELETE.iam.Account
- DELETE.iam.ApiKey
- DELETE.iam.AppRegistration
- DELETE.iam.Certificate
- DELETE.iam.CertificateRequest
- DELETE.iam.DomainNameInfo
- DELETE.iam.EndPointUser
- DELETE.iam.EndPointUserPolicy
- DELETE.iam.EndPointUserRole
- DELETE.iam.GuestAccessSettings
- DELETE.iam.Idp
- DELETE.iam.IpAddress
- DELETE.iam.LdapGroup
- DELETE.iam.LdapPolicy
- DELETE.iam.LdapProvider
- DELETE.iam.OAuthToken
- DELETE.iam.Permission
- DELETE.iam.PrivateKeySpec
- DELETE.iam.PrivilegeSet
- DELETE.iam.Qualifier
- DELETE.iam.ResourceRoles
- DELETE.iam.Session
- DELETE.iam.SessionLimits
- DELETE.iam.SharingRule
- DELETE.iam.TrustPoint
- DELETE.iam.User
- DELETE.iam.UserGroup
- DELETE.iam.UserQualifier
- DELETE.ipmioverlan.Policy
- DELETE.ippool.IpLease
- DELETE.ippool.Pool
- DELETE.ippool.Reservation
- DELETE.iqnpool.Lease
- DELETE.iqnpool.Pool
- DELETE.iqnpool.Reservation
- DELETE.iwotenant.TenantCustomization
- DELETE.kvm.Policy
- DELETE.kvm.TunneledKvmPolicy
- DELETE.macpool.Lease
- DELETE.macpool.Pool
- DELETE.macpool.Reservation
- DELETE.memory.PersistentMemoryPolicy
- DELETE.memory.Policy
- DELETE.metrics.MetricsExploration
- DELETE.mgmt.ConfigBackupFile
- DELETE.mgmt.ConfigBackupInstance
- DELETE.mgmt.ConfigBackupOperation
- DELETE.mgmt.ConfigOperationSetting
- DELETE.mgmt.ConfigRestoreOperation
- DELETE.networkconfig.Policy
- DELETE.notification.AccountSubscription
- DELETE.ntp.Policy
- DELETE.oauth.AccessToken
- DELETE.openapi.ApiMethodMeta
- DELETE.openapi.OpenApiSpecification
- DELETE.openapi.ProcessFile
- DELETE.openapi.TaskGenerationRequest
- DELETE.openapi.TaskGenerationResult
- DELETE.oprs.Deployment
- DELETE.oprs.SyncTargetListMessage
- DELETE.organization.Organization
- DELETE.os.ConfigurationFile
- DELETE.partnerintegration.DeviceConnector
- DELETE.partnerintegration.Etl
- DELETE.partnerintegration.File
- DELETE.partnerintegration.Inventory
- DELETE.partnerintegration.Metrics
- DELETE.partnerintegration.Model
- DELETE.pool.IdMappingPolicy
- DELETE.power.Policy
- DELETE.power.PowerGroup
- DELETE.recovery.BackupConfigPolicy
- DELETE.recovery.BackupProfile
- DELETE.recovery.OnDemandBackup
- DELETE.recovery.Restore
- DELETE.recovery.ScheduleConfigPolicy
- DELETE.resource.Group
- DELETE.resource.Reservation
- DELETE.resource.SelectionCriteria
- DELETE.resourcepool.ChassisQualificationPolicy
- DELETE.resourcepool.Lease
- DELETE.resourcepool.MembershipReservation
- DELETE.resourcepool.Pool
- DELETE.resourcepool.QualificationPolicy
- DELETE.resourcepool.Reservation
- DELETE.scheduler.SchedulePolicy
- DELETE.scheduler.TaskSchedule
- DELETE.sdaaci.Connection
- DELETE.sdaaci.ConnectionDetail
- DELETE.sdcard.Policy
- DELETE.server.DiagnosticStatus
- DELETE.server.Diagnostics
- DELETE.server.MigrationKeyDetails
- DELETE.server.Profile
- DELETE.server.ProfileTemplate
- DELETE.smtp.Policy
- DELETE.smtp.PolicyTest
- DELETE.snmp.Policy
- DELETE.software.ApplianceDistributable
- DELETE.software.HciBundleDistributable
- DELETE.software.HciDistributable
- DELETE.software.HyperflexBundleDistributable
- DELETE.software.HyperflexDistributable
- DELETE.software.IksBundleDistributable
- DELETE.software.ReleaseMeta
- DELETE.software.SolutionDistributable
- DELETE.software.UcsdBundleDistributable
- DELETE.software.UcsdDistributable
- DELETE.softwarerepository.OperatingSystemFile
- DELETE.sol.Policy
- DELETE.ssh.Policy
- DELETE.storage.DriveGroup
- DELETE.storage.DriveSecurityPolicy
- DELETE.storage.StoragePolicy
- DELETE.syslog.Policy
- DELETE.tam.AdvisoryInfo
- DELETE.techsupportmanagement.CollectionControlPolicy
- DELETE.techsupportmanagement.TechSupportBundle
- DELETE.thermal.Policy
- DELETE.ucsd.BackupInfo
- DELETE.uuidpool.Pool
- DELETE.uuidpool.Reservation
- DELETE.uuidpool.UuidLease
- DELETE.virtualization.VirtualMachine
- DELETE.vmedia.Policy
- DELETE.vnic.EthAdapterPolicy
- DELETE.vnic.EthIf
- DELETE.vnic.EthNetworkPolicy
- DELETE.vnic.EthQosPolicy
- DELETE.vnic.FcAdapterPolicy
- DELETE.vnic.FcIf
- DELETE.vnic.FcNetworkPolicy
- DELETE.vnic.FcQosPolicy
- DELETE.vnic.IscsiAdapterPolicy
- DELETE.vnic.IscsiBootPolicy
- DELETE.vnic.IscsiStaticTargetPolicy
- DELETE.vnic.LanConnectivityPolicy
- DELETE.vnic.SanConnectivityPolicy
- DELETE.vnic.VhbaTemplate
- DELETE.vnic.VnicTemplate
- DELETE.vrf.Vrf
- DELETE.webhook.Endpoint
- DELETE.webhook.Schema
- DELETE.workflow.AnsibleBatchExecutor
- DELETE.workflow.BatchApiExecutor
- DELETE.workflow.CatalogItemDefinition
- DELETE.workflow.CatalogServiceRequest
- DELETE.workflow.CustomDataTypeDefinition
- DELETE.workflow.ErrorResponseHandler
- DELETE.workflow.PowerShellBatchApiExecutor
- DELETE.workflow.RollbackWorkflow
- DELETE.workflow.ServiceItemActionDefinition
- DELETE.workflow.ServiceItemActionInstance
- DELETE.workflow.ServiceItemDefinition
- DELETE.workflow.ServiceItemInstance
- DELETE.workflow.ServiceItemOutput
- DELETE.workflow.SshBatchExecutor
- DELETE.workflow.TaskDefinition
- DELETE.workflow.UiDisplayMetadata
- DELETE.workflow.Variable
- DELETE.workflow.WorkflowDefinition
- DELETE.workflow.WorkflowInfo
- DELETE.workload.Blueprint
- DELETE.workload.ClearWorkloadTag
- DELETE.workload.WorkloadDefinition
- DELETE.workload.WorkloadDeployment
- DELETE.workload.WorkloadInstance
- PRIVSET.API keys
- PRIVSET.API keys and OAuth tokens
- PRIVSET.Access and permissions
- PRIVSET.Access domains
- PRIVSET.Access servers
- PRIVSET.Account
- PRIVSET.Account Administrator
- PRIVSET.Acknowledge advisories
- PRIVSET.Acknowledge alarms
- PRIVSET.Activate server profiles
- PRIVSET.Activate webhook
- PRIVSET.Adapter Configuration policies
- PRIVSET.Add OS configuration links
- PRIVSET.Add OS image links
- PRIVSET.Add SCU links
- PRIVSET.Add and remove server profile template tags
- PRIVSET.Add domain names
- PRIVSET.Add explorations to dashboard
- PRIVSET.Add external syslog servers
- PRIVSET.Add firmware links
- PRIVSET.Add identity providers
- PRIVSET.Add notification rule or webhook
- PRIVSET.Add trusted IP ranges
- PRIVSET.Add trusted certificates
- PRIVSET.Alerts
- PRIVSET.Allow or Disallow Data Collection
- PRIVSET.Allow/disallow FI and Unified Edge eCMC CLI launches
- PRIVSET.Allow/disallow tech support bundles
- PRIVSET.Allow/disallow tunneled vKVM configurations
- PRIVSET.Allow/disallow tunneled vKVM launches
- PRIVSET.Appliance authentication
- PRIVSET.Appliance configuration
- PRIVSET.Appliance networking
- PRIVSET.Appliance security & privacy
- PRIVSET.Apply SSL Certificate
- PRIVSET.Approve Publish Requests
- PRIVSET.Assign chassis profiles
- PRIVSET.Assign domain profiles
- PRIVSET.Assign server profiles
- PRIVSET.Attach to and detach from chassis profile templates
- PRIVSET.Attach to and detach from domain profile templates
- PRIVSET.Attach to and detach from server profile templates
- PRIVSET.Audit Log Viewer
- PRIVSET.Audit logs
- PRIVSET.AuditD policies
- PRIVSET.Authentication
- PRIVSET.Authentication settings
- PRIVSET.Automation Governance
- PRIVSET.BIOS policies
- PRIVSET.Boot Order policies
- PRIVSET.Catalog Administrator
- PRIVSET.Catalog User
- PRIVSET.Certificate Management policies
- PRIVSET.Cisco ID
- PRIVSET.Claim Devices
- PRIVSET.Claim targets
- PRIVSET.Clear TPMs
- PRIVSET.Clear configurations
- PRIVSET.Clear foreign configurations
- PRIVSET.Clear system event logs (SEL)
- PRIVSET.Clusters
- PRIVSET.Complete Claim
- PRIVSET.Configure
- PRIVSET.Configure Cisco software download credentials
- PRIVSET.Configure DNS settings
- PRIVSET.Configure IP pools
- PRIVSET.Configure IQN pools
- PRIVSET.Configure LDAP servers
- PRIVSET.Configure Local Users Password Policy
- PRIVSET.Configure MAC pools
- PRIVSET.Configure MFA
- PRIVSET.Configure NTP settings
- PRIVSET.Configure Resource Pool
- PRIVSET.Configure SMTP servers
- PRIVSET.Configure UUID pools
- PRIVSET.Configure WWNN or WWPN pools
- PRIVSET.Configure account details
- PRIVSET.Configure backup schedule
- PRIVSET.Configure banner message
- PRIVSET.Configure chassis profile templates
- PRIVSET.Configure chassis profiles
- PRIVSET.Configure compute policies
- PRIVSET.Configure data collection settings
- PRIVSET.Configure device connector settings
- PRIVSET.Configure domain profile templates
- PRIVSET.Configure domain profiles
- PRIVSET.Configure management policies
- PRIVSET.Configure metrics settings
- PRIVSET.Configure network policies
- PRIVSET.Configure physical chassis
- PRIVSET.Configure physical domains
- PRIVSET.Configure physical servers
- PRIVSET.Configure pools
- PRIVSET.Configure server profile templates
- PRIVSET.Configure server profiles
- PRIVSET.Configure software update settings
- PRIVSET.Configure storage policies
- PRIVSET.Configure vHBA templates
- PRIVSET.Configure vNIC templates
- PRIVSET.Create Approval Request
- PRIVSET.Create CSR
- PRIVSET.Create IP pool address reservations
- PRIVSET.Create IP pools
- PRIVSET.Create IQN pool address reservations
- PRIVSET.Create IQN pools
- PRIVSET.Create MAC pool address reservations
- PRIVSET.Create MAC pools
- PRIVSET.Create Nexus Reports
- PRIVSET.Create OAuth 2.0 grant type applications
- PRIVSET.Create Resource pool address reservations
- PRIVSET.Create Resource pools
- PRIVSET.Create UUID pool address reservations
- PRIVSET.Create UUID pools
- PRIVSET.Create WWNN and WWPN pool address reservations
- PRIVSET.Create WWNN or WWPN pools
- PRIVSET.Create backups
- PRIVSET.Create chassis profile templates from chassis profile
- PRIVSET.Create domain profile templates from domain profile
- PRIVSET.Create integrated systems
- PRIVSET.Create server profile template from server profile
- PRIVSET.Create, clone and edit Adapter Configuration policies
- PRIVSET.Create, clone and edit AuditD policies
- PRIVSET.Create, clone and edit BIOS policies
- PRIVSET.Create, clone and edit Boot Order policies
- PRIVSET.Create, clone and edit Certificate Management policies
- PRIVSET.Create, clone and edit Device Connector policies
- PRIVSET.Create, clone and edit Drive Security policies
- PRIVSET.Create, clone and edit Ethernet Adapter policies
- PRIVSET.Create, clone and edit Ethernet Network Control policies
- PRIVSET.Create, clone and edit Ethernet Network Group policies
- PRIVSET.Create, clone and edit Ethernet Network policies
- PRIVSET.Create, clone and edit Ethernet QoS policies
- PRIVSET.Create, clone and edit FC Zone policies
- PRIVSET.Create, clone and edit Fibre Channel Adapter policies
- PRIVSET.Create, clone and edit Fibre Channel Network policies
- PRIVSET.Create, clone and edit Fibre Channel QoS policies
- PRIVSET.Create, clone and edit Firmware policies
- PRIVSET.Create, clone and edit Flow Control policies
- PRIVSET.Create, clone and edit IMC Access policies
- PRIVSET.Create, clone and edit IPMI over LAN policies
- PRIVSET.Create, clone and edit LAN Connectivity policies
- PRIVSET.Create, clone and edit LDAP policies
- PRIVSET.Create, clone and edit Link Aggregation policies
- PRIVSET.Create, clone and edit Link Control policies
- PRIVSET.Create, clone and edit Local User policies
- PRIVSET.Create, clone and edit Memory policies
- PRIVSET.Create, clone and edit Multicast policies
- PRIVSET.Create, clone and edit NTP policies
- PRIVSET.Create, clone and edit Network Connectivity policies
- PRIVSET.Create, clone and edit Persistent Memory policies
- PRIVSET.Create, clone and edit Port policies
- PRIVSET.Create, clone and edit Power policies
- PRIVSET.Create, clone and edit SAN Connectivity policies
- PRIVSET.Create, clone and edit SD Card policies
- PRIVSET.Create, clone and edit SMTP policies
- PRIVSET.Create, clone and edit SNMP policies
- PRIVSET.Create, clone and edit SSH policies
- PRIVSET.Create, clone and edit Scrub policies
- PRIVSET.Create, clone and edit Serial Over LAN policies
- PRIVSET.Create, clone and edit Storage policies
- PRIVSET.Create, clone and edit Switch Control policies
- PRIVSET.Create, clone and edit Syslog policies
- PRIVSET.Create, clone and edit System QoS policies
- PRIVSET.Create, clone and edit Thermal policies
- PRIVSET.Create, clone and edit VLAN policies
- PRIVSET.Create, clone and edit VSAN policies
- PRIVSET.Create, clone and edit Virtual KVM policies
- PRIVSET.Create, clone and edit Virtual Media policies
- PRIVSET.Create, clone and edit iSCSI Adapter policies
- PRIVSET.Create, clone and edit iSCSI Boot policies
- PRIVSET.Create, clone and edit iSCSI Static Target policies
- PRIVSET.Create, clone, and edit chassis profile templates
- PRIVSET.Create, clone, and edit chassis profiles
- PRIVSET.Create, clone, and edit domain profile templates
- PRIVSET.Create, clone, and edit domain profiles
- PRIVSET.Create, clone, and edit server profile templates
- PRIVSET.Create, clone, and edit server profiles
- PRIVSET.Create, clone, and edit vHBA templates
- PRIVSET.Create, clone, and edit vNIC templates
- PRIVSET.Datacenters
- PRIVSET.Datastore clusters
- PRIVSET.Datastores
- PRIVSET.Decommission Fabric Extender (FEX)
- PRIVSET.Decommission chassis
- PRIVSET.Decommission servers
- PRIVSET.Define and edit chassis profile general properties
- PRIVSET.Define and edit chassis profile template general properties
- PRIVSET.Define and edit domain profile general properties
- PRIVSET.Define and edit domain profile template general properties
- PRIVSET.Define and edit server profile general properties
- PRIVSET.Define and edit server profile template general properties
- PRIVSET.Define and edit vHBA template general properties
- PRIVSET.Define and edit vNIC template general properties
- PRIVSET.Delete API keys
- PRIVSET.Delete Adapter Configuration policies
- PRIVSET.Delete Approval Request
- PRIVSET.Delete AuditD policies
- PRIVSET.Delete BIOS policies
- PRIVSET.Delete Boot Order policies
- PRIVSET.Delete CSR
- PRIVSET.Delete Certificate Management policies
- PRIVSET.Delete Device Connector policies
- PRIVSET.Delete Devices
- PRIVSET.Delete Drive Security policies
- PRIVSET.Delete Ethernet Adapter policies
- PRIVSET.Delete Ethernet Network Control policies
- PRIVSET.Delete Ethernet Network Group policies
- PRIVSET.Delete Ethernet Network policies
- PRIVSET.Delete Ethernet QoS policies
- PRIVSET.Delete FC Zone policies
- PRIVSET.Delete Fibre Channel Adapter policies
- PRIVSET.Delete Fibre Channel Network policies
- PRIVSET.Delete Fibre Channel QoS policies
- PRIVSET.Delete Firmware policies
- PRIVSET.Delete Flow Control policies
- PRIVSET.Delete IMC Access policies
- PRIVSET.Delete IP pool address reservations
- PRIVSET.Delete IP pools
- PRIVSET.Delete IPMI over LAN policies
- PRIVSET.Delete IQN pool address reservations
- PRIVSET.Delete IQN pools
- PRIVSET.Delete LAN Connectivity policies
- PRIVSET.Delete LDAP policies
- PRIVSET.Delete LDAP servers
- PRIVSET.Delete Link Aggregation policies
- PRIVSET.Delete Link Control policies
- PRIVSET.Delete Local User policies
- PRIVSET.Delete MAC pool address reservations
- PRIVSET.Delete MAC pools
- PRIVSET.Delete Memory policies
- PRIVSET.Delete Multicast policies
- PRIVSET.Delete NTP policies
- PRIVSET.Delete Network Connectivity policies
- PRIVSET.Delete OAuth 2.0 grant type applications
- PRIVSET.Delete OAuth 2.0 tokens
- PRIVSET.Delete OS configuration links
- PRIVSET.Delete OS image links
- PRIVSET.Delete Persistent Memory policies
- PRIVSET.Delete Port policies
- PRIVSET.Delete Power policies
- PRIVSET.Delete Resource pool address reservations
- PRIVSET.Delete Resource pools
- PRIVSET.Delete SAN Connectivity policies
- PRIVSET.Delete SCU links
- PRIVSET.Delete SD Card policies
- PRIVSET.Delete SMTP policies
- PRIVSET.Delete SNMP policies
- PRIVSET.Delete SSH policies
- PRIVSET.Delete Scrub policies
- PRIVSET.Delete Serial Over LAN policies
- PRIVSET.Delete Storage policies
- PRIVSET.Delete Switch Control policies
- PRIVSET.Delete Syslog policies
- PRIVSET.Delete System QoS policies
- PRIVSET.Delete Thermal policies
- PRIVSET.Delete UUID pool address reservations
- PRIVSET.Delete UUID pools
- PRIVSET.Delete VLAN policies
- PRIVSET.Delete VSAN policies
- PRIVSET.Delete Virtual KVM policies
- PRIVSET.Delete Virtual Media policies
- PRIVSET.Delete WWNN and WWPN pool address reservations
- PRIVSET.Delete WWNN or WWPN pools
- PRIVSET.Delete chassis profile templates
- PRIVSET.Delete chassis profiles
- PRIVSET.Delete domain names
- PRIVSET.Delete domain profile templates
- PRIVSET.Delete domain profiles
- PRIVSET.Delete explorations
- PRIVSET.Delete external syslog servers
- PRIVSET.Delete firmware links
- PRIVSET.Delete iSCSI Adapter policies
- PRIVSET.Delete iSCSI Boot policies
- PRIVSET.Delete iSCSI Static Target policies
- PRIVSET.Delete identity providers
- PRIVSET.Delete integrated systems
- PRIVSET.Delete notification rule or webhook
- PRIVSET.Delete server profile templates
- PRIVSET.Delete server profiles
- PRIVSET.Delete trusted IP ranges
- PRIVSET.Delete trusted certificates
- PRIVSET.Delete vHBA templates
- PRIVSET.Delete vNIC templates
- PRIVSET.Deploy chassis profiles
- PRIVSET.Deploy domain profiles
- PRIVSET.Deploy server profiles
- PRIVSET.Deregister Smart Licenses
- PRIVSET.Derive profiles from chassis profile templates
- PRIVSET.Derive profiles from domain profile templates
- PRIVSET.Derive server profiles
- PRIVSET.Device Administrator
- PRIVSET.Device Connector policies
- PRIVSET.Device Technician
- PRIVSET.Devices
- PRIVSET.Disable security
- PRIVSET.Disable subscriptions
- PRIVSET.Domain names
- PRIVSET.Download server event logs
- PRIVSET.Drive Security policies
- PRIVSET.Edit API keys
- PRIVSET.Edit Adapter Configuration policies
- PRIVSET.Edit Adapter Configuration policies for server profile
- PRIVSET.Edit Adapter Configuration policies for server profile template
- PRIVSET.Edit AuditD policies
- PRIVSET.Edit AuditD policies for domain profile
- PRIVSET.Edit AuditD policies for domain profile template
- PRIVSET.Edit BIOS policies
- PRIVSET.Edit BIOS policies for server profile
- PRIVSET.Edit BIOS policies for server profile template
- PRIVSET.Edit Boot Order policies
- PRIVSET.Edit Boot Order policies for server profile
- PRIVSET.Edit Boot Order policies for server profile template
- PRIVSET.Edit Certificate Management policies
- PRIVSET.Edit Certificate Management policies for domain profile
- PRIVSET.Edit Certificate Management policies for domain profile template
- PRIVSET.Edit Certificate Management policies for server profile
- PRIVSET.Edit Certificate Management policies for server profile template
- PRIVSET.Edit Device Connector policies
- PRIVSET.Edit Device Connector policies for server profile
- PRIVSET.Edit Device Connector policies for server profile template
- PRIVSET.Edit Drive Security policies
- PRIVSET.Edit Drive Security policies for server profile
- PRIVSET.Edit Drive Security policies for server profile template
- PRIVSET.Edit Ethernet Adapter policies
- PRIVSET.Edit Ethernet Adapter policies for vNIC template
- PRIVSET.Edit Ethernet Network Control policies
- PRIVSET.Edit Ethernet Network Control policies for vNIC template
- PRIVSET.Edit Ethernet Network Group policies
- PRIVSET.Edit Ethernet Network Group policies for vNIC template
- PRIVSET.Edit Ethernet Network policies
- PRIVSET.Edit Ethernet QoS policies
- PRIVSET.Edit Ethernet QoS policies for vNIC template
- PRIVSET.Edit FC Zone policies
- PRIVSET.Edit Fibre Channel Adapter policies
- PRIVSET.Edit Fibre Channel Adapter policies for vHBA template
- PRIVSET.Edit Fibre Channel Network policies
- PRIVSET.Edit Fibre Channel Network policies for vHBA template
- PRIVSET.Edit Fibre Channel QoS policies
- PRIVSET.Edit Fibre Channel QoS policies for vHBA template
- PRIVSET.Edit Fibre Channel Zone policies for vHBA template
- PRIVSET.Edit Firmware policies
- PRIVSET.Edit Firmware policies for server profile
- PRIVSET.Edit Firmware policies for server profile template
- PRIVSET.Edit Flow Control policies
- PRIVSET.Edit IMC Access policies
- PRIVSET.Edit IMC Access policies for chassis profile
- PRIVSET.Edit IMC Access policies for chassis profile template
- PRIVSET.Edit IMC Access policies for server profile
- PRIVSET.Edit IMC Access policies for server profile template
- PRIVSET.Edit IP pools
- PRIVSET.Edit IPMI Over LAN policies for server profile
- PRIVSET.Edit IPMI Over LAN policies for server profile template
- PRIVSET.Edit IPMI over LAN policies
- PRIVSET.Edit IQN pools
- PRIVSET.Edit LAN Connectivity policies
- PRIVSET.Edit LAN Connectivity policies for server profile
- PRIVSET.Edit LAN Connectivity policies for server profile template
- PRIVSET.Edit LDAP policies
- PRIVSET.Edit LDAP policies for domain profile
- PRIVSET.Edit LDAP policies for domain profile template
- PRIVSET.Edit LDAP policies for server profile
- PRIVSET.Edit LDAP policies for server profile template
- PRIVSET.Edit LDAP servers
- PRIVSET.Edit Link Aggregation policies
- PRIVSET.Edit Link Control policies
- PRIVSET.Edit Local User policies
- PRIVSET.Edit Local User policies for domain profile
- PRIVSET.Edit Local User policies for domain profile template
- PRIVSET.Edit Local User policies for server profile
- PRIVSET.Edit Local User policies for server profile template
- PRIVSET.Edit MAC Pools for vNIC template
- PRIVSET.Edit MAC pools
- PRIVSET.Edit Memory policies
- PRIVSET.Edit Memory policies for server profile
- PRIVSET.Edit Memory policies for server profile template
- PRIVSET.Edit Multicast policies
- PRIVSET.Edit NTP policies
- PRIVSET.Edit NTP policies for domain profile
- PRIVSET.Edit NTP policies for domain profile template
- PRIVSET.Edit NTP policies for server profile
- PRIVSET.Edit NTP policies for server profile template
- PRIVSET.Edit Network Connectivity policies
- PRIVSET.Edit Network Connectivity policies for domain profile
- PRIVSET.Edit Network Connectivity policies for domain profile template
- PRIVSET.Edit Network Connectivity policies for server profile
- PRIVSET.Edit Network Connectivity policies for server profile template
- PRIVSET.Edit OAuth 2.0 grant type applications
- PRIVSET.Edit OS configuration links
- PRIVSET.Edit OS image links
- PRIVSET.Edit Persistent Memory policies
- PRIVSET.Edit Persistent Memory policies for server profile
- PRIVSET.Edit Persistent Memory policies for server profile template
- PRIVSET.Edit Port policies
- PRIVSET.Edit Ports Configuration policies for domain profile
- PRIVSET.Edit Ports Configuration policies for domain profile template
- PRIVSET.Edit Power policies
- PRIVSET.Edit Power policies for chassis profile
- PRIVSET.Edit Power policies for chassis profile template
- PRIVSET.Edit Power policies for server profile
- PRIVSET.Edit Power policies for server profile template
- PRIVSET.Edit Resource pools
- PRIVSET.Edit SAN Connectivity policies
- PRIVSET.Edit SAN Connectivity policies for server profile
- PRIVSET.Edit SAN Connectivity policies for server profile template
- PRIVSET.Edit SCU links
- PRIVSET.Edit SD Card policies
- PRIVSET.Edit SD Card policies for server profile
- PRIVSET.Edit SD Card policies for server profile template
- PRIVSET.Edit SMTP policies
- PRIVSET.Edit SMTP policies for server profile
- PRIVSET.Edit SMTP policies for server profile template
- PRIVSET.Edit SNMP policies
- PRIVSET.Edit SNMP policies for chassis profile
- PRIVSET.Edit SNMP policies for chassis profile template
- PRIVSET.Edit SNMP policies for domain profile
- PRIVSET.Edit SNMP policies for domain profile template
- PRIVSET.Edit SNMP policies for server profile
- PRIVSET.Edit SNMP policies for server profile template
- PRIVSET.Edit SSH policies
- PRIVSET.Edit SSH policies for server profile
- PRIVSET.Edit SSH policies for server profile template
- PRIVSET.Edit Scrub policies
- PRIVSET.Edit Scrub policies for server profile
- PRIVSET.Edit Scrub policies for server profile template
- PRIVSET.Edit Serial Over LAN policies
- PRIVSET.Edit Serial Over LAN policies for server profile
- PRIVSET.Edit Serial Over LAN policies for server profile template
- PRIVSET.Edit Storage policies
- PRIVSET.Edit Storage policies for server profile
- PRIVSET.Edit Storage policies for server profile template
- PRIVSET.Edit Switch Control policies
- PRIVSET.Edit Switch Control policies for domain profile
- PRIVSET.Edit Switch Control policies for domain profile template
- PRIVSET.Edit Syslog policies
- PRIVSET.Edit Syslog policies for domain profile
- PRIVSET.Edit Syslog policies for domain profile template
- PRIVSET.Edit Syslog policies for server profile
- PRIVSET.Edit Syslog policies for server profile template
- PRIVSET.Edit System QoS policies
- PRIVSET.Edit System QoS policies for domain profile
- PRIVSET.Edit System QoS policies for domain profile template
- PRIVSET.Edit Thermal policies
- PRIVSET.Edit Thermal policies for chassis profile
- PRIVSET.Edit Thermal policies for chassis profile template
- PRIVSET.Edit Thermal policies for server profile
- PRIVSET.Edit Thermal policies for server profile template
- PRIVSET.Edit UUID pools
- PRIVSET.Edit UUID pools for server profile
- PRIVSET.Edit UUID pools for server profile template
- PRIVSET.Edit VLAN policies
- PRIVSET.Edit VSAN policies
- PRIVSET.Edit Virtual KVM policies
- PRIVSET.Edit Virtual KVM policies for server profile
- PRIVSET.Edit Virtual KVM policies for server profile template
- PRIVSET.Edit Virtual Media policies
- PRIVSET.Edit Virtual Media policies for server profile
- PRIVSET.Edit Virtual Media policies for server profile template
- PRIVSET.Edit WWNN or WWPN pools
- PRIVSET.Edit WWPN pools for vHBA template
- PRIVSET.Edit chassis profile general properties
- PRIVSET.Edit chassis profile policies
- PRIVSET.Edit chassis profile template general properties
- PRIVSET.Edit chassis profile template policies
- PRIVSET.Edit chassis profile templates
- PRIVSET.Edit chassis profiles
- PRIVSET.Edit domain profile general properties
- PRIVSET.Edit domain profile policies
- PRIVSET.Edit domain profile template general properties
- PRIVSET.Edit domain profile template policies
- PRIVSET.Edit domain profile templates
- PRIVSET.Edit domain profiles
- PRIVSET.Edit external syslog servers
- PRIVSET.Edit firmware links
- PRIVSET.Edit iSCSI Adapter policies
- PRIVSET.Edit iSCSI Boot policies
- PRIVSET.Edit iSCSI Boot policies for vNIC template
- PRIVSET.Edit iSCSI Static Target policies
- PRIVSET.Edit identity providers
- PRIVSET.Edit integrated systems
- PRIVSET.Edit notification rule or webhook
- PRIVSET.Edit server profile general properties
- PRIVSET.Edit server profile policies
- PRIVSET.Edit server profile template general properties
- PRIVSET.Edit server profile template policies
- PRIVSET.Edit server profile templates
- PRIVSET.Edit server profiles
- PRIVSET.Edit trusted IP ranges
- PRIVSET.Edit vHBA template general properties
- PRIVSET.Edit vHBA template policies
- PRIVSET.Edit vHBA templates
- PRIVSET.Edit vLAN Configuration policies for domain profile
- PRIVSET.Edit vLAN Configuration policies for domain profile template
- PRIVSET.Edit vNIC template general properties
- PRIVSET.Edit vNIC template policies
- PRIVSET.Edit vNIC templates
- PRIVSET.Edit vSAN Configuration policies for domain profile
- PRIVSET.Edit vSAN Configuration policies for domain profile template
- PRIVSET.Enable and disable API keys
- PRIVSET.Enable and disable OAuth 2.0 grant type applications
- PRIVSET.Enable and disable ports
- PRIVSET.Enable or Disable Port Channels
- PRIVSET.Enable subscription information
- PRIVSET.Enable subscriptions
- PRIVSET.Enable/disable IP access management
- PRIVSET.Enable/disable tunneled vKVM
- PRIVSET.Enter maintenance modes
- PRIVSET.Ethernet Adapter policies
- PRIVSET.Ethernet Network Control policies
- PRIVSET.Ethernet Network Group policies
- PRIVSET.Ethernet Network policies
- PRIVSET.Ethernet QoS policies
- PRIVSET.Execute Workflows
- PRIVSET.Exit maintenance modes
- PRIVSET.Explorations
- PRIVSET.Explorer
- PRIVSET.External Syslog Administrator
- PRIVSET.FC Zone policies
- PRIVSET.Fabric Interconnects
- PRIVSET.Fabric evacuation
- PRIVSET.Fibre Channel Adapter policies
- PRIVSET.Fibre Channel Network policies
- PRIVSET.Fibre Channel QoS policies
- PRIVSET.Firmware links
- PRIVSET.Firmware policies
- PRIVSET.Flow Control policies
- PRIVSET.Generate API keys
- PRIVSET.Generic
- PRIVSET.Global Read Privileges
- PRIVSET.Global System Privileges
- PRIVSET.Global Write Privileges
- PRIVSET.HCI Cluster Administrator
- PRIVSET.HCI Cluster Operator
- PRIVSET.HCI Clusters
- PRIVSET.Hosts
- PRIVSET.HyperFlex Cluster
- PRIVSET.HyperFlex Cluster Access Operator
- PRIVSET.HyperFlex Cluster Administrator
- PRIVSET.HyperFlex Cluster Advanced Security
- PRIVSET.HyperFlex Cluster Backups
- PRIVSET.HyperFlex Cluster Capacity Planning
- PRIVSET.HyperFlex Cluster Data Protection Administrator
- PRIVSET.HyperFlex Cluster Lifecycle Administrator
- PRIVSET.HyperFlex Cluster Operations
- PRIVSET.HyperFlex Cluster Operator
- PRIVSET.HyperFlex Cluster Profiles
- PRIVSET.HyperFlex Cluster Storage Administrator
- PRIVSET.HyperFlex Cluster Syslog Administrator
- PRIVSET.HyperFlex Cluster Syslog Profile Control
- PRIVSET.HyperFlex Cluster System Administrator
- PRIVSET.HyperFlex Cluster System Operator
- PRIVSET.HyperFlex Key Encryption
- PRIVSET.HyperFlex View Only
- PRIVSET.Hypervisors
- PRIVSET.IMC Access policies
- PRIVSET.IP access management
- PRIVSET.IP block mapping
- PRIVSET.IPMI over LAN policies
- PRIVSET.IQN block mapping
- PRIVSET.Import foreign configurations
- PRIVSET.Import server profiles
- PRIVSET.Install operating systems
- PRIVSET.Install updates
- PRIVSET.Integrated Systems Administrator
- PRIVSET.Integrated Systems Operator
- PRIVSET.Integrated systems
- PRIVSET.Kubernetes Administrator
- PRIVSET.Kubernetes Operator
- PRIVSET.LAN Connectivity policies
- PRIVSET.LDAP policies
- PRIVSET.Launch CLI as admin
- PRIVSET.Launch CLI as read-only
- PRIVSET.Launch Endpoint Management Interfaces
- PRIVSET.Launch IMC as admin
- PRIVSET.Launch IMC as read-only
- PRIVSET.Launch UCS Manager as admin
- PRIVSET.Launch UCS Manager as read-only
- PRIVSET.Launch VM consoles
- PRIVSET.Launch host consoles
- PRIVSET.Launch tunneled vKVM sessions
- PRIVSET.Launch vKVM
- PRIVSET.Launch vKVM sessions
- PRIVSET.Licensing
- PRIVSET.Link Aggregation policies
- PRIVSET.Link Control policies
- PRIVSET.Local User policies
- PRIVSET.Location Management
- PRIVSET.Locator LEDs
- PRIVSET.Manage API Keys
- PRIVSET.Manage Access and Permissions
- PRIVSET.Manage Auth Tokens
- PRIVSET.Manage Exports
- PRIVSET.Manage External Syslog
- PRIVSET.Manage Fabric Interconnects
- PRIVSET.Manage Functions
- PRIVSET.Manage Geo Locations
- PRIVSET.Manage HCI Clusters
- PRIVSET.Manage HyperFlex Cluster Profiles
- PRIVSET.Manage HyperFlex Clusters
- PRIVSET.Manage HyperFlex Syslog
- PRIVSET.Manage Hypervisors
- PRIVSET.Manage Identity Providers
- PRIVSET.Manage Imports
- PRIVSET.Manage Language Runtimes
- PRIVSET.Manage Nexus Config
- PRIVSET.Manage Nexus Sites
- PRIVSET.Manage Organizations
- PRIVSET.Manage Server Profiles
- PRIVSET.Manage Servers
- PRIVSET.Manage ServiceItem Instances.
- PRIVSET.Manage Sessions
- PRIVSET.Manage Storage Arrays
- PRIVSET.Manage Switch Profiles
- PRIVSET.Manage Tags
- PRIVSET.Manage Techsupport Bundles
- PRIVSET.Manage Telemetry
- PRIVSET.Manage Unified Edge
- PRIVSET.Manage Unified Edge Profiles
- PRIVSET.Manage Workflow Definitions
- PRIVSET.Manage Workload Definitions
- PRIVSET.Manage Workload Deployments
- PRIVSET.Manage alarm suppression
- PRIVSET.Manage products
- PRIVSET.Manage targets
- PRIVSET.Manage tech support bundles
- PRIVSET.Memory policies
- PRIVSET.Modify security keys
- PRIVSET.Monitor audit logs
- PRIVSET.Multicast policies
- PRIVSET.NTP policies
- PRIVSET.Network Administrator
- PRIVSET.Network Connectivity policies
- PRIVSET.Network Operator
- PRIVSET.Nexus Administrator
- PRIVSET.Nexus Analyst
- PRIVSET.Nexus Config Administrator
- PRIVSET.Nexus Observer
- PRIVSET.Notifications and webhooks
- PRIVSET.OAuth 2.0 applications
- PRIVSET.OAuth2 tokens
- PRIVSET.OS configuration files
- PRIVSET.OS image links
- PRIVSET.Operate
- PRIVSET.Operate IP pools
- PRIVSET.Operate IQN pools
- PRIVSET.Operate MAC pools
- PRIVSET.Operate Resource pools
- PRIVSET.Operate UUID pools
- PRIVSET.Operate WWNN and WWPN pools
- PRIVSET.Operate chassis profiles
- PRIVSET.Operate domain profiles
- PRIVSET.Operate physical chassis
- PRIVSET.Operate physical domains
- PRIVSET.Operate physical server
- PRIVSET.Operate pools
- PRIVSET.Operate server power
- PRIVSET.Operate server profile
- PRIVSET.Operate server storage
- PRIVSET.Operate server system
- PRIVSET.Operate server vHBAs
- PRIVSET.Operate server vNICs
- PRIVSET.Organizations
- PRIVSET.Persistent Memory policies
- PRIVSET.Port policies
- PRIVSET.Power cycle chassis slots
- PRIVSET.Power policies
- PRIVSET.Read Chassis Profiles and Chassis Profile Templates
- PRIVSET.Read Domain Profiles and Domain Profile Templates
- PRIVSET.Read Organizations
- PRIVSET.Read Server Profiles and Server Profile Templates
- PRIVSET.Read Workflows
- PRIVSET.Read all API keys in the account
- PRIVSET.Read all OAuth apps in the account
- PRIVSET.Read-Only
- PRIVSET.Read-only
- PRIVSET.Read-only Adapter Configuration policies
- PRIVSET.Read-only AuditD policies
- PRIVSET.Read-only BIOS policies
- PRIVSET.Read-only Boot Order policies
- PRIVSET.Read-only CLI policies
- PRIVSET.Read-only Certificate Management policies
- PRIVSET.Read-only Device Connector Policies
- PRIVSET.Read-only Drive Security policies
- PRIVSET.Read-only Ethernet Adapter policies
- PRIVSET.Read-only Ethernet Network Control policies
- PRIVSET.Read-only Ethernet Network Group policies
- PRIVSET.Read-only Ethernet Network policies
- PRIVSET.Read-only Ethernet QoS policies
- PRIVSET.Read-only FC Zone policies
- PRIVSET.Read-only Fabric Interconnects
- PRIVSET.Read-only Fibre Channel Adapter policies
- PRIVSET.Read-only Fibre Channel Network policies
- PRIVSET.Read-only Fibre Channel QoS policies
- PRIVSET.Read-only Firmware policies
- PRIVSET.Read-only Flow Control policies
- PRIVSET.Read-only HyperFlex cluster profiles
- PRIVSET.Read-only HyperFlex clusters
- PRIVSET.Read-only IMC Access policies
- PRIVSET.Read-only IP pools
- PRIVSET.Read-only IPMI over LAN policies
- PRIVSET.Read-only IQN pools
- PRIVSET.Read-only Kubernetes cluster profiles
- PRIVSET.Read-only LAN Connectivity policies
- PRIVSET.Read-only LDAP policies
- PRIVSET.Read-only Link Aggregation policies
- PRIVSET.Read-only Link Control policies
- PRIVSET.Read-only Local User policies
- PRIVSET.Read-only MAC pools
- PRIVSET.Read-only Memory policies
- PRIVSET.Read-only Multicast policies
- PRIVSET.Read-only NTP policies
- PRIVSET.Read-only Network Connectivity policies
- PRIVSET.Read-only Persistent Memory policies
- PRIVSET.Read-only Port policies
- PRIVSET.Read-only Power policies
- PRIVSET.Read-only SAN Connectivity policies
- PRIVSET.Read-only SD Card policies
- PRIVSET.Read-only SMTP policies
- PRIVSET.Read-only SNMP policies
- PRIVSET.Read-only SOL policies
- PRIVSET.Read-only SSH policies
- PRIVSET.Read-only SSL Certificates
- PRIVSET.Read-only Scrub policies
- PRIVSET.Read-only Storage policies
- PRIVSET.Read-only Switch Control policies
- PRIVSET.Read-only Syslog policies
- PRIVSET.Read-only System QoS policies
- PRIVSET.Read-only Thermal policies
- PRIVSET.Read-only UCS chassis profile templates
- PRIVSET.Read-only UCS chassis profiles
- PRIVSET.Read-only UCS domain profile templates
- PRIVSET.Read-only UCS domain profiles
- PRIVSET.Read-only UCS server profile templates
- PRIVSET.Read-only UCS server profiles
- PRIVSET.Read-only UUID pools
- PRIVSET.Read-only VLAN policies
- PRIVSET.Read-only VMs
- PRIVSET.Read-only VSAN policies
- PRIVSET.Read-only Virtual KVM policies
- PRIVSET.Read-only WWNN and WWPN pools
- PRIVSET.Read-only all advisories
- PRIVSET.Read-only all alarms
- PRIVSET.Read-only all audit logs
- PRIVSET.Read-only all compute policies
- PRIVSET.Read-only all management policies
- PRIVSET.Read-only all network policies
- PRIVSET.Read-only all policies
- PRIVSET.Read-only all storage policies
- PRIVSET.Read-only chassis
- PRIVSET.Read-only hosts
- PRIVSET.Read-only iSCSI Adapter policies
- PRIVSET.Read-only iSCSI Boot policies
- PRIVSET.Read-only iSCSI Static Target policies
- PRIVSET.Read-only integrated systems
- PRIVSET.Read-only licensing
- PRIVSET.Read-only metrics explorations
- PRIVSET.Read-only networking
- PRIVSET.Read-only pools
- PRIVSET.Read-only profiles
- PRIVSET.Read-only resource pools
- PRIVSET.Read-only servers
- PRIVSET.Read-only software repository
- PRIVSET.Read-only storage
- PRIVSET.Read-only targets
- PRIVSET.Read-only tech support bundles
- PRIVSET.Read-only templates
- PRIVSET.Read-only vHBA templates
- PRIVSET.Read-only vMedia policies
- PRIVSET.Read-only vNIC templates
- PRIVSET.Reboot Fabric Interconnect
- PRIVSET.Reboot management controllers
- PRIVSET.Recommission Fabric Extender (FEX)
- PRIVSET.Recommission chassis
- PRIVSET.Recommission servers
- PRIVSET.Rediscover Fabric Extender (FEX)
- PRIVSET.Rediscover chassis
- PRIVSET.Rediscover servers
- PRIVSET.Regenerate domain names
- PRIVSET.Register licenses
- PRIVSET.Reject Publish Requests
- PRIVSET.Remove Fabric Extender (FEX)
- PRIVSET.Remove chassis
- PRIVSET.Remove servers
- PRIVSET.Renew licenses
- PRIVSET.Replace Fabric Interconnect
- PRIVSET.Reserve licenses
- PRIVSET.Reset CMOS
- PRIVSET.Reset IOMs and IFMs
- PRIVSET.Reset VMs
- PRIVSET.Reset memory errors
- PRIVSET.Reset peer IOMs and IFMs
- PRIVSET.Reset vKVM
- PRIVSET.Restart VMs
- PRIVSET.Return licenses
- PRIVSET.Run Workflows
- PRIVSET.Run interoperability checks
- PRIVSET.SAN Administrator
- PRIVSET.SAN Connectivity policies
- PRIVSET.SAN Operator
- PRIVSET.SCU links
- PRIVSET.SD Card policies
- PRIVSET.SD card operations
- PRIVSET.SMTP policies
- PRIVSET.SNMP policies
- PRIVSET.SSH policies
- PRIVSET.SSL Certificates
- PRIVSET.Save and clone explorations
- PRIVSET.Scrub policies
- PRIVSET.Security and privacy
- PRIVSET.Serial Over LAN policies
- PRIVSET.Server Administrator
- PRIVSET.Server Profiles
- PRIVSET.Server delete virtual drives
- PRIVSET.Server enable and disable vHBAs
- PRIVSET.Server enable and disable vNICs
- PRIVSET.Server hard reset
- PRIVSET.Server power cycle
- PRIVSET.Server power off
- PRIVSET.Server power on
- PRIVSET.Server reset vHBAs
- PRIVSET.Server reset vNICs
- PRIVSET.Server secure erase drives
- PRIVSET.Server set drive states
- PRIVSET.Server shutdown OS
- PRIVSET.Servers
- PRIVSET.Service Designer
- PRIVSET.Service Operator
- PRIVSET.Sessions
- PRIVSET.Set Fabric Interconnect user labels
- PRIVSET.Set IMC certificates
- PRIVSET.Set KMIP client certificates
- PRIVSET.Set and unset IP pool tags
- PRIVSET.Set and unset chassis profile tags
- PRIVSET.Set and unset domain profile tags
- PRIVSET.Set and unset server profile tags
- PRIVSET.Set chassis profile user labels
- PRIVSET.Set chassis user labels
- PRIVSET.Set domain profile user labels
- PRIVSET.Set or Unset Fabric Interconnect Tag
- PRIVSET.Set or Unset IQN Pool Tags
- PRIVSET.Set or Unset MAC Pool Tags
- PRIVSET.Set or Unset Resource Pool Tags
- PRIVSET.Set or Unset Server Tag
- PRIVSET.Set or Unset UUID Pool Tags
- PRIVSET.Set or Unset chassis Tag
- PRIVSET.Set or unset WWNN or WWPN pool tags
- PRIVSET.Set server asset tags
- PRIVSET.Set server license tiers
- PRIVSET.Set server profile user labels
- PRIVSET.Set server user labels
- PRIVSET.Single sign-on
- PRIVSET.Soft stop VMs
- PRIVSET.Software repository
- PRIVSET.Start and resume VMs
- PRIVSET.Stop VMs
- PRIVSET.Storage Administrator
- PRIVSET.Storage Arrays
- PRIVSET.Storage policies
- PRIVSET.Support
- PRIVSET.Support Services
- PRIVSET.Support chassis
- PRIVSET.Support domains
- PRIVSET.Support servers
- PRIVSET.Suspend VMs
- PRIVSET.Sustainability Metrics Viewer
- PRIVSET.Switch Control policies
- PRIVSET.Switch Profiles
- PRIVSET.Switch to Self Signed CSR
- PRIVSET.Sync Smart Licensing
- PRIVSET.Syslog policies
- PRIVSET.System Administration
- PRIVSET.System QoS policies
- PRIVSET.Tag Management
- PRIVSET.Tech support bundles
- PRIVSET.Telemetry
- PRIVSET.Terminate VMs
- PRIVSET.Terminate sessions
- PRIVSET.Thermal policies
- PRIVSET.Traffic mirroring  SPAN session
- PRIVSET.Trusted certificates
- PRIVSET.Turn Fabric Extender locator LED on and off
- PRIVSET.Turn chassis locator LEDs on and off
- PRIVSET.Turn server locator LEDs on and off
- PRIVSET.UCS Domain Administrator
- PRIVSET.Unassign chassis profiles
- PRIVSET.Unassign domain profiles
- PRIVSET.Unassign server profiles
- PRIVSET.Unclaim device connector
- PRIVSET.Unclaim targets
- PRIVSET.Unified Edge
- PRIVSET.Unified Edge Administrator
- PRIVSET.Unified Edge Profiles
- PRIVSET.Unlock and lock front panels
- PRIVSET.Unlock disks
- PRIVSET.Update reserved licenses
- PRIVSET.Upgrade chassis firmware
- PRIVSET.Upgrade domain firmware
- PRIVSET.Upgrade server firmware
- PRIVSET.User Access Administrator
- PRIVSET.VLAN policies
- PRIVSET.VSAN policies
- PRIVSET.Verify domain names
- PRIVSET.View Access and Permissions
- PRIVSET.View Approval Requests
- PRIVSET.View Audit Logs
- PRIVSET.View Datacenters
- PRIVSET.View Devices
- PRIVSET.View Exports
- PRIVSET.View Fabric Interconnects
- PRIVSET.View Functions
- PRIVSET.View HCI Clusters
- PRIVSET.View HyperFlex Cluster Profiles
- PRIVSET.View HyperFlex Clusters
- PRIVSET.View Hypervisors
- PRIVSET.View Imports
- PRIVSET.View Language Runtimes
- PRIVSET.View Licensing Status
- PRIVSET.View Network Switches
- PRIVSET.View Nexus Config
- PRIVSET.View Nexus Reports
- PRIVSET.View Nexus Sites
- PRIVSET.View Organizations
- PRIVSET.View SAN Switches
- PRIVSET.View Server Profiles
- PRIVSET.View Servers
- PRIVSET.View Storage Arrays
- PRIVSET.View Switch Profiles
- PRIVSET.View Telemetry
- PRIVSET.View Unified Edge
- PRIVSET.View Unified Edge Profiles
- PRIVSET.View Workflow Definitions
- PRIVSET.View Workflow Executions
- PRIVSET.View Workload Definitions
- PRIVSET.View Workload Deployments
- PRIVSET.View clusters
- PRIVSET.View datastore clusters
- PRIVSET.View datastores
- PRIVSET.View sessions
- PRIVSET.View virtual machine templates
- PRIVSET.Virtual KVM policies
- PRIVSET.Virtual Media policies
- PRIVSET.Virtual appliance licensing
- PRIVSET.Virtual machines
- PRIVSET.Virtualization Administrator
- PRIVSET.Virtualization hosts
- PRIVSET.Withdraw Approvals
- PRIVSET.Workflow Designer
- PRIVSET.Workload Administrator
- PRIVSET.Workload Designer
- PRIVSET.Workload Operator
- PRIVSET.Workload Optimizer Administrator
- PRIVSET.Workload Optimizer Advisor
- PRIVSET.Workload Optimizer Automator
- PRIVSET.Workload Optimizer Deployer
- PRIVSET.Workload Optimizer Observer
- PRIVSET.iSCSI Adapter policies
- PRIVSET.iSCSI Boot policies
- PRIVSET.iSCSI Static Target policies
- PRIVSET.vKVM Only
- READ.aaa.AuditRecord
- READ.aaa.RetentionConfig
- READ.aaa.RetentionPolicy
- READ.access.IpAddress
- READ.access.Policy
- READ.access.PolicyInventory
- READ.adapter.ConfigPolicy
- READ.adapter.ExtEthInterface
- READ.adapter.HostEthInterface
- READ.adapter.HostFcInterface
- READ.adapter.HostIscsiInterface
- READ.adapter.Unit
- READ.adapter.UnitExpander
- READ.apic.AciPod
- READ.apic.Application
- READ.apic.ApplicationEndpointGroup
- READ.apic.BridgeDomain
- READ.apic.ExternalRoutedLayerThreeDomain
- READ.apic.FabricLeafNode
- READ.apic.FabricLeafNodeInterface
- READ.apic.Out
- READ.apic.Subnet
- READ.apic.Tenant
- READ.apic.VpcGroup
- READ.apic.Vrfs
- READ.apiproxy.AllowList
- READ.appliance.AppOpStatus
- READ.appliance.AppStatus
- READ.appliance.AutoRmaPolicy
- READ.appliance.Backup
- READ.appliance.BackupDownload
- READ.appliance.BackupMonitor
- READ.appliance.BackupPolicy
- READ.appliance.BackupRotateData
- READ.appliance.CertificateSetting
- READ.appliance.ClusterInfo
- READ.appliance.ClusterInstall
- READ.appliance.ClusterReplaceNode
- READ.appliance.ClusterWorkerNode
- READ.appliance.CpuUtilization
- READ.appliance.DataExportPolicy
- READ.appliance.DeviceCertificate
- READ.appliance.DeviceClaim
- READ.appliance.DeviceClusterInstall
- READ.appliance.DeviceState
- READ.appliance.DeviceUpgradePolicy
- READ.appliance.DiagSetting
- READ.appliance.ExternalSyslogSetting
- READ.appliance.FileGateway
- READ.appliance.FileSystemOpStatus
- READ.appliance.FileSystemOpSummary
- READ.appliance.FileSystemStatus
- READ.appliance.FileSystemTelemetry
- READ.appliance.FqdnUpdate
- READ.appliance.GroupOpStatus
- READ.appliance.GroupStatus
- READ.appliance.ImageBundle
- READ.appliance.MemoryUtilization
- READ.appliance.MetaManifest
- READ.appliance.MetricsConfig
- READ.appliance.MetricsIngestionUtilization
- READ.appliance.NetworkLinkStatus
- READ.appliance.NodeInfo
- READ.appliance.NodeIopsMetric
- READ.appliance.NodeOpStatus
- READ.appliance.NodeStatus
- READ.appliance.NodeTelemetry
- READ.appliance.ReleaseNote
- READ.appliance.RemoteFileImport
- READ.appliance.Restore
- READ.appliance.SetupInfo
- READ.appliance.SystemInfo
- READ.appliance.SystemOpStatus
- READ.appliance.SystemStatus
- READ.appliance.Upgrade
- READ.appliance.UpgradePolicy
- READ.appliance.UpgradeTracker
- READ.asset.ClaimToken
- READ.asset.ClusterMember
- READ.asset.Deployment
- READ.asset.DeploymentDevice
- READ.asset.DeviceConfiguration
- READ.asset.DeviceConnectorManager
- READ.asset.DeviceContractInformation
- READ.asset.DeviceRegistration
- READ.asset.GeoLocation
- READ.asset.Subscription
- READ.asset.SubscriptionAccount
- READ.asset.SubscriptionDeviceContractInformation
- READ.asset.Target
- READ.auditd.Policy
- READ.bios.BootDevice
- READ.bios.BootMode
- READ.bios.Policy
- READ.bios.SystemBootOrder
- READ.bios.TokenSettings
- READ.bios.Unit
- READ.bios.VfSelectMemoryRasConfiguration
- READ.boot.CddDevice
- READ.boot.DeviceBootMode
- READ.boot.DeviceBootSecurity
- READ.boot.HddDevice
- READ.boot.IscsiDevice
- READ.boot.NvmeDevice
- READ.boot.PchStorageDevice
- READ.boot.PrecisionPolicy
- READ.boot.PxeDevice
- READ.boot.SanDevice
- READ.boot.SdDevice
- READ.boot.UefiShellDevice
- READ.boot.UsbDevice
- READ.boot.VmediaDevice
- READ.bulk.Export
- READ.bulk.ExportedItem
- READ.bulk.MoCloner
- READ.bulk.MoDeepCloner
- READ.bulk.MoMerger
- READ.bulk.Request
- READ.bulk.Result
- READ.bulk.SubRequestObj
- READ.capability.ActionsMetaData
- READ.capability.AdapterDeprecatedDef
- READ.capability.AdapterFirmwareRequirement
- READ.capability.AdapterUnitDescriptor
- READ.capability.AdapterUpdateConstraintMeta
- READ.capability.AdapterUpgradeSupportMeta
- READ.capability.BiosTokens
- READ.capability.Catalog
- READ.capability.ChassisDescriptor
- READ.capability.ChassisManufacturingDef
- READ.capability.ChassisUpgradeSupportMeta
- READ.capability.CimcFirmwareDescriptor
- READ.capability.CpuEndpointDescriptor
- READ.capability.DimmsEndpointDescriptor
- READ.capability.DomainPolicyRequirement
- READ.capability.DrivesEndpointDescriptor
- READ.capability.EquipmentPhysicalDef
- READ.capability.EquipmentSlotArray
- READ.capability.FanModuleDescriptor
- READ.capability.FanModuleManufacturingDef
- READ.capability.FexCapabilityDef
- READ.capability.FexDescriptor
- READ.capability.FexManufacturingDef
- READ.capability.FexSupportMeta
- READ.capability.GpuEndpointDescriptor
- READ.capability.HsuIsoFileSupportMeta
- READ.capability.IoCardCapabilityDef
- READ.capability.IoCardDescriptor
- READ.capability.IoCardManufacturingDef
- READ.capability.IomUpgradeSupportMeta
- READ.capability.NetworkEquipmentPowerDef
- READ.capability.PolicyConstants
- READ.capability.PortGroupAggregationDef
- READ.capability.ProcessorUnitUpdateConstraintMeta
- READ.capability.PsuDescriptor
- READ.capability.PsuManufacturingDef
- READ.capability.ServerActionsMeta
- READ.capability.ServerDescriptor
- READ.capability.ServerModelsCapabilityDef
- READ.capability.ServerPcieConnectivityCatalog
- READ.capability.ServerSchemaDescriptor
- READ.capability.ServerTopologyMap
- READ.capability.ServerUpgradeSupportMeta
- READ.capability.SiocModuleCapabilityDef
- READ.capability.SiocModuleDescriptor
- READ.capability.SiocModuleManufacturingDef
- READ.capability.StandardRedfishSupportMeta
- READ.capability.StorageControllerUpdateConstraintMeta
- READ.capability.StorageControllersMetaData
- READ.capability.SwitchCapability
- READ.capability.SwitchDescriptor
- READ.capability.SwitchEquipmentInfo
- READ.capability.SwitchManufacturingDef
- READ.capability.SwitchUpgradeSupportMeta
- READ.capability.TemplateCatalog
- READ.capability.TimeZoneMetaData
- READ.capability.UpdateOrderMeta
- READ.capability.VicDescriptor
- READ.catalystsdwan.ConfigGroup
- READ.catalystsdwan.Interface
- READ.catalystsdwan.PhysicalPort
- READ.catalystsdwan.PolicyGroup
- READ.catalystsdwan.PortChannel
- READ.catalystsdwan.VedgeDevice
- READ.catalystsdwan.Vlan
- READ.catalystsdwan.WanEdgeDevice
- READ.certificatemanagement.Policy
- READ.certificatemanagement.PolicyInventory
- READ.chassis.ConfigChangeDetail
- READ.chassis.ConfigImport
- READ.chassis.ConfigResult
- READ.chassis.ConfigResultEntry
- READ.chassis.IomProfile
- READ.chassis.Profile
- READ.chassis.ProfileTemplate
- READ.cli.CliPolicy
- READ.cloud.TfcAgentpool
- READ.cloud.TfcOrganization
- READ.cloud.TfcWorkspace
- READ.comm.HttpProxyPolicy
- READ.comm.TagDefinition
- READ.compute.Blade
- READ.compute.BladeIdentity
- READ.compute.Board
- READ.compute.DownloadStatus
- READ.compute.HostUtilityOperation
- READ.compute.Mapping
- READ.compute.PcieConnectivityPolicy
- READ.compute.PcieConnectivityPolicyInventory
- READ.compute.Personality
- READ.compute.PhysicalSummary
- READ.compute.RackUnit
- READ.compute.RackUnitIdentity
- READ.compute.ScrubPolicy
- READ.compute.ServerIdPool
- READ.compute.ServerPowerParameters
- READ.compute.ServerPowerPolicy
- READ.compute.ServerSetting
- READ.compute.Vmedia
- READ.cond.Alarm
- READ.cond.AlarmAggregation
- READ.cond.AlarmClassification
- READ.cond.AlarmDefinition
- READ.cond.AlarmRule
- READ.cond.AlarmSuppression
- READ.cond.CustomHclBaseline
- READ.cond.CustomHclStatus
- READ.cond.HclStatus
- READ.cond.HclStatusDetail
- READ.cond.HclStatusJob
- READ.cond.ThresholdDefinition
- READ.connectorpack.ConnectorPackUpgrade
- READ.connectorpack.UpgradeImpact
- READ.console.ConsoleConfig
- READ.convergedinfra.AdapterComplianceDetails
- READ.convergedinfra.Pod
- READ.convergedinfra.PodComplianceInfo
- READ.convergedinfra.ServerComplianceDetails
- READ.convergedinfra.StorageComplianceDetails
- READ.convergedinfra.SwitchComplianceDetails
- READ.coremanagement.CoreFile
- READ.coremanagement.Download
- READ.crd.CustomResource
- READ.deviceconnector.Policy
- READ.dnac.Device
- READ.dnac.DeviceInterface
- READ.dnac.ExternalBorderNode
- READ.dnac.ExternalBorderNodeInterface
- READ.dnac.FabricSite
- READ.dnac.Site
- READ.dnac.SiteIpPool
- READ.dnac.Template
- READ.dnac.Transit
- READ.dnac.VirtualNetworkFabricSite
- READ.equipment.Chassis
- READ.equipment.ChassisController
- READ.equipment.ChassisIdPool
- READ.equipment.ChassisIdentity
- READ.equipment.ChassisOperation
- READ.equipment.DeviceSummary
- READ.equipment.EnclosureElement
- READ.equipment.EndPointLog
- READ.equipment.ExpanderModule
- READ.equipment.ExpanderModuleIdentity
- READ.equipment.ExpanderModuleOperation
- READ.equipment.Fan
- READ.equipment.FanControl
- READ.equipment.FanModule
- READ.equipment.Fex
- READ.equipment.FexIdentity
- READ.equipment.FexOperation
- READ.equipment.Fru
- READ.equipment.HybridDriveSlot
- READ.equipment.Interconnect
- READ.equipment.IoCard
- READ.equipment.IoCardOperation
- READ.equipment.IoExpander
- READ.equipment.LocatorLed
- READ.equipment.LogDownload
- READ.equipment.Psu
- READ.equipment.PsuControl
- READ.equipment.RackEnclosure
- READ.equipment.RackEnclosureSlot
- READ.equipment.Riser
- READ.equipment.Sensor
- READ.equipment.SharedAdapterUnit
- READ.equipment.SharedGraphicsCard
- READ.equipment.SharedIoModule
- READ.equipment.SwitchCard
- READ.equipment.SwitchOperation
- READ.equipment.SystemIoController
- READ.equipment.Tpm
- READ.equipment.Transceiver
- READ.ether.HostPort
- READ.ether.InterSwitchPort
- READ.ether.LanPort
- READ.ether.NetworkPort
- READ.ether.PhysicalPort
- READ.ether.PortChannel
- READ.externalsite.Authorization
- READ.fabric.AppliancePcRole
- READ.fabric.ApplianceRole
- READ.fabric.ConfigChangeDetail
- READ.fabric.ConfigResult
- READ.fabric.ConfigResultEntry
- READ.fabric.ElementIdentity
- READ.fabric.EthNetworkControlPolicy
- READ.fabric.EthNetworkControlPolicyInventory
- READ.fabric.EthNetworkGroupPolicy
- READ.fabric.EthNetworkGroupPolicyInventory
- READ.fabric.EthNetworkPolicy
- READ.fabric.FcNetworkPolicy
- READ.fabric.FcStorageRole
- READ.fabric.FcUplinkPcRole
- READ.fabric.FcUplinkRole
- READ.fabric.FcZonePolicy
- READ.fabric.FcoeUplinkPcRole
- READ.fabric.FcoeUplinkRole
- READ.fabric.FlowControlPolicy
- READ.fabric.LanPinGroup
- READ.fabric.LinkAggregationPolicy
- READ.fabric.LinkControlPolicy
- READ.fabric.MacSecPolicy
- READ.fabric.MulticastPolicy
- READ.fabric.NetFlowExporter
- READ.fabric.NetFlowMonitor
- READ.fabric.NetFlowPolicy
- READ.fabric.NetFlowRecord
- READ.fabric.PcMember
- READ.fabric.PcOperation
- READ.fabric.PortMode
- READ.fabric.PortOperation
- READ.fabric.PortPolicy
- READ.fabric.SanPinGroup
- READ.fabric.SecureRouterRole
- READ.fabric.ServerRole
- READ.fabric.SpanDestEthPort
- READ.fabric.SpanSession
- READ.fabric.SpanSourceEthPort
- READ.fabric.SpanSourceEthPortChannel
- READ.fabric.SpanSourceVlan
- READ.fabric.SpanSourceVnicEthIf
- READ.fabric.SwitchClusterProfile
- READ.fabric.SwitchClusterProfileTemplate
- READ.fabric.SwitchControlPolicy
- READ.fabric.SwitchProfile
- READ.fabric.SwitchProfileTemplate
- READ.fabric.SystemQosPolicy
- READ.fabric.UplinkPcRole
- READ.fabric.UplinkRole
- READ.fabric.Vlan
- READ.fabric.VlanInventory
- READ.fabric.VlanSet
- READ.fabric.Vsan
- READ.fabric.VsanInventory
- READ.fault.Instance
- READ.fc.Neighbor
- READ.fc.PhysicalPort
- READ.fc.PortChannel
- READ.fcpool.FcBlock
- READ.fcpool.Lease
- READ.fcpool.Pool
- READ.fcpool.PoolMember
- READ.fcpool.Reservation
- READ.fcpool.Universe
- READ.firmware.BiosDescriptor
- READ.firmware.BoardControllerDescriptor
- READ.firmware.ChassisUpgrade
- READ.firmware.CimcDescriptor
- READ.firmware.DimmDescriptor
- READ.firmware.Distributable
- READ.firmware.DistributableMeta
- READ.firmware.DriveDescriptor
- READ.firmware.DriverDistributable
- READ.firmware.Eula
- READ.firmware.FirmwareSummary
- READ.firmware.GpuDescriptor
- READ.firmware.HbaDescriptor
- READ.firmware.IomDescriptor
- READ.firmware.MswitchDescriptor
- READ.firmware.NxosDescriptor
- READ.firmware.PciNodeUpgrade
- READ.firmware.PcieDescriptor
- READ.firmware.Policy
- READ.firmware.PsuDescriptor
- READ.firmware.PsxDescriptor
- READ.firmware.RunningFirmware
- READ.firmware.SasExpanderDescriptor
- READ.firmware.SecureRouterUpgrade
- READ.firmware.ServerConfigurationUtilityDistributable
- READ.firmware.StorageControllerDescriptor
- READ.firmware.SwitchUpgrade
- READ.firmware.UnsupportedVersionUpgrade
- READ.firmware.Upgrade
- READ.firmware.UpgradeImpactStatus
- READ.firmware.UpgradeStatus
- READ.fmc.Device
- READ.fmc.DeviceHaPair
- READ.fmc.Domain
- READ.fmc.PhysicalInterface
- READ.forecast.Catalog
- READ.forecast.Definition
- READ.forecast.Instance
- READ.graphics.Card
- READ.graphics.Controller
- READ.hci.AhvVm
- READ.hci.AhvVmDisk
- READ.hci.AhvVmGpu
- READ.hci.AhvVmNic
- READ.hci.Alarm
- READ.hci.Cluster
- READ.hci.ClusterOperation
- READ.hci.Compliance
- READ.hci.Disk
- READ.hci.DomainManager
- READ.hci.Entitlement
- READ.hci.EsxiVm
- READ.hci.EsxiVmDisk
- READ.hci.EsxiVmNic
- READ.hci.ExternalStorage
- READ.hci.Gpu
- READ.hci.License
- READ.hci.NccCheckPolicy
- READ.hci.Node
- READ.hci.PhysicalGpu
- READ.hci.StorageContainer
- READ.hci.Violation
- READ.hci.VirtualGpu
- READ.hcl.DataImportLog
- READ.hcl.DriverImage
- READ.hcl.ExemptedCatalog
- READ.hcl.HwCatalogInfo
- READ.hcl.HyperflexSoftwareCompatibilityInfo
- READ.hcl.OperatingSystem
- READ.hcl.OperatingSystemVendor
- READ.hcl.ServerCatalog
- READ.hcl.ServerHwCatalogInfo
- READ.hyperflex.Alarm
- READ.hyperflex.AppCatalog
- READ.hyperflex.AutoSupportPolicy
- READ.hyperflex.BackupCluster
- READ.hyperflex.CapabilityInfo
- READ.hyperflex.Cluster
- READ.hyperflex.ClusterBackupPolicy
- READ.hyperflex.ClusterBackupPolicyDeployment
- READ.hyperflex.ClusterBackupPolicyInventory
- READ.hyperflex.ClusterHealthCheckExecutionSnapshot
- READ.hyperflex.ClusterNetworkPolicy
- READ.hyperflex.ClusterProfile
- READ.hyperflex.ClusterReplicationNetworkPolicy
- READ.hyperflex.ClusterReplicationNetworkPolicyDeployment
- READ.hyperflex.ClusterStoragePolicy
- READ.hyperflex.ConfigResult
- READ.hyperflex.ConfigResultEntry
- READ.hyperflex.DataProtectionPeer
- READ.hyperflex.DatastoreStatistic
- READ.hyperflex.DevicePackageDownloadState
- READ.hyperflex.Drive
- READ.hyperflex.Encryption
- READ.hyperflex.ExtFcStoragePolicy
- READ.hyperflex.ExtIscsiStoragePolicy
- READ.hyperflex.FeatureLimitExternal
- READ.hyperflex.FeatureLimitInternal
- READ.hyperflex.Health
- READ.hyperflex.HealthCheckDefinition
- READ.hyperflex.HealthCheckExecution
- READ.hyperflex.HealthCheckExecutionSnapshot
- READ.hyperflex.HealthCheckPackageChecksum
- READ.hyperflex.HealthCheckSchedulePolicy
- READ.hyperflex.HwCatalog
- READ.hyperflex.HxdpVersion
- READ.hyperflex.HypervisorHost
- READ.hyperflex.HypervisorVirtualMachine
- READ.hyperflex.InitiatorGroup
- READ.hyperflex.IscsiNetwork
- READ.hyperflex.KeyEncryptionKey
- READ.hyperflex.License
- READ.hyperflex.LocalCredentialPolicy
- READ.hyperflex.Lun
- READ.hyperflex.Node
- READ.hyperflex.NodeConfigPolicy
- READ.hyperflex.NodeProfile
- READ.hyperflex.ProtectedCluster
- READ.hyperflex.ProxySettingPolicy
- READ.hyperflex.ReduceReSync
- READ.hyperflex.ServerFirmwareVersion
- READ.hyperflex.ServerFirmwareVersionEntry
- READ.hyperflex.ServerModel
- READ.hyperflex.ServiceAuthToken
- READ.hyperflex.SoftwareDistributionComponent
- READ.hyperflex.SoftwareDistributionEntry
- READ.hyperflex.SoftwareDistributionVersion
- READ.hyperflex.SoftwareVersionPolicy
- READ.hyperflex.StartReduceReSync
- READ.hyperflex.StorageContainer
- READ.hyperflex.SysConfigPolicy
- READ.hyperflex.Target
- READ.hyperflex.UcsmConfigPolicy
- READ.hyperflex.VcenterConfigPolicy
- READ.hyperflex.VmBackupInfo
- READ.hyperflex.VmImportOperation
- READ.hyperflex.VmRestoreOperation
- READ.hyperflex.VmSnapshotInfo
- READ.hyperflex.Volume
- READ.hyperflex.WitnessConfiguration
- READ.iaas.ConnectorPack
- READ.iaas.CustomTaskInfo
- READ.iaas.DeviceStatus
- READ.iaas.DiagnosticMessages
- READ.iaas.LicenseInfo
- READ.iaas.MostRunTasks
- READ.iaas.ServiceRequest
- READ.iaas.SystemTaskInfo
- READ.iaas.UcsdInfo
- READ.iaas.UcsdManagedInfra
- READ.iaas.UcsdMessages
- READ.iam.Account
- READ.iam.AccountExperience
- READ.iam.ApiKey
- READ.iam.AppRegistration
- READ.iam.BannerMessage
- READ.iam.Certificate
- READ.iam.CertificateRequest
- READ.iam.CuiIntegration
- READ.iam.DefaultAuthentication
- READ.iam.DomainGroup
- READ.iam.DomainNameInfo
- READ.iam.EndPointPrivilege
- READ.iam.EndPointRole
- READ.iam.EndPointUser
- READ.iam.EndPointUserInventory
- READ.iam.EndPointUserPolicy
- READ.iam.EndPointUserPolicyInventory
- READ.iam.EndPointUserRole
- READ.iam.EndPointUserRoleInventory
- READ.iam.GuestAccessSettings
- READ.iam.Idp
- READ.iam.IdpReference
- READ.iam.IpAccessManagement
- READ.iam.IpAddress
- READ.iam.LdapConfigParams
- READ.iam.LdapGroup
- READ.iam.LdapGroupInventory
- READ.iam.LdapMeta
- READ.iam.LdapPolicy
- READ.iam.LdapPolicyInventory
- READ.iam.LdapProvider
- READ.iam.LdapProviderInventory
- READ.iam.LocalUserPassword
- READ.iam.LocalUserPasswordPolicy
- READ.iam.OAuthToken
- READ.iam.PasswordHistorySettingCollection
- READ.iam.Permission
- READ.iam.PrivateKeySpec
- READ.iam.Privilege
- READ.iam.PrivilegeSet
- READ.iam.PrivilegeSetMetaInfo
- READ.iam.Qualifier
- READ.iam.ResourceLimits
- READ.iam.ResourcePermission
- READ.iam.ResourceRoles
- READ.iam.Role
- READ.iam.SecurityHolder
- READ.iam.ServiceProvider
- READ.iam.Session
- READ.iam.SessionLimits
- READ.iam.SharingRule
- READ.iam.System
- READ.iam.TestIdpConfiguration
- READ.iam.TrustPoint
- READ.iam.User
- READ.iam.UserGroup
- READ.iam.UserPreference
- READ.iam.UserQualifier
- READ.iam.UserSetting
- READ.inventory.DeviceInfo
- READ.inventory.DnMoBinding
- READ.inventory.GenericInventory
- READ.inventory.GenericInventoryHolder
- READ.ipmioverlan.Policy
- READ.ipmioverlan.PolicyInventory
- READ.ippool.BlockLease
- READ.ippool.IpLease
- READ.ippool.Pool
- READ.ippool.PoolMember
- READ.ippool.Reservation
- READ.ippool.ShadowBlock
- READ.ippool.ShadowPool
- READ.ippool.Universe
- READ.iqnpool.Block
- READ.iqnpool.Lease
- READ.iqnpool.Pool
- READ.iqnpool.PoolMember
- READ.iqnpool.Reservation
- READ.iqnpool.Universe
- READ.iwotenant.MaintenanceNotification
- READ.iwotenant.Migrate
- READ.iwotenant.TenantCustomization
- READ.iwotenant.TenantStatus
- READ.kvm.Policy
- READ.kvm.PolicyInventory
- READ.kvm.Session
- READ.kvm.Tunnel
- READ.kvm.TunneledKvmPolicy
- READ.license.AccountLicenseData
- READ.license.CustomerOp
- READ.license.ErpCustomerOp
- READ.license.ErpLicenseCount
- READ.license.IksCustomerOp
- READ.license.IksLicenseCount
- READ.license.IncCustomerOp
- READ.license.IncLicenseCount
- READ.license.IwoCustomerOp
- READ.license.IwoLicenseCount
- READ.license.LicenseInfo
- READ.license.LicenseInfoView
- READ.license.LicenseRegistrationStatus
- READ.license.LicenseReservationOp
- READ.license.SmartlicenseToken
- READ.ls.ServiceProfile
- READ.macpool.IdBlock
- READ.macpool.Lease
- READ.macpool.Pool
- READ.macpool.PoolMember
- READ.macpool.Reservation
- READ.macpool.Universe
- READ.management.Controller
- READ.management.Entity
- READ.management.Interface
- READ.memory.Array
- READ.memory.PersistentMemoryConfigResult
- READ.memory.PersistentMemoryConfiguration
- READ.memory.PersistentMemoryNamespace
- READ.memory.PersistentMemoryNamespaceConfigResult
- READ.memory.PersistentMemoryPolicy
- READ.memory.PersistentMemoryRegion
- READ.memory.PersistentMemoryUnit
- READ.memory.Policy
- READ.memory.PolicyInventory
- READ.memory.Unit
- READ.meraki.Device
- READ.meraki.Network
- READ.meraki.Organization
- READ.meraki.PortProfile
- READ.meraki.Tag
- READ.meta.Definition
- READ.metrics.Configuration
- READ.metrics.MetricsExploration
- READ.metrics.ResourceConfiguration
- READ.mgmt.BackupCategory
- READ.mgmt.ConfigBackupFile
- READ.mgmt.ConfigBackupInstance
- READ.mgmt.ConfigBackupOperation
- READ.mgmt.ConfigCategorySummary
- READ.mgmt.ConfigOperationSetting
- READ.mgmt.ConfigRestoreCategorySummary
- READ.mgmt.ConfigRestoreOperation
- READ.mgmt.ObjectBackupMeta
- READ.mgmt.OrgBackupOperation
- READ.mgmt.OrgRestoreOperation
- READ.monitoring.HealthStatus
- READ.network.DiscoveredNeighbor
- READ.network.Dns
- READ.network.Element
- READ.network.ElementSummary
- READ.network.FcZoneInfo
- READ.network.FeatureControl
- READ.network.InterfaceList
- READ.network.LicenseFile
- READ.network.SecureRouter
- READ.network.SecureRouterSetting
- READ.network.SupervisorCard
- READ.network.TelemetryCheck
- READ.network.Vethernet
- READ.network.Vfc
- READ.network.VlanPortInfo
- READ.network.VpcDomain
- READ.network.VpcMember
- READ.network.VpcPeer
- READ.network.Vrf
- READ.networkconfig.Policy
- READ.networkconfig.PolicyInventory
- READ.niaapi.ApicCcoPost
- READ.niaapi.ApicFieldNotice
- READ.niaapi.ApicHweol
- READ.niaapi.ApicLatestMaintainedRelease
- READ.niaapi.ApicReleaseRecommend
- READ.niaapi.ApicSweol
- READ.niaapi.DcnmCcoPost
- READ.niaapi.DcnmFieldNotice
- READ.niaapi.DcnmHweol
- READ.niaapi.DcnmLatestMaintainedRelease
- READ.niaapi.DcnmReleaseRecommend
- READ.niaapi.DcnmSweol
- READ.niaapi.FileDownloader
- READ.niaapi.NdEncryptedFileDownload
- READ.niaapi.NdMetadata
- READ.niaapi.NdMetadataFileDownloader
- READ.niaapi.NdMetadataSoftwareDownload
- READ.niaapi.NiaMetadata
- READ.niaapi.NibFileDownloader
- READ.niaapi.NibMetadata
- READ.niaapi.PuvScriptDownloader
- READ.niaapi.SnValidatorMetadata
- READ.niaapi.UpgradeAssistFile
- READ.niaapi.VersionRegex
- READ.niatelemetry.AaaLdapProviderDetails
- READ.niatelemetry.AaaRadiusProviderDetails
- READ.niatelemetry.AaaTacacsProviderDetails
- READ.niatelemetry.Anomaly
- READ.niatelemetry.ApicAppPluginDetails
- READ.niatelemetry.ApicCoreFileDetails
- READ.niatelemetry.ApicDbgexpRsExportDest
- READ.niatelemetry.ApicDbgexpRsTsScheduler
- READ.niatelemetry.ApicFanDetails
- READ.niatelemetry.ApicFexDetails
- READ.niatelemetry.ApicFlashDetails
- READ.niatelemetry.ApicNtpAuth
- READ.niatelemetry.ApicPerformanceData
- READ.niatelemetry.ApicPodData
- READ.niatelemetry.ApicPsuDetails
- READ.niatelemetry.ApicRealmDetails
- READ.niatelemetry.ApicSnmpClientGrpDetails
- READ.niatelemetry.ApicSnmpCommunityAccessDetails
- READ.niatelemetry.ApicSnmpCommunityDetails
- READ.niatelemetry.ApicSnmpTrapDetails
- READ.niatelemetry.ApicSnmpTrapFwdServerDetails
- READ.niatelemetry.ApicSnmpVersionThreeDetails
- READ.niatelemetry.ApicSysLogGrp
- READ.niatelemetry.ApicSysLogSrc
- READ.niatelemetry.ApicTransceiverDetails
- READ.niatelemetry.ApicUiPageCounts
- READ.niatelemetry.ApicVision
- READ.niatelemetry.AppDetails
- READ.niatelemetry.CloudDetails
- READ.niatelemetry.Cluster
- READ.niatelemetry.ClusterNode
- READ.niatelemetry.CommonPolicies
- READ.niatelemetry.Controller
- READ.niatelemetry.DcnmFanDetails
- READ.niatelemetry.DcnmFexDetails
- READ.niatelemetry.DcnmModuleDetails
- READ.niatelemetry.DcnmPsuDetails
- READ.niatelemetry.DcnmTransceiverDetails
- READ.niatelemetry.DomInfoObject
- READ.niatelemetry.DomThresInfoObject
- READ.niatelemetry.Epg
- READ.niatelemetry.Fabric
- READ.niatelemetry.FabricModuleDetails
- READ.niatelemetry.FabricNodeControlDetails
- READ.niatelemetry.FabricPodProfile
- READ.niatelemetry.FabricPodSs
- READ.niatelemetry.Fault
- READ.niatelemetry.HcloudDetails
- READ.niatelemetry.HealthInsightsData
- READ.niatelemetry.HttpsAclContractDetails
- READ.niatelemetry.HttpsAclContractFilterMap
- READ.niatelemetry.HttpsAclEpgContractMap
- READ.niatelemetry.HttpsAclEpgDetails
- READ.niatelemetry.HttpsAclFilterDetails
- READ.niatelemetry.InsightGroupDetails
- READ.niatelemetry.Lc
- READ.niatelemetry.LeafPolGrpDetails
- READ.niatelemetry.Link
- READ.niatelemetry.MdsNeighbors
- READ.niatelemetry.MsoContractDetails
- READ.niatelemetry.MsoEpgDetails
- READ.niatelemetry.MsoSchemaDetails
- READ.niatelemetry.MsoSiteDetails
- READ.niatelemetry.MsoTenantDetails
- READ.niatelemetry.Neighbor
- READ.niatelemetry.Network
- READ.niatelemetry.NexusCloudAccount
- READ.niatelemetry.NexusCloudSite
- READ.niatelemetry.NexusDashboardControllerDetails
- READ.niatelemetry.NexusDashboardDetails
- READ.niatelemetry.NexusDashboardMemoryDetails
- READ.niatelemetry.NexusDashboards
- READ.niatelemetry.NiaFeatureUsage
- READ.niatelemetry.NiaInventory
- READ.niatelemetry.NiaInventoryDcnm
- READ.niatelemetry.NiaInventoryFabric
- READ.niatelemetry.NiaLicenseState
- READ.niatelemetry.Nicc
- READ.niatelemetry.PasswordStrengthCheck
- READ.niatelemetry.PodCommPolicies
- READ.niatelemetry.PodSnmpPolicies
- READ.niatelemetry.PodTimeServerPolicies
- READ.niatelemetry.Route
- READ.niatelemetry.SiteInventory
- READ.niatelemetry.SnmpSrc
- READ.niatelemetry.SpinePolGrpDetails
- READ.niatelemetry.SshVersionTwo
- READ.niatelemetry.SupervisorModuleDetails
- READ.niatelemetry.Switch
- READ.niatelemetry.SwitchInterface
- READ.niatelemetry.SyslogRemoteDest
- READ.niatelemetry.SyslogSysMsg
- READ.niatelemetry.SyslogSysMsgFacFilter
- READ.niatelemetry.SystemControllerDetails
- READ.niatelemetry.Tenant
- READ.notification.AccountSubscription
- READ.ntp.NtpServer
- READ.ntp.Policy
- READ.ntp.PolicyInventory
- READ.oauth.AccessToken
- READ.oauth.Authorization
- READ.onprem.ApplianceSystemInfo
- READ.onprem.AuditRecord
- READ.onprem.Upgrade
- READ.onprem.UserPreference
- READ.openapi.ApiMethodMeta
- READ.openapi.OpenApiSpecification
- READ.openapi.ProcessFile
- READ.openapi.TaskGenerationRequest
- READ.openapi.TaskGenerationResult
- READ.oprs.Deployment
- READ.oprs.SyncTargetListMessage
- READ.organization.Organization
- READ.os.BulkInstallInfo
- READ.os.Catalog
- READ.os.ConfigurationFile
- READ.os.Distribution
- READ.os.Install
- READ.os.SupportedVersion
- READ.os.ValidRemoteTarget
- READ.partnerintegration.DcLogs
- READ.partnerintegration.DeviceConnector
- READ.partnerintegration.DocIssues
- READ.partnerintegration.Etl
- READ.partnerintegration.File
- READ.partnerintegration.Inventory
- READ.partnerintegration.Logs
- READ.partnerintegration.Metrics
- READ.partnerintegration.Model
- READ.pci.CoprocessorCard
- READ.pci.Device
- READ.pci.Endpoint
- READ.pci.Link
- READ.pci.Node
- READ.pci.NodeSetting
- READ.pci.Port
- READ.pci.Slot
- READ.pci.Switch
- READ.pci.Zone
- READ.pool.IdMappingMember
- READ.pool.IdMappingPolicy
- READ.port.Group
- READ.port.MacBinding
- READ.port.SubGroup
- READ.power.ControlState
- READ.power.Policy
- READ.power.PolicyInventory
- READ.power.PowerGroup
- READ.power.PowerGroupMember
- READ.processor.Unit
- READ.rack.UnitPersonality
- READ.recommendation.CapacityRunway
- READ.recommendation.ClusterExpansion
- READ.recommendation.HardwareExpansionRequest
- READ.recommendation.HardwareExpansionRequestItem
- READ.recommendation.PhysicalItem
- READ.recommendation.PurchaseOrderEstimate
- READ.recommendation.PurchaseOrderList
- READ.recommendation.SoftwareItem
- READ.recovery.BackupConfigPolicy
- READ.recovery.BackupProfile
- READ.recovery.ConfigResult
- READ.recovery.ConfigResultEntry
- READ.recovery.OnDemandBackup
- READ.recovery.Restore
- READ.recovery.ScheduleConfigPolicy
- READ.resource.Group
- READ.resource.GroupMember
- READ.resource.LicenseResourceCount
- READ.resource.Membership
- READ.resource.MembershipHolder
- READ.resource.Reservation
- READ.resource.SelectionCriteria
- READ.resource.SharedResourcesInfoHolder
- READ.resourcepool.ChassisQualificationPolicy
- READ.resourcepool.Lease
- READ.resourcepool.LeaseResource
- READ.resourcepool.MembershipReservation
- READ.resourcepool.Pool
- READ.resourcepool.PoolMember
- READ.resourcepool.QualificationPolicy
- READ.resourcepool.Reservation
- READ.resourcepool.Universe
- READ.scheduler.SchedulePolicy
- READ.scheduler.TaskResult
- READ.scheduler.TaskSchedule
- READ.sdaaci.Connection
- READ.sdaaci.ConnectionDetail
- READ.sdcard.Policy
- READ.sdcard.PolicyInventory
- READ.search.SearchItem
- READ.search.TagItem
- READ.security.Unit
- READ.server.ConfigChangeDetail
- READ.server.ConfigImport
- READ.server.ConfigResult
- READ.server.ConfigResultEntry
- READ.server.DiagnosticStatus
- READ.server.Diagnostics
- READ.server.Disruption
- READ.server.MigrationKeyDetails
- READ.server.Profile
- READ.server.ProfilePendingChangeEval
- READ.server.ProfileTemplate
- READ.servicenow.ChangeRequest
- READ.servicenow.ChangeRequestDoc
- READ.servicenow.Incident
- READ.servicenow.IncidentDoc
- READ.smtp.Policy
- READ.smtp.PolicyInventory
- READ.smtp.PolicyTest
- READ.snmp.Policy
- READ.snmp.PolicyInventory
- READ.software.ApplianceDistributable
- READ.software.DownloadHistory
- READ.software.HciBundleDistributable
- READ.software.HciDistributable
- READ.software.HclMeta
- READ.software.HyperflexBundleDistributable
- READ.software.HyperflexDistributable
- READ.software.IksBundleDistributable
- READ.software.ReleaseMeta
- READ.software.SolutionDistributable
- READ.software.UcsdBundleDistributable
- READ.software.UcsdDistributable
- READ.softwarerepository.Authorization
- READ.softwarerepository.CachedImage
- READ.softwarerepository.Catalog
- READ.softwarerepository.CategoryMapper
- READ.softwarerepository.CategoryMapperModel
- READ.softwarerepository.CategorySupportConstraint
- READ.softwarerepository.CategoryUnsupportedModels
- READ.softwarerepository.DownloadSpec
- READ.softwarerepository.OperatingSystemFile
- READ.softwarerepository.Release
- READ.sol.Policy
- READ.sol.PolicyInventory
- READ.ssh.Policy
- READ.ssh.PolicyInventory
- READ.storage.BatteryBackupUnit
- READ.storage.Controller
- READ.storage.ControllerDrive
- READ.storage.DiskGroup
- READ.storage.DiskSlot
- READ.storage.DriveGroup
- READ.storage.DriveSecurityPolicy
- READ.storage.Enclosure
- READ.storage.EnclosureDisk
- READ.storage.EnclosureDiskSlotEp
- READ.storage.FileItem
- READ.storage.FlexFlashController
- READ.storage.FlexFlashControllerProps
- READ.storage.FlexFlashPhysicalDrive
- READ.storage.FlexFlashVirtualDrive
- READ.storage.FlexUtilController
- READ.storage.FlexUtilPhysicalDrive
- READ.storage.FlexUtilVirtualDrive
- READ.storage.HitachiArray
- READ.storage.HitachiController
- READ.storage.HitachiDisk
- READ.storage.HitachiExternalParityGroup
- READ.storage.HitachiExternalPathGroup
- READ.storage.HitachiExternalStorageLun
- READ.storage.HitachiExternalStoragePort
- READ.storage.HitachiHost
- READ.storage.HitachiHostLun
- READ.storage.HitachiNvmSubsystem
- READ.storage.HitachiParityGroup
- READ.storage.HitachiPool
- READ.storage.HitachiPort
- READ.storage.HitachiRemoteCopyPairGad
- READ.storage.HitachiRemoteCopyPairTc
- READ.storage.HitachiRemoteCopyPairUr
- READ.storage.HitachiRemoteReplication
- READ.storage.HitachiSnapshot
- READ.storage.HitachiVolume
- READ.storage.HitachiVolumeMigrationPair
- READ.storage.HyperFlexStorageContainer
- READ.storage.HyperFlexVolume
- READ.storage.Item
- READ.storage.KnoxSecureDriveConfiguration
- READ.storage.NetAppAggregate
- READ.storage.NetAppAggregateEvent
- READ.storage.NetAppBaseDisk
- READ.storage.NetAppCifsService
- READ.storage.NetAppCifsShare
- READ.storage.NetAppCloudTarget
- READ.storage.NetAppCluster
- READ.storage.NetAppClusterEvent
- READ.storage.NetAppClusterSnapMirrorPolicy
- READ.storage.NetAppClusterSnapshotPolicy
- READ.storage.NetAppDataIpInterface
- READ.storage.NetAppDataIpInterfaceEvent
- READ.storage.NetAppDiskEvent
- READ.storage.NetAppEthernetPort
- READ.storage.NetAppEthernetPortEvent
- READ.storage.NetAppExportPolicy
- READ.storage.NetAppFcInterface
- READ.storage.NetAppFcInterfaceEvent
- READ.storage.NetAppFcPort
- READ.storage.NetAppFcPortEvent
- READ.storage.NetAppInitiatorGroup
- READ.storage.NetAppIpInterface
- READ.storage.NetAppIpInterfaceEvent
- READ.storage.NetAppIscsiService
- READ.storage.NetAppLicense
- READ.storage.NetAppLun
- READ.storage.NetAppLunEvent
- READ.storage.NetAppLunMap
- READ.storage.NetAppNamespace
- READ.storage.NetAppNfsClient
- READ.storage.NetAppNfsService
- READ.storage.NetAppNode
- READ.storage.NetAppNodeCdpNeighbor
- READ.storage.NetAppNodeEvent
- READ.storage.NetAppNonDataIpInterface
- READ.storage.NetAppNonDataIpInterfaceEvent
- READ.storage.NetAppNtpServer
- READ.storage.NetAppQtree
- READ.storage.NetAppSchedule
- READ.storage.NetAppSensor
- READ.storage.NetAppSnapMirrorRelationship
- READ.storage.NetAppStorageVm
- READ.storage.NetAppSvmEvent
- READ.storage.NetAppSvmSnapMirrorPolicy
- READ.storage.NetAppSvmSnapshotPolicy
- READ.storage.NetAppVolume
- READ.storage.NetAppVolumeEvent
- READ.storage.NetAppVolumeSnapshot
- READ.storage.NvmeRaidConfiguration
- READ.storage.PhysicalDisk
- READ.storage.PhysicalDiskExtension
- READ.storage.PhysicalDiskUsage
- READ.storage.PureArray
- READ.storage.PureArrayAlerts
- READ.storage.PureBlade
- READ.storage.PureController
- READ.storage.PureDirectory
- READ.storage.PureDirectoryExport
- READ.storage.PureDirectoryPolicy
- READ.storage.PureDirectoryQuota
- READ.storage.PureDirectorySnapshot
- READ.storage.PureDisk
- READ.storage.PureFileSystems
- READ.storage.PureFlashBladeFileSystem
- READ.storage.PureFlashBladeSystem
- READ.storage.PureHost
- READ.storage.PureHostGroup
- READ.storage.PureHostLun
- READ.storage.PureManagementAccessPolicy
- READ.storage.PureNfsPolicyRule
- READ.storage.PureObjectBucket
- READ.storage.PureObjectStoreAccount
- READ.storage.PureObjectStoreUser
- READ.storage.PurePod
- READ.storage.PurePort
- READ.storage.PureProtectionGroup
- READ.storage.PureProtectionGroupSnapshot
- READ.storage.PureQuotaPolicyRule
- READ.storage.PureRealm
- READ.storage.PureReplicationSchedule
- READ.storage.PureSmbPolicyRule
- READ.storage.PureSnapshotSchedule
- READ.storage.PureTargetArray
- READ.storage.PureVolume
- READ.storage.PureVolumeGroup
- READ.storage.PureVolumeSnapshot
- READ.storage.SasExpander
- READ.storage.SasPort
- READ.storage.Span
- READ.storage.StoragePolicy
- READ.storage.VdMemberEp
- READ.storage.VirtualDrive
- READ.storage.VirtualDriveContainer
- READ.storage.VirtualDriveExtension
- READ.storage.VirtualDriveIdentity
- READ.syslog.Policy
- READ.syslog.PolicyInventory
- READ.tam.AdvisoryCount
- READ.tam.AdvisoryDefinition
- READ.tam.AdvisoryInfo
- READ.tam.AdvisoryInstance
- READ.tam.SecurityAdvisory
- READ.techsupportmanagement.CollectionControlPolicy
- READ.techsupportmanagement.Download
- READ.techsupportmanagement.EndPoint
- READ.techsupportmanagement.TechSupportBundle
- READ.techsupportmanagement.TechSupportStatus
- READ.terminal.AuditLog
- READ.thermal.Policy
- READ.thermal.PolicyInventory
- READ.top.System
- READ.ucsd.BackupInfo
- READ.uuidpool.Block
- READ.uuidpool.Pool
- READ.uuidpool.PoolMember
- READ.uuidpool.Reservation
- READ.uuidpool.Universe
- READ.uuidpool.UuidLease
- READ.view.HealthStatus
- READ.view.Server
- READ.virtualization.EsxiConsole
- READ.virtualization.Host
- READ.virtualization.VirtualMachine
- READ.virtualization.VmwareCluster
- READ.virtualization.VmwareDatacenter
- READ.virtualization.VmwareDatastore
- READ.virtualization.VmwareDatastoreCluster
- READ.virtualization.VmwareDistributedNetwork
- READ.virtualization.VmwareDistributedSwitch
- READ.virtualization.VmwareFolder
- READ.virtualization.VmwareHost
- READ.virtualization.VmwareHostGpu
- READ.virtualization.VmwareKernelNetwork
- READ.virtualization.VmwareNetwork
- READ.virtualization.VmwarePhysicalNetworkInterface
- READ.virtualization.VmwareProactiveHa
- READ.virtualization.VmwareUplinkPort
- READ.virtualization.VmwareVcenter
- READ.virtualization.VmwareVirtualDisk
- READ.virtualization.VmwareVirtualMachine
- READ.virtualization.VmwareVirtualMachineGpu
- READ.virtualization.VmwareVirtualMachineSnapshot
- READ.virtualization.VmwareVirtualNetworkInterface
- READ.virtualization.VmwareVirtualSwitch
- READ.vmedia.Policy
- READ.vmedia.PolicyInventory
- READ.vmrc.Console
- READ.vnic.EthAdapterPolicy
- READ.vnic.EthAdapterPolicyInventory
- READ.vnic.EthIf
- READ.vnic.EthIfInventory
- READ.vnic.EthNetworkPolicy
- READ.vnic.EthNetworkPolicyInventory
- READ.vnic.EthQosPolicy
- READ.vnic.EthQosPolicyInventory
- READ.vnic.EthVethInventory
- READ.vnic.EthVnicInventory
- READ.vnic.FcAdapterPolicy
- READ.vnic.FcAdapterPolicyInventory
- READ.vnic.FcIf
- READ.vnic.FcIfInventory
- READ.vnic.FcNetworkPolicy
- READ.vnic.FcNetworkPolicyInventory
- READ.vnic.FcQosPolicy
- READ.vnic.FcQosPolicyInventory
- READ.vnic.FcVethInventory
- READ.vnic.FcVhbaPolicyInventory
- READ.vnic.IscsiAdapterPolicy
- READ.vnic.IscsiAdapterPolicyInventory
- READ.vnic.IscsiBootPolicy
- READ.vnic.IscsiBootPolicyInventory
- READ.vnic.IscsiStaticTargetPolicy
- READ.vnic.IscsiStaticTargetPolicyInventory
- READ.vnic.LanConnectivityPolicy
- READ.vnic.LanConnectivityPolicyInventory
- READ.vnic.LanSettings
- READ.vnic.LcpStatus
- READ.vnic.SanConnectivityPolicy
- READ.vnic.SanConnectivityPolicyInventory
- READ.vnic.SanSettings
- READ.vnic.ScpStatus
- READ.vnic.ServiceEthIf
- READ.vnic.ServiceEthIfInventory
- READ.vnic.VhbaTemplate
- READ.vnic.VifIdPool
- READ.vnic.VnicTemplate
- READ.vrf.Vrf
- READ.webhook.Endpoint
- READ.webhook.Schema
- READ.workflow.AnsibleBatchExecutor
- READ.workflow.BatchApiExecutor
- READ.workflow.Catalog
- READ.workflow.CatalogItemDefinition
- READ.workflow.CatalogServiceRequest
- READ.workflow.CustomDataTypeDefinition
- READ.workflow.ErrorResponseHandler
- READ.workflow.PowerShellBatchApiExecutor
- READ.workflow.RollbackWorkflow
- READ.workflow.ServiceItemActionDefinition
- READ.workflow.ServiceItemActionInstance
- READ.workflow.ServiceItemAttribute
- READ.workflow.ServiceItemDefinition
- READ.workflow.ServiceItemHealthCheckDefinition
- READ.workflow.ServiceItemHealthCheckExecution
- READ.workflow.ServiceItemInstance
- READ.workflow.ServiceItemOutput
- READ.workflow.SshBatchExecutor
- READ.workflow.TaskDebugLog
- READ.workflow.TaskDefinition
- READ.workflow.TaskInfo
- READ.workflow.TaskMetadata
- READ.workflow.TemplateFunctionMeta
- READ.workflow.UiDisplayMetadata
- READ.workflow.Variable
- READ.workflow.WorkflowDefinition
- READ.workflow.WorkflowInfo
- READ.workflow.WorkflowMetadata
- READ.workload.Blueprint
- READ.workload.ClearWorkloadTag
- READ.workload.DeploymentInput
- READ.workload.WorkloadDefinition
- READ.workload.WorkloadDeployment
- READ.workload.WorkloadInstance
- READ.workload.WorkloadMetadata
- ROLE.Account Administrator
- ROLE.Audit Log Viewer
- ROLE.Automation Governance
- ROLE.Catalog Administrator
- ROLE.Catalog User
- ROLE.Complete Claim
- ROLE.Device Administrator
- ROLE.Device Technician
- ROLE.External Syslog Administrator
- ROLE.HCI Cluster Administrator
- ROLE.HCI Cluster Operator
- ROLE.HyperFlex Cluster Access Operator
- ROLE.HyperFlex Cluster Administrator
- ROLE.HyperFlex Cluster Data Protection Administrator
- ROLE.HyperFlex Cluster Lifecycle Administrator
- ROLE.HyperFlex Cluster Operator
- ROLE.HyperFlex Cluster Storage Administrator
- ROLE.HyperFlex Cluster Syslog Administrator
- ROLE.HyperFlex Cluster System Administrator
- ROLE.HyperFlex Cluster System Operator
- ROLE.Integrated Systems Administrator
- ROLE.Integrated Systems Operator
- ROLE.Kubernetes Administrator
- ROLE.Kubernetes Operator
- ROLE.Location Management
- ROLE.Network Administrator
- ROLE.Network Operator
- ROLE.Nexus Administrator
- ROLE.Nexus Analyst
- ROLE.Nexus Config Administrator
- ROLE.Nexus Observer
- ROLE.Read-Only
- ROLE.SAN Administrator
- ROLE.SAN Operator
- ROLE.Server Administrator
- ROLE.Service Designer
- ROLE.Service Operator
- ROLE.Storage Administrator
- ROLE.Support Services
- ROLE.Sustainability Metrics Viewer
- ROLE.Tag Management
- ROLE.UCS Domain Administrator
- ROLE.Unified Edge Administrator
- ROLE.User Access Administrator
- ROLE.Virtualization Administrator
- ROLE.Workflow Designer
- ROLE.Workload Administrator
- ROLE.Workload Operator
- ROLE.Workload Optimizer Administrator
- ROLE.Workload Optimizer Advisor
- ROLE.Workload Optimizer Automator
- ROLE.Workload Optimizer Deployer
- ROLE.Workload Optimizer Observer
- ROLE.vKVM Only
- UPDATE.aaa.RetentionPolicy
- UPDATE.access.Policy
- UPDATE.adapter.ConfigPolicy
- UPDATE.adapter.HostEthInterface
- UPDATE.adapter.HostFcInterface
- UPDATE.appliance.BackupPolicy
- UPDATE.appliance.CertificateSetting
- UPDATE.appliance.ClusterInfo
- UPDATE.appliance.ClusterInstall
- UPDATE.appliance.ClusterReplaceNode
- UPDATE.appliance.ClusterWorkerNode
- UPDATE.appliance.DataExportPolicy
- UPDATE.appliance.DeviceClaim
- UPDATE.appliance.DeviceUpgradePolicy
- UPDATE.appliance.DiagSetting
- UPDATE.appliance.ExternalSyslogSetting
- UPDATE.appliance.FqdnUpdate
- UPDATE.appliance.MetricsConfig
- UPDATE.appliance.SetupInfo
- UPDATE.appliance.Upgrade
- UPDATE.appliance.UpgradePolicy
- UPDATE.asset.DeviceConfiguration
- UPDATE.asset.DeviceContractInformation
- UPDATE.asset.DeviceRegistration
- UPDATE.asset.GeoLocation
- UPDATE.asset.PreClaim
- UPDATE.asset.Target
- UPDATE.auditd.Policy
- UPDATE.bios.BootMode
- UPDATE.bios.Policy
- UPDATE.bios.Unit
- UPDATE.boot.CddDevice
- UPDATE.boot.DeviceBootMode
- UPDATE.boot.DeviceBootSecurity
- UPDATE.boot.HddDevice
- UPDATE.boot.IscsiDevice
- UPDATE.boot.NvmeDevice
- UPDATE.boot.PchStorageDevice
- UPDATE.boot.PrecisionPolicy
- UPDATE.boot.PxeDevice
- UPDATE.boot.SanDevice
- UPDATE.boot.SdDevice
- UPDATE.boot.UefiShellDevice
- UPDATE.boot.UsbDevice
- UPDATE.boot.VmediaDevice
- UPDATE.bulk.Export
- UPDATE.certificatemanagement.Policy
- UPDATE.chassis.Profile
- UPDATE.chassis.ProfileTemplate
- UPDATE.cli.CliPolicy
- UPDATE.comm.HttpProxyPolicy
- UPDATE.comm.TagDefinition
- UPDATE.compute.Blade
- UPDATE.compute.BladeIdentity
- UPDATE.compute.Board
- UPDATE.compute.Mapping
- UPDATE.compute.PcieConnectivityPolicy
- UPDATE.compute.Personality
- UPDATE.compute.RackUnit
- UPDATE.compute.RackUnitIdentity
- UPDATE.compute.ScrubPolicy
- UPDATE.compute.ServerPowerPolicy
- UPDATE.compute.ServerSetting
- UPDATE.cond.Alarm
- UPDATE.cond.AlarmRule
- UPDATE.cond.AlarmSuppression
- UPDATE.cond.CustomHclBaseline
- UPDATE.cond.ThresholdDefinition
- UPDATE.convergedinfra.Pod
- UPDATE.coremanagement.CoreFile
- UPDATE.crd.CustomResource
- UPDATE.deviceconnector.Policy
- UPDATE.equipment.Chassis
- UPDATE.equipment.ChassisController
- UPDATE.equipment.ChassisIdentity
- UPDATE.equipment.ChassisOperation
- UPDATE.equipment.EnclosureElement
- UPDATE.equipment.ExpanderModule
- UPDATE.equipment.ExpanderModuleIdentity
- UPDATE.equipment.ExpanderModuleOperation
- UPDATE.equipment.Fan
- UPDATE.equipment.FanControl
- UPDATE.equipment.FanModule
- UPDATE.equipment.Fex
- UPDATE.equipment.FexIdentity
- UPDATE.equipment.FexOperation
- UPDATE.equipment.Fru
- UPDATE.equipment.IoCard
- UPDATE.equipment.IoCardOperation
- UPDATE.equipment.IoExpander
- UPDATE.equipment.LocatorLed
- UPDATE.equipment.Psu
- UPDATE.equipment.PsuControl
- UPDATE.equipment.RackEnclosure
- UPDATE.equipment.RackEnclosureSlot
- UPDATE.equipment.SharedIoModule
- UPDATE.equipment.SwitchCard
- UPDATE.equipment.SwitchOperation
- UPDATE.equipment.SystemIoController
- UPDATE.equipment.Tpm
- UPDATE.equipment.Transceiver
- UPDATE.ether.HostPort
- UPDATE.ether.NetworkPort
- UPDATE.ether.PhysicalPort
- UPDATE.externalsite.Authorization
- UPDATE.fabric.AppliancePcRole
- UPDATE.fabric.ApplianceRole
- UPDATE.fabric.ElementIdentity
- UPDATE.fabric.EthNetworkControlPolicy
- UPDATE.fabric.EthNetworkGroupPolicy
- UPDATE.fabric.EthNetworkPolicy
- UPDATE.fabric.FcNetworkPolicy
- UPDATE.fabric.FcStorageRole
- UPDATE.fabric.FcUplinkPcRole
- UPDATE.fabric.FcUplinkRole
- UPDATE.fabric.FcZonePolicy
- UPDATE.fabric.FcoeUplinkPcRole
- UPDATE.fabric.FcoeUplinkRole
- UPDATE.fabric.FlowControlPolicy
- UPDATE.fabric.LanPinGroup
- UPDATE.fabric.LinkAggregationPolicy
- UPDATE.fabric.LinkControlPolicy
- UPDATE.fabric.MacSecPolicy
- UPDATE.fabric.MulticastPolicy
- UPDATE.fabric.NetFlowExporter
- UPDATE.fabric.NetFlowMonitor
- UPDATE.fabric.NetFlowPolicy
- UPDATE.fabric.NetFlowRecord
- UPDATE.fabric.PcOperation
- UPDATE.fabric.PortMode
- UPDATE.fabric.PortOperation
- UPDATE.fabric.PortPolicy
- UPDATE.fabric.SanPinGroup
- UPDATE.fabric.SecureRouterRole
- UPDATE.fabric.ServerRole
- UPDATE.fabric.SpanDestEthPort
- UPDATE.fabric.SpanSession
- UPDATE.fabric.SwitchClusterProfile
- UPDATE.fabric.SwitchClusterProfileTemplate
- UPDATE.fabric.SwitchControlPolicy
- UPDATE.fabric.SwitchProfile
- UPDATE.fabric.SwitchProfileTemplate
- UPDATE.fabric.SystemQosPolicy
- UPDATE.fabric.UplinkPcRole
- UPDATE.fabric.UplinkRole
- UPDATE.fabric.Vlan
- UPDATE.fabric.Vsan
- UPDATE.fault.Instance
- UPDATE.fc.PhysicalPort
- UPDATE.fcpool.Pool
- UPDATE.fcpool.Reservation
- UPDATE.feedback.FeedbackPost
- UPDATE.firmware.Distributable
- UPDATE.firmware.DriverDistributable
- UPDATE.firmware.Policy
- UPDATE.firmware.RunningFirmware
- UPDATE.firmware.ServerConfigurationUtilityDistributable
- UPDATE.firmware.UnsupportedVersionUpgrade
- UPDATE.firmware.Upgrade
- UPDATE.forecast.Instance
- UPDATE.graphics.Card
- UPDATE.graphics.Controller
- UPDATE.hci.AhvVm
- UPDATE.hci.Cluster
- UPDATE.hci.ClusterOperation
- UPDATE.hci.EsxiVm
- UPDATE.hci.Node
- UPDATE.hyperflex.AutoSupportPolicy
- UPDATE.hyperflex.CapabilityInfo
- UPDATE.hyperflex.Cluster
- UPDATE.hyperflex.ClusterBackupPolicy
- UPDATE.hyperflex.ClusterBackupPolicyDeployment
- UPDATE.hyperflex.ClusterNetworkPolicy
- UPDATE.hyperflex.ClusterProfile
- UPDATE.hyperflex.ClusterReplicationNetworkPolicy
- UPDATE.hyperflex.ClusterReplicationNetworkPolicyDeployment
- UPDATE.hyperflex.ClusterStoragePolicy
- UPDATE.hyperflex.Drive
- UPDATE.hyperflex.ExtFcStoragePolicy
- UPDATE.hyperflex.ExtIscsiStoragePolicy
- UPDATE.hyperflex.HypervisorHost
- UPDATE.hyperflex.HypervisorVirtualMachine
- UPDATE.hyperflex.InitiatorGroup
- UPDATE.hyperflex.IscsiNetwork
- UPDATE.hyperflex.KeyEncryptionKey
- UPDATE.hyperflex.LocalCredentialPolicy
- UPDATE.hyperflex.Lun
- UPDATE.hyperflex.NodeConfigPolicy
- UPDATE.hyperflex.NodeProfile
- UPDATE.hyperflex.ProxySettingPolicy
- UPDATE.hyperflex.ReduceReSync
- UPDATE.hyperflex.ServiceAuthToken
- UPDATE.hyperflex.SoftwareVersionPolicy
- UPDATE.hyperflex.StorageContainer
- UPDATE.hyperflex.SysConfigPolicy
- UPDATE.hyperflex.Target
- UPDATE.hyperflex.UcsmConfigPolicy
- UPDATE.hyperflex.VcenterConfigPolicy
- UPDATE.hyperflex.Volume
- UPDATE.iaas.UcsdInfo
- UPDATE.iam.Account
- UPDATE.iam.ApiKey
- UPDATE.iam.AppRegistration
- UPDATE.iam.BannerMessage
- UPDATE.iam.Certificate
- UPDATE.iam.CertificateRequest
- UPDATE.iam.CuiIntegration
- UPDATE.iam.DefaultAuthentication
- UPDATE.iam.DomainNameInfo
- UPDATE.iam.EndPointUser
- UPDATE.iam.EndPointUserPolicy
- UPDATE.iam.EndPointUserRole
- UPDATE.iam.GuestAccessSettings
- UPDATE.iam.Idp
- UPDATE.iam.IdpReference
- UPDATE.iam.IpAccessManagement
- UPDATE.iam.IpAddress
- UPDATE.iam.LdapGroup
- UPDATE.iam.LdapPolicy
- UPDATE.iam.LdapProvider
- UPDATE.iam.LocalUserPassword
- UPDATE.iam.LocalUserPasswordPolicy
- UPDATE.iam.Permission
- UPDATE.iam.PrivateKeySpec
- UPDATE.iam.PrivilegeSet
- UPDATE.iam.Qualifier
- UPDATE.iam.ResourceLimits
- UPDATE.iam.ResourceRoles
- UPDATE.iam.SessionLimits
- UPDATE.iam.SharingRule
- UPDATE.iam.TestIdpConfiguration
- UPDATE.iam.User
- UPDATE.iam.UserGroup
- UPDATE.iam.UserPreference
- UPDATE.iam.UserQualifier
- UPDATE.iam.UserSetting
- UPDATE.inventory.GenericInventory
- UPDATE.inventory.GenericInventoryHolder
- UPDATE.ipmioverlan.Policy
- UPDATE.ippool.Pool
- UPDATE.ippool.Reservation
- UPDATE.iqnpool.Pool
- UPDATE.iwotenant.Migrate
- UPDATE.iwotenant.TenantCustomization
- UPDATE.kvm.Policy
- UPDATE.kvm.Session
- UPDATE.kvm.TunneledKvmPolicy
- UPDATE.license.AccountLicenseData
- UPDATE.license.CustomerOp
- UPDATE.license.ErpCustomerOp
- UPDATE.license.IksCustomerOp
- UPDATE.license.IksLicenseCount
- UPDATE.license.IncCustomerOp
- UPDATE.license.IncLicenseCount
- UPDATE.license.IwoCustomerOp
- UPDATE.license.IwoLicenseCount
- UPDATE.license.LicenseInfo
- UPDATE.license.LicenseRegistrationStatus
- UPDATE.license.LicenseReservationOp
- UPDATE.license.SmartlicenseToken
- UPDATE.ls.ServiceProfile
- UPDATE.macpool.Pool
- UPDATE.macpool.Reservation
- UPDATE.management.Controller
- UPDATE.management.Entity
- UPDATE.management.Interface
- UPDATE.memory.Array
- UPDATE.memory.PersistentMemoryConfigResult
- UPDATE.memory.PersistentMemoryConfiguration
- UPDATE.memory.PersistentMemoryNamespace
- UPDATE.memory.PersistentMemoryNamespaceConfigResult
- UPDATE.memory.PersistentMemoryPolicy
- UPDATE.memory.PersistentMemoryRegion
- UPDATE.memory.PersistentMemoryUnit
- UPDATE.memory.Policy
- UPDATE.memory.Unit
- UPDATE.metrics.Configuration
- UPDATE.metrics.MetricsExploration
- UPDATE.metrics.ResourceConfiguration
- UPDATE.mgmt.ConfigBackupFile
- UPDATE.mgmt.ConfigBackupInstance
- UPDATE.mgmt.ConfigBackupOperation
- UPDATE.mgmt.ConfigOperationSetting
- UPDATE.network.Element
- UPDATE.network.FcZoneInfo
- UPDATE.network.SecureRouter
- UPDATE.network.SecureRouterSetting
- UPDATE.network.Vethernet
- UPDATE.network.Vfc
- UPDATE.network.VlanPortInfo
- UPDATE.networkconfig.Policy
- UPDATE.notification.AccountSubscription
- UPDATE.ntp.Policy
- UPDATE.oauth.Authorization
- UPDATE.onprem.Upgrade
- UPDATE.onprem.UserPreference
- UPDATE.openapi.OpenApiSpecification
- UPDATE.openapi.TaskGenerationRequest
- UPDATE.oprs.Deployment
- UPDATE.oprs.SyncTargetListMessage
- UPDATE.organization.Organization
- UPDATE.os.ConfigurationFile
- UPDATE.partnerintegration.DeviceConnector
- UPDATE.partnerintegration.Etl
- UPDATE.partnerintegration.File
- UPDATE.partnerintegration.Inventory
- UPDATE.partnerintegration.Metrics
- UPDATE.partnerintegration.Model
- UPDATE.pci.Device
- UPDATE.pci.Link
- UPDATE.pci.Node
- UPDATE.pci.NodeSetting
- UPDATE.pci.Switch
- UPDATE.pool.IdMappingPolicy
- UPDATE.port.Group
- UPDATE.port.MacBinding
- UPDATE.port.SubGroup
- UPDATE.power.Policy
- UPDATE.power.PowerGroup
- UPDATE.processor.Unit
- UPDATE.rack.UnitPersonality
- UPDATE.recommendation.HardwareExpansionRequest
- UPDATE.recommendation.HardwareExpansionRequestItem
- UPDATE.recommendation.PurchaseOrderEstimate
- UPDATE.recovery.BackupConfigPolicy
- UPDATE.recovery.BackupProfile
- UPDATE.recovery.OnDemandBackup
- UPDATE.recovery.ScheduleConfigPolicy
- UPDATE.resource.Group
- UPDATE.resource.Membership
- UPDATE.resource.Reservation
- UPDATE.resource.SelectionCriteria
- UPDATE.resourcepool.MembershipReservation
- UPDATE.resourcepool.Pool
- UPDATE.resourcepool.QualificationPolicy
- UPDATE.resourcepool.Reservation
- UPDATE.scheduler.SchedulePolicy
- UPDATE.scheduler.TaskSchedule
- UPDATE.sdaaci.Connection
- UPDATE.sdaaci.ConnectionDetail
- UPDATE.sdcard.Policy
- UPDATE.security.Unit
- UPDATE.server.DiagnosticStatus
- UPDATE.server.Diagnostics
- UPDATE.server.Profile
- UPDATE.server.ProfileTemplate
- UPDATE.smtp.Policy
- UPDATE.smtp.PolicyTest
- UPDATE.snmp.Policy
- UPDATE.software.ApplianceDistributable
- UPDATE.software.HciBundleDistributable
- UPDATE.software.HciDistributable
- UPDATE.software.HyperflexBundleDistributable
- UPDATE.software.HyperflexDistributable
- UPDATE.software.IksBundleDistributable
- UPDATE.software.ReleaseMeta
- UPDATE.software.SolutionDistributable
- UPDATE.software.UcsdBundleDistributable
- UPDATE.software.UcsdDistributable
- UPDATE.softwarerepository.Authorization
- UPDATE.softwarerepository.OperatingSystemFile
- UPDATE.sol.Policy
- UPDATE.ssh.Policy
- UPDATE.storage.BatteryBackupUnit
- UPDATE.storage.Controller
- UPDATE.storage.DiskGroup
- UPDATE.storage.DriveGroup
- UPDATE.storage.DriveSecurityPolicy
- UPDATE.storage.Enclosure
- UPDATE.storage.EnclosureDisk
- UPDATE.storage.EnclosureDiskSlotEp
- UPDATE.storage.FlexFlashController
- UPDATE.storage.FlexFlashControllerProps
- UPDATE.storage.FlexFlashPhysicalDrive
- UPDATE.storage.FlexFlashVirtualDrive
- UPDATE.storage.FlexUtilController
- UPDATE.storage.FlexUtilPhysicalDrive
- UPDATE.storage.FlexUtilVirtualDrive
- UPDATE.storage.HitachiArray
- UPDATE.storage.NetAppCluster
- UPDATE.storage.PhysicalDisk
- UPDATE.storage.PhysicalDiskExtension
- UPDATE.storage.PhysicalDiskUsage
- UPDATE.storage.PureArray
- UPDATE.storage.PureFlashBladeSystem
- UPDATE.storage.SasExpander
- UPDATE.storage.SasPort
- UPDATE.storage.Span
- UPDATE.storage.StoragePolicy
- UPDATE.storage.VdMemberEp
- UPDATE.storage.VirtualDrive
- UPDATE.storage.VirtualDriveContainer
- UPDATE.storage.VirtualDriveExtension
- UPDATE.syslog.Policy
- UPDATE.tam.AdvisoryInfo
- UPDATE.techsupportmanagement.CollectionControlPolicy
- UPDATE.thermal.Policy
- UPDATE.top.System
- UPDATE.uuidpool.Pool
- UPDATE.virtualization.EsxiConsole
- UPDATE.virtualization.Host
- UPDATE.virtualization.VirtualMachine
- UPDATE.virtualization.VmwareCluster
- UPDATE.virtualization.VmwareDatacenter
- UPDATE.virtualization.VmwareDatastore
- UPDATE.virtualization.VmwareDatastoreCluster
- UPDATE.virtualization.VmwareDistributedNetwork
- UPDATE.virtualization.VmwareDistributedSwitch
- UPDATE.virtualization.VmwareFolder
- UPDATE.virtualization.VmwareHost
- UPDATE.virtualization.VmwareKernelNetwork
- UPDATE.virtualization.VmwareNetwork
- UPDATE.virtualization.VmwarePhysicalNetworkInterface
- UPDATE.virtualization.VmwareUplinkPort
- UPDATE.virtualization.VmwareVirtualDisk
- UPDATE.virtualization.VmwareVirtualMachine
- UPDATE.virtualization.VmwareVirtualMachineSnapshot
- UPDATE.virtualization.VmwareVirtualNetworkInterface
- UPDATE.virtualization.VmwareVirtualSwitch
- UPDATE.vmedia.Policy
- UPDATE.vmrc.Console
- UPDATE.vnic.EthAdapterPolicy
- UPDATE.vnic.EthIf
- UPDATE.vnic.EthNetworkPolicy
- UPDATE.vnic.EthQosPolicy
- UPDATE.vnic.FcAdapterPolicy
- UPDATE.vnic.FcIf
- UPDATE.vnic.FcNetworkPolicy
- UPDATE.vnic.FcQosPolicy
- UPDATE.vnic.IscsiAdapterPolicy
- UPDATE.vnic.IscsiBootPolicy
- UPDATE.vnic.IscsiStaticTargetPolicy
- UPDATE.vnic.LanConnectivityPolicy
- UPDATE.vnic.SanConnectivityPolicy
- UPDATE.vnic.VhbaTemplate
- UPDATE.vnic.VnicTemplate
- UPDATE.vrf.Vrf
- UPDATE.webhook.Endpoint
- UPDATE.webhook.Schema
- UPDATE.workflow.AnsibleBatchExecutor
- UPDATE.workflow.BatchApiExecutor
- UPDATE.workflow.CatalogItemDefinition
- UPDATE.workflow.CatalogServiceRequest
- UPDATE.workflow.CustomDataTypeDefinition
- UPDATE.workflow.ErrorResponseHandler
- UPDATE.workflow.PowerShellBatchApiExecutor
- UPDATE.workflow.RollbackWorkflow
- UPDATE.workflow.ServiceItemActionDefinition
- UPDATE.workflow.ServiceItemActionInstance
- UPDATE.workflow.ServiceItemDefinition
- UPDATE.workflow.ServiceItemInstance
- UPDATE.workflow.ServiceItemOutput
- UPDATE.workflow.SshBatchExecutor
- UPDATE.workflow.TaskDefinition
- UPDATE.workflow.TaskInfo
- UPDATE.workflow.UiDisplayMetadata
- UPDATE.workflow.Variable
- UPDATE.workflow.WorkflowDefinition
- UPDATE.workflow.WorkflowInfo
- UPDATE.workload.Blueprint
- UPDATE.workload.WorkloadDefinition
- UPDATE.workload.WorkloadDeployment
- UPDATE.workload.WorkloadInstance
- UPDATE.workload.WorkloadMetadata
scopes:
- description: Create a 'aaa.RetentionPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.aaa.RetentionPolicy
- description: Create a 'access.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.access.Policy
- description: Create a 'adapter.ConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.adapter.ConfigPolicy
- description: Create a 'appliance.Backup' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.Backup
- description: Create a 'appliance.BackupPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.BackupPolicy
- description: Create a 'appliance.ClusterInfo' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.ClusterInfo
- description: Create a 'appliance.ClusterReplaceNode' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.ClusterReplaceNode
- description: Create a 'appliance.ClusterWorkerNode' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.ClusterWorkerNode
- description: Create a 'appliance.ClusterWorkerNodeReplace' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.ClusterWorkerNodeReplace
- description: Create a 'appliance.ClusterWorkerNodeReuse' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.ClusterWorkerNodeReuse
- description: Create a 'appliance.DataExportPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.DataExportPolicy
- description: Create a 'appliance.DeviceClaim' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.DeviceClaim
- description: Create a 'appliance.DiagSetting' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.DiagSetting
- description: Create a 'appliance.ExternalSyslogSetting' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.ExternalSyslogSetting
- description: Create a 'appliance.FqdnUpdate' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.FqdnUpdate
- description: Create a 'appliance.RemoteFileImport' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.RemoteFileImport
- description: Create a 'appliance.Restore' resource.
  flows:
  - clientCredentials
  scope: CREATE.appliance.Restore
- description: Create a 'asset.ClaimToken' resource.
  flows:
  - clientCredentials
  scope: CREATE.asset.ClaimToken
- description: Create a 'asset.DeviceClaim' resource.
  flows:
  - clientCredentials
  scope: CREATE.asset.DeviceClaim
- description: Create a 'asset.DeviceContractNotification' resource.
  flows:
  - clientCredentials
  scope: CREATE.asset.DeviceContractNotification
- description: Create a 'asset.GeoLocation' resource.
  flows:
  - clientCredentials
  scope: CREATE.asset.GeoLocation
- description: Create a 'asset.PreClaim' resource.
  flows:
  - clientCredentials
  scope: CREATE.asset.PreClaim
- description: Create a 'asset.Target' resource.
  flows:
  - clientCredentials
  scope: CREATE.asset.Target
- description: Create a 'auditd.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.auditd.Policy
- description: Create a 'bios.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.bios.Policy
- description: Create a 'boot.PrecisionPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.boot.PrecisionPolicy
- description: Create a 'bulk.Export' resource.
  flows:
  - clientCredentials
  scope: CREATE.bulk.Export
- description: Create a 'bulk.MoCloner' resource.
  flows:
  - clientCredentials
  scope: CREATE.bulk.MoCloner
- description: Create a 'bulk.MoDeepCloner' resource.
  flows:
  - clientCredentials
  scope: CREATE.bulk.MoDeepCloner
- description: Create a 'bulk.MoMerger' resource.
  flows:
  - clientCredentials
  scope: CREATE.bulk.MoMerger
- description: Create a 'bulk.Request' resource.
  flows:
  - clientCredentials
  scope: CREATE.bulk.Request
- description: Create a 'certificatemanagement.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.certificatemanagement.Policy
- description: Create a 'chassis.ConfigImport' resource.
  flows:
  - clientCredentials
  scope: CREATE.chassis.ConfigImport
- description: Create a 'chassis.Profile' resource.
  flows:
  - clientCredentials
  scope: CREATE.chassis.Profile
- description: Create a 'chassis.ProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: CREATE.chassis.ProfileTemplate
- description: Create a 'cli.CliPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.cli.CliPolicy
- description: Create a 'cloud.CollectInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.cloud.CollectInventory
- description: Create a 'comm.HttpProxyPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.comm.HttpProxyPolicy
- description: Create a 'comm.TagDefinition' resource.
  flows:
  - clientCredentials
  scope: CREATE.comm.TagDefinition
- description: Create a 'compute.HostUtilityOperation' resource.
  flows:
  - clientCredentials
  scope: CREATE.compute.HostUtilityOperation
- description: Create a 'compute.PcieConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.compute.PcieConnectivityPolicy
- description: Create a 'compute.ScrubPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.compute.ScrubPolicy
- description: Create a 'cond.AlarmRule' resource.
  flows:
  - clientCredentials
  scope: CREATE.cond.AlarmRule
- description: Create a 'cond.AlarmSuppression' resource.
  flows:
  - clientCredentials
  scope: CREATE.cond.AlarmSuppression
- description: Create a 'cond.AlarmSuppressionDryRun' resource.
  flows:
  - clientCredentials
  scope: CREATE.cond.AlarmSuppressionDryRun
- description: Create a 'cond.CustomHclBaseline' resource.
  flows:
  - clientCredentials
  scope: CREATE.cond.CustomHclBaseline
- description: Create a 'cond.CustomHclStatus' resource.
  flows:
  - clientCredentials
  scope: CREATE.cond.CustomHclStatus
- description: Create a 'cond.HclStatusJob' resource.
  flows:
  - clientCredentials
  scope: CREATE.cond.HclStatusJob
- description: Create a 'cond.ThresholdDefinition' resource.
  flows:
  - clientCredentials
  scope: CREATE.cond.ThresholdDefinition
- description: Create a 'connectorpack.ConnectorPackUpgrade' resource.
  flows:
  - clientCredentials
  scope: CREATE.connectorpack.ConnectorPackUpgrade
- description: Create a 'crd.CustomResource' resource.
  flows:
  - clientCredentials
  scope: CREATE.crd.CustomResource
- description: Create a 'deviceconnector.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.deviceconnector.Policy
- description: Create a 'energy.DailyMetrics' resource.
  flows:
  - clientCredentials
  scope: CREATE.energy.DailyMetrics
- description: Create a 'energy.Metrics' resource.
  flows:
  - clientCredentials
  scope: CREATE.energy.Metrics
- description: Create a 'externalsite.Authorization' resource.
  flows:
  - clientCredentials
  scope: CREATE.externalsite.Authorization
- description: Create a 'fabric.AppliancePcRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.AppliancePcRole
- description: Create a 'fabric.ApplianceRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.ApplianceRole
- description: Create a 'fabric.EstimateImpact' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.EstimateImpact
- description: Create a 'fabric.EthNetworkControlPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.EthNetworkControlPolicy
- description: Create a 'fabric.EthNetworkGroupPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.EthNetworkGroupPolicy
- description: Create a 'fabric.EthNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.EthNetworkPolicy
- description: Create a 'fabric.FcNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.FcNetworkPolicy
- description: Create a 'fabric.FcStorageRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.FcStorageRole
- description: Create a 'fabric.FcUplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.FcUplinkPcRole
- description: Create a 'fabric.FcUplinkRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.FcUplinkRole
- description: Create a 'fabric.FcZonePolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.FcZonePolicy
- description: Create a 'fabric.FcoeUplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.FcoeUplinkPcRole
- description: Create a 'fabric.FcoeUplinkRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.FcoeUplinkRole
- description: Create a 'fabric.FlowControlPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.FlowControlPolicy
- description: Create a 'fabric.LanPinGroup' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.LanPinGroup
- description: Create a 'fabric.LinkAggregationPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.LinkAggregationPolicy
- description: Create a 'fabric.LinkControlPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.LinkControlPolicy
- description: Create a 'fabric.MacSecPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.MacSecPolicy
- description: Create a 'fabric.MulticastPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.MulticastPolicy
- description: Create a 'fabric.NetFlowExporter' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.NetFlowExporter
- description: Create a 'fabric.NetFlowMonitor' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.NetFlowMonitor
- description: Create a 'fabric.NetFlowPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.NetFlowPolicy
- description: Create a 'fabric.NetFlowRecord' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.NetFlowRecord
- description: Create a 'fabric.PcOperation' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.PcOperation
- description: Create a 'fabric.PortMode' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.PortMode
- description: Create a 'fabric.PortOperation' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.PortOperation
- description: Create a 'fabric.PortPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.PortPolicy
- description: Create a 'fabric.SanPinGroup' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SanPinGroup
- description: Create a 'fabric.SecureRouterRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SecureRouterRole
- description: Create a 'fabric.ServerRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.ServerRole
- description: Create a 'fabric.SpanDestEthPort' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SpanDestEthPort
- description: Create a 'fabric.SpanSession' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SpanSession
- description: Create a 'fabric.SpanSourceEthPort' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SpanSourceEthPort
- description: Create a 'fabric.SpanSourceEthPortChannel' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SpanSourceEthPortChannel
- description: Create a 'fabric.SpanSourceVlan' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SpanSourceVlan
- description: Create a 'fabric.SpanSourceVnicEthIf' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SpanSourceVnicEthIf
- description: Create a 'fabric.SwitchClusterProfile' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SwitchClusterProfile
- description: Create a 'fabric.SwitchClusterProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SwitchClusterProfileTemplate
- description: Create a 'fabric.SwitchControlPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SwitchControlPolicy
- description: Create a 'fabric.SwitchProfile' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SwitchProfile
- description: Create a 'fabric.SwitchProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SwitchProfileTemplate
- description: Create a 'fabric.SystemQosPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.SystemQosPolicy
- description: Create a 'fabric.UplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.UplinkPcRole
- description: Create a 'fabric.UplinkRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.UplinkRole
- description: Create a 'fabric.Vlan' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.Vlan
- description: Create a 'fabric.Vsan' resource.
  flows:
  - clientCredentials
  scope: CREATE.fabric.Vsan
- description: Create a 'fcpool.Pool' resource.
  flows:
  - clientCredentials
  scope: CREATE.fcpool.Pool
- description: Create a 'fcpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: CREATE.fcpool.Reservation
- description: Create a 'feedback.FeedbackPost' resource.
  flows:
  - clientCredentials
  scope: CREATE.feedback.FeedbackPost
- description: Create a 'firmware.ChassisUpgrade' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.ChassisUpgrade
- description: Create a 'firmware.Distributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.Distributable
- description: Create a 'firmware.DriverDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.DriverDistributable
- description: Create a 'firmware.Eula' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.Eula
- description: Create a 'firmware.PciNodeUpgrade' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.PciNodeUpgrade
- description: Create a 'firmware.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.Policy
- description: Create a 'firmware.SecureRouterUpgrade' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.SecureRouterUpgrade
- description: Create a 'firmware.ServerConfigurationUtilityDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.ServerConfigurationUtilityDistributable
- description: Create a 'firmware.SwitchUpgrade' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.SwitchUpgrade
- description: Create a 'firmware.UnsupportedVersionUpgrade' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.UnsupportedVersionUpgrade
- description: Create a 'firmware.Upgrade' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.Upgrade
- description: Create a 'firmware.UpgradeImpact' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.UpgradeImpact
- description: Create a 'firmware.UpgradeValidity' resource.
  flows:
  - clientCredentials
  scope: CREATE.firmware.UpgradeValidity
- description: Create a 'hcl.CompatibilityStatus' resource.
  flows:
  - clientCredentials
  scope: CREATE.hcl.CompatibilityStatus
- description: Create a 'hcl.SupportedDriverName' resource.
  flows:
  - clientCredentials
  scope: CREATE.hcl.SupportedDriverName
- description: Create a 'hyperflex.AutoSupportPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.AutoSupportPolicy
- description: Create a 'hyperflex.CapabilityInfo' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.CapabilityInfo
- description: Create a 'hyperflex.ClusterBackupPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ClusterBackupPolicy
- description: Create a 'hyperflex.ClusterBackupPolicyDeployment' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ClusterBackupPolicyDeployment
- description: Create a 'hyperflex.ClusterNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ClusterNetworkPolicy
- description: Create a 'hyperflex.ClusterProfile' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ClusterProfile
- description: Create a 'hyperflex.ClusterReplicationNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ClusterReplicationNetworkPolicy
- description: Create a 'hyperflex.ClusterReplicationNetworkPolicyDeployment' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ClusterReplicationNetworkPolicyDeployment
- description: Create a 'hyperflex.ClusterStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ClusterStoragePolicy
- description: Create a 'hyperflex.ExtFcStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ExtFcStoragePolicy
- description: Create a 'hyperflex.ExtIscsiStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ExtIscsiStoragePolicy
- description: Create a 'hyperflex.KeyEncryptionKey' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.KeyEncryptionKey
- description: Create a 'hyperflex.LocalCredentialPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.LocalCredentialPolicy
- description: Create a 'hyperflex.NodeConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.NodeConfigPolicy
- description: Create a 'hyperflex.NodeProfile' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.NodeProfile
- description: Create a 'hyperflex.ProxySettingPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ProxySettingPolicy
- description: Create a 'hyperflex.ReduceReSync' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ReduceReSync
- description: Create a 'hyperflex.ServiceAuthToken' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.ServiceAuthToken
- description: Create a 'hyperflex.SoftwareVersionPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.SoftwareVersionPolicy
- description: Create a 'hyperflex.StartReduceReSync' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.StartReduceReSync
- description: Create a 'hyperflex.SysConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.SysConfigPolicy
- description: Create a 'hyperflex.UcsmConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.UcsmConfigPolicy
- description: Create a 'hyperflex.VcenterConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.VcenterConfigPolicy
- description: Create a 'hyperflex.VmImportOperation' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.VmImportOperation
- description: Create a 'hyperflex.VmRestoreOperation' resource.
  flows:
  - clientCredentials
  scope: CREATE.hyperflex.VmRestoreOperation
- description: Create a 'iam.Account' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.Account
- description: Create a 'iam.ApiKey' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.ApiKey
- description: Create a 'iam.AppRegistration' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.AppRegistration
- description: Create a 'iam.Certificate' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.Certificate
- description: Create a 'iam.CertificateRequest' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.CertificateRequest
- description: Create a 'iam.CuiIntegration' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.CuiIntegration
- description: Create a 'iam.DomainNameInfo' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.DomainNameInfo
- description: Create a 'iam.EndPointUser' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.EndPointUser
- description: Create a 'iam.EndPointUserPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.EndPointUserPolicy
- description: Create a 'iam.EndPointUserRole' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.EndPointUserRole
- description: Create a 'iam.GuestAccessSettings' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.GuestAccessSettings
- description: Create a 'iam.Idp' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.Idp
- description: Create a 'iam.IpAccessManagement' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.IpAccessManagement
- description: Create a 'iam.IpAddress' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.IpAddress
- description: Create a 'iam.LdapGroup' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.LdapGroup
- description: Create a 'iam.LdapPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.LdapPolicy
- description: Create a 'iam.LdapProvider' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.LdapProvider
- description: Create a 'iam.LocalUserPassword' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.LocalUserPassword
- description: Create a 'iam.Permission' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.Permission
- description: Create a 'iam.PrivateKeySpec' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.PrivateKeySpec
- description: Create a 'iam.PrivilegeSet' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.PrivilegeSet
- description: Create a 'iam.PrivilegeSetMetaInfo' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.PrivilegeSetMetaInfo
- description: Create a 'iam.Qualifier' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.Qualifier
- description: Create a 'iam.ResourceRoles' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.ResourceRoles
- description: Create a 'iam.SessionLimits' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.SessionLimits
- description: Create a 'iam.SharingRule' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.SharingRule
- description: Create a 'iam.TrustPoint' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.TrustPoint
- description: Create a 'iam.User' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.User
- description: Create a 'iam.UserGroup' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.UserGroup
- description: Create a 'iam.UserQualifier' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.UserQualifier
- description: Create a 'iam.UserSetting' resource.
  flows:
  - clientCredentials
  scope: CREATE.iam.UserSetting
- description: Create a 'inventory.Request' resource.
  flows:
  - clientCredentials
  scope: CREATE.inventory.Request
- description: Create a 'ipmioverlan.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.ipmioverlan.Policy
- description: Create a 'ippool.Pool' resource.
  flows:
  - clientCredentials
  scope: CREATE.ippool.Pool
- description: Create a 'ippool.Reservation' resource.
  flows:
  - clientCredentials
  scope: CREATE.ippool.Reservation
- description: Create a 'iqnpool.Pool' resource.
  flows:
  - clientCredentials
  scope: CREATE.iqnpool.Pool
- description: Create a 'iqnpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: CREATE.iqnpool.Reservation
- description: Create a 'iwotenant.Migrate' resource.
  flows:
  - clientCredentials
  scope: CREATE.iwotenant.Migrate
- description: Create a 'iwotenant.TenantCustomization' resource.
  flows:
  - clientCredentials
  scope: CREATE.iwotenant.TenantCustomization
- description: Create a 'kvm.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.kvm.Policy
- description: Create a 'kvm.Session' resource.
  flows:
  - clientCredentials
  scope: CREATE.kvm.Session
- description: Create a 'kvm.Tunnel' resource.
  flows:
  - clientCredentials
  scope: CREATE.kvm.Tunnel
- description: Create a 'kvm.TunneledKvmPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.kvm.TunneledKvmPolicy
- description: Create a 'license.ErpLicenseCount' resource.
  flows:
  - clientCredentials
  scope: CREATE.license.ErpLicenseCount
- description: Create a 'license.IksLicenseCount' resource.
  flows:
  - clientCredentials
  scope: CREATE.license.IksLicenseCount
- description: Create a 'license.IncLicenseCount' resource.
  flows:
  - clientCredentials
  scope: CREATE.license.IncLicenseCount
- description: Create a 'license.IwoLicenseCount' resource.
  flows:
  - clientCredentials
  scope: CREATE.license.IwoLicenseCount
- description: Create a 'license.LicenseInfo' resource.
  flows:
  - clientCredentials
  scope: CREATE.license.LicenseInfo
- description: Create a 'license.LicenseReservationOp' resource.
  flows:
  - clientCredentials
  scope: CREATE.license.LicenseReservationOp
- description: Create a 'macpool.Pool' resource.
  flows:
  - clientCredentials
  scope: CREATE.macpool.Pool
- description: Create a 'macpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: CREATE.macpool.Reservation
- description: Create a 'memory.PersistentMemoryPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.memory.PersistentMemoryPolicy
- description: Create a 'memory.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.memory.Policy
- description: Create a 'metrics.MetricsExploration' resource.
  flows:
  - clientCredentials
  scope: CREATE.metrics.MetricsExploration
- description: Create a 'metrics.ResourceConfiguration' resource.
  flows:
  - clientCredentials
  scope: CREATE.metrics.ResourceConfiguration
- description: Create a 'mgmt.ConfigBackupFile' resource.
  flows:
  - clientCredentials
  scope: CREATE.mgmt.ConfigBackupFile
- description: Create a 'mgmt.ConfigBackupOperation' resource.
  flows:
  - clientCredentials
  scope: CREATE.mgmt.ConfigBackupOperation
- description: Create a 'mgmt.ConfigOperationSetting' resource.
  flows:
  - clientCredentials
  scope: CREATE.mgmt.ConfigOperationSetting
- description: Create a 'mgmt.ConfigRestoreOperation' resource.
  flows:
  - clientCredentials
  scope: CREATE.mgmt.ConfigRestoreOperation
- description: Create a 'networkconfig.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.networkconfig.Policy
- description: Create a 'notification.AccountSubscription' resource.
  flows:
  - clientCredentials
  scope: CREATE.notification.AccountSubscription
- description: Create a 'ntp.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.ntp.Policy
- description: Create a 'oauth.Authorization' resource.
  flows:
  - clientCredentials
  scope: CREATE.oauth.Authorization
- description: Create a 'openapi.OpenApiSpecification' resource.
  flows:
  - clientCredentials
  scope: CREATE.openapi.OpenApiSpecification
- description: Create a 'openapi.ProcessFile' resource.
  flows:
  - clientCredentials
  scope: CREATE.openapi.ProcessFile
- description: Create a 'openapi.TaskGenerationRequest' resource.
  flows:
  - clientCredentials
  scope: CREATE.openapi.TaskGenerationRequest
- description: Create a 'oprs.Deployment' resource.
  flows:
  - clientCredentials
  scope: CREATE.oprs.Deployment
- description: Create a 'oprs.SyncTargetListMessage' resource.
  flows:
  - clientCredentials
  scope: CREATE.oprs.SyncTargetListMessage
- description: Create a 'organization.Organization' resource.
  flows:
  - clientCredentials
  scope: CREATE.organization.Organization
- description: Create a 'os.BulkInstallInfo' resource.
  flows:
  - clientCredentials
  scope: CREATE.os.BulkInstallInfo
- description: Create a 'os.ConfigurationFile' resource.
  flows:
  - clientCredentials
  scope: CREATE.os.ConfigurationFile
- description: Create a 'os.Install' resource.
  flows:
  - clientCredentials
  scope: CREATE.os.Install
- description: Create a 'os.OsSupport' resource.
  flows:
  - clientCredentials
  scope: CREATE.os.OsSupport
- description: Create a 'os.TemplateFile' resource.
  flows:
  - clientCredentials
  scope: CREATE.os.TemplateFile
- description: Create a 'os.ValidInstallTarget' resource.
  flows:
  - clientCredentials
  scope: CREATE.os.ValidInstallTarget
- description: Create a 'partnerintegration.DeviceConnector' resource.
  flows:
  - clientCredentials
  scope: CREATE.partnerintegration.DeviceConnector
- description: Create a 'partnerintegration.Etl' resource.
  flows:
  - clientCredentials
  scope: CREATE.partnerintegration.Etl
- description: Create a 'partnerintegration.File' resource.
  flows:
  - clientCredentials
  scope: CREATE.partnerintegration.File
- description: Create a 'partnerintegration.Inventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.partnerintegration.Inventory
- description: Create a 'partnerintegration.Metrics' resource.
  flows:
  - clientCredentials
  scope: CREATE.partnerintegration.Metrics
- description: Create a 'partnerintegration.Model' resource.
  flows:
  - clientCredentials
  scope: CREATE.partnerintegration.Model
- description: Create a 'pool.IdMappingPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.pool.IdMappingPolicy
- description: Create a 'power.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.power.Policy
- description: Create a 'power.PowerGroup' resource.
  flows:
  - clientCredentials
  scope: CREATE.power.PowerGroup
- description: Create a 'recommendation.HardwareExpansionRequest' resource.
  flows:
  - clientCredentials
  scope: CREATE.recommendation.HardwareExpansionRequest
- description: Create a 'recommendation.HardwareExpansionRequestItem' resource.
  flows:
  - clientCredentials
  scope: CREATE.recommendation.HardwareExpansionRequestItem
- description: Create a 'recommendation.PurchaseOrderEstimate' resource.
  flows:
  - clientCredentials
  scope: CREATE.recommendation.PurchaseOrderEstimate
- description: Create a 'recovery.BackupConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.recovery.BackupConfigPolicy
- description: Create a 'recovery.BackupProfile' resource.
  flows:
  - clientCredentials
  scope: CREATE.recovery.BackupProfile
- description: Create a 'recovery.OnDemandBackup' resource.
  flows:
  - clientCredentials
  scope: CREATE.recovery.OnDemandBackup
- description: Create a 'recovery.Restore' resource.
  flows:
  - clientCredentials
  scope: CREATE.recovery.Restore
- description: Create a 'recovery.ScheduleConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.recovery.ScheduleConfigPolicy
- description: Create a 'resource.Group' resource.
  flows:
  - clientCredentials
  scope: CREATE.resource.Group
- description: Create a 'resource.Reservation' resource.
  flows:
  - clientCredentials
  scope: CREATE.resource.Reservation
- description: Create a 'resource.SelectionCriteria' resource.
  flows:
  - clientCredentials
  scope: CREATE.resource.SelectionCriteria
- description: Create a 'resourcepool.Pool' resource.
  flows:
  - clientCredentials
  scope: CREATE.resourcepool.Pool
- description: Create a 'resourcepool.QualificationPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.resourcepool.QualificationPolicy
- description: Create a 'resourcepool.Reservation' resource.
  flows:
  - clientCredentials
  scope: CREATE.resourcepool.Reservation
- description: Create a 'rproxy.ReverseProxy' resource.
  flows:
  - clientCredentials
  scope: CREATE.rproxy.ReverseProxy
- description: Create a 'scheduler.SchedulePolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.scheduler.SchedulePolicy
- description: Create a 'scheduler.TaskSchedule' resource.
  flows:
  - clientCredentials
  scope: CREATE.scheduler.TaskSchedule
- description: Create a 'sdaaci.Connection' resource.
  flows:
  - clientCredentials
  scope: CREATE.sdaaci.Connection
- description: Create a 'sdaaci.ConnectionDetail' resource.
  flows:
  - clientCredentials
  scope: CREATE.sdaaci.ConnectionDetail
- description: Create a 'sdcard.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.sdcard.Policy
- description: ''
  flows: []
  scope: CREATE.search.SuggestItem
- description: Create a 'server.ConfigImport' resource.
  flows:
  - clientCredentials
  scope: CREATE.server.ConfigImport
- description: Create a 'server.DiagnosticStatus' resource.
  flows:
  - clientCredentials
  scope: CREATE.server.DiagnosticStatus
- description: Create a 'server.Diagnostics' resource.
  flows:
  - clientCredentials
  scope: CREATE.server.Diagnostics
- description: Create a 'server.Profile' resource.
  flows:
  - clientCredentials
  scope: CREATE.server.Profile
- description: Create a 'server.ProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: CREATE.server.ProfileTemplate
- description: Create a 'smtp.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.smtp.Policy
- description: Create a 'smtp.PolicyTest' resource.
  flows:
  - clientCredentials
  scope: CREATE.smtp.PolicyTest
- description: Create a 'snmp.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.snmp.Policy
- description: Create a 'software.ApplianceDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.ApplianceDistributable
- description: Create a 'software.HciBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.HciBundleDistributable
- description: Create a 'software.HciDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.HciDistributable
- description: Create a 'software.HyperflexBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.HyperflexBundleDistributable
- description: Create a 'software.HyperflexDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.HyperflexDistributable
- description: Create a 'software.IksBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.IksBundleDistributable
- description: Create a 'software.ReleaseMeta' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.ReleaseMeta
- description: Create a 'software.SolutionDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.SolutionDistributable
- description: Create a 'software.UcsdBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.UcsdBundleDistributable
- description: Create a 'software.UcsdDistributable' resource.
  flows:
  - clientCredentials
  scope: CREATE.software.UcsdDistributable
- description: Create a 'softwarerepository.Authorization' resource.
  flows:
  - clientCredentials
  scope: CREATE.softwarerepository.Authorization
- description: Create a 'softwarerepository.OperatingSystemFile' resource.
  flows:
  - clientCredentials
  scope: CREATE.softwarerepository.OperatingSystemFile
- description: Create a 'sol.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.sol.Policy
- description: Create a 'ssh.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.ssh.Policy
- description: Create a 'storage.DriveGroup' resource.
  flows:
  - clientCredentials
  scope: CREATE.storage.DriveGroup
- description: Create a 'storage.DriveSecurityPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.storage.DriveSecurityPolicy
- description: Create a 'storage.StoragePolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.storage.StoragePolicy
- description: Create a 'syslog.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.syslog.Policy
- description: Create a 'tam.AdvisoryInfo' resource.
  flows:
  - clientCredentials
  scope: CREATE.tam.AdvisoryInfo
- description: Create a 'task.CatalystSdwanScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.CatalystSdwanScopedInventory
- description: Create a 'task.FabricMosScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.FabricMosScopedInventory
- description: Create a 'task.HciScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.HciScopedInventory
- description: Create a 'task.HitachiScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.HitachiScopedInventory
- description: Create a 'task.HyperFlexManagementScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.HyperFlexManagementScopedInventory
- description: Create a 'task.HyperflexScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.HyperflexScopedInventory
- description: Create a 'task.MdsScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.MdsScopedInventory
- description: Create a 'task.MdsSystemScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.MdsSystemScopedInventory
- description: Create a 'task.MerakiScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.MerakiScopedInventory
- description: Create a 'task.NetAppScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.NetAppScopedInventory
- description: Create a 'task.NexusScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.NexusScopedInventory
- description: Create a 'task.NexusSystemScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.NexusSystemScopedInventory
- description: Create a 'task.NexusVlanScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.NexusVlanScopedInventory
- description: Create a 'task.PureFlashBladeScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.PureFlashBladeScopedInventory
- description: Create a 'task.PureScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.PureScopedInventory
- description: Create a 'task.ServerScopedInventory' resource.
  flows:
  - clientCredentials
  scope: CREATE.task.ServerScopedInventory
- description: Create a 'techsupportmanagement.CollectionControlPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.techsupportmanagement.CollectionControlPolicy
- description: Create a 'techsupportmanagement.TechSupportBundle' resource.
  flows:
  - clientCredentials
  scope: CREATE.techsupportmanagement.TechSupportBundle
- description: ''
  flows: []
  scope: CREATE.telemetry.TimeSeries
- description: Create a 'thermal.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.thermal.Policy
- description: Create a 'uuidpool.Pool' resource.
  flows:
  - clientCredentials
  scope: CREATE.uuidpool.Pool
- description: Create a 'uuidpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: CREATE.uuidpool.Reservation
- description: Create a 'virtualization.EsxiConsole' resource.
  flows:
  - clientCredentials
  scope: CREATE.virtualization.EsxiConsole
- description: Create a 'virtualization.VirtualMachine' resource.
  flows:
  - clientCredentials
  scope: CREATE.virtualization.VirtualMachine
- description: Create a 'vmedia.Policy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vmedia.Policy
- description: Create a 'vmrc.Console' resource.
  flows:
  - clientCredentials
  scope: CREATE.vmrc.Console
- description: Create a 'vnic.EthAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.EthAdapterPolicy
- description: Create a 'vnic.EthIf' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.EthIf
- description: Create a 'vnic.EthNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.EthNetworkPolicy
- description: Create a 'vnic.EthQosPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.EthQosPolicy
- description: Create a 'vnic.FcAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.FcAdapterPolicy
- description: Create a 'vnic.FcIf' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.FcIf
- description: Create a 'vnic.FcNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.FcNetworkPolicy
- description: Create a 'vnic.FcQosPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.FcQosPolicy
- description: Create a 'vnic.IscsiAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.IscsiAdapterPolicy
- description: Create a 'vnic.IscsiBootPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.IscsiBootPolicy
- description: Create a 'vnic.IscsiStaticTargetPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.IscsiStaticTargetPolicy
- description: Create a 'vnic.LanConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.LanConnectivityPolicy
- description: Create a 'vnic.SanConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.SanConnectivityPolicy
- description: Create a 'vnic.VhbaTemplate' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.VhbaTemplate
- description: Create a 'vnic.VnicTemplate' resource.
  flows:
  - clientCredentials
  scope: CREATE.vnic.VnicTemplate
- description: Create a 'vrf.Vrf' resource.
  flows:
  - clientCredentials
  scope: CREATE.vrf.Vrf
- description: Create a 'webhook.Endpoint' resource.
  flows:
  - clientCredentials
  scope: CREATE.webhook.Endpoint
- description: Create a 'webhook.Schema' resource.
  flows:
  - clientCredentials
  scope: CREATE.webhook.Schema
- description: Create a 'workflow.AnsibleBatchExecutor' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.AnsibleBatchExecutor
- description: Create a 'workflow.BatchApiExecutor' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.BatchApiExecutor
- description: Create a 'workflow.CatalogItemDefinition' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.CatalogItemDefinition
- description: Create a 'workflow.CatalogServiceRequest' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.CatalogServiceRequest
- description: Create a 'workflow.CustomDataTypeDefinition' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.CustomDataTypeDefinition
- description: Create a 'workflow.ErrorResponseHandler' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.ErrorResponseHandler
- description: Create a 'workflow.PowerShellBatchApiExecutor' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.PowerShellBatchApiExecutor
- description: Create a 'workflow.RollbackWorkflow' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.RollbackWorkflow
- description: Create a 'workflow.ServiceItemActionDefinition' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.ServiceItemActionDefinition
- description: Create a 'workflow.ServiceItemActionInstance' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.ServiceItemActionInstance
- description: Create a 'workflow.ServiceItemDefinition' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.ServiceItemDefinition
- description: Create a 'workflow.ServiceItemInstance' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.ServiceItemInstance
- description: Create a 'workflow.ServiceItemOutput' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.ServiceItemOutput
- description: Create a 'workflow.SshBatchExecutor' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.SshBatchExecutor
- description: Create a 'workflow.TaskDefinition' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.TaskDefinition
- description: Create a 'workflow.TemplateEvaluation' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.TemplateEvaluation
- description: Create a 'workflow.TemplateParser' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.TemplateParser
- description: Create a 'workflow.UiDisplayMetadata' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.UiDisplayMetadata
- description: Create a 'workflow.Variable' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.Variable
- description: Create a 'workflow.WorkflowDefinition' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.WorkflowDefinition
- description: Create a 'workflow.WorkflowInfo' resource.
  flows:
  - clientCredentials
  scope: CREATE.workflow.WorkflowInfo
- description: Create a 'workload.Blueprint' resource.
  flows:
  - clientCredentials
  scope: CREATE.workload.Blueprint
- description: Create a 'workload.ClearWorkloadTag' resource.
  flows:
  - clientCredentials
  scope: CREATE.workload.ClearWorkloadTag
- description: Create a 'workload.WorkloadDefinition' resource.
  flows:
  - clientCredentials
  scope: CREATE.workload.WorkloadDefinition
- description: Create a 'workload.WorkloadDeployment' resource.
  flows:
  - clientCredentials
  scope: CREATE.workload.WorkloadDeployment
- description: Delete a 'access.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.access.Policy
- description: Delete a 'adapter.ConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.adapter.ConfigPolicy
- description: Delete a 'appliance.Backup' resource.
  flows:
  - clientCredentials
  scope: DELETE.appliance.Backup
- description: Delete a 'appliance.ClusterInfo' resource.
  flows:
  - clientCredentials
  scope: DELETE.appliance.ClusterInfo
- description: Delete a 'appliance.ExternalSyslogSetting' resource.
  flows:
  - clientCredentials
  scope: DELETE.appliance.ExternalSyslogSetting
- description: Delete a 'appliance.Restore' resource.
  flows:
  - clientCredentials
  scope: DELETE.appliance.Restore
- description: Delete a 'appliance.Upgrade' resource.
  flows:
  - clientCredentials
  scope: DELETE.appliance.Upgrade
- description: Delete a 'asset.ClaimToken' resource.
  flows:
  - clientCredentials
  scope: DELETE.asset.ClaimToken
- description: Delete a 'asset.DeviceClaim' resource.
  flows:
  - clientCredentials
  scope: DELETE.asset.DeviceClaim
- description: Delete a 'asset.GeoLocation' resource.
  flows:
  - clientCredentials
  scope: DELETE.asset.GeoLocation
- description: Delete a 'asset.Target' resource.
  flows:
  - clientCredentials
  scope: DELETE.asset.Target
- description: Delete a 'auditd.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.auditd.Policy
- description: Delete a 'bios.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.bios.Policy
- description: Delete a 'boot.PrecisionPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.boot.PrecisionPolicy
- description: Delete a 'bulk.Export' resource.
  flows:
  - clientCredentials
  scope: DELETE.bulk.Export
- description: Delete a 'certificatemanagement.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.certificatemanagement.Policy
- description: Delete a 'chassis.Profile' resource.
  flows:
  - clientCredentials
  scope: DELETE.chassis.Profile
- description: Delete a 'chassis.ProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: DELETE.chassis.ProfileTemplate
- description: Delete a 'cli.CliPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.cli.CliPolicy
- description: Delete a 'comm.HttpProxyPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.comm.HttpProxyPolicy
- description: Delete a 'comm.TagDefinition' resource.
  flows:
  - clientCredentials
  scope: DELETE.comm.TagDefinition
- description: Delete a 'compute.PcieConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.compute.PcieConnectivityPolicy
- description: Delete a 'compute.RackUnit' resource.
  flows:
  - clientCredentials
  scope: DELETE.compute.RackUnit
- description: Delete a 'compute.RackUnitIdentity' resource.
  flows:
  - clientCredentials
  scope: DELETE.compute.RackUnitIdentity
- description: Delete a 'compute.ScrubPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.compute.ScrubPolicy
- description: Delete a 'compute.ServerPowerPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.compute.ServerPowerPolicy
- description: Delete a 'cond.AlarmRule' resource.
  flows:
  - clientCredentials
  scope: DELETE.cond.AlarmRule
- description: Delete a 'cond.AlarmSuppression' resource.
  flows:
  - clientCredentials
  scope: DELETE.cond.AlarmSuppression
- description: Delete a 'cond.CustomHclBaseline' resource.
  flows:
  - clientCredentials
  scope: DELETE.cond.CustomHclBaseline
- description: Delete a 'cond.ThresholdDefinition' resource.
  flows:
  - clientCredentials
  scope: DELETE.cond.ThresholdDefinition
- description: Delete a 'connectorpack.ConnectorPackUpgrade' resource.
  flows:
  - clientCredentials
  scope: DELETE.connectorpack.ConnectorPackUpgrade
- description: Delete a 'coremanagement.CoreFile' resource.
  flows:
  - clientCredentials
  scope: DELETE.coremanagement.CoreFile
- description: Delete a 'crd.CustomResource' resource.
  flows:
  - clientCredentials
  scope: DELETE.crd.CustomResource
- description: Delete a 'deviceconnector.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.deviceconnector.Policy
- description: Delete a 'fabric.AppliancePcRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.AppliancePcRole
- description: Delete a 'fabric.ApplianceRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.ApplianceRole
- description: Delete a 'fabric.EthNetworkControlPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.EthNetworkControlPolicy
- description: Delete a 'fabric.EthNetworkGroupPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.EthNetworkGroupPolicy
- description: Delete a 'fabric.EthNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.EthNetworkPolicy
- description: Delete a 'fabric.FcNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.FcNetworkPolicy
- description: Delete a 'fabric.FcStorageRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.FcStorageRole
- description: Delete a 'fabric.FcUplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.FcUplinkPcRole
- description: Delete a 'fabric.FcUplinkRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.FcUplinkRole
- description: Delete a 'fabric.FcZonePolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.FcZonePolicy
- description: Delete a 'fabric.FcoeUplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.FcoeUplinkPcRole
- description: Delete a 'fabric.FcoeUplinkRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.FcoeUplinkRole
- description: Delete a 'fabric.FlowControlPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.FlowControlPolicy
- description: Delete a 'fabric.LanPinGroup' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.LanPinGroup
- description: Delete a 'fabric.LinkAggregationPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.LinkAggregationPolicy
- description: Delete a 'fabric.LinkControlPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.LinkControlPolicy
- description: Delete a 'fabric.MacSecPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.MacSecPolicy
- description: Delete a 'fabric.MulticastPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.MulticastPolicy
- description: Delete a 'fabric.NetFlowExporter' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.NetFlowExporter
- description: Delete a 'fabric.NetFlowMonitor' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.NetFlowMonitor
- description: Delete a 'fabric.NetFlowPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.NetFlowPolicy
- description: Delete a 'fabric.NetFlowRecord' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.NetFlowRecord
- description: Delete a 'fabric.PcOperation' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.PcOperation
- description: Delete a 'fabric.PortMode' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.PortMode
- description: Delete a 'fabric.PortOperation' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.PortOperation
- description: Delete a 'fabric.PortPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.PortPolicy
- description: Delete a 'fabric.SanPinGroup' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SanPinGroup
- description: Delete a 'fabric.SecureRouterRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SecureRouterRole
- description: Delete a 'fabric.ServerRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.ServerRole
- description: Delete a 'fabric.SpanDestEthPort' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SpanDestEthPort
- description: Delete a 'fabric.SpanSession' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SpanSession
- description: Delete a 'fabric.SpanSourceEthPort' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SpanSourceEthPort
- description: Delete a 'fabric.SpanSourceEthPortChannel' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SpanSourceEthPortChannel
- description: Delete a 'fabric.SpanSourceVlan' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SpanSourceVlan
- description: Delete a 'fabric.SpanSourceVnicEthIf' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SpanSourceVnicEthIf
- description: Delete a 'fabric.SwitchClusterProfile' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SwitchClusterProfile
- description: Delete a 'fabric.SwitchClusterProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SwitchClusterProfileTemplate
- description: Delete a 'fabric.SwitchControlPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SwitchControlPolicy
- description: Delete a 'fabric.SwitchProfile' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SwitchProfile
- description: Delete a 'fabric.SwitchProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SwitchProfileTemplate
- description: Delete a 'fabric.SystemQosPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.SystemQosPolicy
- description: Delete a 'fabric.UplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.UplinkPcRole
- description: Delete a 'fabric.UplinkRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.UplinkRole
- description: Delete a 'fabric.Vlan' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.Vlan
- description: Delete a 'fabric.Vsan' resource.
  flows:
  - clientCredentials
  scope: DELETE.fabric.Vsan
- description: Delete a 'fcpool.Lease' resource.
  flows:
  - clientCredentials
  scope: DELETE.fcpool.Lease
- description: Delete a 'fcpool.Pool' resource.
  flows:
  - clientCredentials
  scope: DELETE.fcpool.Pool
- description: Delete a 'fcpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: DELETE.fcpool.Reservation
- description: Delete a 'firmware.ChassisUpgrade' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.ChassisUpgrade
- description: Delete a 'firmware.Distributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.Distributable
- description: Delete a 'firmware.DriverDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.DriverDistributable
- description: Delete a 'firmware.PciNodeUpgrade' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.PciNodeUpgrade
- description: Delete a 'firmware.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.Policy
- description: Delete a 'firmware.SecureRouterUpgrade' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.SecureRouterUpgrade
- description: Delete a 'firmware.ServerConfigurationUtilityDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.ServerConfigurationUtilityDistributable
- description: Delete a 'firmware.SwitchUpgrade' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.SwitchUpgrade
- description: Delete a 'firmware.UnsupportedVersionUpgrade' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.UnsupportedVersionUpgrade
- description: Delete a 'firmware.Upgrade' resource.
  flows:
  - clientCredentials
  scope: DELETE.firmware.Upgrade
- description: Delete a 'hyperflex.AutoSupportPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.AutoSupportPolicy
- description: Delete a 'hyperflex.BackupCluster' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.BackupCluster
- description: Delete a 'hyperflex.ClusterBackupPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ClusterBackupPolicy
- description: Delete a 'hyperflex.ClusterBackupPolicyDeployment' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ClusterBackupPolicyDeployment
- description: Delete a 'hyperflex.ClusterBackupPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ClusterBackupPolicyInventory
- description: Delete a 'hyperflex.ClusterNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ClusterNetworkPolicy
- description: Delete a 'hyperflex.ClusterProfile' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ClusterProfile
- description: Delete a 'hyperflex.ClusterReplicationNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ClusterReplicationNetworkPolicy
- description: Delete a 'hyperflex.ClusterReplicationNetworkPolicyDeployment' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ClusterReplicationNetworkPolicyDeployment
- description: Delete a 'hyperflex.ClusterStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ClusterStoragePolicy
- description: Delete a 'hyperflex.ExtFcStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ExtFcStoragePolicy
- description: Delete a 'hyperflex.ExtIscsiStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ExtIscsiStoragePolicy
- description: Delete a 'hyperflex.KeyEncryptionKey' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.KeyEncryptionKey
- description: Delete a 'hyperflex.LocalCredentialPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.LocalCredentialPolicy
- description: Delete a 'hyperflex.NodeConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.NodeConfigPolicy
- description: Delete a 'hyperflex.NodeProfile' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.NodeProfile
- description: Delete a 'hyperflex.ProxySettingPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ProxySettingPolicy
- description: Delete a 'hyperflex.ServiceAuthToken' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.ServiceAuthToken
- description: Delete a 'hyperflex.SoftwareVersionPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.SoftwareVersionPolicy
- description: Delete a 'hyperflex.SysConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.SysConfigPolicy
- description: Delete a 'hyperflex.UcsmConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.UcsmConfigPolicy
- description: Delete a 'hyperflex.VcenterConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.VcenterConfigPolicy
- description: Delete a 'hyperflex.VmBackupInfo' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.VmBackupInfo
- description: Delete a 'hyperflex.VmImportOperation' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.VmImportOperation
- description: Delete a 'hyperflex.VmRestoreOperation' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.VmRestoreOperation
- description: Delete a 'hyperflex.VmSnapshotInfo' resource.
  flows:
  - clientCredentials
  scope: DELETE.hyperflex.VmSnapshotInfo
- description: Delete a 'iam.Account' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.Account
- description: Delete a 'iam.ApiKey' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.ApiKey
- description: Delete a 'iam.AppRegistration' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.AppRegistration
- description: Delete a 'iam.Certificate' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.Certificate
- description: Delete a 'iam.CertificateRequest' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.CertificateRequest
- description: Delete a 'iam.DomainNameInfo' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.DomainNameInfo
- description: Delete a 'iam.EndPointUser' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.EndPointUser
- description: Delete a 'iam.EndPointUserPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.EndPointUserPolicy
- description: Delete a 'iam.EndPointUserRole' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.EndPointUserRole
- description: Delete a 'iam.GuestAccessSettings' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.GuestAccessSettings
- description: Delete a 'iam.Idp' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.Idp
- description: Delete a 'iam.IpAddress' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.IpAddress
- description: Delete a 'iam.LdapGroup' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.LdapGroup
- description: Delete a 'iam.LdapPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.LdapPolicy
- description: Delete a 'iam.LdapProvider' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.LdapProvider
- description: Delete a 'iam.OAuthToken' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.OAuthToken
- description: Delete a 'iam.Permission' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.Permission
- description: Delete a 'iam.PrivateKeySpec' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.PrivateKeySpec
- description: Delete a 'iam.PrivilegeSet' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.PrivilegeSet
- description: Delete a 'iam.Qualifier' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.Qualifier
- description: Delete a 'iam.ResourceRoles' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.ResourceRoles
- description: Delete a 'iam.Session' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.Session
- description: Delete a 'iam.SessionLimits' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.SessionLimits
- description: Delete a 'iam.SharingRule' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.SharingRule
- description: Delete a 'iam.TrustPoint' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.TrustPoint
- description: Delete a 'iam.User' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.User
- description: Delete a 'iam.UserGroup' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.UserGroup
- description: Delete a 'iam.UserQualifier' resource.
  flows:
  - clientCredentials
  scope: DELETE.iam.UserQualifier
- description: Delete a 'ipmioverlan.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.ipmioverlan.Policy
- description: Delete a 'ippool.IpLease' resource.
  flows:
  - clientCredentials
  scope: DELETE.ippool.IpLease
- description: Delete a 'ippool.Pool' resource.
  flows:
  - clientCredentials
  scope: DELETE.ippool.Pool
- description: Delete a 'ippool.Reservation' resource.
  flows:
  - clientCredentials
  scope: DELETE.ippool.Reservation
- description: Delete a 'iqnpool.Lease' resource.
  flows:
  - clientCredentials
  scope: DELETE.iqnpool.Lease
- description: Delete a 'iqnpool.Pool' resource.
  flows:
  - clientCredentials
  scope: DELETE.iqnpool.Pool
- description: Delete a 'iqnpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: DELETE.iqnpool.Reservation
- description: Delete a 'iwotenant.TenantCustomization' resource.
  flows:
  - clientCredentials
  scope: DELETE.iwotenant.TenantCustomization
- description: Delete a 'kvm.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.kvm.Policy
- description: Delete a 'kvm.TunneledKvmPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.kvm.TunneledKvmPolicy
- description: Delete a 'macpool.Lease' resource.
  flows:
  - clientCredentials
  scope: DELETE.macpool.Lease
- description: Delete a 'macpool.Pool' resource.
  flows:
  - clientCredentials
  scope: DELETE.macpool.Pool
- description: Delete a 'macpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: DELETE.macpool.Reservation
- description: Delete a 'memory.PersistentMemoryPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.memory.PersistentMemoryPolicy
- description: Delete a 'memory.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.memory.Policy
- description: Delete a 'metrics.MetricsExploration' resource.
  flows:
  - clientCredentials
  scope: DELETE.metrics.MetricsExploration
- description: Delete a 'mgmt.ConfigBackupFile' resource.
  flows:
  - clientCredentials
  scope: DELETE.mgmt.ConfigBackupFile
- description: Delete a 'mgmt.ConfigBackupInstance' resource.
  flows:
  - clientCredentials
  scope: DELETE.mgmt.ConfigBackupInstance
- description: Delete a 'mgmt.ConfigBackupOperation' resource.
  flows:
  - clientCredentials
  scope: DELETE.mgmt.ConfigBackupOperation
- description: Delete a 'mgmt.ConfigOperationSetting' resource.
  flows:
  - clientCredentials
  scope: DELETE.mgmt.ConfigOperationSetting
- description: Delete a 'mgmt.ConfigRestoreOperation' resource.
  flows:
  - clientCredentials
  scope: DELETE.mgmt.ConfigRestoreOperation
- description: Delete a 'networkconfig.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.networkconfig.Policy
- description: Delete a 'notification.AccountSubscription' resource.
  flows:
  - clientCredentials
  scope: DELETE.notification.AccountSubscription
- description: Delete a 'ntp.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.ntp.Policy
- description: Delete a 'oauth.AccessToken' resource.
  flows:
  - clientCredentials
  scope: DELETE.oauth.AccessToken
- description: Delete a 'openapi.ApiMethodMeta' resource.
  flows:
  - clientCredentials
  scope: DELETE.openapi.ApiMethodMeta
- description: Delete a 'openapi.OpenApiSpecification' resource.
  flows:
  - clientCredentials
  scope: DELETE.openapi.OpenApiSpecification
- description: Delete a 'openapi.ProcessFile' resource.
  flows:
  - clientCredentials
  scope: DELETE.openapi.ProcessFile
- description: Delete a 'openapi.TaskGenerationRequest' resource.
  flows:
  - clientCredentials
  scope: DELETE.openapi.TaskGenerationRequest
- description: Delete a 'openapi.TaskGenerationResult' resource.
  flows:
  - clientCredentials
  scope: DELETE.openapi.TaskGenerationResult
- description: Delete a 'oprs.Deployment' resource.
  flows:
  - clientCredentials
  scope: DELETE.oprs.Deployment
- description: Delete a 'oprs.SyncTargetListMessage' resource.
  flows:
  - clientCredentials
  scope: DELETE.oprs.SyncTargetListMessage
- description: Delete a 'organization.Organization' resource.
  flows:
  - clientCredentials
  scope: DELETE.organization.Organization
- description: Delete a 'os.ConfigurationFile' resource.
  flows:
  - clientCredentials
  scope: DELETE.os.ConfigurationFile
- description: Delete a 'partnerintegration.DeviceConnector' resource.
  flows:
  - clientCredentials
  scope: DELETE.partnerintegration.DeviceConnector
- description: Delete a 'partnerintegration.Etl' resource.
  flows:
  - clientCredentials
  scope: DELETE.partnerintegration.Etl
- description: Delete a 'partnerintegration.File' resource.
  flows:
  - clientCredentials
  scope: DELETE.partnerintegration.File
- description: Delete a 'partnerintegration.Inventory' resource.
  flows:
  - clientCredentials
  scope: DELETE.partnerintegration.Inventory
- description: Delete a 'partnerintegration.Metrics' resource.
  flows:
  - clientCredentials
  scope: DELETE.partnerintegration.Metrics
- description: Delete a 'partnerintegration.Model' resource.
  flows:
  - clientCredentials
  scope: DELETE.partnerintegration.Model
- description: Delete a 'pool.IdMappingPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.pool.IdMappingPolicy
- description: Delete a 'power.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.power.Policy
- description: Delete a 'power.PowerGroup' resource.
  flows:
  - clientCredentials
  scope: DELETE.power.PowerGroup
- description: Delete a 'recovery.BackupConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.recovery.BackupConfigPolicy
- description: Delete a 'recovery.BackupProfile' resource.
  flows:
  - clientCredentials
  scope: DELETE.recovery.BackupProfile
- description: Delete a 'recovery.OnDemandBackup' resource.
  flows:
  - clientCredentials
  scope: DELETE.recovery.OnDemandBackup
- description: Delete a 'recovery.Restore' resource.
  flows:
  - clientCredentials
  scope: DELETE.recovery.Restore
- description: Delete a 'recovery.ScheduleConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.recovery.ScheduleConfigPolicy
- description: Delete a 'resource.Group' resource.
  flows:
  - clientCredentials
  scope: DELETE.resource.Group
- description: Delete a 'resource.Reservation' resource.
  flows:
  - clientCredentials
  scope: DELETE.resource.Reservation
- description: Delete a 'resource.SelectionCriteria' resource.
  flows:
  - clientCredentials
  scope: DELETE.resource.SelectionCriteria
- description: Delete a 'resourcepool.ChassisQualificationPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.resourcepool.ChassisQualificationPolicy
- description: Delete a 'resourcepool.Lease' resource.
  flows:
  - clientCredentials
  scope: DELETE.resourcepool.Lease
- description: Delete a 'resourcepool.MembershipReservation' resource.
  flows:
  - clientCredentials
  scope: DELETE.resourcepool.MembershipReservation
- description: Delete a 'resourcepool.Pool' resource.
  flows:
  - clientCredentials
  scope: DELETE.resourcepool.Pool
- description: Delete a 'resourcepool.QualificationPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.resourcepool.QualificationPolicy
- description: Delete a 'resourcepool.Reservation' resource.
  flows:
  - clientCredentials
  scope: DELETE.resourcepool.Reservation
- description: Delete a 'scheduler.SchedulePolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.scheduler.SchedulePolicy
- description: Delete a 'scheduler.TaskSchedule' resource.
  flows:
  - clientCredentials
  scope: DELETE.scheduler.TaskSchedule
- description: Delete a 'sdaaci.Connection' resource.
  flows:
  - clientCredentials
  scope: DELETE.sdaaci.Connection
- description: Delete a 'sdaaci.ConnectionDetail' resource.
  flows:
  - clientCredentials
  scope: DELETE.sdaaci.ConnectionDetail
- description: Delete a 'sdcard.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.sdcard.Policy
- description: Delete a 'server.DiagnosticStatus' resource.
  flows:
  - clientCredentials
  scope: DELETE.server.DiagnosticStatus
- description: Delete a 'server.Diagnostics' resource.
  flows:
  - clientCredentials
  scope: DELETE.server.Diagnostics
- description: Delete a 'server.MigrationKeyDetails' resource.
  flows:
  - clientCredentials
  scope: DELETE.server.MigrationKeyDetails
- description: Delete a 'server.Profile' resource.
  flows:
  - clientCredentials
  scope: DELETE.server.Profile
- description: Delete a 'server.ProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: DELETE.server.ProfileTemplate
- description: Delete a 'smtp.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.smtp.Policy
- description: Delete a 'smtp.PolicyTest' resource.
  flows:
  - clientCredentials
  scope: DELETE.smtp.PolicyTest
- description: Delete a 'snmp.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.snmp.Policy
- description: Delete a 'software.ApplianceDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.ApplianceDistributable
- description: Delete a 'software.HciBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.HciBundleDistributable
- description: Delete a 'software.HciDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.HciDistributable
- description: Delete a 'software.HyperflexBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.HyperflexBundleDistributable
- description: Delete a 'software.HyperflexDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.HyperflexDistributable
- description: Delete a 'software.IksBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.IksBundleDistributable
- description: Delete a 'software.ReleaseMeta' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.ReleaseMeta
- description: Delete a 'software.SolutionDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.SolutionDistributable
- description: Delete a 'software.UcsdBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.UcsdBundleDistributable
- description: Delete a 'software.UcsdDistributable' resource.
  flows:
  - clientCredentials
  scope: DELETE.software.UcsdDistributable
- description: Delete a 'softwarerepository.OperatingSystemFile' resource.
  flows:
  - clientCredentials
  scope: DELETE.softwarerepository.OperatingSystemFile
- description: Delete a 'sol.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.sol.Policy
- description: Delete a 'ssh.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.ssh.Policy
- description: Delete a 'storage.DriveGroup' resource.
  flows:
  - clientCredentials
  scope: DELETE.storage.DriveGroup
- description: Delete a 'storage.DriveSecurityPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.storage.DriveSecurityPolicy
- description: Delete a 'storage.StoragePolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.storage.StoragePolicy
- description: Delete a 'syslog.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.syslog.Policy
- description: Delete a 'tam.AdvisoryInfo' resource.
  flows:
  - clientCredentials
  scope: DELETE.tam.AdvisoryInfo
- description: Delete a 'techsupportmanagement.CollectionControlPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.techsupportmanagement.CollectionControlPolicy
- description: Delete a 'techsupportmanagement.TechSupportBundle' resource.
  flows:
  - clientCredentials
  scope: DELETE.techsupportmanagement.TechSupportBundle
- description: Delete a 'thermal.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.thermal.Policy
- description: Delete a 'ucsd.BackupInfo' resource.
  flows:
  - clientCredentials
  scope: DELETE.ucsd.BackupInfo
- description: Delete a 'uuidpool.Pool' resource.
  flows:
  - clientCredentials
  scope: DELETE.uuidpool.Pool
- description: Delete a 'uuidpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: DELETE.uuidpool.Reservation
- description: Delete a 'uuidpool.UuidLease' resource.
  flows:
  - clientCredentials
  scope: DELETE.uuidpool.UuidLease
- description: Delete a 'virtualization.VirtualMachine' resource.
  flows:
  - clientCredentials
  scope: DELETE.virtualization.VirtualMachine
- description: Delete a 'vmedia.Policy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vmedia.Policy
- description: Delete a 'vnic.EthAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.EthAdapterPolicy
- description: Delete a 'vnic.EthIf' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.EthIf
- description: Delete a 'vnic.EthNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.EthNetworkPolicy
- description: Delete a 'vnic.EthQosPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.EthQosPolicy
- description: Delete a 'vnic.FcAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.FcAdapterPolicy
- description: Delete a 'vnic.FcIf' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.FcIf
- description: Delete a 'vnic.FcNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.FcNetworkPolicy
- description: Delete a 'vnic.FcQosPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.FcQosPolicy
- description: Delete a 'vnic.IscsiAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.IscsiAdapterPolicy
- description: Delete a 'vnic.IscsiBootPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.IscsiBootPolicy
- description: Delete a 'vnic.IscsiStaticTargetPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.IscsiStaticTargetPolicy
- description: Delete a 'vnic.LanConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.LanConnectivityPolicy
- description: Delete a 'vnic.SanConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.SanConnectivityPolicy
- description: Delete a 'vnic.VhbaTemplate' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.VhbaTemplate
- description: Delete a 'vnic.VnicTemplate' resource.
  flows:
  - clientCredentials
  scope: DELETE.vnic.VnicTemplate
- description: Delete a 'vrf.Vrf' resource.
  flows:
  - clientCredentials
  scope: DELETE.vrf.Vrf
- description: Delete a 'webhook.Endpoint' resource.
  flows:
  - clientCredentials
  scope: DELETE.webhook.Endpoint
- description: Delete a 'webhook.Schema' resource.
  flows:
  - clientCredentials
  scope: DELETE.webhook.Schema
- description: Delete a 'workflow.AnsibleBatchExecutor' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.AnsibleBatchExecutor
- description: Delete a 'workflow.BatchApiExecutor' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.BatchApiExecutor
- description: Delete a 'workflow.CatalogItemDefinition' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.CatalogItemDefinition
- description: Delete a 'workflow.CatalogServiceRequest' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.CatalogServiceRequest
- description: Delete a 'workflow.CustomDataTypeDefinition' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.CustomDataTypeDefinition
- description: Delete a 'workflow.ErrorResponseHandler' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.ErrorResponseHandler
- description: Delete a 'workflow.PowerShellBatchApiExecutor' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.PowerShellBatchApiExecutor
- description: Delete a 'workflow.RollbackWorkflow' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.RollbackWorkflow
- description: Delete a 'workflow.ServiceItemActionDefinition' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.ServiceItemActionDefinition
- description: Delete a 'workflow.ServiceItemActionInstance' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.ServiceItemActionInstance
- description: Delete a 'workflow.ServiceItemDefinition' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.ServiceItemDefinition
- description: Delete a 'workflow.ServiceItemInstance' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.ServiceItemInstance
- description: Delete a 'workflow.ServiceItemOutput' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.ServiceItemOutput
- description: Delete a 'workflow.SshBatchExecutor' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.SshBatchExecutor
- description: Delete a 'workflow.TaskDefinition' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.TaskDefinition
- description: Delete a 'workflow.UiDisplayMetadata' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.UiDisplayMetadata
- description: Delete a 'workflow.Variable' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.Variable
- description: Delete a 'workflow.WorkflowDefinition' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.WorkflowDefinition
- description: Delete a 'workflow.WorkflowInfo' resource.
  flows:
  - clientCredentials
  scope: DELETE.workflow.WorkflowInfo
- description: Delete a 'workload.Blueprint' resource.
  flows:
  - clientCredentials
  scope: DELETE.workload.Blueprint
- description: Delete a 'workload.ClearWorkloadTag' resource.
  flows:
  - clientCredentials
  scope: DELETE.workload.ClearWorkloadTag
- description: Delete a 'workload.WorkloadDefinition' resource.
  flows:
  - clientCredentials
  scope: DELETE.workload.WorkloadDefinition
- description: Delete a 'workload.WorkloadDeployment' resource.
  flows:
  - clientCredentials
  scope: DELETE.workload.WorkloadDeployment
- description: Delete a 'workload.WorkloadInstance' resource.
  flows:
  - clientCredentials
  scope: DELETE.workload.WorkloadInstance
- description: Manage API keys used for secure access to system resources and services.
  flows:
  - clientCredentials
  scope: PRIVSET.API keys
- description: Manage API keys and OAuth tokens used for secure access to system resources and services.
  flows:
  - clientCredentials
  scope: PRIVSET.API keys and OAuth tokens
- description: Manage access of users, user groups; and organizations, resource groups, and roles; and IP access management.
  flows:
  - clientCredentials
  scope: PRIVSET.Access and permissions
- description: Log in and interact with domain settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Access domains
- description: Log in and interact with servers to perform operations based on privileges.
  flows:
  - clientCredentials
  scope: PRIVSET.Access servers
- description: Manage Intersight account settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Account
- description: A set of privileges that provides complete access to all services and resources in Intersight.
  flows:
  - clientCredentials
  scope: PRIVSET.Account Administrator
- description: Acknowledge the filed notices, end-of-life and security advisories.
  flows:
  - clientCredentials
  scope: PRIVSET.Acknowledge advisories
- description: Acknowledge the alarms.
  flows:
  - clientCredentials
  scope: PRIVSET.Acknowledge alarms
- description: Activate the profile on the attached server.
  flows:
  - clientCredentials
  scope: PRIVSET.Activate server profiles
- description: As an Activate Webhooks user, you can enable webhooks, allowing them to start receiving and processing notifications and data from the system.
  flows:
  - clientCredentials
  scope: PRIVSET.Activate webhook
- description: Configure Ethernet and Fibre Channel settings for the Virtual Interface Card (VIC), including features like VXLAN, NVGRE, and TCP Offload settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Adapter Configuration policies
- description: Upload an OS configuration file for automated and unattended OS installation on servers to improve deployment efficiency.
  flows:
  - clientCredentials
  scope: PRIVSET.Add OS configuration links
- description: Add the image source of the operating system, specifying the file share location and protocol (CIFS/NFS/HTTPS) to the software repository.
  flows:
  - clientCredentials
  scope: PRIVSET.Add OS image links
- description: Add the Server Configuration Utility (SCU) for automated OS installation, specifying file share locations using NFS, CIFS, or HTTP protocols.
  flows:
  - clientCredentials
  scope: PRIVSET.Add SCU links
- description: Assign and manage tags for server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Add and remove server profile template tags
- description: Configure and add a domain name to the system for proper network addressing and identification of resources.
  flows:
  - clientCredentials
  scope: PRIVSET.Add domain names
- description: Add an exploration to the Intersight dashboard.
  flows:
  - clientCredentials
  scope: PRIVSET.Add explorations to dashboard
- description: 'Configure and add external Syslog servers to the system for centralized collection and management of log data from various sources. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Add external syslog servers
- description: Add a firmware source to the software repository by specifying the file share location and protocol (NFS/CIFS/HTTP[S]) for firmware upgrades.
  flows:
  - clientCredentials
  scope: PRIVSET.Add firmware links
- description: Configure and add a new identity provider (IdP) to the system, enabling authentication and access management through external or federated identity services.
  flows:
  - clientCredentials
  scope: PRIVSET.Add identity providers
- description: Create and configure new notification rules, defining criteria and actions for alerting users based on specific events or conditions.
  flows:
  - clientCredentials
  scope: PRIVSET.Add notification rule or webhook
- description: Add trusted IP ranges.
  flows:
  - clientCredentials
  scope: PRIVSET.Add trusted IP ranges
- description: Upload and install certificates that are trusted by the system, enabling secure communications and verifying connection authenticity.
  flows:
  - clientCredentials
  scope: PRIVSET.Add trusted certificates
- description: Manage the alerts from advisories, and alarms.
  flows:
  - clientCredentials
  scope: PRIVSET.Alerts
- description: Enable and disable proactive RMA, tech support bundle collection, sending additional system information to Cisco.
  flows:
  - clientCredentials
  scope: PRIVSET.Allow or Disallow Data Collection
- description: Enable or disable launch of FI and Unified Edge eCMC CLI.
  flows:
  - clientCredentials
  scope: PRIVSET.Allow/disallow FI and Unified Edge eCMC CLI launches
- description: Enable or disable tech support incident bundle collection.
  flows:
  - clientCredentials
  scope: PRIVSET.Allow/disallow tech support bundles
- description: Enable or disable configuration of tunneled vKVM access.
  flows:
  - clientCredentials
  scope: PRIVSET.Allow/disallow tunneled vKVM configurations
- description: Enable or disable launch of tunneled vKVM access.
  flows:
  - clientCredentials
  scope: PRIVSET.Allow/disallow tunneled vKVM launches
- description: 'Manage authentication in Intersight appliance using Single sign-on (SSO), Cisco ID, SSL/TLS Certificate and LDAP. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Appliance authentication
- description: 'Manage the configuration settings of the Intersight appliance. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Appliance configuration
- description: 'Manage networking settings related to the appliance. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Appliance networking
- description: 'Managing system maintenance and data sharing features related to Proactive RMA feature and option to send supplementary diagnostic and operational data to Cisco. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Appliance security & privacy
- description: 'As a user with the ability to apply SSL certificates, you can install and configure SSL certificates for secure communications. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Apply SSL Certificate
- description: Approve Publish Requests
  flows:
  - clientCredentials
  scope: PRIVSET.Approve Publish Requests
- description: Link domain profiles to servers for management.
  flows:
  - clientCredentials
  scope: PRIVSET.Assign chassis profiles
- description: Link domain profiles for server management.
  flows:
  - clientCredentials
  scope: PRIVSET.Assign domain profiles
- description: Assign a server to the server profile.
  flows:
  - clientCredentials
  scope: PRIVSET.Assign server profiles
- description: It allows to attach any policies to server profile and removal of policies from chassis profile.
  flows:
  - clientCredentials
  scope: PRIVSET.Attach to and detach from chassis profile templates
- description: It allows to attach any policies to domain profile template and removal of policies from domain profile template.
  flows:
  - clientCredentials
  scope: PRIVSET.Attach to and detach from domain profile templates
- description: It allows to attach any policies to server profile and removal of policies from server profile.
  flows:
  - clientCredentials
  scope: PRIVSET.Attach to and detach from server profile templates
- description: As an Audit Log Viewer, you can view audit logs.
  flows:
  - clientCredentials
  scope: PRIVSET.Audit Log Viewer
- description: Manage and view audit logs.
  flows:
  - clientCredentials
  scope: PRIVSET.Audit logs
- description: Manage logging of user activities, configuration changes, and operational commands for FIs, leveraging the Linux audit daemon framework (auditd).
  flows:
  - clientCredentials
  scope: PRIVSET.AuditD policies
- description: Manage authentication methods and policies for securing system access.
  flows:
  - clientCredentials
  scope: PRIVSET.Authentication
- description: As a user with access to Authentication settings, you can manage and configure the authentication methods and policies for securing access to the system.
  flows:
  - clientCredentials
  scope: PRIVSET.Authentication settings
- description: As Automation Governor, you can approve or reject approval requests.
  flows:
  - clientCredentials
  scope: PRIVSET.Automation Governance
- description: Set the BIOS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.BIOS policies
- description: Set the BIOS boot mode, and enable secure boot.
  flows:
  - clientCredentials
  scope: PRIVSET.Boot Order policies
- description: As a Catalog Administrator, you can create tasks, workflows, custom datatypes, resource selection criteria, service items and use these building blocks to create catalog items. You can validate these catalog items by deploying them and performing post-deployment operations on the deployed resources. The catalog administrator can publish the catalog items to an organization so that these can be consumed by the catalog users in that organization.
  flows:
  - clientCredentials
  scope: PRIVSET.Catalog Administrator
- description: As a Catalog User, you can view the catalog items assigned to you, deploy the catalog item, track the service requests, view the service item instance that you have created or are assigned to you, and perform post-deployment operations on the resource.
  flows:
  - clientCredentials
  scope: PRIVSET.Catalog User
- description: Specify and attach external certificate details to servers, supporting Root CA and IMC certificates.
  flows:
  - clientCredentials
  scope: PRIVSET.Certificate Management policies
- description: Manage Cisco identification credentials and settings used for accessing Cisco services.
  flows:
  - clientCredentials
  scope: PRIVSET.Cisco ID
- description: Claim devices.
  flows:
  - clientCredentials
  scope: PRIVSET.Claim Devices
- description: Assign or register a target to the system for management or monitoring purposes.
  flows:
  - clientCredentials
  scope: PRIVSET.Claim targets
- description: Clear the Trusted Platform Module (TPM) on servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Clear TPMs
- description: Remove foreign configurations not integrated with current setups.
  flows:
  - clientCredentials
  scope: PRIVSET.Clear configurations
- description: Remove foreign configurations from a server's storage system to clear external storage setups that are not integrated with the server's current configuration.
  flows:
  - clientCredentials
  scope: PRIVSET.Clear foreign configurations
- description: Erase the system event log (SEL), clearing recorded events.
  flows:
  - clientCredentials
  scope: PRIVSET.Clear system event logs (SEL)
- description: Manage and configure clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.Clusters
- description: As a Complete Claim user you can complete the claim of a previously created Target by providing the security token of the device. You do not have access to read the status or details of any devices within the account.
  flows:
  - clientCredentials
  scope: PRIVSET.Complete Claim
- description: Configure physical servers, chassis, and domains along with their respective profiles and templates, while managing compute, management, network, and storage policies, and configuring pools of Intersight Infrastructure Services.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure
- description: Set up and manage credentials required for accessing and downloading Cisco software to ensure secure and authorized access to updates and resources.Set up and manage credentials required for accessing and downloading Cisco software to ensure secure and authorized access to updates and resources.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure Cisco software download credentials
- description: 'Set up and manage Domain Name System (DNS) configurations, including DNS servers, domain names, and search domains to ensure proper name resolution and network connectivity. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure DNS settings
- description: Manages the collection of IP addresses that can be dynamically assigned to services running on network elements. It supports both IPv4 and IPv6 addresses and can be configured at either the pool level or block level.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure IP pools
- description: Define and manage iSCSI Qualified Names (IQNs) pools for organized iSCSI identifier assignment.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure IQN pools
- description: 'Set up and manage LDAP server settings, including server address, port, authentication methods, and directory structures to enable directory services and authentication. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure LDAP servers
- description: 'Set up and manage the password policy for local users, including requirements for password complexity, expiration, and reset procedures to ensure secure access control. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure Local Users Password Policy
- description: Manage the collection of MAC addresses that are unique in their Layer 2 environment, used to assign to vNICs on a server. This helps in automating the assignment of MAC addresses in server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure MAC pools
- description: Set up and manage Multi-Factor Authentication (MFA) settings, including configuring authentication methods, policies, and user access requirements to enhance security.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure MFA
- description: 'Set up and manage Network Time Protocol (NTP) configurations, including NTP servers and time synchronization settings to ensure accurate and consistent time across the network. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure NTP settings
- description: Manage pool aggregation of homogeneous resources, such as servers, to manage their utilization efficiently. It allows for logical grouping and management of resources for server profiles
  flows:
  - clientCredentials
  scope: PRIVSET.Configure Resource Pool
- description: 'Set up and manage Simple Mail Transfer Protocol (SMTP) server settings, including server address, port, authentication, and security settings to enable and configure email functionality. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure SMTP servers
- description: Manage universally unique identifier (UUID) for each server associated with a server profile, ensuring that each server has a unique identifier.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure UUID pools
- description: Manage world wide node name (WWNN) or world wide port name (WWPN) pools to provide unique IDs for Fibre Channel nodes and ports on a server.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure WWNN or WWPN pools
- description: Set up and modify account information, including user credentials, contact details, and other account-specific settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure account details
- description: 'Set up and modify schedules for automated backups, defining timing, frequency, and scope to ensure regular and reliable data protection. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure backup schedule
- description: 'Set up and modify banner messages displayed to users, providing important information, warnings, or notifications within the system interface. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure banner message
- description: Manage chassis profile template settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure chassis profile templates
- description: Manage chassis profile settings to ensure configurations align with operational requirements and organizational standards.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure chassis profiles
- description: Create, Clone, Edit or Delete the compute policies of Cisco UCS which define the configuration parameters for server resources.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure compute policies
- description: 'As a user with the ability to Configure Data Collection Settings, you can manage the proactive return merchandise authorization settings for the system. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure data collection settings
- description: 'Set up and manage the configuration for device connectors, including network settings and parameters needed for device communication and integration within the appliance networking environment. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure device connector settings
- description: Manage domain profile template.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure domain profile templates
- description: Manage domain profiles to define and apply network, storage, and compute configurations across systems.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure domain profiles
- description: Create, Clone, Edit or Delete the policies that manage different aspects of network management, such as adapter and ethernet policies, fibre channel and iSCSI policies, traffic and flow control, connectivity and control, virtualization and group management. It includes certificate management, device connector, IPMI over LAN, LDAP, local user, network connectivity, NTP, serial over LAN, SMTP, SNMP, SSH, Syslog, and virtual KVM policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure management policies
- description: 'Set up and manage the configuration of metrics collection and reporting, defining which metrics are tracked, how they are recorded, and how they are displayed for analysis. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure metrics settings
- description: It allows setting up various policies to manage Ethernet and Fibre Channel settings, as well as network communication resources between servers and the LAN or SAN. It includes adapter configuration, iSCSI boot, LAN connectivity, and SAN connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure network policies
- description: Manage settings of a physical chassis to ensure optimal configuration and operation of chassis components within your infrastructure.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure physical chassis
- description: Manage settings of physical domains.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure physical domains
- description: Configure settings and perform actions on physical servers to ensure they meet operational requirements.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure physical servers
- description: Manage resource pools like IP, MAC, WWPN, and storage pools for efficient resource allocation.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure pools
- description: Create or modify server profiles templates by setting up specific configurations, assigning resources, and updating settings to ensure the server operates according to required specifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure server profile templates
- description: Create or modify server profiles by setting up specific configurations, assigning resources, and updating settings to ensure the server operates according to required specifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure server profiles
- description: 'Set up and manage settings related to software updates, including scheduling, sources, and policies to ensure that software remains current and secure. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Configure software update settings
- description: It allows setting up various policies to manage storage resources effectively. It includes Drive Security, SD Card, and Storage policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure storage policies
- description: Manage vHBA Templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure vHBA templates
- description: Manage vNIC Templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Configure vNIC templates
- description: Create Approval Request
  flows:
  - clientCredentials
  scope: PRIVSET.Create Approval Request
- description: 'As a user with the ability to create Certificate Signing Requests (CSR), you can generate requests for digital certificates to establish secure communications. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Create CSR
- description: Reserve specific IP addresses within pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Create IP pool address reservations
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create IP pools
- description: Reserve specific iSCSI Qualified Names (IQNs) within an IQN pool to ensure allocation for particular devices and restrict general assignment.
  flows:
  - clientCredentials
  scope: PRIVSET.Create IQN pool address reservations
- description: Create new iSCSI Qualified Name (IQN) pools, configuring settings for iSCSI targets.
  flows:
  - clientCredentials
  scope: PRIVSET.Create IQN pools
- description: Reserve specific MAC addresses within pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Create MAC pool address reservations
- description: Create new MAC address pools, configuring settings for network devices.
  flows:
  - clientCredentials
  scope: PRIVSET.Create MAC pools
- description: A set of privileges that allow the users to create nexus reports.
  flows:
  - clientCredentials
  scope: PRIVSET.Create Nexus Reports
- description: Register new applications with OAuth 2.0 grant types, defining their authentication and authorization settings for secure access.
  flows:
  - clientCredentials
  scope: PRIVSET.Create OAuth 2.0 grant type applications
- description: Reserve specific resources within a resource pool to ensure allocation for particular uses and restrict general assignment.
  flows:
  - clientCredentials
  scope: PRIVSET.Create Resource pool address reservations
- description: Create new resource pools, configuring settings for system resource allocation.
  flows:
  - clientCredentials
  scope: PRIVSET.Create Resource pools
- description: Reserve specific UUIDs within a UUID pool to ensure allocation for particular devices and restrict general assignment.
  flows:
  - clientCredentials
  scope: PRIVSET.Create UUID pool address reservations
- description: Create new universally unique identifier (UUID) pools, configuring settings for devices or services.
  flows:
  - clientCredentials
  scope: PRIVSET.Create UUID pools
- description: Reserve specific World Wide Node Names (WWNNs) or World Wide Port Names (WWPNs) within their respective pools to ensure allocation for particular devices and restrict general assignment.
  flows:
  - clientCredentials
  scope: PRIVSET.Create WWNN and WWPN pool address reservations
- description: Create new WWNN or WWPN pools, managing identifiers for devices.
  flows:
  - clientCredentials
  scope: PRIVSET.Create WWNN or WWPN pools
- description: 'Initiate the creation of backup copies of data to ensure important information is saved and can be restored in case of data loss or corruption. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Create backups
- description: Create chassis profile templates to serve as the foundation for multiple derived chassis profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Create chassis profile templates from chassis profile
- description: Create domain profile templates from domain profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Create domain profile templates from domain profile
- description: Create new integrated systems.
  flows:
  - clientCredentials
  scope: PRIVSET.Create integrated systems
- description: Generate new server profile templates from an existing server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Create server profile template from server profile
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Adapter Configuration policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit AuditD policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit BIOS policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Boot Order policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Certificate Management policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Device Connector policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Drive Security policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Ethernet Adapter policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Ethernet Network Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Ethernet Network Group policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Ethernet Network policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Ethernet QoS policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit FC Zone policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Fibre Channel Adapter policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Fibre Channel Network policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Fibre Channel QoS policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Firmware policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Flow Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit IMC Access policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit IPMI over LAN policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit LAN Connectivity policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit LDAP policies
- description: As a Create or Clone Link Aggregation Policy user, you can define and establish new policies for link aggregation, configuring settings to combine multiple network connections into a single logical link for improved performance and redundancy.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Link Aggregation policies
- description: As a Create or Clone Link Control Policy user, you can define and establish new policies for link control, configuring settings to manage and optimize network link behavior and performance.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Link Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Local User policies
- description: As a Create or Clone Memory Policy user, you can define and establish new memory policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Memory policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Multicast policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit NTP policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Network Connectivity policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Persistent Memory policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Port policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Power policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit SAN Connectivity policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit SD Card policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit SMTP policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit SNMP policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit SSH policies
- description: As a Create or Clone Scrub Policy user, you can define and establish new Scrub policies within the system, configuring virtual media access and management settings for devices.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Scrub policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Serial Over LAN policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Storage policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Switch Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Syslog policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit System QoS policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Thermal policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit VLAN policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit VSAN policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Virtual KVM policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit Virtual Media policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit iSCSI Adapter policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit iSCSI Boot policies
- description: As a Create or Clone iSCSI Static Target Policy user, you can define and establish new policies for iSCSI static targets, configuring settings to manage and optimize the connections to specific iSCSI targets within the storage network.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone and edit iSCSI Static Target policies
- description: Create, clone and edit chassis profile templates to define and manage configuration settings for physical chassis.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone, and edit chassis profile templates
- description: Create and manage chassis profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone, and edit chassis profiles
- description: Create, clone and edit domain profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone, and edit domain profile templates
- description: Create, clone and edit domain profiles by configuring settings and policies to standardize domain operations.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone, and edit domain profiles
- description: Create and manage server profiles templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone, and edit server profile templates
- description: Create and manage server profiles, attach/detach policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone, and edit server profiles
- description: Create, clone and edit vHBA Templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone, and edit vHBA templates
- description: Create, clone and edit vNIC Templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Create, clone, and edit vNIC templates
- description: Manage and configure datacenters.
  flows:
  - clientCredentials
  scope: PRIVSET.Datacenters
- description: Manage and configure datastore clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.Datastore clusters
- description: Manage and configure datastores.
  flows:
  - clientCredentials
  scope: PRIVSET.Datastores
- description: Safely retire and remove Fabric Extenders (FEX), deactivating related connections and updating the system status.
  flows:
  - clientCredentials
  scope: PRIVSET.Decommission Fabric Extender (FEX)
- description: Safely retire and remove chassis.
  flows:
  - clientCredentials
  scope: PRIVSET.Decommission chassis
- description: Safely shut down servers, disconnect from the network, and ensure data is erased and backed up in alignment with policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Decommission servers
- description: Set or edit name, description, organization and tag of chassis profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Define and edit chassis profile general properties
- description: Set or edit name, description, organization and tag of chassis profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Define and edit chassis profile template general properties
- description: Add or edit name, description, organization and tag for UCS domain profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Define and edit domain profile general properties
- description: Set or edit name, description, organization and tag of domain profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Define and edit domain profile template general properties
- description: Set or edit the Organization, name, description, tag of Server Profile.
  flows:
  - clientCredentials
  scope: PRIVSET.Define and edit server profile general properties
- description: Set or edit name, description, organization and tag of server profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Define and edit server profile template general properties
- description: Set or edit name, description, organization and tag of vHBA templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Define and edit vHBA template general properties
- description: Add or edit the name, description and tag for the vNIC templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Define and edit vNIC template general properties
- description: Remove API keys from the system, terminating their access to system APIs and ensuring they are no longer valid for integration or automation purposes.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete API keys
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Adapter Configuration policies
- description: Delete Approval Request
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Approval Request
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete AuditD policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete BIOS policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Boot Order policies
- description: 'As a user with the ability to delete Certificate Signing Requests (CSR), you can remove existing requests for digital certificates from the system. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Delete CSR
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Certificate Management policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Device Connector policies
- description: Delete Devices.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Devices
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Drive Security policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Ethernet Adapter policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Ethernet Network Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Ethernet Network Group policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Ethernet Network policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Ethernet QoS policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete FC Zone policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Fibre Channel Adapter policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Fibre Channel Network policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Fibre Channel QoS policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Firmware policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Flow Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete IMC Access policies
- description: Remove IP address reservations, freeing them for use.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete IP pool address reservations
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete IP pools
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete IPMI over LAN policies
- description: Remove specific IQN reservations from an IQN pool to make them available for general assignment.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete IQN pool address reservations
- description: Remove existing iSCSI Qualified Name (IQN) pools, managing outdated IQN allocations.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete IQN pools
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete LAN Connectivity policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete LDAP policies
- description: 'Remove the configuration of LDAP servers, ceasing the directory services and authentication provided by those servers. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Delete LDAP servers
- description: As a Delete Link Aggregation Policy user, you can remove existing link aggregation policies, managing outdated or unnecessary settings related to network connection combinations.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Link Aggregation policies
- description: As a Delete Link Control Policy user, you can remove existing link control policies, managing outdated or unnecessary settings related to network link management.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Link Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Local User policies
- description: Remove MAC address reservations, freeing them for use.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete MAC pool address reservations
- description: Remove existing MAC pools, managing outdated MAC address allocations.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete MAC pools
- description: As a Delete Memory Policy user, you can remove existing Memory policies, managing outdated or unnecessary permissions and access settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Memory policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Multicast policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete NTP policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Network Connectivity policies
- description: Remove OAuth 2.0 grant type applications from the system, revoking their access and associated permissions.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete OAuth 2.0 grant type applications
- description: Remove OAuth 2.0 tokens from the system, revoking their access and preventing their use for authentication and authorization.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete OAuth 2.0 tokens
- description: Remove the OS configuration file for automated and unattended OS installation on servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete OS configuration links
- description: Remove the image source of the operating system from the software repository, deleting file share location and protocol (CIFS/NFS/HTTPS).
  flows:
  - clientCredentials
  scope: PRIVSET.Delete OS image links
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Persistent Memory policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Port policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Power policies
- description: Remove specific resource reservations from a resource pool to make them available for general assignment.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Resource pool address reservations
- description: Remove existing resource pools, managing outdated allocations.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Resource pools
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete SAN Connectivity policies
- description: Remove the Server Configuration Utility (SCU) for automated OS installation, deleting file share locations using NFS, CIFS, or HTTP protocols.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete SCU links
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete SD Card policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete SMTP policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete SNMP policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete SSH policies
- description: As a Delete Scrub Policy user, you can remove existing Scrub policies from the system, managing outdated or unnecessary virtual media configurations.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Scrub policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Serial Over LAN policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Storage policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Switch Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Syslog policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete System QoS policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Thermal policies
- description: Remove specific UUID reservations from a UUID pool to make them available for general assignment.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete UUID pool address reservations
- description: Remove existing universally unique identifier (UUID) pools, managing outdated UUID allocations.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete UUID pools
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete VLAN policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete VSAN policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Virtual KVM policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete Virtual Media policies
- description: Remove specific WWNN or WWPN reservations from pools to make them available for general assignment.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete WWNN and WWPN pool address reservations
- description: Remove existing WWNN or WWPN pools, managing outdated allocations.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete WWNN or WWPN pools
- description: Remove existing chassis profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete chassis profile templates
- description: Remove existing chassis profiles from your infrastructure, ensuring outdated or unnecessary configurations are managed.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete chassis profiles
- description: Remove existing domain names from the system, ceasing their use for network addressing and identification of resources.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete domain names
- description: Delete domain profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete domain profile templates
- description: Delete domain profiles from the system, ensuring associated configurations are managed.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete domain profiles
- description: Delete an existing exploration.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete explorations
- description: 'Remove the configuration of external Syslog servers from the system, ceasing the collection and management of log data from those servers. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Delete external syslog servers
- description: Remove the firmware source from the software repository by deleting the file share location and protocol (NFS/CIFS/HTTP[S]).
  flows:
  - clientCredentials
  scope: PRIVSET.Delete firmware links
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete iSCSI Adapter policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Delete iSCSI Boot policies
- description: As a Delete iSCSI Static Target Policy user, you can remove existing iSCSI static target policies, managing outdated or unnecessary settings related to specific iSCSI target connections.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete iSCSI Static Target policies
- description: Remove existing IdPs from the system, discontinuing associated authentication and access management services.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete identity providers
- description: Delete an existing integrated system.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete integrated systems
- description: Remove existing notification rules, stopping the triggering and management of alerts and notifications based on those rules.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete notification rule or webhook
- description: Remove server profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete server profile templates
- description: Remove server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete server profiles
- description: Delete the trusted IP range.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete trusted IP ranges
- description: Remove certificates from the system's list of trusted certificates, ceasing their use for secure communications.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete trusted certificates
- description: Delete vHBA Templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete vHBA templates
- description: Delete vNIC Templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Delete vNIC templates
- description: Apply domain profiles to servers, implementing settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Deploy chassis profiles
- description: Apply domain profiles, implementing server settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Deploy domain profiles
- description: Deploy the profile to the attached server.
  flows:
  - clientCredentials
  scope: PRIVSET.Deploy server profiles
- description: Cancel the registration of your device.
  flows:
  - clientCredentials
  scope: PRIVSET.Deregister Smart Licenses
- description: Create profiles derived from chassis profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Derive profiles from chassis profile templates
- description: Create profiles derived from domain profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Derive profiles from domain profile templates
- description: Create new server profiles using existing profiles or templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Derive server profiles
- description: As a Device Administrator, you can claim and unclaim a device in Intersight, view the device details, license status, a list of all the claimed devices, and generate API keys. You cannot perform any other management or administrative task in this role.
  flows:
  - clientCredentials
  scope: PRIVSET.Device Administrator
- description: Control configuration changes allowed from Cisco IMC, ensuring that changes are managed through Intersight.
  flows:
  - clientCredentials
  scope: PRIVSET.Device Connector policies
- description: As a Device Technician you can claim a device, view the device details, license status, a list of the claimed devices, and generate API keys. You cannot perform any other management or administrative task in this role.
  flows:
  - clientCredentials
  scope: PRIVSET.Device Technician
- description: A set of privileges that allows the access to manage devices e.g. view device details, claim and delete devices.
  flows:
  - clientCredentials
  scope: PRIVSET.Devices
- description: Deactivate security features on storage systems.
  flows:
  - clientCredentials
  scope: PRIVSET.Disable security
- description: 'Disable visibility of subscription details in the Intersight appliance. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Disable subscriptions
- description: Manage the configurations and settings related to domain names within the system.
  flows:
  - clientCredentials
  scope: PRIVSET.Domain names
- description: Download the server's event log (SEL) to review and analyse recorded events and errors for diagnostics.
  flows:
  - clientCredentials
  scope: PRIVSET.Download server event logs
- description: Define self-encrypting drives (SEDs) management to ensure data security using a Key-Encryption Key (KEK) and a Key Management Interoperability Protocol (KMIP) for remote key management.
  flows:
  - clientCredentials
  scope: PRIVSET.Drive Security policies
- description: Modify settings and permissions associated with existing API keys, managing their scope and access to ensure proper integration and security.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit API keys
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Adapter Configuration policies
- description: Attach/detach Adapter Configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Adapter Configuration policies for server profile
- description: Attach/detach Adapter Configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Adapter Configuration policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit AuditD policies
- description: Attach/detach AuditD policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit AuditD policies for domain profile
- description: Attach/detach AuditD policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit AuditD policies for domain profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit BIOS policies
- description: Attach/detach BIOS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit BIOS policies for server profile
- description: Attach/detach BIOS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit BIOS policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Boot Order policies
- description: Attach/detach Boot Order policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Boot Order policies for server profile
- description: Attach/detach Boot Order policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Boot Order policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Certificate Management policies
- description: Attach/detach Certificate Management policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Certificate Management policies for domain profile
- description: Attach/detach Certificate Management policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Certificate Management policies for domain profile template
- description: Attach/detach Certificate Management policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Certificate Management policies for server profile
- description: Attach/detach Certificate Management policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Certificate Management policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Device Connector policies
- description: Attach/detach Device Connector policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Device Connector policies for server profile
- description: Attach/detach Device Connector policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Device Connector policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Drive Security policies
- description: Attach/detach Drive Security policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Drive Security policies for server profile
- description: Attach/detach Drive Security policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Drive Security policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ethernet Adapter policies
- description: Attach/detach Ethernet Adapter policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ethernet Adapter policies for vNIC template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ethernet Network Control policies
- description: Attach/detach Ethernet Network Control policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ethernet Network Control policies for vNIC template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ethernet Network Group policies
- description: Attach/detach Ethernet Network Group policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ethernet Network Group policies for vNIC template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ethernet Network policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ethernet QoS policies
- description: Attach/detach Ethernet QoS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ethernet QoS policies for vNIC template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit FC Zone policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Fibre Channel Adapter policies
- description: Attach/detach Fibre Channel Adapter policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Fibre Channel Adapter policies for vHBA template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Fibre Channel Network policies
- description: Attach/detach Fibre Channel Network policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Fibre Channel Network policies for vHBA template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Fibre Channel QoS policies
- description: Attach/detach Fibre Channel QoS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Fibre Channel QoS policies for vHBA template
- description: Attach/detach Fibre Channel Zone policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Fibre Channel Zone policies for vHBA template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Firmware policies
- description: Attach/detach Firmware policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Firmware policies for server profile
- description: Attach/detach Firmware policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Firmware policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Flow Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IMC Access policies
- description: Attach/detach IMC Access policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IMC Access policies for chassis profile
- description: Attach/detach IMC Access policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IMC Access policies for chassis profile template
- description: As a Edit IMC Access policies for server profile user, you can adjust IMC access policies for server profiles. This includes updating access settings and ensuring that configurations are correctly applied to servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IMC Access policies for server profile
- description: As a Edit IMC Access policies for server profile template user, you can adjust IMC access policies for server profile templates. This includes updating access settings and ensuring that configurations are correctly applied to templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IMC Access policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IP pools
- description: Attach/detach IPMI Over LAN policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IPMI Over LAN policies for server profile
- description: Attach/detach IPMI Over LAN policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IPMI Over LAN policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IPMI over LAN policies
- description: Modify existing iSCSI Qualified Name (IQN) pools, optimizing IQN management.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit IQN pools
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit LAN Connectivity policies
- description: Attach/detach LAN Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit LAN Connectivity policies for server profile
- description: Attach/detach LAN Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit LAN Connectivity policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit LDAP policies
- description: Attach/detach LDAP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit LDAP policies for domain profile
- description: Attach/detach LDAP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit LDAP policies for domain profile template
- description: Attach/detach LDAP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit LDAP policies for server profile
- description: Attach/detach LDAP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit LDAP policies for server profile template
- description: 'Modify the configuration of existing LDAP servers by updating server address, port, authentication methods, and directory structures to ensure proper directory services and authentication. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Edit LDAP servers
- description: As an Edit Link Aggregation Policy user, you can modify existing link aggregation policies, adjusting settings to optimize the performance and redundancy of combined network connections.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Link Aggregation policies
- description: As an Edit Link Control Policy user, you can modify existing link control policies, adjusting settings to enhance network link behavior and performance.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Link Control policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Local User policies
- description: Attach/detach Local User policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Local User policies for domain profile
- description: Attach/detach Local User policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Local User policies for domain profile template
- description: Attach/detach Local User policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Local User policies for server profile
- description: Attach/detach Local User policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Local User policies for server profile template
- description: Attach/detach MAC Pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit MAC Pools for vNIC template
- description: Modify existing MAC pools, optimizing MAC address management.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit MAC pools
- description: As an Edit Memory Policy user, you can modify existing memory policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Memory policies
- description: Attach/detach Memory policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Memory policies for server profile
- description: Attach/detach Memory policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Memory policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Multicast policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit NTP policies
- description: Attach/detach NTP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit NTP policies for domain profile
- description: Attach/detach NTP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit NTP policies for domain profile template
- description: Attach/detach NTP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit NTP policies for server profile
- description: Attach/detach NTP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit NTP policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Network Connectivity policies
- description: Attach/detach LDAP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Network Connectivity policies for domain profile
- description: Attach/detach Network Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Network Connectivity policies for domain profile template
- description: Attach/detach Network Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Network Connectivity policies for server profile
- description: Attach/detach Network Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Network Connectivity policies for server profile template
- description: Modify settings of existing OAuth 2.0 grant type applications, including their grant types, permissions, and configurations.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit OAuth 2.0 grant type applications
- description: Modify the OS configuration file for automated and unattended OS installation on servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit OS configuration links
- description: Modify the image source of the operating system in the software repository, updating file share location and protocol (CIFS/NFS/HTTPS).
  flows:
  - clientCredentials
  scope: PRIVSET.Edit OS image links
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Persistent Memory policies
- description: Attach/detach Persistent Memory policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Persistent Memory policies for server profile
- description: Attach/detach Persistent Memory policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Persistent Memory policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Port policies
- description: Attach/detach Ports Configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ports Configuration policies for domain profile
- description: Attach/detach Ports Configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Ports Configuration policies for domain profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Power policies
- description: Attach/detach Power policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Power policies for chassis profile
- description: Attach/detach Power policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Power policies for chassis profile template
- description: Attach/detach Power policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Power policies for server profile
- description: Attach/detach Power policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Power policies for server profile template
- description: Modify existing resource pools to optimize resource management.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Resource pools
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SAN Connectivity policies
- description: Attach/detach SAN Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SAN Connectivity policies for server profile
- description: Attach/detach SAN Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SAN Connectivity policies for server profile template
- description: Modify the Server Configuration Utility (SCU) for automated OS installation, editing file share locations using NFS, CIFS, or HTTP protocols.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SCU links
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SD Card policies
- description: Attach/detach SD Card policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SD Card policies for server profile
- description: Attach/detach SD Card policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SD Card policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SMTP policies
- description: Attach/detach SMTP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SMTP policies for server profile
- description: Attach/detach SMTP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SMTP policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SNMP policies
- description: Attach/detach SNMP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SNMP policies for chassis profile
- description: Attach/detach SNMP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SNMP policies for chassis profile template
- description: Attach/detach SNMP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SNMP policies for domain profile
- description: Attach/detach SNMP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SNMP policies for domain profile template
- description: Attach/detach SNMP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SNMP policies for server profile
- description: Attach/detach SNMP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SNMP policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SSH policies
- description: Attach/detach SSH policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SSH policies for server profile
- description: Attach/detach SSH policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit SSH policies for server profile template
- description: As an Edit Scrub Policy user, you can modify existing Scrub policies within the system to adjust virtual media access and management settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Scrub policies
- description: As a Edit Scrub policies for server profile user, you can adjust scrub policies for Server Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Scrub policies for server profile
- description: As a Edit Scrub policies for server profile user, you can adjust scrub policies for Server Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Scrub policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Serial Over LAN policies
- description: Attach/detach Serial Over LAN policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Serial Over LAN policies for server profile
- description: Attach/detach Serial Over LAN policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Serial Over LAN policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Storage policies
- description: Attach/detach Storage policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Storage policies for server profile
- description: Attach/detach Storage policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Storage policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Switch Control policies
- description: Attach/detach Switch Control policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Switch Control policies for domain profile
- description: Attach/detach Switch Control policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Switch Control policies for domain profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Syslog policies
- description: Attach/detach Syslog policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Syslog policies for domain profile
- description: Attach/detach Syslog policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Syslog policies for domain profile template
- description: Attach/detach Syslog policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Syslog policies for server profile
- description: Attach/detach Syslog policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Syslog policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit System QoS policies
- description: Attach/detach System QoS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit System QoS policies for domain profile
- description: Attach/detach System QoS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit System QoS policies for domain profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Thermal policies
- description: Attach/detach Thermal policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Thermal policies for chassis profile
- description: Attach/detach Thermal policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Thermal policies for chassis profile template
- description: Attach/detach Thermal policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Thermal policies for server profile
- description: Attach/detach Thermal policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Thermal policies for server profile template
- description: Modify existing universally unique identifier (UUID) pools, optimizing UUID management.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit UUID pools
- description: As a Modify UUID Pool for Server Profile user, you can adjust UUID pools for server profiles. This includes updating UUID settings and ensuring that configurations are correctly applied to servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit UUID pools for server profile
- description: As a Modify UUID Pool for Server Profile Template user, you can adjust UUID pools for server profile templates. This includes updating UUID settings and ensuring that configurations are correctly applied to templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit UUID pools for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit VLAN policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit VSAN policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Virtual KVM policies
- description: Attach/detach Virtual KVM policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Virtual KVM policies for server profile
- description: Attach/detach Virtual KVM policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Virtual KVM policies for server profile template
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Virtual Media policies
- description: Attach/detach Virtual Media policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Virtual Media policies for server profile
- description: Attach/detach Virtual Media policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit Virtual Media policies for server profile template
- description: Modify existing WWNN or WWPN pools to optimize management.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit WWNN or WWPN pools
- description: Attach/detach WWPN Pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit WWPN pools for vHBA template
- description: Edit name, description, organization and tag of chassis profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit chassis profile general properties
- description: Attach/detach the policies associated with chassis profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit chassis profile policies
- description: Edit name, description, organization and tag of chassis profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit chassis profile template general properties
- description: Attach/detach the policies associated with chassis profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit chassis profile template policies
- description: Modify chassis profile templates to update and manage configuration settings for physical chassis.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit chassis profile templates
- description: Edit chassis profiles to update and manage configuration settings for physical chassis.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit chassis profiles
- description: Edit name, description, organization and tag for UCS domain profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit domain profile general properties
- description: Attach/detach the policies for domain profile.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit domain profile policies
- description: Edit name, description, organization and tag of domain profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit domain profile template general properties
- description: Attach/detach the policies associated with domain profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit domain profile template policies
- description: Modify existing chassis profile templates to update and manage configuration settings for domain.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit domain profile templates
- description: Edit the settings and policies of domain profiles to update and optimize operations.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit domain profiles
- description: 'Modify the configuration of existing external Syslog servers by adjusting settings and parameters to ensure effective log data collection and management. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Edit external syslog servers
- description: Modify the firmware source in the software repository by changing the file share location and protocol (NFS/CIFS/HTTP[S]).
  flows:
  - clientCredentials
  scope: PRIVSET.Edit firmware links
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit iSCSI Adapter policies
- description: ''
  flows:
  - clientCredentials
  scope: PRIVSET.Edit iSCSI Boot policies
- description: Attach/detach iSCSI Boot policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit iSCSI Boot policies for vNIC template
- description: As an Edit iSCSI Static Target Policy user, you can modify existing iSCSI static target policies, adjusting settings to enhance the management and performance of connections to specific iSCSI targets within the storage network.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit iSCSI Static Target policies
- description: Modify the configuration of existing IdPs by updating settings, credentials, and trust relationships to maintain or enhance authentication and access management.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit identity providers
- description: Edit the configuration of an existing integrated system.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit integrated systems
- description: Modify existing notification rules, adjusting criteria and actions to refine how alerts and notifications are triggered and managed.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit notification rule or webhook
- description: Edit name, description, organization and tag of server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit server profile general properties
- description: Attach/detach the policies associated with server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit server profile policies
- description: Edit name, description, organization and tag of server profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit server profile template general properties
- description: Attach/detach the policies associated with server profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit server profile template policies
- description: Edit, attach/detach policies associated with server profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit server profile templates
- description: Edit, attach/detach the policies associated with server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit server profiles
- description: Edit the trusted IP ranges.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit trusted IP ranges
- description: Set or edit name, description, organization and tag of vHBA templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vHBA template general properties
- description: Attach/detach the policies and pools associated with vHBA templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vHBA template policies
- description: Edit vHBA templates to update and manage configuration settings for vHBA.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vHBA templates
- description: Attach/detach vLAN Configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vLAN Configuration policies for domain profile
- description: Attach/detach vLAN Configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vLAN Configuration policies for domain profile template
- description: Set or edit name, description, organization and tag of vNIC templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vNIC template general properties
- description: Attach/detach the policies and pools associated with vNIC templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vNIC template policies
- description: Edit the settings and policies of vNIC Templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vNIC templates
- description: Attach/detach vSAN Configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vSAN Configuration policies for domain profile
- description: Attach/detach vSAN Configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Edit vSAN Configuration policies for domain profile template
- description: As a user with the ability to Enable or Disable API Keys, you can Activate & deactivate API keys, restricting access to the system's services.
  flows:
  - clientCredentials
  scope: PRIVSET.Enable and disable API keys
- description: Activate or deactivate OAuth 2.0 grant type applications to control their availability for authentication and authorization processes.
  flows:
  - clientCredentials
  scope: PRIVSET.Enable and disable OAuth 2.0 grant type applications
- description: Activate or deactivate network ports to manage connectivity.
  flows:
  - clientCredentials
  scope: PRIVSET.Enable and disable ports
- description: As an Enable or Disable Port user, you can activate or deactivate network ports, controlling their operational status to manage network connectivity and configuration.
  flows:
  - clientCredentials
  scope: PRIVSET.Enable or Disable Port Channels
- description: Obtain subscription details such as usage, status, and next expiration date.
  flows:
  - clientCredentials
  scope: PRIVSET.Enable subscription information
- description: 'Enable visibility of subscription details in the Intersight appliance. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Enable subscriptions
- description: Enable or disable IP access management.
  flows:
  - clientCredentials
  scope: PRIVSET.Enable/disable IP access management
- description: Enable or disable tunneled virtual keyboard, video, and mouse (vKVM) on servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Enable/disable tunneled vKVM
- description: Enter maintenance mode for a VM host.
  flows:
  - clientCredentials
  scope: PRIVSET.Enter maintenance modes
- description: Configure Ethernet adapter settings, impacting network properties such as MAC address pools, speed, and media modes.
  flows:
  - clientCredentials
  scope: PRIVSET.Ethernet Adapter policies
- description: Manage server discoverability through protocols like Cisco Discovery Protocol and Link Layer Discovery Protocol.
  flows:
  - clientCredentials
  scope: PRIVSET.Ethernet Network Control policies
- description: Manage QinQ VLAN and native VLAN settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Ethernet Network Group policies
- description: Manage VLAN mode and default VLAN settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Ethernet Network policies
- description: Assigns a system class to outgoing traffic for a vNIC, determining the quality of service.
  flows:
  - clientCredentials
  scope: PRIVSET.Ethernet QoS policies
- description: A set of privileges that allow the users to execute workflows and manage running workflows in IO.
  flows:
  - clientCredentials
  scope: PRIVSET.Execute Workflows
- description: Exit maintenance mode for a VM host.
  flows:
  - clientCredentials
  scope: PRIVSET.Exit maintenance modes
- description: Manage and configure explorations.
  flows:
  - clientCredentials
  scope: PRIVSET.Explorations
- description: Manage and configure the metric explorer.
  flows:
  - clientCredentials
  scope: PRIVSET.Explorer
- description: As an External Syslog Administrator, you can configure an external syslog server on an on-prem appliance.
  flows:
  - clientCredentials
  scope: PRIVSET.External Syslog Administrator
- description: Manage FC target zoning type and target settings.
  flows:
  - clientCredentials
  scope: PRIVSET.FC Zone policies
- description: A set of privileges that allows to perform operations related to Fabric Interconnect e.g. view fabric interconnect summary or detailed information about fabric connect. Fabric Interconnect privilege set is the top level privilege set of other privilege set(s) which are mapped to privileges related to Fabric Interconnect.
  flows:
  - clientCredentials
  scope: PRIVSET.Fabric Interconnects
- description: Initiate fabric resource evacuation for maintenance.
  flows:
  - clientCredentials
  scope: PRIVSET.Fabric evacuation
- description: Manages host-side behaviour of Fibre Channel adapters, including error recovery and performance settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Fibre Channel Adapter policies
- description: Manage the default VLAN and VSAN ID settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Fibre Channel Network policies
- description: Manage network traffic prioritization in Fibre Channel environments by assigning different levels of service (Platinum, Gold, Silver, Bronze).
  flows:
  - clientCredentials
  scope: PRIVSET.Fibre Channel QoS policies
- description: Manage firmware links.
  flows:
  - clientCredentials
  scope: PRIVSET.Firmware links
- description: Manage the current firmware, including option to exclude upgrade of drives and storage controllers.
  flows:
  - clientCredentials
  scope: PRIVSET.Firmware policies
- description: Configure the Priority Flow Control (PFC) for each port.
  flows:
  - clientCredentials
  scope: PRIVSET.Flow Control policies
- description: Create new API keys to enable secure access and interaction with system APIs for integration and automation purposes.
  flows:
  - clientCredentials
  scope: PRIVSET.Generate API keys
- description: 'Manage the general configuration settings of the appliance. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Generic
- description: A set of privileges that are common to all privilege sets. These are read-only privileges that will be common to all the hierarchial privileges
  flows:
  - clientCredentials
  scope: PRIVSET.Global Read Privileges
- description: A set of privileges that are common to all system packaged, system defined and internal privilege sets. Global System Privileges will not be part of the user created privilege sets.
  flows:
  - clientCredentials
  scope: PRIVSET.Global System Privileges
- description: A set of privileges that are common to all privilege sets. These are write privileges that will be common to all the hierarchial privileges
  flows:
  - clientCredentials
  scope: PRIVSET.Global Write Privileges
- description: As an HCI Cluster Administrator, you can view and manage HCI Clusters, view all the cluster dashboard widgets, view cluster details. This role does not include the ability to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.HCI Cluster Administrator
- description: As an HCI Cluster Operator, you can view and manage HCI Clusters, view all the cluster dashboard widgets, view cluster details. This role provides view only access to hypervisor, storage related inventory and dashboards. This role does not include the ability to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.HCI Cluster Operator
- description: A set of privileges that allows the access to manage HCI clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.HCI Clusters
- description: Manage and configure VM hosts.
  flows:
  - clientCredentials
  scope: PRIVSET.Hosts
- description: A set of privileges that allows the access to manage HyperFlex clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster
- description: As a HyperFlex Cluster Access Operator, you can cross launch CLI and HXConnect.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Access Operator
- description: As a HyperFlex Cluster Administrator, you can create, edit, deploy, and manage HyperFlex Clusters, view all the cluster dashboard widgets, view cluster details, create HyperFlex policies and profiles, execute capacity planning, and launch HyperFlex Connect. This role does not include the ability to claim a device. It also allows the user to run workflows, manage VMs on HyperFlexAP, and manage connected storage. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Administrator
- description: A set of privileges that allows the configuration and deployment of advanced security profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Advanced Security
- description: A set of privileges that allows the configuration and deployment of HyperFlex Cluster backup policy and restore.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Backups
- description: A set of privileges that allows users to execute capacity planning.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Capacity Planning
- description: As a HyperFlex Cluster Data Protection Administrator, you can perform N:1 backups.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Data Protection Administrator
- description: As a HyperFlex Cluster Lifecycle Administrator, you can install, expand, upgrade a HX cluster, execute capacity planning, OS installation, VC plugin installation, security hardening, and launch HyperFlex Connect as admin.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Lifecycle Administrator
- description: A set of privileges that allows the viewing of cluster operation related functionality.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Operations
- description: As a HyperFlex Cluster Operator, you can perform health checks. However, you cannot change cluster configuration.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Operator
- description: A set of privileges that allows to manage HyperFlex policies and profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Profiles
- description: As a HyperFlex Cluster Storage Administrator, you can perform datastore, iSCSI, and storage container CRUD operations.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Storage Administrator
- description: As a HyperFlex Cluster Syslog Administrator, you can configure the external HX Syslog profile.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Syslog Administrator
- description: This allows write access to the Remote Syslog Advanced Security Profile
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster Syslog Profile Control
- description: As a HyperFlex Cluster System Administrator, you can perform most of the system administrator tasks.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster System Administrator
- description: As a HyperFlex Cluster System Operator, you can perform encryption, health checks, and post-install tasks.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Cluster System Operator
- description: A set of privileges that allows users to configure encryption keys.
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex Key Encryption
- description: A set of privileges that grants view only to HyperFlex related functionality
  flows:
  - clientCredentials
  scope: PRIVSET.HyperFlex View Only
- description: A set of privileges that allows the access to detailed hypervisor information and to perform hypervisor related actions. Hypervisors privilege set is the top level privilege set of other privilege set(s) which are mapped to privileges related to hypervisors.
  flows:
  - clientCredentials
  scope: PRIVSET.Hypervisors
- description: Configure network settings and associates IP addresses with servers, supporting both in-band and out-of-band management.
  flows:
  - clientCredentials
  scope: PRIVSET.IMC Access policies
- description: Manage and allow access to Intersight, only for users from trusted IP addresses.
  flows:
  - clientCredentials
  scope: PRIVSET.IP access management
- description: Manage the mapping of IP blocks on servers.
  flows:
  - clientCredentials
  scope: PRIVSET.IP block mapping
- description: Define protocols for interfacing with the server's service processor via the Intelligent Platform Management Interface (IPMI).
  flows:
  - clientCredentials
  scope: PRIVSET.IPMI over LAN policies
- description: Manage the pool containing iSCSI Qualified Names (IQNs) used as initiator identifiers by iSCSI vNICs.
  flows:
  - clientCredentials
  scope: PRIVSET.IQN block mapping
- description: Import and apply foreign configurations, integrating external storage setups.
  flows:
  - clientCredentials
  scope: PRIVSET.Import foreign configurations
- description: Import server profiles from external sources.
  flows:
  - clientCredentials
  scope: PRIVSET.Import server profiles
- description: Install and configure an operating system on a server to make it operational.
  flows:
  - clientCredentials
  scope: PRIVSET.Install operating systems
- description: 'Apply and execute software updates to ensure the latest features, improvements, and security patches are installed on the system. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Install updates
- description: As an Integrated Systems Administrator, you can perform all actions related to Integrated Systems (e.g., FlexPod) like create/edit/delete of an Integrated System. In addition you can perform administrative and management tasks related to devices (including claim), servers, server profiles, UCS domain, switch profiles, hypervisors, network/SAN switches, storage devices. Also, you can define workflow and task definitions and can execute them and view workflow executions.
  flows:
  - clientCredentials
  scope: PRIVSET.Integrated Systems Administrator
- description: As an Integrated Systems Operator, you can view Integrated Systems (e.g., FlexPod) and can run inventory based actions (e.g., Interoperability check). In addition you can view devices, servers, server profiles, UCS domain, switch profiles, hypervisors, network/SAN switches, storage devices and workflows. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - clientCredentials
  scope: PRIVSET.Integrated Systems Operator
- description: Manage and configure integrated systems.
  flows:
  - clientCredentials
  scope: PRIVSET.Integrated systems
- description: As a Kubernetes Administrator, you can create, edit, deploy, and manage Kubernetes Clusters. You can also view all the cluster dashboard widgets, and view cluster details. In addition, you also have privileges to view and manage storage devices associated with the Kubernetes clusters. The capability to view and execute workflows against the Kubernetes clusters is also granted. It also allows the user to run workflows to manage VMs on hypervisor endpoints, and manage connected storage, and creat/view ip pools. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.Kubernetes Administrator
- description: As a Kubernetes Operator, you can view Kubernetes Clusters. You can also view all the cluster dashboard widgets, and view cluster details. In addition, you also have privileges to view storage devices associated with the Kubernetes clusters. The capability to view workflows is also granted. It also allows the user to view VMs on hypervisor endpoints. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.Kubernetes Operator
- description: Manage the network settings for server connectivity within a Local Area Network (LAN).
  flows:
  - clientCredentials
  scope: PRIVSET.LAN Connectivity policies
- description: Attach/detach LDAP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.LDAP policies
- description: As a Launch CLI user, you can access the command-line interface (CLI) for managing and configuring UCS systems, allowing for command execution and system administration tasks.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch CLI as admin
- description: As a Launch CLI as read-only user, you can access the command-line interface (CLI) for UCS systems with read-only permissions, allowing you to view system configurations and status without making changes.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch CLI as read-only
- description: Launch Endpoint Management Interfaces.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch Endpoint Management Interfaces
- description: Manage servers through the IMC interface with administrative privileges.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch IMC as admin
- description: Access servers via the IMC interface with read-only permissions.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch IMC as read-only
- description: Access and manage UCS Manager with full privileges.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch UCS Manager as admin
- description: View UCS Manager interface without changes.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch UCS Manager as read-only
- description: Launch the console for a virtual machine (VM).
  flows:
  - clientCredentials
  scope: PRIVSET.Launch VM consoles
- description: Launch the console for a VM host.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch host consoles
- description: Allows access to a server's KVM console even if the user is not in the same network as the server and the KVM IP is not reachable.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch tunneled vKVM sessions
- description: Allows to launch the virtual keyboard, video, and mouse (KVM) console directly for Fabric Interconnect-attached and standalone servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch vKVM
- description: Allows to launch the virtual keyboard, video, and mouse (KVM) console directly for Fabric Interconnect-attached and standalone servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Launch vKVM sessions
- description: Manage and configure licensing.
  flows:
  - clientCredentials
  scope: PRIVSET.Licensing
- description: Configure throughput and redundancy using Link Aggregation Control Protocol (LACP) for efficient failure detection.
  flows:
  - clientCredentials
  scope: PRIVSET.Link Aggregation policies
- description: Configure Unidirectional Link Detection (UDLD) Admin state and mode.
  flows:
  - clientCredentials
  scope: PRIVSET.Link Control policies
- description: Configure local user preferences, and password properties.
  flows:
  - clientCredentials
  scope: PRIVSET.Local User policies
- description: Users can view and manage locations. This role provides location management privileges to an user.
  flows:
  - clientCredentials
  scope: PRIVSET.Location Management
- description: Control the locator LED functionality to visually locate and identify specific hardware components within a rack.
  flows:
  - clientCredentials
  scope: PRIVSET.Locator LEDs
- description: Manage API Keys.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage API Keys
- description: Manage access control rules and permissions.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Access and Permissions
- description: Manage Authentication and Authorization Tokens.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Auth Tokens
- description: A set of privileges that allow the users to export Intersight managed objects.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Exports
- description: Manage External Syslog.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage External Syslog
- description: Manage Fabric Interconnects.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Fabric Interconnects
- description: A set of privileges that allows the users to manage serverless functions.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Functions
- description: A set of privileges that allows the users to manage geo locations.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Geo Locations
- description: Manage HyperConverged Infrastructure Clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage HCI Clusters
- description: Manage HyperFlex Cluster Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage HyperFlex Cluster Profiles
- description: Manage HyperFlex Clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage HyperFlex Clusters
- description: Manage HyperFlex Advanced Syslog Configuration
  flows:
  - clientCredentials
  scope: PRIVSET.Manage HyperFlex Syslog
- description: A set of privileges that allow the users to execute workflows related to hypervisor and virtual machines management.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Hypervisors
- description: Manage Single Sign On identity providers.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Identity Providers
- description: A set of privileges that allow the users to import Intersight managed objects.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Imports
- description: A set of privileges that allows the users to manage language runtimes for serverless functions.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Language Runtimes
- description: A set of privileges that allows users to add, remove, or alter site templates and policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Nexus Config
- description: A set of privileges that allows users to add, remove, or alter sites.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Nexus Sites
- description: A set of privileges that allows the access to manage Organizations.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Organizations
- description: Manage server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Server Profiles
- description: Manage Servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Servers
- description: A set of privileges that allow the users to manage ServiceItem Instances.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage ServiceItem Instances.
- description: Manage user login sessions.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Sessions
- description: A set of privileges that allow the user to execute workflows related to storage arrays.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Storage Arrays
- description: Manage Switch Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Switch Profiles
- description: A set of privileges that allows the users to manage tag definitions.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Tags
- description: Collect and download techsupport bundles.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Techsupport Bundles
- description: Manage Telemetry allows [READ of broker information](http://druid.io/docs/latest/operations/api-reference.html#broker).
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Telemetry
- description: Manage Unified Edge.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Unified Edge
- description: Manage Unified Edge Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Unified Edge Profiles
- description: A set of privileges that allow the users to manage workflow and custom data type definitions.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Workflow Definitions
- description: A set of privileges that allow the users to manage workload definitions.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Workload Definitions
- description: A set of privileges that allow the users to manage workload deployments.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage Workload Deployments
- description: Suppress and unsuppress alarms.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage alarm suppression
- description: Select products to be enabled for the Intersight account.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage products
- description: Manage targets in the system by adding, claiming, and unclaiming.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage targets
- description: Add a new tech support bundle.
  flows:
  - clientCredentials
  scope: PRIVSET.Manage tech support bundles
- description: Attach/detach Memory policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Memory policies
- description: Change security keys to update encryption or access controls.
  flows:
  - clientCredentials
  scope: PRIVSET.Modify security keys
- description: View and analyze audit logs.
  flows:
  - clientCredentials
  scope: PRIVSET.Monitor audit logs
- description: Configure the snooping, quierer and source IP proxy states.
  flows:
  - clientCredentials
  scope: PRIVSET.Multicast policies
- description: Attach/detach NTP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.NTP policies
- description: As a Network Administrator, you can create, update, delete and view the Managed Network switch objects. The capability to view and execute workflows against the Network switches is also granted. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - clientCredentials
  scope: PRIVSET.Network Administrator
- description: Configure and assign IPv4 and IPv6 addresses, enable dynamic DNS.
  flows:
  - clientCredentials
  scope: PRIVSET.Network Connectivity policies
- description: As a Network Operator, you can view the Managed Network switch objects. The capability to view workflows against the Network switches is also granted. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - clientCredentials
  scope: PRIVSET.Network Operator
- description: As a Nexus Administrator, you have the privileges to perform all Nexus related operations. This includes claiming devices, view license, updating policy configuration, and monitoring the system.
  flows:
  - clientCredentials
  scope: PRIVSET.Nexus Administrator
- description: As a Nexus Analyst, you can run and update the available Nexus Cloud analyzes such as Sustainability, Conformance, Compliance, and others.
  flows:
  - clientCredentials
  scope: PRIVSET.Nexus Analyst
- description: As a Nexus Config Administrator, you can create or modify policy configuration, view license and can initiate the workflow that will activate policy changes. This role does not allow you to claim or remove devices.
  flows:
  - clientCredentials
  scope: PRIVSET.Nexus Config Administrator
- description: As a Nexus Observer, you can generally view the state of all devices. Additional items include things like viewing configured policies, license status and monitoring active flows. This role does not include any permission which allows the system to be changed.
  flows:
  - clientCredentials
  scope: PRIVSET.Nexus Observer
- description: Manage notification rules.
  flows:
  - clientCredentials
  scope: PRIVSET.Notifications and webhooks
- description: Manage OAuth 2.0 applications, including creating, editing, enabling/disabling, and deleting them.
  flows:
  - clientCredentials
  scope: PRIVSET.OAuth 2.0 applications
- description: Manage OAuth 2.0 tokens, including deleting tokens to control access to the system's resources.
  flows:
  - clientCredentials
  scope: PRIVSET.OAuth2 tokens
- description: Manage OS configuration files.
  flows:
  - clientCredentials
  scope: PRIVSET.OS configuration files
- description: Manage OS image links.
  flows:
  - clientCredentials
  scope: PRIVSET.OS image links
- description: Access and operate physical servers, chassis, and domains, along with their respective profiles and pools of Intersight Infrastructure Services.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate
- description: Manage IP pools, including creation and modification.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate IP pools
- description: As an IQN Pool user, you can create, manage, and delete IQN pools to organize and allocate IQNs for network storage resources efficiently.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate IQN pools
- description: Manage MAC pools, including creation and modification.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate MAC pools
- description: Manage resource pools by creating, modifying, deleting pools, and handling resource allocation within them.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate Resource pools
- description: Manage UUID pools by creating, modifying, deleting, and handling the allocation and reservation of UUIDs within those pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate UUID pools
- description: Manage world wide node names (WWNNs) or world wide port name (WWPNs) pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate WWNN and WWPN pools
- description: Operate chassis profiles, deploying and assigning profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate chassis profiles
- description: Manage domain profiles, deploying and assigning them.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate domain profiles
- description: Perform chassis operations like power cycling and resetting.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate physical chassis
- description: Manage physical domain operations related to hardware.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate physical domains
- description: 'Manage physical server operations like powering on/off and resetting. This involves several key actions: server power management, virtual network and host bus adapters (vNIC/vHBA), server storage operations, system maintenance: Covers tasks such as resetting the CMOS, virtual KVM, monitoring and metrics.'
  flows:
  - clientCredentials
  scope: PRIVSET.Operate physical server
- description: Manage resource pool operations like attaching or detaching.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate pools
- description: Manage server power actions.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate server power
- description: Manage server profile operations like deployment and activation.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate server profile
- description: Operate server storage, including clearing configurations and managing security keys.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate server storage
- description: Perform server system operations like rebooting and resetting CMOS.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate server system
- description: Perform operations on virtual host bus adapters (vHBAs), including enabling, disabling, and resetting.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate server vHBAs
- description: Perform operations on virtual network interface cards (vNICs), including enabling, disabling, and resetting.
  flows:
  - clientCredentials
  scope: PRIVSET.Operate server vNICs
- description: A set of privileges that allows the access to manage Organizations.
  flows:
  - clientCredentials
  scope: PRIVSET.Organizations
- description: Configure security, goals, and namespaces for persistent memory modules, ensuring data retention across power cycles.
  flows:
  - clientCredentials
  scope: PRIVSET.Persistent Memory policies
- description: Manage Fabric Interconnect ports, including port roles, types (Ethernet or Fibre Channel), and connection modes.
  flows:
  - clientCredentials
  scope: PRIVSET.Port policies
- description: Power cycle chassis slots to refresh components.
  flows:
  - clientCredentials
  scope: PRIVSET.Power cycle chassis slots
- description: Manage power settings for FI-attached servers and chassis, including profiling and priority.
  flows:
  - clientCredentials
  scope: PRIVSET.Power policies
- description: A set of privileges that allows read access to chassis profiles and chassis profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Read Chassis Profiles and Chassis Profile Templates
- description: A set of privileges that allows read access to domain profiles and domain profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Read Domain Profiles and Domain Profile Templates
- description: As a Read Organizations user, you can view the configuration and status of the organization without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read Organizations
- description: A set of privileges that allows read access to server profiles and server profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Read Server Profiles and Server Profile Templates
- description: As a Read Workflows user, you can view the configuration and status of workflows without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read Workflows
- description: Read-only access to configuration and status of all API keys associated with the account.
  flows:
  - clientCredentials
  scope: PRIVSET.Read all API keys in the account
- description: Read-only access to configuration and status of all OAuth tokens associated with the account.
  flows:
  - clientCredentials
  scope: PRIVSET.Read all OAuth apps in the account
- description: A set of privileges that provides read-only access to services and resources in Intersight.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-Only
- description: Read-only access to configuration and status of all Intersight Infrastructure Services.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only
- description: Read-only access to configuration and status of Adapter Configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Adapter Configuration policies
- description: Read-only access to configuration and status of AuditD policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only AuditD policies
- description: Read-only access to configuration and status of BIOS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only BIOS policies
- description: Read-only access to configuration and status of Boot policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Boot Order policies
- description: Read-only access to configuration and status of CLI policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only CLI policies
- description: Read-only access to configuration and status of Certificate Management policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Certificate Management policies
- description: Read-only access to configuration and status of Device Connector policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Device Connector Policies
- description: Read-only access to configuration and status of Drive Security policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Drive Security policies
- description: Read-only access to configuration and status of Ethernet Adapter policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Ethernet Adapter policies
- description: Read-only access to configuration and status of Ethernet Network Control policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Ethernet Network Control policies
- description: Read-only access to configuration and status of Ethernet Network Group policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Ethernet Network Group policies
- description: Read-only access to configuration and status of Ethernet Network policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Ethernet Network policies
- description: Read-only access to configuration and status of Ethernet QoS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Ethernet QoS policies
- description: Read-only access to configuration and status of FC Zone policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only FC Zone policies
- description: Read-only access to configuration and status of fabric interconnects (FIs).
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Fabric Interconnects
- description: As a Read-only Fibre Channel Adapter Policy user, you can view the configuration and status of Fibre Channel adapter policies without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Fibre Channel Adapter policies
- description: Read-only access to configuration and status of Fibre Channel Network policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Fibre Channel Network policies
- description: Read-only access to configuration and status of Fibre Channel QoS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Fibre Channel QoS policies
- description: Read-only access to configuration and status of Firmware policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Firmware policies
- description: Read-only access to configuration and status of Flow Control policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Flow Control policies
- description: Read-only access to configuration and status of HyperFlex Cluster Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only HyperFlex cluster profiles
- description: Read-only access to configuration and status of HyperFlex (HX) clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only HyperFlex clusters
- description: Read-only access to configuration and status of IMC Access policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only IMC Access policies
- description: Read-only access to configuration and status of IP pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only IP pools
- description: Read-only access to configuration and status of IPMI over LAN policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only IPMI over LAN policies
- description: Read-only access to configuration and status of IQN pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only IQN pools
- description: Read-only access to configuration and status of Kubernetes Cluster Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Kubernetes cluster profiles
- description: Read-only access to configuration and status of LAN Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only LAN Connectivity policies
- description: As a LDAP Policy user, you can view the configuration and status of system QoS policies without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only LDAP policies
- description: Read-only access to configuration and status of Link Aggregation policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Link Aggregation policies
- description: Read-only access to configuration and status of Link Control policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Link Control policies
- description: Read-only access to configuration and status of Local User policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Local User policies
- description: Read-only access to configuration and status of MAC pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only MAC pools
- description: As a Read-only Memory Policy user, you can view the configuration and status of Memory policies without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Memory policies
- description: Read-only access to configuration and status of Multicast policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Multicast policies
- description: Read-only access to configuration and status of NTP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only NTP policies
- description: Read-only access to configuration and status of Network Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Network Connectivity policies
- description: Read-only access to configuration and status of Persistent Memory policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Persistent Memory policies
- description: Read-only access to configuration and status of Port policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Port policies
- description: Read-only access to configuration and status of Power policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Power policies
- description: Read-only access to configuration and status of SAN Connectivity policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only SAN Connectivity policies
- description: Read-only access to configuration and status of SD Card policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only SD Card policies
- description: Read-only access to configuration and status of SMTP policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only SMTP policies
- description: Read-only access to configuration and status of SNMP policies
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only SNMP policies
- description: Read-only access to configuration and status of SOL policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only SOL policies
- description: Read-only access to configuration and status of SSH policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only SSH policies
- description: As a Read-only SSL Certificates user, you can view the configuration and status of SSL certificates without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only SSL Certificates
- description: As a Read-only Scrub Policy user, you can view the configuration and status of Scrub policies without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Scrub policies
- description: Read-only access to configuration and status of Storage policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Storage policies
- description: Read-only access to configuration and status of Switch Control policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Switch Control policies
- description: Read-only access to configuration and status of Syslog policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Syslog policies
- description: Read-only access to configuration and status of System QoS policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only System QoS policies
- description: Read-only access to configuration and status of Thermal policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Thermal policies
- description: Read-only access to configuration and status of UCS Chassis Profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only UCS chassis profile templates
- description: Read-only access to configuration and status of UCS Chassis Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only UCS chassis profiles
- description: Read-only access to configuration and status of UCS Domain Profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only UCS domain profile templates
- description: Read-only access to configuration and status of UCS Domain Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only UCS domain profiles
- description: Read-only access to configuration and status of UCS Server Profile templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only UCS server profile templates
- description: Read-only access to configuration and status of UCS Server Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only UCS server profiles
- description: Read-only access to configuration and status of UUID pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only UUID pools
- description: Read-only access to configuration and status of VLAN policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only VLAN policies
- description: Read-only access to configuration and status of virtual machines (VMs).
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only VMs
- description: Read-only access to configuration and status of VSAN policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only VSAN policies
- description: Read-only access to configuration and status of Virtual KVM policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only Virtual KVM policies
- description: Read-only access to configuration and status of WWNN or WWPN pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only WWNN and WWPN pools
- description: As a Read-only Advisories user, you can view the configuration and status of all advisories without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only all advisories
- description: Read-only access to configuration and status of all alarms.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only all alarms
- description: Read-only access to configuration and details of all audit logs.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only all audit logs
- description: Read-only access to configuration and status of Compute policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only all compute policies
- description: Read-only access to configuration and status of all Management policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only all management policies
- description: Read-only access to configuration and status of all Network policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only all network policies
- description: Read-only access to configuration and status of all policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only all policies
- description: Read-only access to configuration and status of Storage policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only all storage policies
- description: Read-only access to configuration and status of chassis.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only chassis
- description: As a Read-only Hosts user, you can view the configuration and status of hosts without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only hosts
- description: Read-only access to configuration and status of iSCSI Adapter policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only iSCSI Adapter policies
- description: Read-only access to configuration and status of iSCSI Boot policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only iSCSI Boot policies
- description: Read-only access to configuration and status of iSCSI Static Target policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only iSCSI Static Target policies
- description: Read-only access to configuration and status of integrated systems.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only integrated systems
- description: As a Read-only licensing user, you can view the configuration and status of licensing without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only licensing
- description: Read-only access to configuration and status of metrics explorations.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only metrics explorations
- description: Read-only access to configuration and status of networking settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only networking
- description: Read-only access to configuration and status of all pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only pools
- description: Read-only access to configuration and status of all Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only profiles
- description: Read-only access to configuration and status of Resource pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only resource pools
- description: Read-only access to configuration and status of servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only servers
- description: As a Red-only Software Repository user, you can view the configuration and status of the software repository without making any modifications.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only software repository
- description: Read-only access to configuration and status of storage.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only storage
- description: Read-only access to configuration and status of targets.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only targets
- description: Read-only access to configuration and status of Tech Support Bundles
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only tech support bundles
- description: Read-only access to configuration and status of all templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only templates
- description: Read-only access to configuration and status of vHBA templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only vHBA templates
- description: Read-only access to configuration and status of vMedia policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only vMedia policies
- description: Read-only access to configuration and status of vNIC templates.
  flows:
  - clientCredentials
  scope: PRIVSET.Read-only vNIC templates
- description: As a Reboot Fabric Interconnect user, you can restart the fabric interconnect, allowing for system updates, configuration changes, or recovery from issues.
  flows:
  - clientCredentials
  scope: PRIVSET.Reboot Fabric Interconnect
- description: Restart the management controller of a server.
  flows:
  - clientCredentials
  scope: PRIVSET.Reboot management controllers
- description: Reactivate and restore a previously decommissioned Fabric Extenders (FEX), reestablishing connections and updating the system status.
  flows:
  - clientCredentials
  scope: PRIVSET.Recommission Fabric Extender (FEX)
- description: Reactivate and restore previously decommissioned chassis.
  flows:
  - clientCredentials
  scope: PRIVSET.Recommission chassis
- description: Bring a previously decommissioned server back into operational status. Allows read access to Fabric Interconnect.
  flows:
  - clientCredentials
  scope: PRIVSET.Recommission servers
- description: As a Rediscover Fabric Extender user, you can initiate a rediscovery process for fabric extenders,
  flows:
  - clientCredentials
  scope: PRIVSET.Rediscover Fabric Extender (FEX)
- description: Initiate a process to re-scan and identify chassis in the network, updating their status and configurations.
  flows:
  - clientCredentials
  scope: PRIVSET.Rediscover chassis
- description: Initiate a process to re-scan and identify servers in the network, updating their status and configurations.
  flows:
  - clientCredentials
  scope: PRIVSET.Rediscover servers
- description: Refresh or recreate a domain name within the system, updating its configuration or resolving issues related to network addressing and resource identification.
  flows:
  - clientCredentials
  scope: PRIVSET.Regenerate domain names
- description: 'Register Intersight licenses with Cisco Smart Licensing. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Register licenses
- description: Reject Publish Requests
  flows:
  - clientCredentials
  scope: PRIVSET.Reject Publish Requests
- description: Safely disconnect and remove Fabric Extenders (FEX) from the system, ensuring proper management of dependencies.
  flows:
  - clientCredentials
  scope: PRIVSET.Remove Fabric Extender (FEX)
- description: Safely disconnect and remove chassis, ensuring all dependencies are managed.
  flows:
  - clientCredentials
  scope: PRIVSET.Remove chassis
- description: Disconnect the server from the network, erase all data, and update inventory records to reflect the change.
  flows:
  - clientCredentials
  scope: PRIVSET.Remove servers
- description: 'Update the Intersight license to include any changes on Cisco Smart Software Manager. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Renew licenses
- description: Oversee the replacement process for Fabric Interconnects (FIs).
  flows:
  - clientCredentials
  scope: PRIVSET.Replace Fabric Interconnect
- description: 'Reserve licensing slots for specific private virtual appliance (PVA). Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Reserve licenses
- description: AReset CMOS settings, restoring BIOS to default.
  flows:
  - clientCredentials
  scope: PRIVSET.Reset CMOS
- description: Reboot Input/Output Module (IOM) or Intelligent Fabric Module (IFM).
  flows:
  - clientCredentials
  scope: PRIVSET.Reset IOMs and IFMs
- description: Reset a virtual machine (VM).
  flows:
  - clientCredentials
  scope: PRIVSET.Reset VMs
- description: Reset memory errors on servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Reset memory errors
- description: Reboot peer IOM or IFM to resolve issues.
  flows:
  - clientCredentials
  scope: PRIVSET.Reset peer IOMs and IFMs
- description: Reset vKVM session, restarting the interface.
  flows:
  - clientCredentials
  scope: PRIVSET.Reset vKVM
- description: Restart a virtual machine (VM).
  flows:
  - clientCredentials
  scope: PRIVSET.Restart VMs
- description: 'Deregister the Intersight private virtual appliance (PVA) license after the initial setup. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Return licenses
- description: As a Run Workflows user, you can execute workflows in the system.
  flows:
  - clientCredentials
  scope: PRIVSET.Run Workflows
- description: Run an interoperability check on integrated systems.
  flows:
  - clientCredentials
  scope: PRIVSET.Run interoperability checks
- description: As a SAN Administrator, you can create, update, delete and view the Managed SAN switch objects. The capability to view and execute workflows against the SAN switches is also granted. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - clientCredentials
  scope: PRIVSET.SAN Administrator
- description: Manage storage area network (SAN) settings for servers.
  flows:
  - clientCredentials
  scope: PRIVSET.SAN Connectivity policies
- description: As a SAN Operator, you can view the Managed SAN switch objects. The capability to view workflows against the SAN switches is also granted. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - clientCredentials
  scope: PRIVSET.SAN Operator
- description: Manage server configuration utility (SCU) links.
  flows:
  - clientCredentials
  scope: PRIVSET.SCU links
- description: Configure the Cisco FlexFlash and FlexUtil Secure Digital (SD) cards for Cisco UCS servers. This policy specifies details of virtual drives on the SD cards and allows configuration in different modes such as Operating System Only, Utility Only, or Operating System + Utility modes.
  flows:
  - clientCredentials
  scope: PRIVSET.SD Card policies
- description: Manage SD card operations like mounting and formatting.
  flows:
  - clientCredentials
  scope: PRIVSET.SD card operations
- description: Set SMTP client preferences for outgoing communications on managed devices.
  flows:
  - clientCredentials
  scope: PRIVSET.SMTP policies
- description: Manage SNMP settings for sending alerts and traps from managed devices.
  flows:
  - clientCredentials
  scope: PRIVSET.SNMP policies
- description: Manage access control and settings for Secure Shell (SSH) connections, allowing secure remote management.
  flows:
  - clientCredentials
  scope: PRIVSET.SSH policies
- description: 'As a user with access to SSL Certificates, you can view and manage the SSL certificates used for secure communications within the system. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.SSL Certificates
- description: Save or clone an existing exploration.
  flows:
  - clientCredentials
  scope: PRIVSET.Save and clone explorations
- description: As a Scrub Policy user, you can create, edit, delete, and manage virtual media policies, allowing you to configure and control remote media access for servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Scrub policies
- description: Configure data collection and connection to Intersight.
  flows:
  - clientCredentials
  scope: PRIVSET.Security and privacy
- description: Manage remote access to the management console through the server's management interface, facilitating troubleshooting and server management without a direct connection.
  flows:
  - clientCredentials
  scope: PRIVSET.Serial Over LAN policies
- description: As a Server Administrator, you can view and manage UCS Servers and Fabric Interconnects, view all the server and Fabric Interconnect dashboard widgets, perform server actions, view server details, launch management interfaces and the CLI, create and deploy server policies and profiles, and manage API keys. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.Server Administrator
- description: A set of privileges that allows to manage server policies and server profiles. Server Policy Management privilege set is the top level privilege set of other privilege set(s) which are mapped to privileges related to server policy management.
  flows:
  - clientCredentials
  scope: PRIVSET.Server Profiles
- description: Remove virtual drives, managing storage volumes.
  flows:
  - clientCredentials
  scope: PRIVSET.Server delete virtual drives
- description: Enable or disable vHBAs to control storage operations.
  flows:
  - clientCredentials
  scope: PRIVSET.Server enable and disable vHBAs
- description: Enable or disable vNICs to manage network participation.
  flows:
  - clientCredentials
  scope: PRIVSET.Server enable and disable vNICs
- description: Initiate a hard reset on servers, restarting hardware without a graceful shutdown.
  flows:
  - clientCredentials
  scope: PRIVSET.Server hard reset
- description: Perform a power cycle on servers, rebooting hardware.
  flows:
  - clientCredentials
  scope: PRIVSET.Server power cycle
- description: Safely power off servers, terminating operations.
  flows:
  - clientCredentials
  scope: PRIVSET.Server power off
- description: Initiate the power-on sequence for server activation.
  flows:
  - clientCredentials
  scope: PRIVSET.Server power on
- description: Reset vHBAs to resolve issues or refresh state.
  flows:
  - clientCredentials
  scope: PRIVSET.Server reset vHBAs
- description: Reset vNICs to resolve issues or refresh state.
  flows:
  - clientCredentials
  scope: PRIVSET.Server reset vNICs
- description: Perform a secure erase on drives, permanently removing data.
  flows:
  - clientCredentials
  scope: PRIVSET.Server secure erase drives
- description: Change drive states to control availability.
  flows:
  - clientCredentials
  scope: PRIVSET.Server set drive states
- description: Initiate a graceful shutdown, ensuring services close properly before powering down.
  flows:
  - clientCredentials
  scope: PRIVSET.Server shutdown OS
- description: A set of privileges that allows the access to detailed server information and to perform server related actions. Servers privilege set is the top level privilege set of other privilege set(s) which are mapped to privileges related to servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Servers
- description: As a Service Designer, you can create tasks, workflows, custom datatypes, resource selection criteria, and use these building blocks to create service items. The service items are used to create resources with attributes in Intersight and associate with deploy, maintenance, and decommission actions on the resource.
  flows:
  - clientCredentials
  scope: PRIVSET.Service Designer
- description: As a Service Operator, you can view and update the catalog items, service items, and workflows. You can deploy these resources and validate the catalog or service items.
  flows:
  - clientCredentials
  scope: PRIVSET.Service Operator
- description: Manage and view active sessions.
  flows:
  - clientCredentials
  scope: PRIVSET.Sessions
- description: Assign and manage user labels for Fabric Interconnect.
  flows:
  - clientCredentials
  scope: PRIVSET.Set Fabric Interconnect user labels
- description: Assign and manage integrated management controller (IMC) certificates on servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Set IMC certificates
- description: Assign and manage key management interoperability protocol (KMIP) in Intersight for cryptographic keys and client certificates on servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Set KMIP client certificates
- description: Assign or unassign tags to IP address pools for categorization.
  flows:
  - clientCredentials
  scope: PRIVSET.Set and unset IP pool tags
- description: As a Set or Unset chassis profile Tag user, you can apply tags to chassis profiles to categorize and manage them more effectively within your infrastructure.
  flows:
  - clientCredentials
  scope: PRIVSET.Set and unset chassis profile tags
- description: As a Set or Unset Domain Profile Tag user, you can assign, update or remove tags on a chassis profile.
  flows:
  - clientCredentials
  scope: PRIVSET.Set and unset domain profile tags
- description: As a Set Server or Unset Profile Tag user, you can assign, remove and manage tags for server profiles. This includes creating, updating, and ensuring tags are correctly applied for improved categorization and identification.
  flows:
  - clientCredentials
  scope: PRIVSET.Set and unset server profile tags
- description: Assign and manage user labels for chassis profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Set chassis profile user labels
- description: Assign and manage user labels for chassis.
  flows:
  - clientCredentials
  scope: PRIVSET.Set chassis user labels
- description: Assign and manage user labels for domain profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Set domain profile user labels
- description: As a Set or Unset Fabric Interconnect Tag user, you can assign, update or remove tags.
  flows:
  - clientCredentials
  scope: PRIVSET.Set or Unset Fabric Interconnect Tag
- description: As a Set or Unset IQN Pool Tags user, you can assign tags to IQN pools or you can remove tags from IQN pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Set or Unset IQN Pool Tags
- description: As a Set or Unset MAC Pool Tags user, you can assign tags to MAC address pools or you can remove tags from MAC address pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Set or Unset MAC Pool Tags
- description: As a Set or Unset Resource Pool Tags user, you can assign tags to resource pools or you can remove tags from resource pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Set or Unset Resource Pool Tags
- description: As a Set or unset Server Tag user, you can assign, remove and manage tags for servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Set or Unset Server Tag
- description: As a Set or Unset UUID Pool Tags user, you can assign tags to UUID pools or you can remove tags from UUID pools.
  flows:
  - clientCredentials
  scope: PRIVSET.Set or Unset UUID Pool Tags
- description: As a Set or Unset chassis Tag user, you can assign update or remove tags on a chassis for better identification and management.
  flows:
  - clientCredentials
  scope: PRIVSET.Set or Unset chassis Tag
- description: Set or remove unique IDs for Fibre Channel resources on a server.
  flows:
  - clientCredentials
  scope: PRIVSET.Set or unset WWNN or WWPN pool tags
- description: Assign and manage asset tags for servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Set server asset tags
- description: Assign and manage Intersight license tiers for servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Set server license tiers
- description: Assign and manage user labels for server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.Set server profile user labels
- description: Assign and manage user labels for servers.
  flows:
  - clientCredentials
  scope: PRIVSET.Set server user labels
- description: Manage single sign-on (SSO) integrations and authentication methods for seamless access to multiple applications.
  flows:
  - clientCredentials
  scope: PRIVSET.Single sign-on
- description: Perform a soft stop on a virtual machine (VM).
  flows:
  - clientCredentials
  scope: PRIVSET.Soft stop VMs
- description: Manage the software repository.
  flows:
  - clientCredentials
  scope: PRIVSET.Software repository
- description: Start or resume a virtual machine (VM).
  flows:
  - clientCredentials
  scope: PRIVSET.Start and resume VMs
- description: Stop a virtual machine (VM).
  flows:
  - clientCredentials
  scope: PRIVSET.Stop VMs
- description: As a Storage Administrator, a user can view and manage Storage devices, view and execute workflows and view all the storage dashboard widgets. This privilege does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.Storage Administrator
- description: A set of privileges that allows the access to detailed storage array information and to perform storage array related actions. Storage Arrays privilege set is the top level privilege set of other privilege set(s) which are mapped to privileges related to storage arrays.
  flows:
  - clientCredentials
  scope: PRIVSET.Storage Arrays
- description: Manage storage resources (such as local drives, RAID configurations, and external storage).
  flows:
  - clientCredentials
  scope: PRIVSET.Storage policies
- description: Download server event logs, rediscover servers and chassis, control server and chassis locator LEDs, and start server alarm suppression in Intersight Infrastructure Services.
  flows:
  - clientCredentials
  scope: PRIVSET.Support
- description: As a Support Services user, you can view the dashboard and table views of managed devices, change your user preferences, collect tech support bundles, and generate API keys. In this role, you cannot claim targets, add or remove users, configure Identity Providers, or perform server actions.
  flows:
  - clientCredentials
  scope: PRIVSET.Support Services
- description: Perform chassis support functions such as diagnostics, troubleshooting, and managing chassis health.
  flows:
  - clientCredentials
  scope: PRIVSET.Support chassis
- description: Perform domain support functions such as diagnostics, troubleshooting, and managing domain health.
  flows:
  - clientCredentials
  scope: PRIVSET.Support domains
- description: Perform server support functions such as diagnostics, troubleshooting, and managing server health.
  flows:
  - clientCredentials
  scope: PRIVSET.Support servers
- description: Suspend a virtual machine (VM).
  flows:
  - clientCredentials
  scope: PRIVSET.Suspend VMs
- description: As a Sustainability Metrics Viewer user, you have read access to the Energy Management Capability (EMC) features and the ability register an OAuth2 application for programmatic access to the APIs.
  flows:
  - clientCredentials
  scope: PRIVSET.Sustainability Metrics Viewer
- description: Configure changes on the Fabric Interconnects for transitioning between in-host and switching modes, enabling VLAN Port optimization and managing system VLAN settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Switch Control policies
- description: A set of privileges that allows to manage Switch Profiles and Network configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Switch Profiles
- description: 'As a user with the ability to switch to self-signed Certificate Signing Requests (CSR), you can change the configuration to use self-signed certificates for secure communications. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Switch to Self Signed CSR
- description: Manage and track Cisco licenses directly from the Intersight platform to ensure seamless monitoring of compliance and usage.
  flows:
  - clientCredentials
  scope: PRIVSET.Sync Smart Licensing
- description: Manage local and remote logging capabilities.
  flows:
  - clientCredentials
  scope: PRIVSET.Syslog policies
- description: System related settings of Intersight Infrastructure Services. (Selecting any privilege under this hierarchy will change the scope of privilege set to 'All' and can not be used for 'Organization' scope in Role creation.)
  flows:
  - clientCredentials
  scope: PRIVSET.System Administration
- description: Configure network traffic prioritization by assigning system classes for individual vNICs.
  flows:
  - clientCredentials
  scope: PRIVSET.System QoS policies
- description: Users can view and manage tag definitions. This role provides tag management privileges to an user.
  flows:
  - clientCredentials
  scope: PRIVSET.Tag Management
- description: Manage and configure tech support bundles.
  flows:
  - clientCredentials
  scope: PRIVSET.Tech support bundles
- description: A set of privileges that allows to access to telemetry data. Telemetry privilege set is the top level privilege set of other privilege set(s) which are mapped to privileges related to Telemetry. View Telemetry allows [POST of a Druid query](http://druid.io/docs/latest/querying/querying). Manage Telemetry allows [READ of broker information](http://druid.io/docs/latest/operations/api-reference.html#broker).
  flows:
  - clientCredentials
  scope: PRIVSET.Telemetry
- description: Terminate a virtual machine (VM).
  flows:
  - clientCredentials
  scope: PRIVSET.Terminate VMs
- description: Terminate active vKVM, Tunneled vKVM, and VMRC console sessions launched from Intersight.
  flows:
  - clientCredentials
  scope: PRIVSET.Terminate sessions
- description: Set the fan control mode.
  flows:
  - clientCredentials
  scope: PRIVSET.Thermal policies
- description: As a Manage Traffic Mirroring Sessions user, you can set up and control traffic mirroring sessions to capture and analyze network traffic for monitoring, troubleshooting, or performance analysis.
  flows:
  - clientCredentials
  scope: PRIVSET.Traffic mirroring  SPAN session
- description: Manage trusted certificates for secure communications.
  flows:
  - clientCredentials
  scope: PRIVSET.Trusted certificates
- description: Turn on or off the LED locator on the selected FEX.
  flows:
  - clientCredentials
  scope: PRIVSET.Turn Fabric Extender locator LED on and off
- description: Toggle the locator LED on or off for the chassis to visually locate it within a rack or data center for maintenance.
  flows:
  - clientCredentials
  scope: PRIVSET.Turn chassis locator LEDs on and off
- description: Toggle the locator LED on or off to visually locate the server within a rack or data center for maintenance.
  flows:
  - clientCredentials
  scope: PRIVSET.Turn server locator LEDs on and off
- description: As a UCS Domain Administrator, you can view and manage Switch Profiles and Network Configuration Policies, view Fabric Interconnect dashboard widgets, perform actions on Switch, launch management interfaces and the CLI, create and deploy switch policies and profiles, and manage API keys. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.UCS Domain Administrator
- description: Remove domain profiles from servers, disconnecting settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Unassign chassis profiles
- description: Remove domain profiles, disconnecting server settings.
  flows:
  - clientCredentials
  scope: PRIVSET.Unassign domain profiles
- description: Unassign the server from the profile.
  flows:
  - clientCredentials
  scope: PRIVSET.Unassign server profiles
- description: 'Remove the association of a device connector from its current claim to allow reconfiguration or reassignment to a different system or user. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Unclaim device connector
- description: Remove a target from the system's management or monitoring scope.
  flows:
  - clientCredentials
  scope: PRIVSET.Unclaim targets
- description: A set of privileges that allows to perform operations related to Unified Edge chassis.
  flows:
  - clientCredentials
  scope: PRIVSET.Unified Edge
- description: As a Unified Edge Administrator, you can view and manage Switch Profiles and Network Configuration Policies, view Unified Edge dashboard widgets, perform actions on Switch, launch management interfaces and the CLI, create and deploy switch policies and profiles, and manage API keys. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.Unified Edge Administrator
- description: A set of privileges that allows to manage Unified Edge Profiles, Network and Chassis configuration policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Unified Edge Profiles
- description: Control access to the server's front panel.
  flows:
  - clientCredentials
  scope: PRIVSET.Unlock and lock front panels
- description: Unlock encrypted disks to grant data access.
  flows:
  - clientCredentials
  scope: PRIVSET.Unlock disks
- description: 'Reserve licenses again and generate a new authorization code in Smart Licensing Manager. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Update reserved licenses
- description: Update the firmware of a chassis.
  flows:
  - clientCredentials
  scope: PRIVSET.Upgrade chassis firmware
- description: Update the firmware for a Domain.
  flows:
  - clientCredentials
  scope: PRIVSET.Upgrade domain firmware
- description: Disconnect the server from the network, erase all data, and update inventory records to reflect the change.
  flows:
  - clientCredentials
  scope: PRIVSET.Upgrade server firmware
- description: As a User Access Administrator, you can add and manage Users and Groups in Intersight, view account details and audit logs, manage the IdPs, roles, sessions and API keys for non Account Administrator users. However, you cannot claim a device or perform any management tasks in Intersight. You cannot add or manage a user with Account Administrator role.
  flows:
  - clientCredentials
  scope: PRIVSET.User Access Administrator
- description: Set up network segmentation by defining VLANs specific to organizations.
  flows:
  - clientCredentials
  scope: PRIVSET.VLAN policies
- description: Configure Virtual Storage Area Networks (VSANs) on fabric fibre channel uplinks.
  flows:
  - clientCredentials
  scope: PRIVSET.VSAN policies
- description: Perform checks and validations on domain names to ensure correctness and functionality for network addressing and resource identification.
  flows:
  - clientCredentials
  scope: PRIVSET.Verify domain names
- description: View access control rules and permissions.
  flows:
  - clientCredentials
  scope: PRIVSET.View Access and Permissions
- description: View Approval Requests
  flows:
  - clientCredentials
  scope: PRIVSET.View Approval Requests
- description: View audit logs.
  flows:
  - clientCredentials
  scope: PRIVSET.View Audit Logs
- description: View and monitor datacenters.
  flows:
  - clientCredentials
  scope: PRIVSET.View Datacenters
- description: A set of privileges that allows read access to devices.
  flows:
  - clientCredentials
  scope: PRIVSET.View Devices
- description: A set of privileges that allow users to view export operations.
  flows:
  - clientCredentials
  scope: PRIVSET.View Exports
- description: View Fabric Interconnects.
  flows:
  - clientCredentials
  scope: PRIVSET.View Fabric Interconnects
- description: A set of privileges that allows the users to view serverless functions.
  flows:
  - clientCredentials
  scope: PRIVSET.View Functions
- description: View HyperConverged Infrastructure Clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.View HCI Clusters
- description: View HyperFlex Cluster Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.View HyperFlex Cluster Profiles
- description: View HyperFlex Clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.View HyperFlex Clusters
- description: A set of privileges that allow users to view hypervisor and virtual machines related inventory and dashboards.
  flows:
  - clientCredentials
  scope: PRIVSET.View Hypervisors
- description: A set of privileges that allow users to view the import operations.
  flows:
  - clientCredentials
  scope: PRIVSET.View Imports
- description: A set of privileges that allows the users to view language runtimes for serverless functions.
  flows:
  - clientCredentials
  scope: PRIVSET.View Language Runtimes
- description: View Licensing Status
  flows:
  - clientCredentials
  scope: PRIVSET.View Licensing Status
- description: A set of privileges that allow the users to view the network switches.
  flows:
  - clientCredentials
  scope: PRIVSET.View Network Switches
- description: A set of privileges that allows users to view their site templates and policies.
  flows:
  - clientCredentials
  scope: PRIVSET.View Nexus Config
- description: A set of privileges that allow the users to view nexus reports.
  flows:
  - clientCredentials
  scope: PRIVSET.View Nexus Reports
- description: A set of privileges that allows users to view their onboarded sites and status.
  flows:
  - clientCredentials
  scope: PRIVSET.View Nexus Sites
- description: View Organizations
  flows:
  - clientCredentials
  scope: PRIVSET.View Organizations
- description: A set of privileges that allow the users to view the SAN switches.
  flows:
  - clientCredentials
  scope: PRIVSET.View SAN Switches
- description: View server profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.View Server Profiles
- description: View Servers.
  flows:
  - clientCredentials
  scope: PRIVSET.View Servers
- description: A set of privileges that allow the users to view storage related inventory and dashboards.
  flows:
  - clientCredentials
  scope: PRIVSET.View Storage Arrays
- description: View Switch Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.View Switch Profiles
- description: allows [POST of a Druid query](http://druid.io/docs/latest/querying/querying).
  flows:
  - clientCredentials
  scope: PRIVSET.View Telemetry
- description: View Unified Edge.
  flows:
  - clientCredentials
  scope: PRIVSET.View Unified Edge
- description: View Unified Edge Profiles.
  flows:
  - clientCredentials
  scope: PRIVSET.View Unified Edge Profiles
- description: A set of privileges that allow the users to view the workflow, task and custom data type definitions.
  flows:
  - clientCredentials
  scope: PRIVSET.View Workflow Definitions
- description: A set of privileges that allow the users to view the running instances of the workflows.
  flows:
  - clientCredentials
  scope: PRIVSET.View Workflow Executions
- description: A set of privileges that allow the users to view workload definitions.
  flows:
  - clientCredentials
  scope: PRIVSET.View Workload Definitions
- description: A set of privileges that allow the users to view workload deployments.
  flows:
  - clientCredentials
  scope: PRIVSET.View Workload Deployments
- description: View and monitor clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.View clusters
- description: View and monitor datastore clusters.
  flows:
  - clientCredentials
  scope: PRIVSET.View datastore clusters
- description: View and monitor datastores.
  flows:
  - clientCredentials
  scope: PRIVSET.View datastores
- description: View and terminate active vKVM, Tunneled vKVM, and VMRC console sessions launched from Intersight, and view session history.
  flows:
  - clientCredentials
  scope: PRIVSET.View sessions
- description: Manage and configure virtual machine (VM) templates.
  flows:
  - clientCredentials
  scope: PRIVSET.View virtual machine templates
- description: Attach/detach Virtual KVM policies.
  flows:
  - clientCredentials
  scope: PRIVSET.Virtual KVM policies
- description: Enable the virtual media service on the endpoint, encryption of all communications and low power USB.
  flows:
  - clientCredentials
  scope: PRIVSET.Virtual Media policies
- description: 'Manage the licensing for virtual appliance (VA). Learn more, Introduction to Licensing. Note: This is a virtual appliance only privilege.'
  flows:
  - clientCredentials
  scope: PRIVSET.Virtual appliance licensing
- description: Manage and configure virtual machines (VMs).
  flows:
  - clientCredentials
  scope: PRIVSET.Virtual machines
- description: As a Virtualization Administrator, a user can view and manage hypervisor resources, view and execute workflows. This privilege does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - clientCredentials
  scope: PRIVSET.Virtualization Administrator
- description: Manage and configure virtualization hosts.
  flows:
  - clientCredentials
  scope: PRIVSET.Virtualization hosts
- description: Withdraw Approvals
  flows:
  - clientCredentials
  scope: PRIVSET.Withdraw Approvals
- description: As a Workflow Designer, you can define workflow definitions and custom data types, view workflow definitions, task definitions and custom data types, execute workflows and view workflow executions.
  flows:
  - clientCredentials
  scope: PRIVSET.Workflow Designer
- description: As a Workload Administrator, you can define workload definitions using Blueprints and underlying ServiceItems and workflow definitions. You can also define workload deployments using Workload Definitions and deploy workloads to target devices.
  flows:
  - clientCredentials
  scope: PRIVSET.Workload Administrator
- description: As a Workload Designer, you can define workload definitions using Blueprints and underlying ServiceItems and workflow definitions.
  flows:
  - clientCredentials
  scope: PRIVSET.Workload Designer
- description: As a Workload Operator, you can define workload deployments using Workload Definitions and deploy workloads to target devices.
  flows:
  - clientCredentials
  scope: PRIVSET.Workload Operator
- description: As a Workload Optimizer Administrator, you can access all Workload Optimizer features and perform administrative tasks to configure Workload Optimizer.
  flows:
  - clientCredentials
  scope: PRIVSET.Workload Optimizer Administrator
- description: As a Workload Optimizer Advisor, you can view workload optimization state and recommended actions, run plans for workload optimization.
  flows:
  - clientCredentials
  scope: PRIVSET.Workload Optimizer Advisor
- description: As a Workload Optimizer Automator, you can view workload optimization state, recommended actions, run plans for workload optimization, execute workload optimization actions, and deploy workloads.
  flows:
  - clientCredentials
  scope: PRIVSET.Workload Optimizer Automator
- description: As a Workload Optimizer Deployer, you can view all Workload Optimizer charts and data, deploy workloads, and create policies and templates. You cannot run plans or execute any recommended actions.
  flows:
  - clientCredentials
  scope: PRIVSET.Workload Optimizer Deployer
- description: As a Workload Optimizer Observer, you can view workload optimization state and recommended actions.
  flows:
  - clientCredentials
  scope: PRIVSET.Workload Optimizer Observer
- description: Configure settings for iSCSI traffic management, including TCP Connection Timeout, DHCP Timeout, and Retry Count for busy LUN IDs, optimizing iSCSI boot configurations.
  flows:
  - clientCredentials
  scope: PRIVSET.iSCSI Adapter policies
- description: Configure settings required to enable a server to boot from an iSCSI-based storage device.
  flows:
  - clientCredentials
  scope: PRIVSET.iSCSI Boot policies
- description: Define static iSCSI target configuration settings for servers that need to connect to specific storage devices over the iSCSI protocol.
  flows:
  - clientCredentials
  scope: PRIVSET.iSCSI Static Target policies
- description: As a vKVM-only user, you can launch vKVM and tunneled vKVM sessions to a server from Intersight. In addition you can view servers, chassis and the running workflows. In this role, you cannot perform any server actions from Intersight apart from launching vKVM.
  flows:
  - clientCredentials
  scope: PRIVSET.vKVM Only
- description: Read a 'aaa.AuditRecord' resource.
  flows:
  - clientCredentials
  scope: READ.aaa.AuditRecord
- description: Read a 'aaa.RetentionConfig' resource.
  flows:
  - clientCredentials
  scope: READ.aaa.RetentionConfig
- description: Read a 'aaa.RetentionPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.aaa.RetentionPolicy
- description: Read a 'access.IpAddress' resource.
  flows:
  - clientCredentials
  scope: READ.access.IpAddress
- description: Read a 'access.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.access.Policy
- description: Read a 'access.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.access.PolicyInventory
- description: Read a 'adapter.ConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.adapter.ConfigPolicy
- description: Read a 'adapter.ExtEthInterface' resource.
  flows:
  - clientCredentials
  scope: READ.adapter.ExtEthInterface
- description: Read a 'adapter.HostEthInterface' resource.
  flows:
  - clientCredentials
  scope: READ.adapter.HostEthInterface
- description: Read a 'adapter.HostFcInterface' resource.
  flows:
  - clientCredentials
  scope: READ.adapter.HostFcInterface
- description: Read a 'adapter.HostIscsiInterface' resource.
  flows:
  - clientCredentials
  scope: READ.adapter.HostIscsiInterface
- description: Read a 'adapter.Unit' resource.
  flows:
  - clientCredentials
  scope: READ.adapter.Unit
- description: Read a 'adapter.UnitExpander' resource.
  flows:
  - clientCredentials
  scope: READ.adapter.UnitExpander
- description: Read a 'apic.AciPod' resource.
  flows:
  - clientCredentials
  scope: READ.apic.AciPod
- description: Read a 'apic.Application' resource.
  flows:
  - clientCredentials
  scope: READ.apic.Application
- description: Read a 'apic.ApplicationEndpointGroup' resource.
  flows:
  - clientCredentials
  scope: READ.apic.ApplicationEndpointGroup
- description: Read a 'apic.BridgeDomain' resource.
  flows:
  - clientCredentials
  scope: READ.apic.BridgeDomain
- description: Read a 'apic.ExternalRoutedLayerThreeDomain' resource.
  flows:
  - clientCredentials
  scope: READ.apic.ExternalRoutedLayerThreeDomain
- description: Read a 'apic.FabricLeafNode' resource.
  flows:
  - clientCredentials
  scope: READ.apic.FabricLeafNode
- description: Read a 'apic.FabricLeafNodeInterface' resource.
  flows:
  - clientCredentials
  scope: READ.apic.FabricLeafNodeInterface
- description: Read a 'apic.Out' resource.
  flows:
  - clientCredentials
  scope: READ.apic.Out
- description: Read a 'apic.Subnet' resource.
  flows:
  - clientCredentials
  scope: READ.apic.Subnet
- description: Read a 'apic.Tenant' resource.
  flows:
  - clientCredentials
  scope: READ.apic.Tenant
- description: Read a 'apic.VpcGroup' resource.
  flows:
  - clientCredentials
  scope: READ.apic.VpcGroup
- description: Read a 'apic.Vrfs' resource.
  flows:
  - clientCredentials
  scope: READ.apic.Vrfs
- description: Read a 'apiproxy.AllowList' resource.
  flows:
  - clientCredentials
  scope: READ.apiproxy.AllowList
- description: Read a 'appliance.AppOpStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.AppOpStatus
- description: Read a 'appliance.AppStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.AppStatus
- description: Read a 'appliance.AutoRmaPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.AutoRmaPolicy
- description: Read a 'appliance.Backup' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.Backup
- description: Read a 'appliance.BackupDownload' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.BackupDownload
- description: Read a 'appliance.BackupMonitor' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.BackupMonitor
- description: Read a 'appliance.BackupPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.BackupPolicy
- description: Read a 'appliance.BackupRotateData' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.BackupRotateData
- description: Read a 'appliance.CertificateSetting' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.CertificateSetting
- description: Read a 'appliance.ClusterInfo' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.ClusterInfo
- description: Read a 'appliance.ClusterInstall' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.ClusterInstall
- description: Read a 'appliance.ClusterReplaceNode' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.ClusterReplaceNode
- description: Read a 'appliance.ClusterWorkerNode' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.ClusterWorkerNode
- description: Read a 'appliance.CpuUtilization' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.CpuUtilization
- description: Read a 'appliance.DataExportPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.DataExportPolicy
- description: Read a 'appliance.DeviceCertificate' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.DeviceCertificate
- description: Read a 'appliance.DeviceClaim' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.DeviceClaim
- description: Read a 'appliance.DeviceClusterInstall' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.DeviceClusterInstall
- description: Read a 'appliance.DeviceState' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.DeviceState
- description: Read a 'appliance.DeviceUpgradePolicy' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.DeviceUpgradePolicy
- description: Read a 'appliance.DiagSetting' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.DiagSetting
- description: Read a 'appliance.ExternalSyslogSetting' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.ExternalSyslogSetting
- description: Read a 'appliance.FileGateway' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.FileGateway
- description: Read a 'appliance.FileSystemOpStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.FileSystemOpStatus
- description: Read a 'appliance.FileSystemOpSummary' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.FileSystemOpSummary
- description: Read a 'appliance.FileSystemStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.FileSystemStatus
- description: Read a 'appliance.FileSystemTelemetry' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.FileSystemTelemetry
- description: Read a 'appliance.FqdnUpdate' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.FqdnUpdate
- description: Read a 'appliance.GroupOpStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.GroupOpStatus
- description: Read a 'appliance.GroupStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.GroupStatus
- description: Read a 'appliance.ImageBundle' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.ImageBundle
- description: Read a 'appliance.MemoryUtilization' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.MemoryUtilization
- description: Read a 'appliance.MetaManifest' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.MetaManifest
- description: Read a 'appliance.MetricsConfig' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.MetricsConfig
- description: Read a 'appliance.MetricsIngestionUtilization' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.MetricsIngestionUtilization
- description: Read a 'appliance.NetworkLinkStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.NetworkLinkStatus
- description: Read a 'appliance.NodeInfo' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.NodeInfo
- description: Read a 'appliance.NodeIopsMetric' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.NodeIopsMetric
- description: Read a 'appliance.NodeOpStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.NodeOpStatus
- description: Read a 'appliance.NodeStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.NodeStatus
- description: Read a 'appliance.NodeTelemetry' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.NodeTelemetry
- description: Read a 'appliance.ReleaseNote' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.ReleaseNote
- description: Read a 'appliance.RemoteFileImport' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.RemoteFileImport
- description: Read a 'appliance.Restore' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.Restore
- description: Read a 'appliance.SetupInfo' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.SetupInfo
- description: Read a 'appliance.SystemInfo' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.SystemInfo
- description: Read a 'appliance.SystemOpStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.SystemOpStatus
- description: Read a 'appliance.SystemStatus' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.SystemStatus
- description: Read a 'appliance.Upgrade' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.Upgrade
- description: Read a 'appliance.UpgradePolicy' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.UpgradePolicy
- description: Read a 'appliance.UpgradeTracker' resource.
  flows:
  - clientCredentials
  scope: READ.appliance.UpgradeTracker
- description: Read a 'asset.ClaimToken' resource.
  flows:
  - clientCredentials
  scope: READ.asset.ClaimToken
- description: Read a 'asset.ClusterMember' resource.
  flows:
  - clientCredentials
  scope: READ.asset.ClusterMember
- description: Read a 'asset.Deployment' resource.
  flows:
  - clientCredentials
  scope: READ.asset.Deployment
- description: Read a 'asset.DeploymentDevice' resource.
  flows:
  - clientCredentials
  scope: READ.asset.DeploymentDevice
- description: Read a 'asset.DeviceConfiguration' resource.
  flows:
  - clientCredentials
  scope: READ.asset.DeviceConfiguration
- description: Read a 'asset.DeviceConnectorManager' resource.
  flows:
  - clientCredentials
  scope: READ.asset.DeviceConnectorManager
- description: Read a 'asset.DeviceContractInformation' resource.
  flows:
  - clientCredentials
  scope: READ.asset.DeviceContractInformation
- description: Read a 'asset.DeviceRegistration' resource.
  flows:
  - clientCredentials
  scope: READ.asset.DeviceRegistration
- description: Read a 'asset.GeoLocation' resource.
  flows:
  - clientCredentials
  scope: READ.asset.GeoLocation
- description: Read a 'asset.Subscription' resource.
  flows:
  - clientCredentials
  scope: READ.asset.Subscription
- description: Read a 'asset.SubscriptionAccount' resource.
  flows:
  - clientCredentials
  scope: READ.asset.SubscriptionAccount
- description: Read a 'asset.SubscriptionDeviceContractInformation' resource.
  flows:
  - clientCredentials
  scope: READ.asset.SubscriptionDeviceContractInformation
- description: Read a 'asset.Target' resource.
  flows:
  - clientCredentials
  scope: READ.asset.Target
- description: Read a 'auditd.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.auditd.Policy
- description: Read a 'bios.BootDevice' resource.
  flows:
  - clientCredentials
  scope: READ.bios.BootDevice
- description: Read a 'bios.BootMode' resource.
  flows:
  - clientCredentials
  scope: READ.bios.BootMode
- description: Read a 'bios.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.bios.Policy
- description: Read a 'bios.SystemBootOrder' resource.
  flows:
  - clientCredentials
  scope: READ.bios.SystemBootOrder
- description: Read a 'bios.TokenSettings' resource.
  flows:
  - clientCredentials
  scope: READ.bios.TokenSettings
- description: Read a 'bios.Unit' resource.
  flows:
  - clientCredentials
  scope: READ.bios.Unit
- description: Read a 'bios.VfSelectMemoryRasConfiguration' resource.
  flows:
  - clientCredentials
  scope: READ.bios.VfSelectMemoryRasConfiguration
- description: Read a 'boot.CddDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.CddDevice
- description: Read a 'boot.DeviceBootMode' resource.
  flows:
  - clientCredentials
  scope: READ.boot.DeviceBootMode
- description: Read a 'boot.DeviceBootSecurity' resource.
  flows:
  - clientCredentials
  scope: READ.boot.DeviceBootSecurity
- description: Read a 'boot.HddDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.HddDevice
- description: Read a 'boot.IscsiDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.IscsiDevice
- description: Read a 'boot.NvmeDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.NvmeDevice
- description: Read a 'boot.PchStorageDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.PchStorageDevice
- description: Read a 'boot.PrecisionPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.boot.PrecisionPolicy
- description: Read a 'boot.PxeDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.PxeDevice
- description: Read a 'boot.SanDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.SanDevice
- description: Read a 'boot.SdDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.SdDevice
- description: Read a 'boot.UefiShellDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.UefiShellDevice
- description: Read a 'boot.UsbDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.UsbDevice
- description: Read a 'boot.VmediaDevice' resource.
  flows:
  - clientCredentials
  scope: READ.boot.VmediaDevice
- description: Read a 'bulk.Export' resource.
  flows:
  - clientCredentials
  scope: READ.bulk.Export
- description: Read a 'bulk.ExportedItem' resource.
  flows:
  - clientCredentials
  scope: READ.bulk.ExportedItem
- description: Read a 'bulk.MoCloner' resource.
  flows:
  - clientCredentials
  scope: READ.bulk.MoCloner
- description: Read a 'bulk.MoDeepCloner' resource.
  flows:
  - clientCredentials
  scope: READ.bulk.MoDeepCloner
- description: Read a 'bulk.MoMerger' resource.
  flows:
  - clientCredentials
  scope: READ.bulk.MoMerger
- description: Read a 'bulk.Request' resource.
  flows:
  - clientCredentials
  scope: READ.bulk.Request
- description: Read a 'bulk.Result' resource.
  flows:
  - clientCredentials
  scope: READ.bulk.Result
- description: Read a 'bulk.SubRequestObj' resource.
  flows:
  - clientCredentials
  scope: READ.bulk.SubRequestObj
- description: Read a 'capability.ActionsMetaData' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ActionsMetaData
- description: Read a 'capability.AdapterDeprecatedDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.AdapterDeprecatedDef
- description: Read a 'capability.AdapterFirmwareRequirement' resource.
  flows:
  - clientCredentials
  scope: READ.capability.AdapterFirmwareRequirement
- description: Read a 'capability.AdapterUnitDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.AdapterUnitDescriptor
- description: Read a 'capability.AdapterUpdateConstraintMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.AdapterUpdateConstraintMeta
- description: Read a 'capability.AdapterUpgradeSupportMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.AdapterUpgradeSupportMeta
- description: Read a 'capability.BiosTokens' resource.
  flows:
  - clientCredentials
  scope: READ.capability.BiosTokens
- description: Read a 'capability.Catalog' resource.
  flows:
  - clientCredentials
  scope: READ.capability.Catalog
- description: Read a 'capability.ChassisDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ChassisDescriptor
- description: Read a 'capability.ChassisManufacturingDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ChassisManufacturingDef
- description: Read a 'capability.ChassisUpgradeSupportMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ChassisUpgradeSupportMeta
- description: Read a 'capability.CimcFirmwareDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.CimcFirmwareDescriptor
- description: Read a 'capability.CpuEndpointDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.CpuEndpointDescriptor
- description: Read a 'capability.DimmsEndpointDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.DimmsEndpointDescriptor
- description: Read a 'capability.DomainPolicyRequirement' resource.
  flows:
  - clientCredentials
  scope: READ.capability.DomainPolicyRequirement
- description: Read a 'capability.DrivesEndpointDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.DrivesEndpointDescriptor
- description: Read a 'capability.EquipmentPhysicalDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.EquipmentPhysicalDef
- description: Read a 'capability.EquipmentSlotArray' resource.
  flows:
  - clientCredentials
  scope: READ.capability.EquipmentSlotArray
- description: Read a 'capability.FanModuleDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.FanModuleDescriptor
- description: Read a 'capability.FanModuleManufacturingDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.FanModuleManufacturingDef
- description: Read a 'capability.FexCapabilityDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.FexCapabilityDef
- description: Read a 'capability.FexDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.FexDescriptor
- description: Read a 'capability.FexManufacturingDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.FexManufacturingDef
- description: Read a 'capability.FexSupportMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.FexSupportMeta
- description: Read a 'capability.GpuEndpointDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.GpuEndpointDescriptor
- description: Read a 'capability.HsuIsoFileSupportMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.HsuIsoFileSupportMeta
- description: Read a 'capability.IoCardCapabilityDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.IoCardCapabilityDef
- description: Read a 'capability.IoCardDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.IoCardDescriptor
- description: Read a 'capability.IoCardManufacturingDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.IoCardManufacturingDef
- description: Read a 'capability.IomUpgradeSupportMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.IomUpgradeSupportMeta
- description: Read a 'capability.NetworkEquipmentPowerDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.NetworkEquipmentPowerDef
- description: Read a 'capability.PolicyConstants' resource.
  flows:
  - clientCredentials
  scope: READ.capability.PolicyConstants
- description: Read a 'capability.PortGroupAggregationDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.PortGroupAggregationDef
- description: Read a 'capability.ProcessorUnitUpdateConstraintMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ProcessorUnitUpdateConstraintMeta
- description: Read a 'capability.PsuDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.PsuDescriptor
- description: Read a 'capability.PsuManufacturingDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.PsuManufacturingDef
- description: Read a 'capability.ServerActionsMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ServerActionsMeta
- description: Read a 'capability.ServerDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ServerDescriptor
- description: Read a 'capability.ServerModelsCapabilityDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ServerModelsCapabilityDef
- description: Read a 'capability.ServerPcieConnectivityCatalog' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ServerPcieConnectivityCatalog
- description: Read a 'capability.ServerSchemaDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ServerSchemaDescriptor
- description: Read a 'capability.ServerTopologyMap' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ServerTopologyMap
- description: Read a 'capability.ServerUpgradeSupportMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.ServerUpgradeSupportMeta
- description: Read a 'capability.SiocModuleCapabilityDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.SiocModuleCapabilityDef
- description: Read a 'capability.SiocModuleDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.SiocModuleDescriptor
- description: Read a 'capability.SiocModuleManufacturingDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.SiocModuleManufacturingDef
- description: Read a 'capability.StandardRedfishSupportMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.StandardRedfishSupportMeta
- description: Read a 'capability.StorageControllerUpdateConstraintMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.StorageControllerUpdateConstraintMeta
- description: Read a 'capability.StorageControllersMetaData' resource.
  flows:
  - clientCredentials
  scope: READ.capability.StorageControllersMetaData
- description: Read a 'capability.SwitchCapability' resource.
  flows:
  - clientCredentials
  scope: READ.capability.SwitchCapability
- description: Read a 'capability.SwitchDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.SwitchDescriptor
- description: Read a 'capability.SwitchEquipmentInfo' resource.
  flows:
  - clientCredentials
  scope: READ.capability.SwitchEquipmentInfo
- description: Read a 'capability.SwitchManufacturingDef' resource.
  flows:
  - clientCredentials
  scope: READ.capability.SwitchManufacturingDef
- description: Read a 'capability.SwitchUpgradeSupportMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.SwitchUpgradeSupportMeta
- description: Read a 'capability.TemplateCatalog' resource.
  flows:
  - clientCredentials
  scope: READ.capability.TemplateCatalog
- description: Read a 'capability.TimeZoneMetaData' resource.
  flows:
  - clientCredentials
  scope: READ.capability.TimeZoneMetaData
- description: Read a 'capability.UpdateOrderMeta' resource.
  flows:
  - clientCredentials
  scope: READ.capability.UpdateOrderMeta
- description: Read a 'capability.VicDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.capability.VicDescriptor
- description: Read a 'catalystsdwan.ConfigGroup' resource.
  flows:
  - clientCredentials
  scope: READ.catalystsdwan.ConfigGroup
- description: Read a 'catalystsdwan.Interface' resource.
  flows:
  - clientCredentials
  scope: READ.catalystsdwan.Interface
- description: Read a 'catalystsdwan.PhysicalPort' resource.
  flows:
  - clientCredentials
  scope: READ.catalystsdwan.PhysicalPort
- description: Read a 'catalystsdwan.PolicyGroup' resource.
  flows:
  - clientCredentials
  scope: READ.catalystsdwan.PolicyGroup
- description: Read a 'catalystsdwan.PortChannel' resource.
  flows:
  - clientCredentials
  scope: READ.catalystsdwan.PortChannel
- description: Read a 'catalystsdwan.VedgeDevice' resource.
  flows:
  - clientCredentials
  scope: READ.catalystsdwan.VedgeDevice
- description: Read a 'catalystsdwan.Vlan' resource.
  flows:
  - clientCredentials
  scope: READ.catalystsdwan.Vlan
- description: Read a 'catalystsdwan.WanEdgeDevice' resource.
  flows:
  - clientCredentials
  scope: READ.catalystsdwan.WanEdgeDevice
- description: Read a 'certificatemanagement.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.certificatemanagement.Policy
- description: Read a 'certificatemanagement.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.certificatemanagement.PolicyInventory
- description: Read a 'chassis.ConfigChangeDetail' resource.
  flows:
  - clientCredentials
  scope: READ.chassis.ConfigChangeDetail
- description: Read a 'chassis.ConfigImport' resource.
  flows:
  - clientCredentials
  scope: READ.chassis.ConfigImport
- description: Read a 'chassis.ConfigResult' resource.
  flows:
  - clientCredentials
  scope: READ.chassis.ConfigResult
- description: Read a 'chassis.ConfigResultEntry' resource.
  flows:
  - clientCredentials
  scope: READ.chassis.ConfigResultEntry
- description: Read a 'chassis.IomProfile' resource.
  flows:
  - clientCredentials
  scope: READ.chassis.IomProfile
- description: Read a 'chassis.Profile' resource.
  flows:
  - clientCredentials
  scope: READ.chassis.Profile
- description: Read a 'chassis.ProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: READ.chassis.ProfileTemplate
- description: Read a 'cli.CliPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.cli.CliPolicy
- description: Read a 'cloud.TfcAgentpool' resource.
  flows:
  - clientCredentials
  scope: READ.cloud.TfcAgentpool
- description: Read a 'cloud.TfcOrganization' resource.
  flows:
  - clientCredentials
  scope: READ.cloud.TfcOrganization
- description: Read a 'cloud.TfcWorkspace' resource.
  flows:
  - clientCredentials
  scope: READ.cloud.TfcWorkspace
- description: Read a 'comm.HttpProxyPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.comm.HttpProxyPolicy
- description: Read a 'comm.TagDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.comm.TagDefinition
- description: Read a 'compute.Blade' resource.
  flows:
  - clientCredentials
  scope: READ.compute.Blade
- description: Read a 'compute.BladeIdentity' resource.
  flows:
  - clientCredentials
  scope: READ.compute.BladeIdentity
- description: Read a 'compute.Board' resource.
  flows:
  - clientCredentials
  scope: READ.compute.Board
- description: Read a 'compute.DownloadStatus' resource.
  flows:
  - clientCredentials
  scope: READ.compute.DownloadStatus
- description: Read a 'compute.HostUtilityOperation' resource.
  flows:
  - clientCredentials
  scope: READ.compute.HostUtilityOperation
- description: Read a 'compute.Mapping' resource.
  flows:
  - clientCredentials
  scope: READ.compute.Mapping
- description: Read a 'compute.PcieConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.compute.PcieConnectivityPolicy
- description: Read a 'compute.PcieConnectivityPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.compute.PcieConnectivityPolicyInventory
- description: Read a 'compute.Personality' resource.
  flows:
  - clientCredentials
  scope: READ.compute.Personality
- description: Read a 'compute.PhysicalSummary' resource.
  flows:
  - clientCredentials
  scope: READ.compute.PhysicalSummary
- description: Read a 'compute.RackUnit' resource.
  flows:
  - clientCredentials
  scope: READ.compute.RackUnit
- description: Read a 'compute.RackUnitIdentity' resource.
  flows:
  - clientCredentials
  scope: READ.compute.RackUnitIdentity
- description: Read a 'compute.ScrubPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.compute.ScrubPolicy
- description: Read a 'compute.ServerIdPool' resource.
  flows:
  - clientCredentials
  scope: READ.compute.ServerIdPool
- description: Read a 'compute.ServerPowerParameters' resource.
  flows:
  - clientCredentials
  scope: READ.compute.ServerPowerParameters
- description: Read a 'compute.ServerPowerPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.compute.ServerPowerPolicy
- description: Read a 'compute.ServerSetting' resource.
  flows:
  - clientCredentials
  scope: READ.compute.ServerSetting
- description: Read a 'compute.Vmedia' resource.
  flows:
  - clientCredentials
  scope: READ.compute.Vmedia
- description: Read a 'cond.Alarm' resource.
  flows:
  - clientCredentials
  scope: READ.cond.Alarm
- description: Read a 'cond.AlarmAggregation' resource.
  flows:
  - clientCredentials
  scope: READ.cond.AlarmAggregation
- description: Read a 'cond.AlarmClassification' resource.
  flows:
  - clientCredentials
  scope: READ.cond.AlarmClassification
- description: Read a 'cond.AlarmDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.cond.AlarmDefinition
- description: Read a 'cond.AlarmRule' resource.
  flows:
  - clientCredentials
  scope: READ.cond.AlarmRule
- description: Read a 'cond.AlarmSuppression' resource.
  flows:
  - clientCredentials
  scope: READ.cond.AlarmSuppression
- description: Read a 'cond.CustomHclBaseline' resource.
  flows:
  - clientCredentials
  scope: READ.cond.CustomHclBaseline
- description: Read a 'cond.CustomHclStatus' resource.
  flows:
  - clientCredentials
  scope: READ.cond.CustomHclStatus
- description: Read a 'cond.HclStatus' resource.
  flows:
  - clientCredentials
  scope: READ.cond.HclStatus
- description: Read a 'cond.HclStatusDetail' resource.
  flows:
  - clientCredentials
  scope: READ.cond.HclStatusDetail
- description: Read a 'cond.HclStatusJob' resource.
  flows:
  - clientCredentials
  scope: READ.cond.HclStatusJob
- description: Read a 'cond.ThresholdDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.cond.ThresholdDefinition
- description: Read a 'connectorpack.ConnectorPackUpgrade' resource.
  flows:
  - clientCredentials
  scope: READ.connectorpack.ConnectorPackUpgrade
- description: Read a 'connectorpack.UpgradeImpact' resource.
  flows:
  - clientCredentials
  scope: READ.connectorpack.UpgradeImpact
- description: Read a 'console.ConsoleConfig' resource.
  flows:
  - clientCredentials
  scope: READ.console.ConsoleConfig
- description: Read a 'convergedinfra.AdapterComplianceDetails' resource.
  flows:
  - clientCredentials
  scope: READ.convergedinfra.AdapterComplianceDetails
- description: Read a 'convergedinfra.Pod' resource.
  flows:
  - clientCredentials
  scope: READ.convergedinfra.Pod
- description: Read a 'convergedinfra.PodComplianceInfo' resource.
  flows:
  - clientCredentials
  scope: READ.convergedinfra.PodComplianceInfo
- description: Read a 'convergedinfra.ServerComplianceDetails' resource.
  flows:
  - clientCredentials
  scope: READ.convergedinfra.ServerComplianceDetails
- description: Read a 'convergedinfra.StorageComplianceDetails' resource.
  flows:
  - clientCredentials
  scope: READ.convergedinfra.StorageComplianceDetails
- description: Read a 'convergedinfra.SwitchComplianceDetails' resource.
  flows:
  - clientCredentials
  scope: READ.convergedinfra.SwitchComplianceDetails
- description: Read a 'coremanagement.CoreFile' resource.
  flows:
  - clientCredentials
  scope: READ.coremanagement.CoreFile
- description: Read a 'coremanagement.Download' resource.
  flows:
  - clientCredentials
  scope: READ.coremanagement.Download
- description: Read a 'crd.CustomResource' resource.
  flows:
  - clientCredentials
  scope: READ.crd.CustomResource
- description: Read a 'deviceconnector.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.deviceconnector.Policy
- description: Read a 'dnac.Device' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.Device
- description: Read a 'dnac.DeviceInterface' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.DeviceInterface
- description: Read a 'dnac.ExternalBorderNode' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.ExternalBorderNode
- description: Read a 'dnac.ExternalBorderNodeInterface' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.ExternalBorderNodeInterface
- description: Read a 'dnac.FabricSite' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.FabricSite
- description: Read a 'dnac.Site' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.Site
- description: Read a 'dnac.SiteIpPool' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.SiteIpPool
- description: Read a 'dnac.Template' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.Template
- description: Read a 'dnac.Transit' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.Transit
- description: Read a 'dnac.VirtualNetworkFabricSite' resource.
  flows:
  - clientCredentials
  scope: READ.dnac.VirtualNetworkFabricSite
- description: Read a 'equipment.Chassis' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Chassis
- description: Read a 'equipment.ChassisController' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.ChassisController
- description: Read a 'equipment.ChassisIdPool' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.ChassisIdPool
- description: Read a 'equipment.ChassisIdentity' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.ChassisIdentity
- description: Read a 'equipment.ChassisOperation' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.ChassisOperation
- description: Read a 'equipment.DeviceSummary' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.DeviceSummary
- description: Read a 'equipment.EnclosureElement' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.EnclosureElement
- description: Read a 'equipment.EndPointLog' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.EndPointLog
- description: Read a 'equipment.ExpanderModule' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.ExpanderModule
- description: Read a 'equipment.ExpanderModuleIdentity' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.ExpanderModuleIdentity
- description: Read a 'equipment.ExpanderModuleOperation' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.ExpanderModuleOperation
- description: Read a 'equipment.Fan' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Fan
- description: Read a 'equipment.FanControl' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.FanControl
- description: Read a 'equipment.FanModule' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.FanModule
- description: Read a 'equipment.Fex' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Fex
- description: Read a 'equipment.FexIdentity' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.FexIdentity
- description: Read a 'equipment.FexOperation' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.FexOperation
- description: Read a 'equipment.Fru' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Fru
- description: Read a 'equipment.HybridDriveSlot' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.HybridDriveSlot
- description: Read a 'equipment.Interconnect' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Interconnect
- description: Read a 'equipment.IoCard' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.IoCard
- description: Read a 'equipment.IoCardOperation' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.IoCardOperation
- description: Read a 'equipment.IoExpander' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.IoExpander
- description: Read a 'equipment.LocatorLed' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.LocatorLed
- description: Read a 'equipment.LogDownload' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.LogDownload
- description: Read a 'equipment.Psu' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Psu
- description: Read a 'equipment.PsuControl' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.PsuControl
- description: Read a 'equipment.RackEnclosure' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.RackEnclosure
- description: Read a 'equipment.RackEnclosureSlot' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.RackEnclosureSlot
- description: Read a 'equipment.Riser' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Riser
- description: Read a 'equipment.Sensor' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Sensor
- description: Read a 'equipment.SharedAdapterUnit' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.SharedAdapterUnit
- description: Read a 'equipment.SharedGraphicsCard' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.SharedGraphicsCard
- description: Read a 'equipment.SharedIoModule' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.SharedIoModule
- description: Read a 'equipment.SwitchCard' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.SwitchCard
- description: Read a 'equipment.SwitchOperation' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.SwitchOperation
- description: Read a 'equipment.SystemIoController' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.SystemIoController
- description: Read a 'equipment.Tpm' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Tpm
- description: Read a 'equipment.Transceiver' resource.
  flows:
  - clientCredentials
  scope: READ.equipment.Transceiver
- description: Read a 'ether.HostPort' resource.
  flows:
  - clientCredentials
  scope: READ.ether.HostPort
- description: Read a 'ether.InterSwitchPort' resource.
  flows:
  - clientCredentials
  scope: READ.ether.InterSwitchPort
- description: Read a 'ether.LanPort' resource.
  flows:
  - clientCredentials
  scope: READ.ether.LanPort
- description: Read a 'ether.NetworkPort' resource.
  flows:
  - clientCredentials
  scope: READ.ether.NetworkPort
- description: Read a 'ether.PhysicalPort' resource.
  flows:
  - clientCredentials
  scope: READ.ether.PhysicalPort
- description: Read a 'ether.PortChannel' resource.
  flows:
  - clientCredentials
  scope: READ.ether.PortChannel
- description: Read a 'externalsite.Authorization' resource.
  flows:
  - clientCredentials
  scope: READ.externalsite.Authorization
- description: Read a 'fabric.AppliancePcRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.AppliancePcRole
- description: Read a 'fabric.ApplianceRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.ApplianceRole
- description: Read a 'fabric.ConfigChangeDetail' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.ConfigChangeDetail
- description: Read a 'fabric.ConfigResult' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.ConfigResult
- description: Read a 'fabric.ConfigResultEntry' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.ConfigResultEntry
- description: Read a 'fabric.ElementIdentity' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.ElementIdentity
- description: Read a 'fabric.EthNetworkControlPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.EthNetworkControlPolicy
- description: Read a 'fabric.EthNetworkControlPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.EthNetworkControlPolicyInventory
- description: Read a 'fabric.EthNetworkGroupPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.EthNetworkGroupPolicy
- description: Read a 'fabric.EthNetworkGroupPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.EthNetworkGroupPolicyInventory
- description: Read a 'fabric.EthNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.EthNetworkPolicy
- description: Read a 'fabric.FcNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.FcNetworkPolicy
- description: Read a 'fabric.FcStorageRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.FcStorageRole
- description: Read a 'fabric.FcUplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.FcUplinkPcRole
- description: Read a 'fabric.FcUplinkRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.FcUplinkRole
- description: Read a 'fabric.FcZonePolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.FcZonePolicy
- description: Read a 'fabric.FcoeUplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.FcoeUplinkPcRole
- description: Read a 'fabric.FcoeUplinkRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.FcoeUplinkRole
- description: Read a 'fabric.FlowControlPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.FlowControlPolicy
- description: Read a 'fabric.LanPinGroup' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.LanPinGroup
- description: Read a 'fabric.LinkAggregationPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.LinkAggregationPolicy
- description: Read a 'fabric.LinkControlPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.LinkControlPolicy
- description: Read a 'fabric.MacSecPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.MacSecPolicy
- description: Read a 'fabric.MulticastPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.MulticastPolicy
- description: Read a 'fabric.NetFlowExporter' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.NetFlowExporter
- description: Read a 'fabric.NetFlowMonitor' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.NetFlowMonitor
- description: Read a 'fabric.NetFlowPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.NetFlowPolicy
- description: Read a 'fabric.NetFlowRecord' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.NetFlowRecord
- description: Read a 'fabric.PcMember' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.PcMember
- description: Read a 'fabric.PcOperation' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.PcOperation
- description: Read a 'fabric.PortMode' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.PortMode
- description: Read a 'fabric.PortOperation' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.PortOperation
- description: Read a 'fabric.PortPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.PortPolicy
- description: Read a 'fabric.SanPinGroup' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SanPinGroup
- description: Read a 'fabric.SecureRouterRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SecureRouterRole
- description: Read a 'fabric.ServerRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.ServerRole
- description: Read a 'fabric.SpanDestEthPort' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SpanDestEthPort
- description: Read a 'fabric.SpanSession' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SpanSession
- description: Read a 'fabric.SpanSourceEthPort' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SpanSourceEthPort
- description: Read a 'fabric.SpanSourceEthPortChannel' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SpanSourceEthPortChannel
- description: Read a 'fabric.SpanSourceVlan' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SpanSourceVlan
- description: Read a 'fabric.SpanSourceVnicEthIf' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SpanSourceVnicEthIf
- description: Read a 'fabric.SwitchClusterProfile' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SwitchClusterProfile
- description: Read a 'fabric.SwitchClusterProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SwitchClusterProfileTemplate
- description: Read a 'fabric.SwitchControlPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SwitchControlPolicy
- description: Read a 'fabric.SwitchProfile' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SwitchProfile
- description: Read a 'fabric.SwitchProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SwitchProfileTemplate
- description: Read a 'fabric.SystemQosPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.SystemQosPolicy
- description: Read a 'fabric.UplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.UplinkPcRole
- description: Read a 'fabric.UplinkRole' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.UplinkRole
- description: Read a 'fabric.Vlan' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.Vlan
- description: Read a 'fabric.VlanInventory' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.VlanInventory
- description: Read a 'fabric.VlanSet' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.VlanSet
- description: Read a 'fabric.Vsan' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.Vsan
- description: Read a 'fabric.VsanInventory' resource.
  flows:
  - clientCredentials
  scope: READ.fabric.VsanInventory
- description: Read a 'fault.Instance' resource.
  flows:
  - clientCredentials
  scope: READ.fault.Instance
- description: Read a 'fc.Neighbor' resource.
  flows:
  - clientCredentials
  scope: READ.fc.Neighbor
- description: Read a 'fc.PhysicalPort' resource.
  flows:
  - clientCredentials
  scope: READ.fc.PhysicalPort
- description: Read a 'fc.PortChannel' resource.
  flows:
  - clientCredentials
  scope: READ.fc.PortChannel
- description: Read a 'fcpool.FcBlock' resource.
  flows:
  - clientCredentials
  scope: READ.fcpool.FcBlock
- description: Read a 'fcpool.Lease' resource.
  flows:
  - clientCredentials
  scope: READ.fcpool.Lease
- description: Read a 'fcpool.Pool' resource.
  flows:
  - clientCredentials
  scope: READ.fcpool.Pool
- description: Read a 'fcpool.PoolMember' resource.
  flows:
  - clientCredentials
  scope: READ.fcpool.PoolMember
- description: Read a 'fcpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: READ.fcpool.Reservation
- description: Read a 'fcpool.Universe' resource.
  flows:
  - clientCredentials
  scope: READ.fcpool.Universe
- description: Read a 'firmware.BiosDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.BiosDescriptor
- description: Read a 'firmware.BoardControllerDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.BoardControllerDescriptor
- description: Read a 'firmware.ChassisUpgrade' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.ChassisUpgrade
- description: Read a 'firmware.CimcDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.CimcDescriptor
- description: Read a 'firmware.DimmDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.DimmDescriptor
- description: Read a 'firmware.Distributable' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.Distributable
- description: Read a 'firmware.DistributableMeta' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.DistributableMeta
- description: Read a 'firmware.DriveDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.DriveDescriptor
- description: Read a 'firmware.DriverDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.DriverDistributable
- description: Read a 'firmware.Eula' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.Eula
- description: Read a 'firmware.FirmwareSummary' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.FirmwareSummary
- description: Read a 'firmware.GpuDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.GpuDescriptor
- description: Read a 'firmware.HbaDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.HbaDescriptor
- description: Read a 'firmware.IomDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.IomDescriptor
- description: Read a 'firmware.MswitchDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.MswitchDescriptor
- description: Read a 'firmware.NxosDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.NxosDescriptor
- description: Read a 'firmware.PciNodeUpgrade' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.PciNodeUpgrade
- description: Read a 'firmware.PcieDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.PcieDescriptor
- description: Read a 'firmware.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.Policy
- description: Read a 'firmware.PsuDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.PsuDescriptor
- description: Read a 'firmware.PsxDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.PsxDescriptor
- description: Read a 'firmware.RunningFirmware' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.RunningFirmware
- description: Read a 'firmware.SasExpanderDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.SasExpanderDescriptor
- description: Read a 'firmware.SecureRouterUpgrade' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.SecureRouterUpgrade
- description: Read a 'firmware.ServerConfigurationUtilityDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.ServerConfigurationUtilityDistributable
- description: Read a 'firmware.StorageControllerDescriptor' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.StorageControllerDescriptor
- description: Read a 'firmware.SwitchUpgrade' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.SwitchUpgrade
- description: Read a 'firmware.UnsupportedVersionUpgrade' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.UnsupportedVersionUpgrade
- description: Read a 'firmware.Upgrade' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.Upgrade
- description: Read a 'firmware.UpgradeImpactStatus' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.UpgradeImpactStatus
- description: Read a 'firmware.UpgradeStatus' resource.
  flows:
  - clientCredentials
  scope: READ.firmware.UpgradeStatus
- description: Read a 'fmc.Device' resource.
  flows:
  - clientCredentials
  scope: READ.fmc.Device
- description: Read a 'fmc.DeviceHaPair' resource.
  flows:
  - clientCredentials
  scope: READ.fmc.DeviceHaPair
- description: Read a 'fmc.Domain' resource.
  flows:
  - clientCredentials
  scope: READ.fmc.Domain
- description: Read a 'fmc.PhysicalInterface' resource.
  flows:
  - clientCredentials
  scope: READ.fmc.PhysicalInterface
- description: Read a 'forecast.Catalog' resource.
  flows:
  - clientCredentials
  scope: READ.forecast.Catalog
- description: Read a 'forecast.Definition' resource.
  flows:
  - clientCredentials
  scope: READ.forecast.Definition
- description: Read a 'forecast.Instance' resource.
  flows:
  - clientCredentials
  scope: READ.forecast.Instance
- description: Read a 'graphics.Card' resource.
  flows:
  - clientCredentials
  scope: READ.graphics.Card
- description: Read a 'graphics.Controller' resource.
  flows:
  - clientCredentials
  scope: READ.graphics.Controller
- description: Read a 'hci.AhvVm' resource.
  flows:
  - clientCredentials
  scope: READ.hci.AhvVm
- description: Read a 'hci.AhvVmDisk' resource.
  flows:
  - clientCredentials
  scope: READ.hci.AhvVmDisk
- description: Read a 'hci.AhvVmGpu' resource.
  flows:
  - clientCredentials
  scope: READ.hci.AhvVmGpu
- description: Read a 'hci.AhvVmNic' resource.
  flows:
  - clientCredentials
  scope: READ.hci.AhvVmNic
- description: Read a 'hci.Alarm' resource.
  flows:
  - clientCredentials
  scope: READ.hci.Alarm
- description: Read a 'hci.Cluster' resource.
  flows:
  - clientCredentials
  scope: READ.hci.Cluster
- description: Read a 'hci.ClusterOperation' resource.
  flows:
  - clientCredentials
  scope: READ.hci.ClusterOperation
- description: Read a 'hci.Compliance' resource.
  flows:
  - clientCredentials
  scope: READ.hci.Compliance
- description: Read a 'hci.Disk' resource.
  flows:
  - clientCredentials
  scope: READ.hci.Disk
- description: Read a 'hci.DomainManager' resource.
  flows:
  - clientCredentials
  scope: READ.hci.DomainManager
- description: Read a 'hci.Entitlement' resource.
  flows:
  - clientCredentials
  scope: READ.hci.Entitlement
- description: Read a 'hci.EsxiVm' resource.
  flows:
  - clientCredentials
  scope: READ.hci.EsxiVm
- description: Read a 'hci.EsxiVmDisk' resource.
  flows:
  - clientCredentials
  scope: READ.hci.EsxiVmDisk
- description: Read a 'hci.EsxiVmNic' resource.
  flows:
  - clientCredentials
  scope: READ.hci.EsxiVmNic
- description: Read a 'hci.ExternalStorage' resource.
  flows:
  - clientCredentials
  scope: READ.hci.ExternalStorage
- description: Read a 'hci.Gpu' resource.
  flows:
  - clientCredentials
  scope: READ.hci.Gpu
- description: Read a 'hci.License' resource.
  flows:
  - clientCredentials
  scope: READ.hci.License
- description: Read a 'hci.NccCheckPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hci.NccCheckPolicy
- description: Read a 'hci.Node' resource.
  flows:
  - clientCredentials
  scope: READ.hci.Node
- description: Read a 'hci.PhysicalGpu' resource.
  flows:
  - clientCredentials
  scope: READ.hci.PhysicalGpu
- description: Read a 'hci.StorageContainer' resource.
  flows:
  - clientCredentials
  scope: READ.hci.StorageContainer
- description: Read a 'hci.Violation' resource.
  flows:
  - clientCredentials
  scope: READ.hci.Violation
- description: Read a 'hci.VirtualGpu' resource.
  flows:
  - clientCredentials
  scope: READ.hci.VirtualGpu
- description: Read a 'hcl.DataImportLog' resource.
  flows:
  - clientCredentials
  scope: READ.hcl.DataImportLog
- description: Read a 'hcl.DriverImage' resource.
  flows:
  - clientCredentials
  scope: READ.hcl.DriverImage
- description: Read a 'hcl.ExemptedCatalog' resource.
  flows:
  - clientCredentials
  scope: READ.hcl.ExemptedCatalog
- description: Read a 'hcl.HwCatalogInfo' resource.
  flows:
  - clientCredentials
  scope: READ.hcl.HwCatalogInfo
- description: Read a 'hcl.HyperflexSoftwareCompatibilityInfo' resource.
  flows:
  - clientCredentials
  scope: READ.hcl.HyperflexSoftwareCompatibilityInfo
- description: Read a 'hcl.OperatingSystem' resource.
  flows:
  - clientCredentials
  scope: READ.hcl.OperatingSystem
- description: Read a 'hcl.OperatingSystemVendor' resource.
  flows:
  - clientCredentials
  scope: READ.hcl.OperatingSystemVendor
- description: Read a 'hcl.ServerCatalog' resource.
  flows:
  - clientCredentials
  scope: READ.hcl.ServerCatalog
- description: Read a 'hcl.ServerHwCatalogInfo' resource.
  flows:
  - clientCredentials
  scope: READ.hcl.ServerHwCatalogInfo
- description: Read a 'hyperflex.Alarm' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.Alarm
- description: Read a 'hyperflex.AppCatalog' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.AppCatalog
- description: Read a 'hyperflex.AutoSupportPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.AutoSupportPolicy
- description: Read a 'hyperflex.BackupCluster' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.BackupCluster
- description: Read a 'hyperflex.CapabilityInfo' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.CapabilityInfo
- description: Read a 'hyperflex.Cluster' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.Cluster
- description: Read a 'hyperflex.ClusterBackupPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ClusterBackupPolicy
- description: Read a 'hyperflex.ClusterBackupPolicyDeployment' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ClusterBackupPolicyDeployment
- description: Read a 'hyperflex.ClusterBackupPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ClusterBackupPolicyInventory
- description: Read a 'hyperflex.ClusterHealthCheckExecutionSnapshot' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ClusterHealthCheckExecutionSnapshot
- description: Read a 'hyperflex.ClusterNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ClusterNetworkPolicy
- description: Read a 'hyperflex.ClusterProfile' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ClusterProfile
- description: Read a 'hyperflex.ClusterReplicationNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ClusterReplicationNetworkPolicy
- description: Read a 'hyperflex.ClusterReplicationNetworkPolicyDeployment' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ClusterReplicationNetworkPolicyDeployment
- description: Read a 'hyperflex.ClusterStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ClusterStoragePolicy
- description: Read a 'hyperflex.ConfigResult' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ConfigResult
- description: Read a 'hyperflex.ConfigResultEntry' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ConfigResultEntry
- description: Read a 'hyperflex.DataProtectionPeer' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.DataProtectionPeer
- description: Read a 'hyperflex.DatastoreStatistic' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.DatastoreStatistic
- description: Read a 'hyperflex.DevicePackageDownloadState' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.DevicePackageDownloadState
- description: Read a 'hyperflex.Drive' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.Drive
- description: Read a 'hyperflex.Encryption' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.Encryption
- description: Read a 'hyperflex.ExtFcStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ExtFcStoragePolicy
- description: Read a 'hyperflex.ExtIscsiStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ExtIscsiStoragePolicy
- description: Read a 'hyperflex.FeatureLimitExternal' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.FeatureLimitExternal
- description: Read a 'hyperflex.FeatureLimitInternal' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.FeatureLimitInternal
- description: Read a 'hyperflex.Health' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.Health
- description: Read a 'hyperflex.HealthCheckDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.HealthCheckDefinition
- description: Read a 'hyperflex.HealthCheckExecution' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.HealthCheckExecution
- description: Read a 'hyperflex.HealthCheckExecutionSnapshot' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.HealthCheckExecutionSnapshot
- description: Read a 'hyperflex.HealthCheckPackageChecksum' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.HealthCheckPackageChecksum
- description: Read a 'hyperflex.HealthCheckSchedulePolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.HealthCheckSchedulePolicy
- description: Read a 'hyperflex.HwCatalog' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.HwCatalog
- description: Read a 'hyperflex.HxdpVersion' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.HxdpVersion
- description: Read a 'hyperflex.HypervisorHost' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.HypervisorHost
- description: Read a 'hyperflex.HypervisorVirtualMachine' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.HypervisorVirtualMachine
- description: Read a 'hyperflex.InitiatorGroup' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.InitiatorGroup
- description: Read a 'hyperflex.IscsiNetwork' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.IscsiNetwork
- description: Read a 'hyperflex.KeyEncryptionKey' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.KeyEncryptionKey
- description: Read a 'hyperflex.License' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.License
- description: Read a 'hyperflex.LocalCredentialPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.LocalCredentialPolicy
- description: Read a 'hyperflex.Lun' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.Lun
- description: Read a 'hyperflex.Node' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.Node
- description: Read a 'hyperflex.NodeConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.NodeConfigPolicy
- description: Read a 'hyperflex.NodeProfile' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.NodeProfile
- description: Read a 'hyperflex.ProtectedCluster' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ProtectedCluster
- description: Read a 'hyperflex.ProxySettingPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ProxySettingPolicy
- description: Read a 'hyperflex.ReduceReSync' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ReduceReSync
- description: Read a 'hyperflex.ServerFirmwareVersion' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ServerFirmwareVersion
- description: Read a 'hyperflex.ServerFirmwareVersionEntry' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ServerFirmwareVersionEntry
- description: Read a 'hyperflex.ServerModel' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ServerModel
- description: Read a 'hyperflex.ServiceAuthToken' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.ServiceAuthToken
- description: Read a 'hyperflex.SoftwareDistributionComponent' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.SoftwareDistributionComponent
- description: Read a 'hyperflex.SoftwareDistributionEntry' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.SoftwareDistributionEntry
- description: Read a 'hyperflex.SoftwareDistributionVersion' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.SoftwareDistributionVersion
- description: Read a 'hyperflex.SoftwareVersionPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.SoftwareVersionPolicy
- description: Read a 'hyperflex.StartReduceReSync' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.StartReduceReSync
- description: Read a 'hyperflex.StorageContainer' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.StorageContainer
- description: Read a 'hyperflex.SysConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.SysConfigPolicy
- description: Read a 'hyperflex.Target' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.Target
- description: Read a 'hyperflex.UcsmConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.UcsmConfigPolicy
- description: Read a 'hyperflex.VcenterConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.VcenterConfigPolicy
- description: Read a 'hyperflex.VmBackupInfo' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.VmBackupInfo
- description: Read a 'hyperflex.VmImportOperation' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.VmImportOperation
- description: Read a 'hyperflex.VmRestoreOperation' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.VmRestoreOperation
- description: Read a 'hyperflex.VmSnapshotInfo' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.VmSnapshotInfo
- description: Read a 'hyperflex.Volume' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.Volume
- description: Read a 'hyperflex.WitnessConfiguration' resource.
  flows:
  - clientCredentials
  scope: READ.hyperflex.WitnessConfiguration
- description: Read a 'iaas.ConnectorPack' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.ConnectorPack
- description: Read a 'iaas.CustomTaskInfo' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.CustomTaskInfo
- description: Read a 'iaas.DeviceStatus' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.DeviceStatus
- description: Read a 'iaas.DiagnosticMessages' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.DiagnosticMessages
- description: Read a 'iaas.LicenseInfo' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.LicenseInfo
- description: Read a 'iaas.MostRunTasks' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.MostRunTasks
- description: Read a 'iaas.ServiceRequest' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.ServiceRequest
- description: Read a 'iaas.SystemTaskInfo' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.SystemTaskInfo
- description: Read a 'iaas.UcsdInfo' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.UcsdInfo
- description: Read a 'iaas.UcsdManagedInfra' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.UcsdManagedInfra
- description: Read a 'iaas.UcsdMessages' resource.
  flows:
  - clientCredentials
  scope: READ.iaas.UcsdMessages
- description: Read a 'iam.Account' resource.
  flows:
  - clientCredentials
  scope: READ.iam.Account
- description: Read a 'iam.AccountExperience' resource.
  flows:
  - clientCredentials
  scope: READ.iam.AccountExperience
- description: Read a 'iam.ApiKey' resource.
  flows:
  - clientCredentials
  scope: READ.iam.ApiKey
- description: Read a 'iam.AppRegistration' resource.
  flows:
  - clientCredentials
  scope: READ.iam.AppRegistration
- description: Read a 'iam.BannerMessage' resource.
  flows:
  - clientCredentials
  scope: READ.iam.BannerMessage
- description: Read a 'iam.Certificate' resource.
  flows:
  - clientCredentials
  scope: READ.iam.Certificate
- description: Read a 'iam.CertificateRequest' resource.
  flows:
  - clientCredentials
  scope: READ.iam.CertificateRequest
- description: Read a 'iam.CuiIntegration' resource.
  flows:
  - clientCredentials
  scope: READ.iam.CuiIntegration
- description: Read a 'iam.DefaultAuthentication' resource.
  flows:
  - clientCredentials
  scope: READ.iam.DefaultAuthentication
- description: Read a 'iam.DomainGroup' resource.
  flows:
  - clientCredentials
  scope: READ.iam.DomainGroup
- description: Read a 'iam.DomainNameInfo' resource.
  flows:
  - clientCredentials
  scope: READ.iam.DomainNameInfo
- description: Read a 'iam.EndPointPrivilege' resource.
  flows:
  - clientCredentials
  scope: READ.iam.EndPointPrivilege
- description: Read a 'iam.EndPointRole' resource.
  flows:
  - clientCredentials
  scope: READ.iam.EndPointRole
- description: Read a 'iam.EndPointUser' resource.
  flows:
  - clientCredentials
  scope: READ.iam.EndPointUser
- description: Read a 'iam.EndPointUserInventory' resource.
  flows:
  - clientCredentials
  scope: READ.iam.EndPointUserInventory
- description: Read a 'iam.EndPointUserPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.iam.EndPointUserPolicy
- description: Read a 'iam.EndPointUserPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.iam.EndPointUserPolicyInventory
- description: Read a 'iam.EndPointUserRole' resource.
  flows:
  - clientCredentials
  scope: READ.iam.EndPointUserRole
- description: Read a 'iam.EndPointUserRoleInventory' resource.
  flows:
  - clientCredentials
  scope: READ.iam.EndPointUserRoleInventory
- description: Read a 'iam.GuestAccessSettings' resource.
  flows:
  - clientCredentials
  scope: READ.iam.GuestAccessSettings
- description: Read a 'iam.Idp' resource.
  flows:
  - clientCredentials
  scope: READ.iam.Idp
- description: Read a 'iam.IdpReference' resource.
  flows:
  - clientCredentials
  scope: READ.iam.IdpReference
- description: Read a 'iam.IpAccessManagement' resource.
  flows:
  - clientCredentials
  scope: READ.iam.IpAccessManagement
- description: Read a 'iam.IpAddress' resource.
  flows:
  - clientCredentials
  scope: READ.iam.IpAddress
- description: Read a 'iam.LdapConfigParams' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LdapConfigParams
- description: Read a 'iam.LdapGroup' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LdapGroup
- description: Read a 'iam.LdapGroupInventory' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LdapGroupInventory
- description: Read a 'iam.LdapMeta' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LdapMeta
- description: Read a 'iam.LdapPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LdapPolicy
- description: Read a 'iam.LdapPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LdapPolicyInventory
- description: Read a 'iam.LdapProvider' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LdapProvider
- description: Read a 'iam.LdapProviderInventory' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LdapProviderInventory
- description: Read a 'iam.LocalUserPassword' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LocalUserPassword
- description: Read a 'iam.LocalUserPasswordPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.iam.LocalUserPasswordPolicy
- description: Read a 'iam.OAuthToken' resource.
  flows:
  - clientCredentials
  scope: READ.iam.OAuthToken
- description: Read a 'iam.PasswordHistorySettingCollection' resource.
  flows:
  - clientCredentials
  scope: READ.iam.PasswordHistorySettingCollection
- description: Read a 'iam.Permission' resource.
  flows:
  - clientCredentials
  scope: READ.iam.Permission
- description: Read a 'iam.PrivateKeySpec' resource.
  flows:
  - clientCredentials
  scope: READ.iam.PrivateKeySpec
- description: Read a 'iam.Privilege' resource.
  flows:
  - clientCredentials
  scope: READ.iam.Privilege
- description: Read a 'iam.PrivilegeSet' resource.
  flows:
  - clientCredentials
  scope: READ.iam.PrivilegeSet
- description: Read a 'iam.PrivilegeSetMetaInfo' resource.
  flows:
  - clientCredentials
  scope: READ.iam.PrivilegeSetMetaInfo
- description: Read a 'iam.Qualifier' resource.
  flows:
  - clientCredentials
  scope: READ.iam.Qualifier
- description: Read a 'iam.ResourceLimits' resource.
  flows:
  - clientCredentials
  scope: READ.iam.ResourceLimits
- description: Read a 'iam.ResourcePermission' resource.
  flows:
  - clientCredentials
  scope: READ.iam.ResourcePermission
- description: Read a 'iam.ResourceRoles' resource.
  flows:
  - clientCredentials
  scope: READ.iam.ResourceRoles
- description: Read a 'iam.Role' resource.
  flows:
  - clientCredentials
  scope: READ.iam.Role
- description: Read a 'iam.SecurityHolder' resource.
  flows:
  - clientCredentials
  scope: READ.iam.SecurityHolder
- description: Read a 'iam.ServiceProvider' resource.
  flows:
  - clientCredentials
  scope: READ.iam.ServiceProvider
- description: Read a 'iam.Session' resource.
  flows:
  - clientCredentials
  scope: READ.iam.Session
- description: Read a 'iam.SessionLimits' resource.
  flows:
  - clientCredentials
  scope: READ.iam.SessionLimits
- description: Read a 'iam.SharingRule' resource.
  flows:
  - clientCredentials
  scope: READ.iam.SharingRule
- description: Read a 'iam.System' resource.
  flows:
  - clientCredentials
  scope: READ.iam.System
- description: Read a 'iam.TestIdpConfiguration' resource.
  flows:
  - clientCredentials
  scope: READ.iam.TestIdpConfiguration
- description: Read a 'iam.TrustPoint' resource.
  flows:
  - clientCredentials
  scope: READ.iam.TrustPoint
- description: Read a 'iam.User' resource.
  flows:
  - clientCredentials
  scope: READ.iam.User
- description: Read a 'iam.UserGroup' resource.
  flows:
  - clientCredentials
  scope: READ.iam.UserGroup
- description: Read a 'iam.UserPreference' resource.
  flows:
  - clientCredentials
  scope: READ.iam.UserPreference
- description: Read a 'iam.UserQualifier' resource.
  flows:
  - clientCredentials
  scope: READ.iam.UserQualifier
- description: Read a 'iam.UserSetting' resource.
  flows:
  - clientCredentials
  scope: READ.iam.UserSetting
- description: Read a 'inventory.DeviceInfo' resource.
  flows:
  - clientCredentials
  scope: READ.inventory.DeviceInfo
- description: Read a 'inventory.DnMoBinding' resource.
  flows:
  - clientCredentials
  scope: READ.inventory.DnMoBinding
- description: Read a 'inventory.GenericInventory' resource.
  flows:
  - clientCredentials
  scope: READ.inventory.GenericInventory
- description: Read a 'inventory.GenericInventoryHolder' resource.
  flows:
  - clientCredentials
  scope: READ.inventory.GenericInventoryHolder
- description: Read a 'ipmioverlan.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.ipmioverlan.Policy
- description: Read a 'ipmioverlan.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.ipmioverlan.PolicyInventory
- description: Read a 'ippool.BlockLease' resource.
  flows:
  - clientCredentials
  scope: READ.ippool.BlockLease
- description: Read a 'ippool.IpLease' resource.
  flows:
  - clientCredentials
  scope: READ.ippool.IpLease
- description: Read a 'ippool.Pool' resource.
  flows:
  - clientCredentials
  scope: READ.ippool.Pool
- description: Read a 'ippool.PoolMember' resource.
  flows:
  - clientCredentials
  scope: READ.ippool.PoolMember
- description: Read a 'ippool.Reservation' resource.
  flows:
  - clientCredentials
  scope: READ.ippool.Reservation
- description: Read a 'ippool.ShadowBlock' resource.
  flows:
  - clientCredentials
  scope: READ.ippool.ShadowBlock
- description: Read a 'ippool.ShadowPool' resource.
  flows:
  - clientCredentials
  scope: READ.ippool.ShadowPool
- description: Read a 'ippool.Universe' resource.
  flows:
  - clientCredentials
  scope: READ.ippool.Universe
- description: Read a 'iqnpool.Block' resource.
  flows:
  - clientCredentials
  scope: READ.iqnpool.Block
- description: Read a 'iqnpool.Lease' resource.
  flows:
  - clientCredentials
  scope: READ.iqnpool.Lease
- description: Read a 'iqnpool.Pool' resource.
  flows:
  - clientCredentials
  scope: READ.iqnpool.Pool
- description: Read a 'iqnpool.PoolMember' resource.
  flows:
  - clientCredentials
  scope: READ.iqnpool.PoolMember
- description: Read a 'iqnpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: READ.iqnpool.Reservation
- description: Read a 'iqnpool.Universe' resource.
  flows:
  - clientCredentials
  scope: READ.iqnpool.Universe
- description: Read a 'iwotenant.MaintenanceNotification' resource.
  flows:
  - clientCredentials
  scope: READ.iwotenant.MaintenanceNotification
- description: Read a 'iwotenant.Migrate' resource.
  flows:
  - clientCredentials
  scope: READ.iwotenant.Migrate
- description: Read a 'iwotenant.TenantCustomization' resource.
  flows:
  - clientCredentials
  scope: READ.iwotenant.TenantCustomization
- description: Read a 'iwotenant.TenantStatus' resource.
  flows:
  - clientCredentials
  scope: READ.iwotenant.TenantStatus
- description: Read a 'kvm.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.kvm.Policy
- description: Read a 'kvm.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.kvm.PolicyInventory
- description: Read a 'kvm.Session' resource.
  flows:
  - clientCredentials
  scope: READ.kvm.Session
- description: Read a 'kvm.Tunnel' resource.
  flows:
  - clientCredentials
  scope: READ.kvm.Tunnel
- description: Read a 'kvm.TunneledKvmPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.kvm.TunneledKvmPolicy
- description: Read a 'license.AccountLicenseData' resource.
  flows:
  - clientCredentials
  scope: READ.license.AccountLicenseData
- description: Read a 'license.CustomerOp' resource.
  flows:
  - clientCredentials
  scope: READ.license.CustomerOp
- description: Read a 'license.ErpCustomerOp' resource.
  flows:
  - clientCredentials
  scope: READ.license.ErpCustomerOp
- description: Read a 'license.ErpLicenseCount' resource.
  flows:
  - clientCredentials
  scope: READ.license.ErpLicenseCount
- description: Read a 'license.IksCustomerOp' resource.
  flows:
  - clientCredentials
  scope: READ.license.IksCustomerOp
- description: Read a 'license.IksLicenseCount' resource.
  flows:
  - clientCredentials
  scope: READ.license.IksLicenseCount
- description: Read a 'license.IncCustomerOp' resource.
  flows:
  - clientCredentials
  scope: READ.license.IncCustomerOp
- description: Read a 'license.IncLicenseCount' resource.
  flows:
  - clientCredentials
  scope: READ.license.IncLicenseCount
- description: Read a 'license.IwoCustomerOp' resource.
  flows:
  - clientCredentials
  scope: READ.license.IwoCustomerOp
- description: Read a 'license.IwoLicenseCount' resource.
  flows:
  - clientCredentials
  scope: READ.license.IwoLicenseCount
- description: Read a 'license.LicenseInfo' resource.
  flows:
  - clientCredentials
  scope: READ.license.LicenseInfo
- description: Read a 'license.LicenseInfoView' resource.
  flows:
  - clientCredentials
  scope: READ.license.LicenseInfoView
- description: Read a 'license.LicenseRegistrationStatus' resource.
  flows:
  - clientCredentials
  scope: READ.license.LicenseRegistrationStatus
- description: Read a 'license.LicenseReservationOp' resource.
  flows:
  - clientCredentials
  scope: READ.license.LicenseReservationOp
- description: Read a 'license.SmartlicenseToken' resource.
  flows:
  - clientCredentials
  scope: READ.license.SmartlicenseToken
- description: Read a 'ls.ServiceProfile' resource.
  flows:
  - clientCredentials
  scope: READ.ls.ServiceProfile
- description: Read a 'macpool.IdBlock' resource.
  flows:
  - clientCredentials
  scope: READ.macpool.IdBlock
- description: Read a 'macpool.Lease' resource.
  flows:
  - clientCredentials
  scope: READ.macpool.Lease
- description: Read a 'macpool.Pool' resource.
  flows:
  - clientCredentials
  scope: READ.macpool.Pool
- description: Read a 'macpool.PoolMember' resource.
  flows:
  - clientCredentials
  scope: READ.macpool.PoolMember
- description: Read a 'macpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: READ.macpool.Reservation
- description: Read a 'macpool.Universe' resource.
  flows:
  - clientCredentials
  scope: READ.macpool.Universe
- description: Read a 'management.Controller' resource.
  flows:
  - clientCredentials
  scope: READ.management.Controller
- description: Read a 'management.Entity' resource.
  flows:
  - clientCredentials
  scope: READ.management.Entity
- description: Read a 'management.Interface' resource.
  flows:
  - clientCredentials
  scope: READ.management.Interface
- description: Read a 'memory.Array' resource.
  flows:
  - clientCredentials
  scope: READ.memory.Array
- description: Read a 'memory.PersistentMemoryConfigResult' resource.
  flows:
  - clientCredentials
  scope: READ.memory.PersistentMemoryConfigResult
- description: Read a 'memory.PersistentMemoryConfiguration' resource.
  flows:
  - clientCredentials
  scope: READ.memory.PersistentMemoryConfiguration
- description: Read a 'memory.PersistentMemoryNamespace' resource.
  flows:
  - clientCredentials
  scope: READ.memory.PersistentMemoryNamespace
- description: Read a 'memory.PersistentMemoryNamespaceConfigResult' resource.
  flows:
  - clientCredentials
  scope: READ.memory.PersistentMemoryNamespaceConfigResult
- description: Read a 'memory.PersistentMemoryPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.memory.PersistentMemoryPolicy
- description: Read a 'memory.PersistentMemoryRegion' resource.
  flows:
  - clientCredentials
  scope: READ.memory.PersistentMemoryRegion
- description: Read a 'memory.PersistentMemoryUnit' resource.
  flows:
  - clientCredentials
  scope: READ.memory.PersistentMemoryUnit
- description: Read a 'memory.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.memory.Policy
- description: Read a 'memory.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.memory.PolicyInventory
- description: Read a 'memory.Unit' resource.
  flows:
  - clientCredentials
  scope: READ.memory.Unit
- description: Read a 'meraki.Device' resource.
  flows:
  - clientCredentials
  scope: READ.meraki.Device
- description: Read a 'meraki.Network' resource.
  flows:
  - clientCredentials
  scope: READ.meraki.Network
- description: Read a 'meraki.Organization' resource.
  flows:
  - clientCredentials
  scope: READ.meraki.Organization
- description: Read a 'meraki.PortProfile' resource.
  flows:
  - clientCredentials
  scope: READ.meraki.PortProfile
- description: Read a 'meraki.Tag' resource.
  flows:
  - clientCredentials
  scope: READ.meraki.Tag
- description: Read a 'meta.Definition' resource.
  flows:
  - clientCredentials
  scope: READ.meta.Definition
- description: Read a 'metrics.Configuration' resource.
  flows:
  - clientCredentials
  scope: READ.metrics.Configuration
- description: Read a 'metrics.MetricsExploration' resource.
  flows:
  - clientCredentials
  scope: READ.metrics.MetricsExploration
- description: Read a 'metrics.ResourceConfiguration' resource.
  flows:
  - clientCredentials
  scope: READ.metrics.ResourceConfiguration
- description: Read a 'mgmt.BackupCategory' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.BackupCategory
- description: Read a 'mgmt.ConfigBackupFile' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.ConfigBackupFile
- description: Read a 'mgmt.ConfigBackupInstance' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.ConfigBackupInstance
- description: Read a 'mgmt.ConfigBackupOperation' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.ConfigBackupOperation
- description: Read a 'mgmt.ConfigCategorySummary' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.ConfigCategorySummary
- description: Read a 'mgmt.ConfigOperationSetting' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.ConfigOperationSetting
- description: Read a 'mgmt.ConfigRestoreCategorySummary' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.ConfigRestoreCategorySummary
- description: Read a 'mgmt.ConfigRestoreOperation' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.ConfigRestoreOperation
- description: Read a 'mgmt.ObjectBackupMeta' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.ObjectBackupMeta
- description: Read a 'mgmt.OrgBackupOperation' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.OrgBackupOperation
- description: Read a 'mgmt.OrgRestoreOperation' resource.
  flows:
  - clientCredentials
  scope: READ.mgmt.OrgRestoreOperation
- description: Read a 'monitoring.HealthStatus' resource.
  flows:
  - clientCredentials
  scope: READ.monitoring.HealthStatus
- description: Read a 'network.DiscoveredNeighbor' resource.
  flows:
  - clientCredentials
  scope: READ.network.DiscoveredNeighbor
- description: Read a 'network.Dns' resource.
  flows:
  - clientCredentials
  scope: READ.network.Dns
- description: Read a 'network.Element' resource.
  flows:
  - clientCredentials
  scope: READ.network.Element
- description: Read a 'network.ElementSummary' resource.
  flows:
  - clientCredentials
  scope: READ.network.ElementSummary
- description: Read a 'network.FcZoneInfo' resource.
  flows:
  - clientCredentials
  scope: READ.network.FcZoneInfo
- description: Read a 'network.FeatureControl' resource.
  flows:
  - clientCredentials
  scope: READ.network.FeatureControl
- description: Read a 'network.InterfaceList' resource.
  flows:
  - clientCredentials
  scope: READ.network.InterfaceList
- description: Read a 'network.LicenseFile' resource.
  flows:
  - clientCredentials
  scope: READ.network.LicenseFile
- description: Read a 'network.SecureRouter' resource.
  flows:
  - clientCredentials
  scope: READ.network.SecureRouter
- description: Read a 'network.SecureRouterSetting' resource.
  flows:
  - clientCredentials
  scope: READ.network.SecureRouterSetting
- description: Read a 'network.SupervisorCard' resource.
  flows:
  - clientCredentials
  scope: READ.network.SupervisorCard
- description: Read a 'network.TelemetryCheck' resource.
  flows:
  - clientCredentials
  scope: READ.network.TelemetryCheck
- description: Read a 'network.Vethernet' resource.
  flows:
  - clientCredentials
  scope: READ.network.Vethernet
- description: Read a 'network.Vfc' resource.
  flows:
  - clientCredentials
  scope: READ.network.Vfc
- description: Read a 'network.VlanPortInfo' resource.
  flows:
  - clientCredentials
  scope: READ.network.VlanPortInfo
- description: Read a 'network.VpcDomain' resource.
  flows:
  - clientCredentials
  scope: READ.network.VpcDomain
- description: Read a 'network.VpcMember' resource.
  flows:
  - clientCredentials
  scope: READ.network.VpcMember
- description: Read a 'network.VpcPeer' resource.
  flows:
  - clientCredentials
  scope: READ.network.VpcPeer
- description: Read a 'network.Vrf' resource.
  flows:
  - clientCredentials
  scope: READ.network.Vrf
- description: Read a 'networkconfig.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.networkconfig.Policy
- description: Read a 'networkconfig.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.networkconfig.PolicyInventory
- description: Read a 'niaapi.ApicCcoPost' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.ApicCcoPost
- description: Read a 'niaapi.ApicFieldNotice' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.ApicFieldNotice
- description: Read a 'niaapi.ApicHweol' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.ApicHweol
- description: Read a 'niaapi.ApicLatestMaintainedRelease' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.ApicLatestMaintainedRelease
- description: Read a 'niaapi.ApicReleaseRecommend' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.ApicReleaseRecommend
- description: Read a 'niaapi.ApicSweol' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.ApicSweol
- description: Read a 'niaapi.DcnmCcoPost' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.DcnmCcoPost
- description: Read a 'niaapi.DcnmFieldNotice' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.DcnmFieldNotice
- description: Read a 'niaapi.DcnmHweol' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.DcnmHweol
- description: Read a 'niaapi.DcnmLatestMaintainedRelease' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.DcnmLatestMaintainedRelease
- description: Read a 'niaapi.DcnmReleaseRecommend' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.DcnmReleaseRecommend
- description: Read a 'niaapi.DcnmSweol' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.DcnmSweol
- description: Read a 'niaapi.FileDownloader' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.FileDownloader
- description: Read a 'niaapi.NdEncryptedFileDownload' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.NdEncryptedFileDownload
- description: Read a 'niaapi.NdMetadata' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.NdMetadata
- description: Read a 'niaapi.NdMetadataFileDownloader' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.NdMetadataFileDownloader
- description: Read a 'niaapi.NdMetadataSoftwareDownload' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.NdMetadataSoftwareDownload
- description: Read a 'niaapi.NiaMetadata' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.NiaMetadata
- description: Read a 'niaapi.NibFileDownloader' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.NibFileDownloader
- description: Read a 'niaapi.NibMetadata' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.NibMetadata
- description: Read a 'niaapi.PuvScriptDownloader' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.PuvScriptDownloader
- description: Read a 'niaapi.SnValidatorMetadata' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.SnValidatorMetadata
- description: Read a 'niaapi.UpgradeAssistFile' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.UpgradeAssistFile
- description: Read a 'niaapi.VersionRegex' resource.
  flows:
  - clientCredentials
  scope: READ.niaapi.VersionRegex
- description: Read a 'niatelemetry.AaaLdapProviderDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.AaaLdapProviderDetails
- description: Read a 'niatelemetry.AaaRadiusProviderDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.AaaRadiusProviderDetails
- description: Read a 'niatelemetry.AaaTacacsProviderDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.AaaTacacsProviderDetails
- description: Read a 'niatelemetry.Anomaly' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Anomaly
- description: Read a 'niatelemetry.ApicAppPluginDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicAppPluginDetails
- description: Read a 'niatelemetry.ApicCoreFileDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicCoreFileDetails
- description: Read a 'niatelemetry.ApicDbgexpRsExportDest' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicDbgexpRsExportDest
- description: Read a 'niatelemetry.ApicDbgexpRsTsScheduler' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicDbgexpRsTsScheduler
- description: Read a 'niatelemetry.ApicFanDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicFanDetails
- description: Read a 'niatelemetry.ApicFexDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicFexDetails
- description: Read a 'niatelemetry.ApicFlashDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicFlashDetails
- description: Read a 'niatelemetry.ApicNtpAuth' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicNtpAuth
- description: Read a 'niatelemetry.ApicPerformanceData' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicPerformanceData
- description: Read a 'niatelemetry.ApicPodData' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicPodData
- description: Read a 'niatelemetry.ApicPsuDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicPsuDetails
- description: Read a 'niatelemetry.ApicRealmDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicRealmDetails
- description: Read a 'niatelemetry.ApicSnmpClientGrpDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicSnmpClientGrpDetails
- description: Read a 'niatelemetry.ApicSnmpCommunityAccessDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicSnmpCommunityAccessDetails
- description: Read a 'niatelemetry.ApicSnmpCommunityDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicSnmpCommunityDetails
- description: Read a 'niatelemetry.ApicSnmpTrapDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicSnmpTrapDetails
- description: Read a 'niatelemetry.ApicSnmpTrapFwdServerDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicSnmpTrapFwdServerDetails
- description: Read a 'niatelemetry.ApicSnmpVersionThreeDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicSnmpVersionThreeDetails
- description: Read a 'niatelemetry.ApicSysLogGrp' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicSysLogGrp
- description: Read a 'niatelemetry.ApicSysLogSrc' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicSysLogSrc
- description: Read a 'niatelemetry.ApicTransceiverDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicTransceiverDetails
- description: Read a 'niatelemetry.ApicUiPageCounts' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicUiPageCounts
- description: Read a 'niatelemetry.ApicVision' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ApicVision
- description: Read a 'niatelemetry.AppDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.AppDetails
- description: Read a 'niatelemetry.CloudDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.CloudDetails
- description: Read a 'niatelemetry.Cluster' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Cluster
- description: Read a 'niatelemetry.ClusterNode' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.ClusterNode
- description: Read a 'niatelemetry.CommonPolicies' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.CommonPolicies
- description: Read a 'niatelemetry.Controller' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Controller
- description: Read a 'niatelemetry.DcnmFanDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.DcnmFanDetails
- description: Read a 'niatelemetry.DcnmFexDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.DcnmFexDetails
- description: Read a 'niatelemetry.DcnmModuleDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.DcnmModuleDetails
- description: Read a 'niatelemetry.DcnmPsuDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.DcnmPsuDetails
- description: Read a 'niatelemetry.DcnmTransceiverDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.DcnmTransceiverDetails
- description: Read a 'niatelemetry.DomInfoObject' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.DomInfoObject
- description: Read a 'niatelemetry.DomThresInfoObject' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.DomThresInfoObject
- description: Read a 'niatelemetry.Epg' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Epg
- description: Read a 'niatelemetry.Fabric' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Fabric
- description: Read a 'niatelemetry.FabricModuleDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.FabricModuleDetails
- description: Read a 'niatelemetry.FabricNodeControlDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.FabricNodeControlDetails
- description: Read a 'niatelemetry.FabricPodProfile' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.FabricPodProfile
- description: Read a 'niatelemetry.FabricPodSs' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.FabricPodSs
- description: Read a 'niatelemetry.Fault' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Fault
- description: Read a 'niatelemetry.HcloudDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.HcloudDetails
- description: Read a 'niatelemetry.HealthInsightsData' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.HealthInsightsData
- description: Read a 'niatelemetry.HttpsAclContractDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.HttpsAclContractDetails
- description: Read a 'niatelemetry.HttpsAclContractFilterMap' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.HttpsAclContractFilterMap
- description: Read a 'niatelemetry.HttpsAclEpgContractMap' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.HttpsAclEpgContractMap
- description: Read a 'niatelemetry.HttpsAclEpgDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.HttpsAclEpgDetails
- description: Read a 'niatelemetry.HttpsAclFilterDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.HttpsAclFilterDetails
- description: Read a 'niatelemetry.InsightGroupDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.InsightGroupDetails
- description: Read a 'niatelemetry.Lc' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Lc
- description: Read a 'niatelemetry.LeafPolGrpDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.LeafPolGrpDetails
- description: Read a 'niatelemetry.Link' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Link
- description: Read a 'niatelemetry.MdsNeighbors' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.MdsNeighbors
- description: Read a 'niatelemetry.MsoContractDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.MsoContractDetails
- description: Read a 'niatelemetry.MsoEpgDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.MsoEpgDetails
- description: Read a 'niatelemetry.MsoSchemaDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.MsoSchemaDetails
- description: Read a 'niatelemetry.MsoSiteDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.MsoSiteDetails
- description: Read a 'niatelemetry.MsoTenantDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.MsoTenantDetails
- description: Read a 'niatelemetry.Neighbor' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Neighbor
- description: Read a 'niatelemetry.Network' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Network
- description: Read a 'niatelemetry.NexusCloudAccount' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NexusCloudAccount
- description: Read a 'niatelemetry.NexusCloudSite' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NexusCloudSite
- description: Read a 'niatelemetry.NexusDashboardControllerDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NexusDashboardControllerDetails
- description: Read a 'niatelemetry.NexusDashboardDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NexusDashboardDetails
- description: Read a 'niatelemetry.NexusDashboardMemoryDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NexusDashboardMemoryDetails
- description: Read a 'niatelemetry.NexusDashboards' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NexusDashboards
- description: Read a 'niatelemetry.NiaFeatureUsage' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NiaFeatureUsage
- description: Read a 'niatelemetry.NiaInventory' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NiaInventory
- description: Read a 'niatelemetry.NiaInventoryDcnm' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NiaInventoryDcnm
- description: Read a 'niatelemetry.NiaInventoryFabric' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NiaInventoryFabric
- description: Read a 'niatelemetry.NiaLicenseState' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.NiaLicenseState
- description: Read a 'niatelemetry.Nicc' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Nicc
- description: Read a 'niatelemetry.PasswordStrengthCheck' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.PasswordStrengthCheck
- description: Read a 'niatelemetry.PodCommPolicies' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.PodCommPolicies
- description: Read a 'niatelemetry.PodSnmpPolicies' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.PodSnmpPolicies
- description: Read a 'niatelemetry.PodTimeServerPolicies' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.PodTimeServerPolicies
- description: Read a 'niatelemetry.Route' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Route
- description: Read a 'niatelemetry.SiteInventory' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SiteInventory
- description: Read a 'niatelemetry.SnmpSrc' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SnmpSrc
- description: Read a 'niatelemetry.SpinePolGrpDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SpinePolGrpDetails
- description: Read a 'niatelemetry.SshVersionTwo' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SshVersionTwo
- description: Read a 'niatelemetry.SupervisorModuleDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SupervisorModuleDetails
- description: Read a 'niatelemetry.Switch' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Switch
- description: Read a 'niatelemetry.SwitchInterface' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SwitchInterface
- description: Read a 'niatelemetry.SyslogRemoteDest' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SyslogRemoteDest
- description: Read a 'niatelemetry.SyslogSysMsg' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SyslogSysMsg
- description: Read a 'niatelemetry.SyslogSysMsgFacFilter' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SyslogSysMsgFacFilter
- description: Read a 'niatelemetry.SystemControllerDetails' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.SystemControllerDetails
- description: Read a 'niatelemetry.Tenant' resource.
  flows:
  - clientCredentials
  scope: READ.niatelemetry.Tenant
- description: Read a 'notification.AccountSubscription' resource.
  flows:
  - clientCredentials
  scope: READ.notification.AccountSubscription
- description: Read a 'ntp.NtpServer' resource.
  flows:
  - clientCredentials
  scope: READ.ntp.NtpServer
- description: Read a 'ntp.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.ntp.Policy
- description: Read a 'ntp.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.ntp.PolicyInventory
- description: Read a 'oauth.AccessToken' resource.
  flows:
  - clientCredentials
  scope: READ.oauth.AccessToken
- description: Read a 'oauth.Authorization' resource.
  flows:
  - clientCredentials
  scope: READ.oauth.Authorization
- description: Read a 'onprem.ApplianceSystemInfo' resource.
  flows:
  - clientCredentials
  scope: READ.onprem.ApplianceSystemInfo
- description: Read a 'onprem.AuditRecord' resource.
  flows:
  - clientCredentials
  scope: READ.onprem.AuditRecord
- description: Read a 'onprem.Upgrade' resource.
  flows:
  - clientCredentials
  scope: READ.onprem.Upgrade
- description: Read a 'onprem.UserPreference' resource.
  flows:
  - clientCredentials
  scope: READ.onprem.UserPreference
- description: Read a 'openapi.ApiMethodMeta' resource.
  flows:
  - clientCredentials
  scope: READ.openapi.ApiMethodMeta
- description: Read a 'openapi.OpenApiSpecification' resource.
  flows:
  - clientCredentials
  scope: READ.openapi.OpenApiSpecification
- description: Read a 'openapi.ProcessFile' resource.
  flows:
  - clientCredentials
  scope: READ.openapi.ProcessFile
- description: Read a 'openapi.TaskGenerationRequest' resource.
  flows:
  - clientCredentials
  scope: READ.openapi.TaskGenerationRequest
- description: Read a 'openapi.TaskGenerationResult' resource.
  flows:
  - clientCredentials
  scope: READ.openapi.TaskGenerationResult
- description: Read a 'oprs.Deployment' resource.
  flows:
  - clientCredentials
  scope: READ.oprs.Deployment
- description: Read a 'oprs.SyncTargetListMessage' resource.
  flows:
  - clientCredentials
  scope: READ.oprs.SyncTargetListMessage
- description: Read a 'organization.Organization' resource.
  flows:
  - clientCredentials
  scope: READ.organization.Organization
- description: Read a 'os.BulkInstallInfo' resource.
  flows:
  - clientCredentials
  scope: READ.os.BulkInstallInfo
- description: Read a 'os.Catalog' resource.
  flows:
  - clientCredentials
  scope: READ.os.Catalog
- description: Read a 'os.ConfigurationFile' resource.
  flows:
  - clientCredentials
  scope: READ.os.ConfigurationFile
- description: Read a 'os.Distribution' resource.
  flows:
  - clientCredentials
  scope: READ.os.Distribution
- description: Read a 'os.Install' resource.
  flows:
  - clientCredentials
  scope: READ.os.Install
- description: Read a 'os.SupportedVersion' resource.
  flows:
  - clientCredentials
  scope: READ.os.SupportedVersion
- description: Read a 'os.ValidRemoteTarget' resource.
  flows:
  - clientCredentials
  scope: READ.os.ValidRemoteTarget
- description: Read a 'partnerintegration.DcLogs' resource.
  flows:
  - clientCredentials
  scope: READ.partnerintegration.DcLogs
- description: Read a 'partnerintegration.DeviceConnector' resource.
  flows:
  - clientCredentials
  scope: READ.partnerintegration.DeviceConnector
- description: Read a 'partnerintegration.DocIssues' resource.
  flows:
  - clientCredentials
  scope: READ.partnerintegration.DocIssues
- description: Read a 'partnerintegration.Etl' resource.
  flows:
  - clientCredentials
  scope: READ.partnerintegration.Etl
- description: Read a 'partnerintegration.File' resource.
  flows:
  - clientCredentials
  scope: READ.partnerintegration.File
- description: Read a 'partnerintegration.Inventory' resource.
  flows:
  - clientCredentials
  scope: READ.partnerintegration.Inventory
- description: Read a 'partnerintegration.Logs' resource.
  flows:
  - clientCredentials
  scope: READ.partnerintegration.Logs
- description: Read a 'partnerintegration.Metrics' resource.
  flows:
  - clientCredentials
  scope: READ.partnerintegration.Metrics
- description: Read a 'partnerintegration.Model' resource.
  flows:
  - clientCredentials
  scope: READ.partnerintegration.Model
- description: Read a 'pci.CoprocessorCard' resource.
  flows:
  - clientCredentials
  scope: READ.pci.CoprocessorCard
- description: Read a 'pci.Device' resource.
  flows:
  - clientCredentials
  scope: READ.pci.Device
- description: Read a 'pci.Endpoint' resource.
  flows:
  - clientCredentials
  scope: READ.pci.Endpoint
- description: Read a 'pci.Link' resource.
  flows:
  - clientCredentials
  scope: READ.pci.Link
- description: Read a 'pci.Node' resource.
  flows:
  - clientCredentials
  scope: READ.pci.Node
- description: Read a 'pci.NodeSetting' resource.
  flows:
  - clientCredentials
  scope: READ.pci.NodeSetting
- description: Read a 'pci.Port' resource.
  flows:
  - clientCredentials
  scope: READ.pci.Port
- description: Read a 'pci.Slot' resource.
  flows:
  - clientCredentials
  scope: READ.pci.Slot
- description: Read a 'pci.Switch' resource.
  flows:
  - clientCredentials
  scope: READ.pci.Switch
- description: Read a 'pci.Zone' resource.
  flows:
  - clientCredentials
  scope: READ.pci.Zone
- description: Read a 'pool.IdMappingMember' resource.
  flows:
  - clientCredentials
  scope: READ.pool.IdMappingMember
- description: Read a 'pool.IdMappingPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.pool.IdMappingPolicy
- description: Read a 'port.Group' resource.
  flows:
  - clientCredentials
  scope: READ.port.Group
- description: Read a 'port.MacBinding' resource.
  flows:
  - clientCredentials
  scope: READ.port.MacBinding
- description: Read a 'port.SubGroup' resource.
  flows:
  - clientCredentials
  scope: READ.port.SubGroup
- description: Read a 'power.ControlState' resource.
  flows:
  - clientCredentials
  scope: READ.power.ControlState
- description: Read a 'power.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.power.Policy
- description: Read a 'power.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.power.PolicyInventory
- description: Read a 'power.PowerGroup' resource.
  flows:
  - clientCredentials
  scope: READ.power.PowerGroup
- description: Read a 'power.PowerGroupMember' resource.
  flows:
  - clientCredentials
  scope: READ.power.PowerGroupMember
- description: Read a 'processor.Unit' resource.
  flows:
  - clientCredentials
  scope: READ.processor.Unit
- description: Read a 'rack.UnitPersonality' resource.
  flows:
  - clientCredentials
  scope: READ.rack.UnitPersonality
- description: Read a 'recommendation.CapacityRunway' resource.
  flows:
  - clientCredentials
  scope: READ.recommendation.CapacityRunway
- description: Read a 'recommendation.ClusterExpansion' resource.
  flows:
  - clientCredentials
  scope: READ.recommendation.ClusterExpansion
- description: Read a 'recommendation.HardwareExpansionRequest' resource.
  flows:
  - clientCredentials
  scope: READ.recommendation.HardwareExpansionRequest
- description: Read a 'recommendation.HardwareExpansionRequestItem' resource.
  flows:
  - clientCredentials
  scope: READ.recommendation.HardwareExpansionRequestItem
- description: Read a 'recommendation.PhysicalItem' resource.
  flows:
  - clientCredentials
  scope: READ.recommendation.PhysicalItem
- description: Read a 'recommendation.PurchaseOrderEstimate' resource.
  flows:
  - clientCredentials
  scope: READ.recommendation.PurchaseOrderEstimate
- description: Read a 'recommendation.PurchaseOrderList' resource.
  flows:
  - clientCredentials
  scope: READ.recommendation.PurchaseOrderList
- description: Read a 'recommendation.SoftwareItem' resource.
  flows:
  - clientCredentials
  scope: READ.recommendation.SoftwareItem
- description: Read a 'recovery.BackupConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.recovery.BackupConfigPolicy
- description: Read a 'recovery.BackupProfile' resource.
  flows:
  - clientCredentials
  scope: READ.recovery.BackupProfile
- description: Read a 'recovery.ConfigResult' resource.
  flows:
  - clientCredentials
  scope: READ.recovery.ConfigResult
- description: Read a 'recovery.ConfigResultEntry' resource.
  flows:
  - clientCredentials
  scope: READ.recovery.ConfigResultEntry
- description: Read a 'recovery.OnDemandBackup' resource.
  flows:
  - clientCredentials
  scope: READ.recovery.OnDemandBackup
- description: Read a 'recovery.Restore' resource.
  flows:
  - clientCredentials
  scope: READ.recovery.Restore
- description: Read a 'recovery.ScheduleConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.recovery.ScheduleConfigPolicy
- description: Read a 'resource.Group' resource.
  flows:
  - clientCredentials
  scope: READ.resource.Group
- description: Read a 'resource.GroupMember' resource.
  flows:
  - clientCredentials
  scope: READ.resource.GroupMember
- description: Read a 'resource.LicenseResourceCount' resource.
  flows:
  - clientCredentials
  scope: READ.resource.LicenseResourceCount
- description: Read a 'resource.Membership' resource.
  flows:
  - clientCredentials
  scope: READ.resource.Membership
- description: Read a 'resource.MembershipHolder' resource.
  flows:
  - clientCredentials
  scope: READ.resource.MembershipHolder
- description: Read a 'resource.Reservation' resource.
  flows:
  - clientCredentials
  scope: READ.resource.Reservation
- description: Read a 'resource.SelectionCriteria' resource.
  flows:
  - clientCredentials
  scope: READ.resource.SelectionCriteria
- description: Read a 'resource.SharedResourcesInfoHolder' resource.
  flows:
  - clientCredentials
  scope: READ.resource.SharedResourcesInfoHolder
- description: Read a 'resourcepool.ChassisQualificationPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.resourcepool.ChassisQualificationPolicy
- description: Read a 'resourcepool.Lease' resource.
  flows:
  - clientCredentials
  scope: READ.resourcepool.Lease
- description: Read a 'resourcepool.LeaseResource' resource.
  flows:
  - clientCredentials
  scope: READ.resourcepool.LeaseResource
- description: Read a 'resourcepool.MembershipReservation' resource.
  flows:
  - clientCredentials
  scope: READ.resourcepool.MembershipReservation
- description: Read a 'resourcepool.Pool' resource.
  flows:
  - clientCredentials
  scope: READ.resourcepool.Pool
- description: Read a 'resourcepool.PoolMember' resource.
  flows:
  - clientCredentials
  scope: READ.resourcepool.PoolMember
- description: Read a 'resourcepool.QualificationPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.resourcepool.QualificationPolicy
- description: Read a 'resourcepool.Reservation' resource.
  flows:
  - clientCredentials
  scope: READ.resourcepool.Reservation
- description: Read a 'resourcepool.Universe' resource.
  flows:
  - clientCredentials
  scope: READ.resourcepool.Universe
- description: Read a 'scheduler.SchedulePolicy' resource.
  flows:
  - clientCredentials
  scope: READ.scheduler.SchedulePolicy
- description: Read a 'scheduler.TaskResult' resource.
  flows:
  - clientCredentials
  scope: READ.scheduler.TaskResult
- description: Read a 'scheduler.TaskSchedule' resource.
  flows:
  - clientCredentials
  scope: READ.scheduler.TaskSchedule
- description: Read a 'sdaaci.Connection' resource.
  flows:
  - clientCredentials
  scope: READ.sdaaci.Connection
- description: Read a 'sdaaci.ConnectionDetail' resource.
  flows:
  - clientCredentials
  scope: READ.sdaaci.ConnectionDetail
- description: Read a 'sdcard.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.sdcard.Policy
- description: Read a 'sdcard.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.sdcard.PolicyInventory
- description: Read a 'search.SearchItem' resource.
  flows:
  - clientCredentials
  scope: READ.search.SearchItem
- description: Read a 'search.TagItem' resource.
  flows:
  - clientCredentials
  scope: READ.search.TagItem
- description: Read a 'security.Unit' resource.
  flows:
  - clientCredentials
  scope: READ.security.Unit
- description: Read a 'server.ConfigChangeDetail' resource.
  flows:
  - clientCredentials
  scope: READ.server.ConfigChangeDetail
- description: Read a 'server.ConfigImport' resource.
  flows:
  - clientCredentials
  scope: READ.server.ConfigImport
- description: Read a 'server.ConfigResult' resource.
  flows:
  - clientCredentials
  scope: READ.server.ConfigResult
- description: Read a 'server.ConfigResultEntry' resource.
  flows:
  - clientCredentials
  scope: READ.server.ConfigResultEntry
- description: Read a 'server.DiagnosticStatus' resource.
  flows:
  - clientCredentials
  scope: READ.server.DiagnosticStatus
- description: Read a 'server.Diagnostics' resource.
  flows:
  - clientCredentials
  scope: READ.server.Diagnostics
- description: Read a 'server.Disruption' resource.
  flows:
  - clientCredentials
  scope: READ.server.Disruption
- description: Read a 'server.MigrationKeyDetails' resource.
  flows:
  - clientCredentials
  scope: READ.server.MigrationKeyDetails
- description: Read a 'server.Profile' resource.
  flows:
  - clientCredentials
  scope: READ.server.Profile
- description: Read a 'server.ProfilePendingChangeEval' resource.
  flows:
  - clientCredentials
  scope: READ.server.ProfilePendingChangeEval
- description: Read a 'server.ProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: READ.server.ProfileTemplate
- description: Read a 'servicenow.ChangeRequest' resource.
  flows:
  - clientCredentials
  scope: READ.servicenow.ChangeRequest
- description: Read a 'servicenow.ChangeRequestDoc' resource.
  flows:
  - clientCredentials
  scope: READ.servicenow.ChangeRequestDoc
- description: Read a 'servicenow.Incident' resource.
  flows:
  - clientCredentials
  scope: READ.servicenow.Incident
- description: Read a 'servicenow.IncidentDoc' resource.
  flows:
  - clientCredentials
  scope: READ.servicenow.IncidentDoc
- description: Read a 'smtp.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.smtp.Policy
- description: Read a 'smtp.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.smtp.PolicyInventory
- description: Read a 'smtp.PolicyTest' resource.
  flows:
  - clientCredentials
  scope: READ.smtp.PolicyTest
- description: Read a 'snmp.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.snmp.Policy
- description: Read a 'snmp.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.snmp.PolicyInventory
- description: Read a 'software.ApplianceDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.software.ApplianceDistributable
- description: Read a 'software.DownloadHistory' resource.
  flows:
  - clientCredentials
  scope: READ.software.DownloadHistory
- description: Read a 'software.HciBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.software.HciBundleDistributable
- description: Read a 'software.HciDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.software.HciDistributable
- description: Read a 'software.HclMeta' resource.
  flows:
  - clientCredentials
  scope: READ.software.HclMeta
- description: Read a 'software.HyperflexBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.software.HyperflexBundleDistributable
- description: Read a 'software.HyperflexDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.software.HyperflexDistributable
- description: Read a 'software.IksBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.software.IksBundleDistributable
- description: Read a 'software.ReleaseMeta' resource.
  flows:
  - clientCredentials
  scope: READ.software.ReleaseMeta
- description: Read a 'software.SolutionDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.software.SolutionDistributable
- description: Read a 'software.UcsdBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.software.UcsdBundleDistributable
- description: Read a 'software.UcsdDistributable' resource.
  flows:
  - clientCredentials
  scope: READ.software.UcsdDistributable
- description: Read a 'softwarerepository.Authorization' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.Authorization
- description: Read a 'softwarerepository.CachedImage' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.CachedImage
- description: Read a 'softwarerepository.Catalog' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.Catalog
- description: Read a 'softwarerepository.CategoryMapper' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.CategoryMapper
- description: Read a 'softwarerepository.CategoryMapperModel' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.CategoryMapperModel
- description: Read a 'softwarerepository.CategorySupportConstraint' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.CategorySupportConstraint
- description: Read a 'softwarerepository.CategoryUnsupportedModels' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.CategoryUnsupportedModels
- description: Read a 'softwarerepository.DownloadSpec' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.DownloadSpec
- description: Read a 'softwarerepository.OperatingSystemFile' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.OperatingSystemFile
- description: Read a 'softwarerepository.Release' resource.
  flows:
  - clientCredentials
  scope: READ.softwarerepository.Release
- description: Read a 'sol.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.sol.Policy
- description: Read a 'sol.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.sol.PolicyInventory
- description: Read a 'ssh.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.ssh.Policy
- description: Read a 'ssh.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.ssh.PolicyInventory
- description: Read a 'storage.BatteryBackupUnit' resource.
  flows:
  - clientCredentials
  scope: READ.storage.BatteryBackupUnit
- description: Read a 'storage.Controller' resource.
  flows:
  - clientCredentials
  scope: READ.storage.Controller
- description: Read a 'storage.ControllerDrive' resource.
  flows:
  - clientCredentials
  scope: READ.storage.ControllerDrive
- description: Read a 'storage.DiskGroup' resource.
  flows:
  - clientCredentials
  scope: READ.storage.DiskGroup
- description: Read a 'storage.DiskSlot' resource.
  flows:
  - clientCredentials
  scope: READ.storage.DiskSlot
- description: Read a 'storage.DriveGroup' resource.
  flows:
  - clientCredentials
  scope: READ.storage.DriveGroup
- description: Read a 'storage.DriveSecurityPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.storage.DriveSecurityPolicy
- description: Read a 'storage.Enclosure' resource.
  flows:
  - clientCredentials
  scope: READ.storage.Enclosure
- description: Read a 'storage.EnclosureDisk' resource.
  flows:
  - clientCredentials
  scope: READ.storage.EnclosureDisk
- description: Read a 'storage.EnclosureDiskSlotEp' resource.
  flows:
  - clientCredentials
  scope: READ.storage.EnclosureDiskSlotEp
- description: Read a 'storage.FileItem' resource.
  flows:
  - clientCredentials
  scope: READ.storage.FileItem
- description: Read a 'storage.FlexFlashController' resource.
  flows:
  - clientCredentials
  scope: READ.storage.FlexFlashController
- description: Read a 'storage.FlexFlashControllerProps' resource.
  flows:
  - clientCredentials
  scope: READ.storage.FlexFlashControllerProps
- description: Read a 'storage.FlexFlashPhysicalDrive' resource.
  flows:
  - clientCredentials
  scope: READ.storage.FlexFlashPhysicalDrive
- description: Read a 'storage.FlexFlashVirtualDrive' resource.
  flows:
  - clientCredentials
  scope: READ.storage.FlexFlashVirtualDrive
- description: Read a 'storage.FlexUtilController' resource.
  flows:
  - clientCredentials
  scope: READ.storage.FlexUtilController
- description: Read a 'storage.FlexUtilPhysicalDrive' resource.
  flows:
  - clientCredentials
  scope: READ.storage.FlexUtilPhysicalDrive
- description: Read a 'storage.FlexUtilVirtualDrive' resource.
  flows:
  - clientCredentials
  scope: READ.storage.FlexUtilVirtualDrive
- description: Read a 'storage.HitachiArray' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiArray
- description: Read a 'storage.HitachiController' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiController
- description: Read a 'storage.HitachiDisk' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiDisk
- description: Read a 'storage.HitachiExternalParityGroup' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiExternalParityGroup
- description: Read a 'storage.HitachiExternalPathGroup' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiExternalPathGroup
- description: Read a 'storage.HitachiExternalStorageLun' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiExternalStorageLun
- description: Read a 'storage.HitachiExternalStoragePort' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiExternalStoragePort
- description: Read a 'storage.HitachiHost' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiHost
- description: Read a 'storage.HitachiHostLun' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiHostLun
- description: Read a 'storage.HitachiNvmSubsystem' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiNvmSubsystem
- description: Read a 'storage.HitachiParityGroup' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiParityGroup
- description: Read a 'storage.HitachiPool' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiPool
- description: Read a 'storage.HitachiPort' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiPort
- description: Read a 'storage.HitachiRemoteCopyPairGad' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiRemoteCopyPairGad
- description: Read a 'storage.HitachiRemoteCopyPairTc' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiRemoteCopyPairTc
- description: Read a 'storage.HitachiRemoteCopyPairUr' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiRemoteCopyPairUr
- description: Read a 'storage.HitachiRemoteReplication' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiRemoteReplication
- description: Read a 'storage.HitachiSnapshot' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiSnapshot
- description: Read a 'storage.HitachiVolume' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiVolume
- description: Read a 'storage.HitachiVolumeMigrationPair' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HitachiVolumeMigrationPair
- description: Read a 'storage.HyperFlexStorageContainer' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HyperFlexStorageContainer
- description: Read a 'storage.HyperFlexVolume' resource.
  flows:
  - clientCredentials
  scope: READ.storage.HyperFlexVolume
- description: Read a 'storage.Item' resource.
  flows:
  - clientCredentials
  scope: READ.storage.Item
- description: Read a 'storage.KnoxSecureDriveConfiguration' resource.
  flows:
  - clientCredentials
  scope: READ.storage.KnoxSecureDriveConfiguration
- description: Read a 'storage.NetAppAggregate' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppAggregate
- description: Read a 'storage.NetAppAggregateEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppAggregateEvent
- description: Read a 'storage.NetAppBaseDisk' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppBaseDisk
- description: Read a 'storage.NetAppCifsService' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppCifsService
- description: Read a 'storage.NetAppCifsShare' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppCifsShare
- description: Read a 'storage.NetAppCloudTarget' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppCloudTarget
- description: Read a 'storage.NetAppCluster' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppCluster
- description: Read a 'storage.NetAppClusterEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppClusterEvent
- description: Read a 'storage.NetAppClusterSnapMirrorPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppClusterSnapMirrorPolicy
- description: Read a 'storage.NetAppClusterSnapshotPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppClusterSnapshotPolicy
- description: Read a 'storage.NetAppDataIpInterface' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppDataIpInterface
- description: Read a 'storage.NetAppDataIpInterfaceEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppDataIpInterfaceEvent
- description: Read a 'storage.NetAppDiskEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppDiskEvent
- description: Read a 'storage.NetAppEthernetPort' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppEthernetPort
- description: Read a 'storage.NetAppEthernetPortEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppEthernetPortEvent
- description: Read a 'storage.NetAppExportPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppExportPolicy
- description: Read a 'storage.NetAppFcInterface' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppFcInterface
- description: Read a 'storage.NetAppFcInterfaceEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppFcInterfaceEvent
- description: Read a 'storage.NetAppFcPort' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppFcPort
- description: Read a 'storage.NetAppFcPortEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppFcPortEvent
- description: Read a 'storage.NetAppInitiatorGroup' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppInitiatorGroup
- description: Read a 'storage.NetAppIpInterface' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppIpInterface
- description: Read a 'storage.NetAppIpInterfaceEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppIpInterfaceEvent
- description: Read a 'storage.NetAppIscsiService' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppIscsiService
- description: Read a 'storage.NetAppLicense' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppLicense
- description: Read a 'storage.NetAppLun' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppLun
- description: Read a 'storage.NetAppLunEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppLunEvent
- description: Read a 'storage.NetAppLunMap' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppLunMap
- description: Read a 'storage.NetAppNamespace' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppNamespace
- description: Read a 'storage.NetAppNfsClient' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppNfsClient
- description: Read a 'storage.NetAppNfsService' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppNfsService
- description: Read a 'storage.NetAppNode' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppNode
- description: Read a 'storage.NetAppNodeCdpNeighbor' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppNodeCdpNeighbor
- description: Read a 'storage.NetAppNodeEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppNodeEvent
- description: Read a 'storage.NetAppNonDataIpInterface' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppNonDataIpInterface
- description: Read a 'storage.NetAppNonDataIpInterfaceEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppNonDataIpInterfaceEvent
- description: Read a 'storage.NetAppNtpServer' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppNtpServer
- description: Read a 'storage.NetAppQtree' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppQtree
- description: Read a 'storage.NetAppSchedule' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppSchedule
- description: Read a 'storage.NetAppSensor' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppSensor
- description: Read a 'storage.NetAppSnapMirrorRelationship' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppSnapMirrorRelationship
- description: Read a 'storage.NetAppStorageVm' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppStorageVm
- description: Read a 'storage.NetAppSvmEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppSvmEvent
- description: Read a 'storage.NetAppSvmSnapMirrorPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppSvmSnapMirrorPolicy
- description: Read a 'storage.NetAppSvmSnapshotPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppSvmSnapshotPolicy
- description: Read a 'storage.NetAppVolume' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppVolume
- description: Read a 'storage.NetAppVolumeEvent' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppVolumeEvent
- description: Read a 'storage.NetAppVolumeSnapshot' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NetAppVolumeSnapshot
- description: Read a 'storage.NvmeRaidConfiguration' resource.
  flows:
  - clientCredentials
  scope: READ.storage.NvmeRaidConfiguration
- description: Read a 'storage.PhysicalDisk' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PhysicalDisk
- description: Read a 'storage.PhysicalDiskExtension' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PhysicalDiskExtension
- description: Read a 'storage.PhysicalDiskUsage' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PhysicalDiskUsage
- description: Read a 'storage.PureArray' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureArray
- description: Read a 'storage.PureArrayAlerts' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureArrayAlerts
- description: Read a 'storage.PureBlade' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureBlade
- description: Read a 'storage.PureController' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureController
- description: Read a 'storage.PureDirectory' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureDirectory
- description: Read a 'storage.PureDirectoryExport' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureDirectoryExport
- description: Read a 'storage.PureDirectoryPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureDirectoryPolicy
- description: Read a 'storage.PureDirectoryQuota' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureDirectoryQuota
- description: Read a 'storage.PureDirectorySnapshot' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureDirectorySnapshot
- description: Read a 'storage.PureDisk' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureDisk
- description: Read a 'storage.PureFileSystems' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureFileSystems
- description: Read a 'storage.PureFlashBladeFileSystem' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureFlashBladeFileSystem
- description: Read a 'storage.PureFlashBladeSystem' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureFlashBladeSystem
- description: Read a 'storage.PureHost' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureHost
- description: Read a 'storage.PureHostGroup' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureHostGroup
- description: Read a 'storage.PureHostLun' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureHostLun
- description: Read a 'storage.PureManagementAccessPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureManagementAccessPolicy
- description: Read a 'storage.PureNfsPolicyRule' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureNfsPolicyRule
- description: Read a 'storage.PureObjectBucket' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureObjectBucket
- description: Read a 'storage.PureObjectStoreAccount' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureObjectStoreAccount
- description: Read a 'storage.PureObjectStoreUser' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureObjectStoreUser
- description: Read a 'storage.PurePod' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PurePod
- description: Read a 'storage.PurePort' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PurePort
- description: Read a 'storage.PureProtectionGroup' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureProtectionGroup
- description: Read a 'storage.PureProtectionGroupSnapshot' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureProtectionGroupSnapshot
- description: Read a 'storage.PureQuotaPolicyRule' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureQuotaPolicyRule
- description: Read a 'storage.PureRealm' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureRealm
- description: Read a 'storage.PureReplicationSchedule' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureReplicationSchedule
- description: Read a 'storage.PureSmbPolicyRule' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureSmbPolicyRule
- description: Read a 'storage.PureSnapshotSchedule' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureSnapshotSchedule
- description: Read a 'storage.PureTargetArray' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureTargetArray
- description: Read a 'storage.PureVolume' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureVolume
- description: Read a 'storage.PureVolumeGroup' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureVolumeGroup
- description: Read a 'storage.PureVolumeSnapshot' resource.
  flows:
  - clientCredentials
  scope: READ.storage.PureVolumeSnapshot
- description: Read a 'storage.SasExpander' resource.
  flows:
  - clientCredentials
  scope: READ.storage.SasExpander
- description: Read a 'storage.SasPort' resource.
  flows:
  - clientCredentials
  scope: READ.storage.SasPort
- description: Read a 'storage.Span' resource.
  flows:
  - clientCredentials
  scope: READ.storage.Span
- description: Read a 'storage.StoragePolicy' resource.
  flows:
  - clientCredentials
  scope: READ.storage.StoragePolicy
- description: Read a 'storage.VdMemberEp' resource.
  flows:
  - clientCredentials
  scope: READ.storage.VdMemberEp
- description: Read a 'storage.VirtualDrive' resource.
  flows:
  - clientCredentials
  scope: READ.storage.VirtualDrive
- description: Read a 'storage.VirtualDriveContainer' resource.
  flows:
  - clientCredentials
  scope: READ.storage.VirtualDriveContainer
- description: Read a 'storage.VirtualDriveExtension' resource.
  flows:
  - clientCredentials
  scope: READ.storage.VirtualDriveExtension
- description: Read a 'storage.VirtualDriveIdentity' resource.
  flows:
  - clientCredentials
  scope: READ.storage.VirtualDriveIdentity
- description: Read a 'syslog.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.syslog.Policy
- description: Read a 'syslog.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.syslog.PolicyInventory
- description: Read a 'tam.AdvisoryCount' resource.
  flows:
  - clientCredentials
  scope: READ.tam.AdvisoryCount
- description: Read a 'tam.AdvisoryDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.tam.AdvisoryDefinition
- description: Read a 'tam.AdvisoryInfo' resource.
  flows:
  - clientCredentials
  scope: READ.tam.AdvisoryInfo
- description: Read a 'tam.AdvisoryInstance' resource.
  flows:
  - clientCredentials
  scope: READ.tam.AdvisoryInstance
- description: Read a 'tam.SecurityAdvisory' resource.
  flows:
  - clientCredentials
  scope: READ.tam.SecurityAdvisory
- description: Read a 'techsupportmanagement.CollectionControlPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.techsupportmanagement.CollectionControlPolicy
- description: Read a 'techsupportmanagement.Download' resource.
  flows:
  - clientCredentials
  scope: READ.techsupportmanagement.Download
- description: Read a 'techsupportmanagement.EndPoint' resource.
  flows:
  - clientCredentials
  scope: READ.techsupportmanagement.EndPoint
- description: Read a 'techsupportmanagement.TechSupportBundle' resource.
  flows:
  - clientCredentials
  scope: READ.techsupportmanagement.TechSupportBundle
- description: Read a 'techsupportmanagement.TechSupportStatus' resource.
  flows:
  - clientCredentials
  scope: READ.techsupportmanagement.TechSupportStatus
- description: Read a 'terminal.AuditLog' resource.
  flows:
  - clientCredentials
  scope: READ.terminal.AuditLog
- description: Read a 'thermal.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.thermal.Policy
- description: Read a 'thermal.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.thermal.PolicyInventory
- description: Read a 'top.System' resource.
  flows:
  - clientCredentials
  scope: READ.top.System
- description: Read a 'ucsd.BackupInfo' resource.
  flows:
  - clientCredentials
  scope: READ.ucsd.BackupInfo
- description: Read a 'uuidpool.Block' resource.
  flows:
  - clientCredentials
  scope: READ.uuidpool.Block
- description: Read a 'uuidpool.Pool' resource.
  flows:
  - clientCredentials
  scope: READ.uuidpool.Pool
- description: Read a 'uuidpool.PoolMember' resource.
  flows:
  - clientCredentials
  scope: READ.uuidpool.PoolMember
- description: Read a 'uuidpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: READ.uuidpool.Reservation
- description: Read a 'uuidpool.Universe' resource.
  flows:
  - clientCredentials
  scope: READ.uuidpool.Universe
- description: Read a 'uuidpool.UuidLease' resource.
  flows:
  - clientCredentials
  scope: READ.uuidpool.UuidLease
- description: Read a 'view.HealthStatus' resource.
  flows:
  - clientCredentials
  scope: READ.view.HealthStatus
- description: Read a 'view.Server' resource.
  flows:
  - clientCredentials
  scope: READ.view.Server
- description: Read a 'virtualization.EsxiConsole' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.EsxiConsole
- description: Read a 'virtualization.Host' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.Host
- description: Read a 'virtualization.VirtualMachine' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VirtualMachine
- description: Read a 'virtualization.VmwareCluster' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareCluster
- description: Read a 'virtualization.VmwareDatacenter' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareDatacenter
- description: Read a 'virtualization.VmwareDatastore' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareDatastore
- description: Read a 'virtualization.VmwareDatastoreCluster' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareDatastoreCluster
- description: Read a 'virtualization.VmwareDistributedNetwork' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareDistributedNetwork
- description: Read a 'virtualization.VmwareDistributedSwitch' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareDistributedSwitch
- description: Read a 'virtualization.VmwareFolder' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareFolder
- description: Read a 'virtualization.VmwareHost' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareHost
- description: Read a 'virtualization.VmwareHostGpu' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareHostGpu
- description: Read a 'virtualization.VmwareKernelNetwork' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareKernelNetwork
- description: Read a 'virtualization.VmwareNetwork' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareNetwork
- description: Read a 'virtualization.VmwarePhysicalNetworkInterface' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwarePhysicalNetworkInterface
- description: Read a 'virtualization.VmwareProactiveHa' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareProactiveHa
- description: Read a 'virtualization.VmwareUplinkPort' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareUplinkPort
- description: Read a 'virtualization.VmwareVcenter' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareVcenter
- description: Read a 'virtualization.VmwareVirtualDisk' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareVirtualDisk
- description: Read a 'virtualization.VmwareVirtualMachine' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareVirtualMachine
- description: Read a 'virtualization.VmwareVirtualMachineGpu' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareVirtualMachineGpu
- description: Read a 'virtualization.VmwareVirtualMachineSnapshot' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareVirtualMachineSnapshot
- description: Read a 'virtualization.VmwareVirtualNetworkInterface' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareVirtualNetworkInterface
- description: Read a 'virtualization.VmwareVirtualSwitch' resource.
  flows:
  - clientCredentials
  scope: READ.virtualization.VmwareVirtualSwitch
- description: Read a 'vmedia.Policy' resource.
  flows:
  - clientCredentials
  scope: READ.vmedia.Policy
- description: Read a 'vmedia.PolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vmedia.PolicyInventory
- description: Read a 'vmrc.Console' resource.
  flows:
  - clientCredentials
  scope: READ.vmrc.Console
- description: Read a 'vnic.EthAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthAdapterPolicy
- description: Read a 'vnic.EthAdapterPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthAdapterPolicyInventory
- description: Read a 'vnic.EthIf' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthIf
- description: Read a 'vnic.EthIfInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthIfInventory
- description: Read a 'vnic.EthNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthNetworkPolicy
- description: Read a 'vnic.EthNetworkPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthNetworkPolicyInventory
- description: Read a 'vnic.EthQosPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthQosPolicy
- description: Read a 'vnic.EthQosPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthQosPolicyInventory
- description: Read a 'vnic.EthVethInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthVethInventory
- description: Read a 'vnic.EthVnicInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.EthVnicInventory
- description: Read a 'vnic.FcAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcAdapterPolicy
- description: Read a 'vnic.FcAdapterPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcAdapterPolicyInventory
- description: Read a 'vnic.FcIf' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcIf
- description: Read a 'vnic.FcIfInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcIfInventory
- description: Read a 'vnic.FcNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcNetworkPolicy
- description: Read a 'vnic.FcNetworkPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcNetworkPolicyInventory
- description: Read a 'vnic.FcQosPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcQosPolicy
- description: Read a 'vnic.FcQosPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcQosPolicyInventory
- description: Read a 'vnic.FcVethInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcVethInventory
- description: Read a 'vnic.FcVhbaPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.FcVhbaPolicyInventory
- description: Read a 'vnic.IscsiAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.IscsiAdapterPolicy
- description: Read a 'vnic.IscsiAdapterPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.IscsiAdapterPolicyInventory
- description: Read a 'vnic.IscsiBootPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.IscsiBootPolicy
- description: Read a 'vnic.IscsiBootPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.IscsiBootPolicyInventory
- description: Read a 'vnic.IscsiStaticTargetPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.IscsiStaticTargetPolicy
- description: Read a 'vnic.IscsiStaticTargetPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.IscsiStaticTargetPolicyInventory
- description: Read a 'vnic.LanConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.LanConnectivityPolicy
- description: Read a 'vnic.LanConnectivityPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.LanConnectivityPolicyInventory
- description: Read a 'vnic.LanSettings' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.LanSettings
- description: Read a 'vnic.LcpStatus' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.LcpStatus
- description: Read a 'vnic.SanConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.SanConnectivityPolicy
- description: Read a 'vnic.SanConnectivityPolicyInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.SanConnectivityPolicyInventory
- description: Read a 'vnic.SanSettings' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.SanSettings
- description: Read a 'vnic.ScpStatus' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.ScpStatus
- description: Read a 'vnic.ServiceEthIf' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.ServiceEthIf
- description: Read a 'vnic.ServiceEthIfInventory' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.ServiceEthIfInventory
- description: Read a 'vnic.VhbaTemplate' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.VhbaTemplate
- description: Read a 'vnic.VifIdPool' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.VifIdPool
- description: Read a 'vnic.VnicTemplate' resource.
  flows:
  - clientCredentials
  scope: READ.vnic.VnicTemplate
- description: Read a 'vrf.Vrf' resource.
  flows:
  - clientCredentials
  scope: READ.vrf.Vrf
- description: Read a 'webhook.Endpoint' resource.
  flows:
  - clientCredentials
  scope: READ.webhook.Endpoint
- description: Read a 'webhook.Schema' resource.
  flows:
  - clientCredentials
  scope: READ.webhook.Schema
- description: Read a 'workflow.AnsibleBatchExecutor' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.AnsibleBatchExecutor
- description: Read a 'workflow.BatchApiExecutor' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.BatchApiExecutor
- description: Read a 'workflow.Catalog' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.Catalog
- description: Read a 'workflow.CatalogItemDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.CatalogItemDefinition
- description: Read a 'workflow.CatalogServiceRequest' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.CatalogServiceRequest
- description: Read a 'workflow.CustomDataTypeDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.CustomDataTypeDefinition
- description: Read a 'workflow.ErrorResponseHandler' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.ErrorResponseHandler
- description: Read a 'workflow.PowerShellBatchApiExecutor' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.PowerShellBatchApiExecutor
- description: Read a 'workflow.RollbackWorkflow' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.RollbackWorkflow
- description: Read a 'workflow.ServiceItemActionDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.ServiceItemActionDefinition
- description: Read a 'workflow.ServiceItemActionInstance' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.ServiceItemActionInstance
- description: Read a 'workflow.ServiceItemAttribute' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.ServiceItemAttribute
- description: Read a 'workflow.ServiceItemDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.ServiceItemDefinition
- description: Read a 'workflow.ServiceItemHealthCheckDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.ServiceItemHealthCheckDefinition
- description: Read a 'workflow.ServiceItemHealthCheckExecution' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.ServiceItemHealthCheckExecution
- description: Read a 'workflow.ServiceItemInstance' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.ServiceItemInstance
- description: Read a 'workflow.ServiceItemOutput' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.ServiceItemOutput
- description: Read a 'workflow.SshBatchExecutor' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.SshBatchExecutor
- description: Read a 'workflow.TaskDebugLog' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.TaskDebugLog
- description: Read a 'workflow.TaskDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.TaskDefinition
- description: Read a 'workflow.TaskInfo' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.TaskInfo
- description: Read a 'workflow.TaskMetadata' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.TaskMetadata
- description: Read a 'workflow.TemplateFunctionMeta' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.TemplateFunctionMeta
- description: Read a 'workflow.UiDisplayMetadata' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.UiDisplayMetadata
- description: Read a 'workflow.Variable' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.Variable
- description: Read a 'workflow.WorkflowDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.WorkflowDefinition
- description: Read a 'workflow.WorkflowInfo' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.WorkflowInfo
- description: Read a 'workflow.WorkflowMetadata' resource.
  flows:
  - clientCredentials
  scope: READ.workflow.WorkflowMetadata
- description: Read a 'workload.Blueprint' resource.
  flows:
  - clientCredentials
  scope: READ.workload.Blueprint
- description: Read a 'workload.ClearWorkloadTag' resource.
  flows:
  - clientCredentials
  scope: READ.workload.ClearWorkloadTag
- description: Read a 'workload.DeploymentInput' resource.
  flows:
  - clientCredentials
  scope: READ.workload.DeploymentInput
- description: Read a 'workload.WorkloadDefinition' resource.
  flows:
  - clientCredentials
  scope: READ.workload.WorkloadDefinition
- description: Read a 'workload.WorkloadDeployment' resource.
  flows:
  - clientCredentials
  scope: READ.workload.WorkloadDeployment
- description: Read a 'workload.WorkloadInstance' resource.
  flows:
  - clientCredentials
  scope: READ.workload.WorkloadInstance
- description: Read a 'workload.WorkloadMetadata' resource.
  flows:
  - clientCredentials
  scope: READ.workload.WorkloadMetadata
- description: As an Account administrator, you have complete access to all services and resources in Intersight. You can perform all administrative and management tasks, including claim and manage devices, create and deploy Server and HyperFlex Cluster profiles, upgrade firmware, perform server actions, cross launch devices, add and manage users and groups, configure Identity providers and more.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Account Administrator
- description: As an Audit Log Viewer, you can view audit logs.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Audit Log Viewer
- description: As an Automation Governor, you can approve or reject requests to publish generic objects, including Workflows, Tasks, CDTs, FaaS, and Service Items. Each request is created for a generic asset, enabling automation governance to publish these assets.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Automation Governance
- description: As a Catalog Administrator, you can create workflows, custom data types, resource selection policies, service items, catalog items, execute catalog item, and view and perform post-deployment operations on the service item instance. Also, you can view and publish the catalog items.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Catalog Administrator
- description: As a Catalog User, you can view the catalog items that are assigned to you. You can deploy the catalog item, track the catalog item execution, view the service item instance that is created or assigned to you, and perform post-deployment operations on the service item instances.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Catalog User
- description: As a Complete Claim user you can complete the claim of a previously created Target by providing the security token of the device. You do not have access to read the status or details of any devices within the account.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Complete Claim
- description: As a Device Administrator, you can claim and unclaim a device in Intersight, view the device details, license status, a list of all the claimed devices, and generate API keys. You cannot perform any other management or administrative task in this role.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Device Administrator
- description: As a Device Technician you can claim a device, view the device details, license status, a list of the claimed devices, and generate API keys. You cannot perform any other management or administrative task in this role.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Device Technician
- description: As an External Syslog Administrator, you can configure an external syslog server on an on-prem appliance.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.External Syslog Administrator
- description: As an HCI Cluster Administrator, you can view and manage HCI Clusters, view all the cluster dashboard widgets, view cluster details. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HCI Cluster Administrator
- description: As an HCI Cluster Operator, you can view and manage HCI Clusters, view all the cluster dashboard widgets, view cluster details. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HCI Cluster Operator
- description: As a HyperFlex Cluster Access Operator, you can cross launch CLI and HXConnect.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HyperFlex Cluster Access Operator
- description: As a HyperFlex Cluster Administrator, you can create, edit, deploy, and manage HyperFlex Clusters, view all the cluster dashboard widgets, view cluster details, create HyperFlex policies and profiles, execute capacity planning, and launch HyperFlex Connect. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HyperFlex Cluster Administrator
- description: As a HyperFlex Cluster Data Protection Administrator, you can perform N:1 backups.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HyperFlex Cluster Data Protection Administrator
- description: As a HyperFlex Cluster Lifecycle Administrator, you can install, expand, upgrade a HX cluster, execute capacity planning, OS installation, VC plugin installation, security hardening, and launch HyperFlex Connect as admin.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HyperFlex Cluster Lifecycle Administrator
- description: As a HyperFlex Cluster Operator, you can perform health checks and launch HyperFlex Connect. However, you cannot change cluster configuration.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HyperFlex Cluster Operator
- description: As a HyperFlex Cluster Storage Administrator, you can perform datastore, iSCSI, and storage container CRUD operations.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HyperFlex Cluster Storage Administrator
- description: As a HyperFlex Cluster Syslog Administrator, you can configure the external HX Syslog profile.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HyperFlex Cluster Syslog Administrator
- description: As a HyperFlex Cluster System Administrator, you can perform most system administrator tasks, create backups, view syslogs, and configure encryption.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HyperFlex Cluster System Administrator
- description: As a HyperFlex Cluster System Operator, you can perform encryption, health checks, and post-install tasks.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.HyperFlex Cluster System Operator
- description: As an Integrated Systems Administrator, you can perform all actions related to Integrated Systems (e.g., FlexPod) like create/edit/delete of an Integrated System. In addition you can perform administrative and management tasks related to devices (including claim), servers, server profiles, UCS domain, switch profiles, hypervisors, network/SAN switches, storage devices. Also, you can define workflow and task definitions and can execute them and view workflow executions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Integrated Systems Administrator
- description: As an Integrated Systems Operator, you can view Integrated Systems (e.g., FlexPod) and can run inventory based actions (e.g., Interoperability check) In addition you can view devices, servers, server profiles, UCS domain, switch profiles, hypervisors, network/SAN switches, storage devices and workflows. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Integrated Systems Operator
- description: As a Kubernetes Administrator, you can create, edit, deploy, and manage Kubernetes Clusters. Also, you can view all the cluster dashboard widgets, and view cluster details. In addition, you also have privileges to view and manage storage targets associated with the Kubernetes clusters. The capability to view and execute workflows against the Kubernetes clusters is also granted. It also allows the user to run workflows to manage VMs on hypervisor endpoints, and manage connected storage. The ability to create and view IP pools is also allowed. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Kubernetes Administrator
- description: As a Kubernetes Operator, you can view Kubernetes Clusters. Also, you can view all the cluster dashboard widgets, and view cluster details. In addition, you also have privileges to view storage targets associated with the Kubernetes clusters. The capability to view workflows is also granted. It also allows the user to view VMs on hypervisor endpoints. This role also provides the capability to view IP pools. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Kubernetes Operator
- description: As a user with location management privileges, you can manage location, including creating, updating, and deleting.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Location Management
- description: As a Network Administrator, you can create, update, delete and view the Managed network device objects. The capability to view and execute workflows against the network device is also granted. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Network Administrator
- description: As a Network Operator, you can view the Managed network device objects. The capability to view workflows against the network device is also granted. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Network Operator
- description: As a Nexus Administrator, you have the privileges to perform all Nexus related operations. This includes claiming devices, updating policy configuration, and monitoring the system.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Nexus Administrator
- description: As a Nexus Analyst, you can run and update the available Nexus Cloud analyses such as Sustainability, Conformance, Compliance, and others.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Nexus Analyst
- description: As a Nexus Config Administrator, you can create or modify policy configuration and can initiate the workflow that will activate policy changes. This role does not allow you to claim or remove devices.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Nexus Config Administrator
- description: As a Nexus Observer, you can generally view the state of all devices. Additional items include things like viewing configured policies and monitoring active flows. This role does not include any permission which allows the system to be changed.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Nexus Observer
- description: As a Read-Only user, you can view the dashboard, table views of the managed devices, change your user preferences, and generate API keys. You cannot claim a device, add or remove a user, configure Identity providers or perform any server actions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Read-Only
- description: As a SAN Administrator, you can create, update, delete and view the Managed SAN switch objects. The capability to view and execute workflows against the SAN switches is also granted. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.SAN Administrator
- description: As a SAN Operator, you can view the Managed SAN switch objects. The capability to view workflows against the SAN switches is also granted. This role does not include the ability to claim a target. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a target.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.SAN Operator
- description: As a Server Administrator, you can view and manage UCS Servers and Fabric Interconnects, view all the server and Fabric Interconnect dashboard widgets, perform server actions, view server details, launch management interfaces and the CLI, create and deploy server policies and profiles, and manage API keys. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Server Administrator
- description: As a Service Designer, you can create custom data types, tasks, workflows, resource selection criteria, and use these to design the service items. The service designer can validate the service items by using the deployment and post-deployment actions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Service Designer
- description: As a Service Operator, you can view and update the catalog items, service items, and workflows. Also, you can execute the workflow and validate the catalog or service items.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Service Operator
- description: As a Storage Administrator, a user can view and manage Storage devices, view and execute workflows and view all the storage dashboard widgets. This privilege does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Storage Administrator
- description: As a Support Services user, you can view the dashboard and table views of managed devices, change your user preferences, collect tech support bundles, and generate API keys. In this role, you cannot claim targets, add or remove users, configure Identity Providers, or perform server actions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Support Services
- description: As a Sustainability Metrics Viewer user, you have read access to the Energy Management Capability (EMC) features and the ability register an OAuth2 application for programmatic access to the APIs.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Sustainability Metrics Viewer
- description: As a user with tag management privileges, you can manage tag definitions, including creating, updating, and deleting tags.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Tag Management
- description: As a UCS Domain Administrator, you can view and manage Switch Profiles and Network Configuration Policies, view Fabric Interconnect dashboard widgets, perform actions on Switch, launch management interfaces and the CLI, create and deploy switch policies and profiles, and manage API keys. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.UCS Domain Administrator
- description: As a Unified Edge Administrator, you can view and manage Switch Profiles, Network and Chassis Configuration Policies, view Unified Edge dashboard widgets, perform actions on Switch and Chassis, launch management interfaces and the CLI, and manage API keys. This role does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Unified Edge Administrator
- description: As a User Access Administrator, you can add and manage Users and Groups in Intersight, view account details and audit logs, manage the IdPs, roles, sessions and API keys for non Account Administrator users. However, you cannot claim a device or perform any management tasks in Intersight. You cannot add or manage a user with Account Administrator role.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.User Access Administrator
- description: As a Virtualization Administrator, a user can view and manage hypervisor resources, view and execute workflows. This privilege does not include the ability to claim a device. You must have a Device Technician, Device Administrator, or an Account Administrator role to claim a device.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Virtualization Administrator
- description: As a Workflow Designer, you can define workflow definitions and custom data types, view workflow definitions, task definitions and custom data types, execute workflows and view workflow executions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Workflow Designer
- description: As a Workload Administrator you can view and manage Workload Definitions and Workload Deployments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Workload Administrator
- description: As a Workload Operator you can view and manage Workload Deployments and view Workload Definitions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Workload Operator
- description: As a Workload Optimizer Administrator, you can access all Workload Optimizer features and perform administrative tasks to configure Workload Optimizer.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Workload Optimizer Administrator
- description: As a Workload Optimizer Advisor, you can view workload optimization state and recommended actions, run plans for workload optimization.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Workload Optimizer Advisor
- description: As a Workload Optimizer Automator, you can view workload optimization state, recommended actions, run plans for workload optimization, execute workload optimization actions, and deploy workloads.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Workload Optimizer Automator
- description: As a Workload Optimizer Deployer, you can view all Workload Optimizer charts and data, deploy workloads, and create policies and templates. You cannot run plans or execute any recommended actions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Workload Optimizer Deployer
- description: As a Workload Optimizer Observer, you can view workload optimization state and recommended actions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.Workload Optimizer Observer
- description: As a vKVM-only user, you can launch vKVM and tunneled vKVM sessions to a server from Intersight. In addition you can view servers, chassis and the running workflows. In this role, you cannot perform any server actions from Intersight apart from launching vKVM.
  flows:
  - authorizationCode
  - clientCredentials
  scope: ROLE.vKVM Only
- description: Update a 'aaa.RetentionPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.aaa.RetentionPolicy
- description: Update a 'access.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.access.Policy
- description: Update a 'adapter.ConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.adapter.ConfigPolicy
- description: Update a 'adapter.HostEthInterface' resource.
  flows:
  - clientCredentials
  scope: UPDATE.adapter.HostEthInterface
- description: Update a 'adapter.HostFcInterface' resource.
  flows:
  - clientCredentials
  scope: UPDATE.adapter.HostFcInterface
- description: Update a 'appliance.BackupPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.BackupPolicy
- description: Update a 'appliance.CertificateSetting' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.CertificateSetting
- description: Update a 'appliance.ClusterInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.ClusterInfo
- description: Update a 'appliance.ClusterInstall' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.ClusterInstall
- description: Update a 'appliance.ClusterReplaceNode' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.ClusterReplaceNode
- description: Update a 'appliance.ClusterWorkerNode' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.ClusterWorkerNode
- description: Update a 'appliance.DataExportPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.DataExportPolicy
- description: Update a 'appliance.DeviceClaim' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.DeviceClaim
- description: Update a 'appliance.DeviceUpgradePolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.DeviceUpgradePolicy
- description: Update a 'appliance.DiagSetting' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.DiagSetting
- description: Update a 'appliance.ExternalSyslogSetting' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.ExternalSyslogSetting
- description: Update a 'appliance.FqdnUpdate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.FqdnUpdate
- description: Update a 'appliance.MetricsConfig' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.MetricsConfig
- description: Update a 'appliance.SetupInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.SetupInfo
- description: Update a 'appliance.Upgrade' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.Upgrade
- description: Update a 'appliance.UpgradePolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.appliance.UpgradePolicy
- description: Update a 'asset.DeviceConfiguration' resource.
  flows:
  - clientCredentials
  scope: UPDATE.asset.DeviceConfiguration
- description: Update a 'asset.DeviceContractInformation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.asset.DeviceContractInformation
- description: Updates the resource representing the device connector. For example, this can be used to annotate the device connector resource with user-specified tags.
  flows:
  - clientCredentials
  scope: UPDATE.asset.DeviceRegistration
- description: Update a 'asset.GeoLocation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.asset.GeoLocation
- description: Update a 'asset.PreClaim' resource.
  flows:
  - clientCredentials
  scope: UPDATE.asset.PreClaim
- description: Update a 'asset.Target' resource.
  flows:
  - clientCredentials
  scope: UPDATE.asset.Target
- description: Update a 'auditd.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.auditd.Policy
- description: Update a 'bios.BootMode' resource.
  flows:
  - clientCredentials
  scope: UPDATE.bios.BootMode
- description: Update a 'bios.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.bios.Policy
- description: Update a 'bios.Unit' resource.
  flows:
  - clientCredentials
  scope: UPDATE.bios.Unit
- description: Update a 'boot.CddDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.CddDevice
- description: Update a 'boot.DeviceBootMode' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.DeviceBootMode
- description: Update a 'boot.DeviceBootSecurity' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.DeviceBootSecurity
- description: Update a 'boot.HddDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.HddDevice
- description: Update a 'boot.IscsiDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.IscsiDevice
- description: Update a 'boot.NvmeDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.NvmeDevice
- description: Update a 'boot.PchStorageDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.PchStorageDevice
- description: Update a 'boot.PrecisionPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.PrecisionPolicy
- description: Update a 'boot.PxeDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.PxeDevice
- description: Update a 'boot.SanDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.SanDevice
- description: Update a 'boot.SdDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.SdDevice
- description: Update a 'boot.UefiShellDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.UefiShellDevice
- description: Update a 'boot.UsbDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.UsbDevice
- description: Update a 'boot.VmediaDevice' resource.
  flows:
  - clientCredentials
  scope: UPDATE.boot.VmediaDevice
- description: Update a 'bulk.Export' resource.
  flows:
  - clientCredentials
  scope: UPDATE.bulk.Export
- description: Update a 'certificatemanagement.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.certificatemanagement.Policy
- description: Update a 'chassis.Profile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.chassis.Profile
- description: Update a 'chassis.ProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.chassis.ProfileTemplate
- description: Update a 'cli.CliPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.cli.CliPolicy
- description: Update a 'comm.HttpProxyPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.comm.HttpProxyPolicy
- description: Update a 'comm.TagDefinition' resource.
  flows:
  - clientCredentials
  scope: UPDATE.comm.TagDefinition
- description: Update a 'compute.Blade' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.Blade
- description: Update a 'compute.BladeIdentity' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.BladeIdentity
- description: Update a 'compute.Board' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.Board
- description: Update a 'compute.Mapping' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.Mapping
- description: Update a 'compute.PcieConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.PcieConnectivityPolicy
- description: Update a 'compute.Personality' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.Personality
- description: Update a 'compute.RackUnit' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.RackUnit
- description: Update a 'compute.RackUnitIdentity' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.RackUnitIdentity
- description: Update a 'compute.ScrubPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.ScrubPolicy
- description: Update a 'compute.ServerPowerPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.ServerPowerPolicy
- description: Update a 'compute.ServerSetting' resource.
  flows:
  - clientCredentials
  scope: UPDATE.compute.ServerSetting
- description: Update a 'cond.Alarm' resource.
  flows:
  - clientCredentials
  scope: UPDATE.cond.Alarm
- description: Update a 'cond.AlarmRule' resource.
  flows:
  - clientCredentials
  scope: UPDATE.cond.AlarmRule
- description: Update a 'cond.AlarmSuppression' resource.
  flows:
  - clientCredentials
  scope: UPDATE.cond.AlarmSuppression
- description: Update a 'cond.CustomHclBaseline' resource.
  flows:
  - clientCredentials
  scope: UPDATE.cond.CustomHclBaseline
- description: Update a 'cond.ThresholdDefinition' resource.
  flows:
  - clientCredentials
  scope: UPDATE.cond.ThresholdDefinition
- description: Update a 'convergedinfra.Pod' resource.
  flows:
  - clientCredentials
  scope: UPDATE.convergedinfra.Pod
- description: Update a 'coremanagement.CoreFile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.coremanagement.CoreFile
- description: Update a 'crd.CustomResource' resource.
  flows:
  - clientCredentials
  scope: UPDATE.crd.CustomResource
- description: Update a 'deviceconnector.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.deviceconnector.Policy
- description: Update a 'equipment.Chassis' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.Chassis
- description: Update a 'equipment.ChassisController' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.ChassisController
- description: Update a 'equipment.ChassisIdentity' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.ChassisIdentity
- description: Update a 'equipment.ChassisOperation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.ChassisOperation
- description: Update a 'equipment.EnclosureElement' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.EnclosureElement
- description: Update a 'equipment.ExpanderModule' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.ExpanderModule
- description: Update a 'equipment.ExpanderModuleIdentity' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.ExpanderModuleIdentity
- description: Update a 'equipment.ExpanderModuleOperation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.ExpanderModuleOperation
- description: Update a 'equipment.Fan' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.Fan
- description: Update a 'equipment.FanControl' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.FanControl
- description: Update a 'equipment.FanModule' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.FanModule
- description: Update a 'equipment.Fex' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.Fex
- description: Update a 'equipment.FexIdentity' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.FexIdentity
- description: Update a 'equipment.FexOperation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.FexOperation
- description: Update a 'equipment.Fru' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.Fru
- description: Update a 'equipment.IoCard' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.IoCard
- description: Update a 'equipment.IoCardOperation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.IoCardOperation
- description: Update a 'equipment.IoExpander' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.IoExpander
- description: Update a 'equipment.LocatorLed' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.LocatorLed
- description: Update a 'equipment.Psu' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.Psu
- description: Update a 'equipment.PsuControl' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.PsuControl
- description: Update a 'equipment.RackEnclosure' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.RackEnclosure
- description: Update a 'equipment.RackEnclosureSlot' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.RackEnclosureSlot
- description: Update a 'equipment.SharedIoModule' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.SharedIoModule
- description: Update a 'equipment.SwitchCard' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.SwitchCard
- description: Update a 'equipment.SwitchOperation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.SwitchOperation
- description: Update a 'equipment.SystemIoController' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.SystemIoController
- description: Update a 'equipment.Tpm' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.Tpm
- description: Update a 'equipment.Transceiver' resource.
  flows:
  - clientCredentials
  scope: UPDATE.equipment.Transceiver
- description: Update a 'ether.HostPort' resource.
  flows:
  - clientCredentials
  scope: UPDATE.ether.HostPort
- description: Update a 'ether.NetworkPort' resource.
  flows:
  - clientCredentials
  scope: UPDATE.ether.NetworkPort
- description: Update a 'ether.PhysicalPort' resource.
  flows:
  - clientCredentials
  scope: UPDATE.ether.PhysicalPort
- description: Update a 'externalsite.Authorization' resource.
  flows:
  - clientCredentials
  scope: UPDATE.externalsite.Authorization
- description: Update a 'fabric.AppliancePcRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.AppliancePcRole
- description: Update a 'fabric.ApplianceRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.ApplianceRole
- description: Update a 'fabric.ElementIdentity' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.ElementIdentity
- description: Update a 'fabric.EthNetworkControlPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.EthNetworkControlPolicy
- description: Update a 'fabric.EthNetworkGroupPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.EthNetworkGroupPolicy
- description: Update a 'fabric.EthNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.EthNetworkPolicy
- description: Update a 'fabric.FcNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.FcNetworkPolicy
- description: Update a 'fabric.FcStorageRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.FcStorageRole
- description: Update a 'fabric.FcUplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.FcUplinkPcRole
- description: Update a 'fabric.FcUplinkRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.FcUplinkRole
- description: Update a 'fabric.FcZonePolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.FcZonePolicy
- description: Update a 'fabric.FcoeUplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.FcoeUplinkPcRole
- description: Update a 'fabric.FcoeUplinkRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.FcoeUplinkRole
- description: Update a 'fabric.FlowControlPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.FlowControlPolicy
- description: Update a 'fabric.LanPinGroup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.LanPinGroup
- description: Update a 'fabric.LinkAggregationPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.LinkAggregationPolicy
- description: Update a 'fabric.LinkControlPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.LinkControlPolicy
- description: Update a 'fabric.MacSecPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.MacSecPolicy
- description: Update a 'fabric.MulticastPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.MulticastPolicy
- description: Update a 'fabric.NetFlowExporter' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.NetFlowExporter
- description: Update a 'fabric.NetFlowMonitor' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.NetFlowMonitor
- description: Update a 'fabric.NetFlowPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.NetFlowPolicy
- description: Update a 'fabric.NetFlowRecord' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.NetFlowRecord
- description: Update a 'fabric.PcOperation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.PcOperation
- description: Update a 'fabric.PortMode' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.PortMode
- description: Update a 'fabric.PortOperation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.PortOperation
- description: Update a 'fabric.PortPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.PortPolicy
- description: Update a 'fabric.SanPinGroup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SanPinGroup
- description: Update a 'fabric.SecureRouterRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SecureRouterRole
- description: Update a 'fabric.ServerRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.ServerRole
- description: Update a 'fabric.SpanDestEthPort' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SpanDestEthPort
- description: Update a 'fabric.SpanSession' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SpanSession
- description: Update a 'fabric.SwitchClusterProfile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SwitchClusterProfile
- description: Update a 'fabric.SwitchClusterProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SwitchClusterProfileTemplate
- description: Update a 'fabric.SwitchControlPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SwitchControlPolicy
- description: Update a 'fabric.SwitchProfile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SwitchProfile
- description: Update a 'fabric.SwitchProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SwitchProfileTemplate
- description: Update a 'fabric.SystemQosPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.SystemQosPolicy
- description: Update a 'fabric.UplinkPcRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.UplinkPcRole
- description: Update a 'fabric.UplinkRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.UplinkRole
- description: Update a 'fabric.Vlan' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.Vlan
- description: Update a 'fabric.Vsan' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fabric.Vsan
- description: Update a 'fault.Instance' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fault.Instance
- description: Update a 'fc.PhysicalPort' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fc.PhysicalPort
- description: Update a 'fcpool.Pool' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fcpool.Pool
- description: Update a 'fcpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.fcpool.Reservation
- description: Update a 'feedback.FeedbackPost' resource.
  flows:
  - clientCredentials
  scope: UPDATE.feedback.FeedbackPost
- description: Update a 'firmware.Distributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.firmware.Distributable
- description: Update a 'firmware.DriverDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.firmware.DriverDistributable
- description: Update a 'firmware.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.firmware.Policy
- description: Update a 'firmware.RunningFirmware' resource.
  flows:
  - clientCredentials
  scope: UPDATE.firmware.RunningFirmware
- description: Update a 'firmware.ServerConfigurationUtilityDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.firmware.ServerConfigurationUtilityDistributable
- description: Update a 'firmware.UnsupportedVersionUpgrade' resource.
  flows:
  - clientCredentials
  scope: UPDATE.firmware.UnsupportedVersionUpgrade
- description: Update a 'firmware.Upgrade' resource.
  flows:
  - clientCredentials
  scope: UPDATE.firmware.Upgrade
- description: Update a 'forecast.Instance' resource.
  flows:
  - clientCredentials
  scope: UPDATE.forecast.Instance
- description: Update a 'graphics.Card' resource.
  flows:
  - clientCredentials
  scope: UPDATE.graphics.Card
- description: Update a 'graphics.Controller' resource.
  flows:
  - clientCredentials
  scope: UPDATE.graphics.Controller
- description: Update a 'hci.AhvVm' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hci.AhvVm
- description: Update a 'hci.Cluster' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hci.Cluster
- description: Update a 'hci.ClusterOperation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hci.ClusterOperation
- description: Update a 'hci.EsxiVm' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hci.EsxiVm
- description: Update a 'hci.Node' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hci.Node
- description: Update a 'hyperflex.AutoSupportPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.AutoSupportPolicy
- description: Update a 'hyperflex.CapabilityInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.CapabilityInfo
- description: Update a 'hyperflex.Cluster' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.Cluster
- description: Update a 'hyperflex.ClusterBackupPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ClusterBackupPolicy
- description: Update a 'hyperflex.ClusterBackupPolicyDeployment' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ClusterBackupPolicyDeployment
- description: Update a 'hyperflex.ClusterNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ClusterNetworkPolicy
- description: Update a 'hyperflex.ClusterProfile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ClusterProfile
- description: Update a 'hyperflex.ClusterReplicationNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ClusterReplicationNetworkPolicy
- description: Update a 'hyperflex.ClusterReplicationNetworkPolicyDeployment' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ClusterReplicationNetworkPolicyDeployment
- description: Update a 'hyperflex.ClusterStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ClusterStoragePolicy
- description: Update a 'hyperflex.Drive' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.Drive
- description: Update a 'hyperflex.ExtFcStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ExtFcStoragePolicy
- description: Update a 'hyperflex.ExtIscsiStoragePolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ExtIscsiStoragePolicy
- description: Update a 'hyperflex.HypervisorHost' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.HypervisorHost
- description: Update a 'hyperflex.HypervisorVirtualMachine' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.HypervisorVirtualMachine
- description: Update a 'hyperflex.InitiatorGroup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.InitiatorGroup
- description: Update a 'hyperflex.IscsiNetwork' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.IscsiNetwork
- description: Update a 'hyperflex.KeyEncryptionKey' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.KeyEncryptionKey
- description: Update a 'hyperflex.LocalCredentialPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.LocalCredentialPolicy
- description: Update a 'hyperflex.Lun' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.Lun
- description: Update a 'hyperflex.NodeConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.NodeConfigPolicy
- description: Update a 'hyperflex.NodeProfile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.NodeProfile
- description: Update a 'hyperflex.ProxySettingPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ProxySettingPolicy
- description: Update a 'hyperflex.ReduceReSync' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ReduceReSync
- description: Update a 'hyperflex.ServiceAuthToken' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.ServiceAuthToken
- description: Update a 'hyperflex.SoftwareVersionPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.SoftwareVersionPolicy
- description: Update a 'hyperflex.StorageContainer' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.StorageContainer
- description: Update a 'hyperflex.SysConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.SysConfigPolicy
- description: Update a 'hyperflex.Target' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.Target
- description: Update a 'hyperflex.UcsmConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.UcsmConfigPolicy
- description: Update a 'hyperflex.VcenterConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.VcenterConfigPolicy
- description: Update a 'hyperflex.Volume' resource.
  flows:
  - clientCredentials
  scope: UPDATE.hyperflex.Volume
- description: Update a 'iaas.UcsdInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iaas.UcsdInfo
- description: Update a 'iam.Account' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.Account
- description: Update a 'iam.ApiKey' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.ApiKey
- description: Update a 'iam.AppRegistration' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.AppRegistration
- description: Update a 'iam.BannerMessage' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.BannerMessage
- description: Update a 'iam.Certificate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.Certificate
- description: Update a 'iam.CertificateRequest' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.CertificateRequest
- description: Update a 'iam.CuiIntegration' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.CuiIntegration
- description: Update a 'iam.DefaultAuthentication' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.DefaultAuthentication
- description: Update a 'iam.DomainNameInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.DomainNameInfo
- description: Update a 'iam.EndPointUser' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.EndPointUser
- description: Update a 'iam.EndPointUserPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.EndPointUserPolicy
- description: Update a 'iam.EndPointUserRole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.EndPointUserRole
- description: Update a 'iam.GuestAccessSettings' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.GuestAccessSettings
- description: Update a 'iam.Idp' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.Idp
- description: Update a 'iam.IdpReference' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.IdpReference
- description: Update a 'iam.IpAccessManagement' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.IpAccessManagement
- description: Update a 'iam.IpAddress' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.IpAddress
- description: Update a 'iam.LdapGroup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.LdapGroup
- description: Update a 'iam.LdapPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.LdapPolicy
- description: Update a 'iam.LdapProvider' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.LdapProvider
- description: Update a 'iam.LocalUserPassword' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.LocalUserPassword
- description: Update a 'iam.LocalUserPasswordPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.LocalUserPasswordPolicy
- description: Update a 'iam.Permission' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.Permission
- description: Update a 'iam.PrivateKeySpec' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.PrivateKeySpec
- description: Update a 'iam.PrivilegeSet' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.PrivilegeSet
- description: Update a 'iam.Qualifier' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.Qualifier
- description: Update a 'iam.ResourceLimits' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.ResourceLimits
- description: Update a 'iam.ResourceRoles' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.ResourceRoles
- description: Update a 'iam.SessionLimits' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.SessionLimits
- description: Update a 'iam.SharingRule' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.SharingRule
- description: Update a 'iam.TestIdpConfiguration' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.TestIdpConfiguration
- description: Update a 'iam.User' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.User
- description: Update a 'iam.UserGroup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.UserGroup
- description: Update a 'iam.UserPreference' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.UserPreference
- description: Update a 'iam.UserQualifier' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.UserQualifier
- description: Update a 'iam.UserSetting' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iam.UserSetting
- description: Update a 'inventory.GenericInventory' resource.
  flows:
  - clientCredentials
  scope: UPDATE.inventory.GenericInventory
- description: Update a 'inventory.GenericInventoryHolder' resource.
  flows:
  - clientCredentials
  scope: UPDATE.inventory.GenericInventoryHolder
- description: Update a 'ipmioverlan.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.ipmioverlan.Policy
- description: Update a 'ippool.Pool' resource.
  flows:
  - clientCredentials
  scope: UPDATE.ippool.Pool
- description: Update a 'ippool.Reservation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.ippool.Reservation
- description: Update a 'iqnpool.Pool' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iqnpool.Pool
- description: Update a 'iwotenant.Migrate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iwotenant.Migrate
- description: Update a 'iwotenant.TenantCustomization' resource.
  flows:
  - clientCredentials
  scope: UPDATE.iwotenant.TenantCustomization
- description: Update a 'kvm.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.kvm.Policy
- description: Update a 'kvm.Session' resource.
  flows:
  - clientCredentials
  scope: UPDATE.kvm.Session
- description: Update a 'kvm.TunneledKvmPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.kvm.TunneledKvmPolicy
- description: Update a 'license.AccountLicenseData' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.AccountLicenseData
- description: Update a 'license.CustomerOp' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.CustomerOp
- description: Update a 'license.ErpCustomerOp' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.ErpCustomerOp
- description: Update a 'license.IksCustomerOp' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.IksCustomerOp
- description: Update a 'license.IksLicenseCount' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.IksLicenseCount
- description: Update a 'license.IncCustomerOp' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.IncCustomerOp
- description: Update a 'license.IncLicenseCount' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.IncLicenseCount
- description: Update a 'license.IwoCustomerOp' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.IwoCustomerOp
- description: Update a 'license.IwoLicenseCount' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.IwoLicenseCount
- description: Update a 'license.LicenseInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.LicenseInfo
- description: Update a 'license.LicenseRegistrationStatus' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.LicenseRegistrationStatus
- description: Update a 'license.LicenseReservationOp' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.LicenseReservationOp
- description: Update a 'license.SmartlicenseToken' resource.
  flows:
  - clientCredentials
  scope: UPDATE.license.SmartlicenseToken
- description: Update a 'ls.ServiceProfile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.ls.ServiceProfile
- description: Update a 'macpool.Pool' resource.
  flows:
  - clientCredentials
  scope: UPDATE.macpool.Pool
- description: Update a 'macpool.Reservation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.macpool.Reservation
- description: Update a 'management.Controller' resource.
  flows:
  - clientCredentials
  scope: UPDATE.management.Controller
- description: Update a 'management.Entity' resource.
  flows:
  - clientCredentials
  scope: UPDATE.management.Entity
- description: Update a 'management.Interface' resource.
  flows:
  - clientCredentials
  scope: UPDATE.management.Interface
- description: Update a 'memory.Array' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.Array
- description: Update a 'memory.PersistentMemoryConfigResult' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.PersistentMemoryConfigResult
- description: Update a 'memory.PersistentMemoryConfiguration' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.PersistentMemoryConfiguration
- description: Update a 'memory.PersistentMemoryNamespace' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.PersistentMemoryNamespace
- description: Update a 'memory.PersistentMemoryNamespaceConfigResult' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.PersistentMemoryNamespaceConfigResult
- description: Update a 'memory.PersistentMemoryPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.PersistentMemoryPolicy
- description: Update a 'memory.PersistentMemoryRegion' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.PersistentMemoryRegion
- description: Update a 'memory.PersistentMemoryUnit' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.PersistentMemoryUnit
- description: Update a 'memory.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.Policy
- description: Update a 'memory.Unit' resource.
  flows:
  - clientCredentials
  scope: UPDATE.memory.Unit
- description: Update a 'metrics.Configuration' resource.
  flows:
  - clientCredentials
  scope: UPDATE.metrics.Configuration
- description: Update a 'metrics.MetricsExploration' resource.
  flows:
  - clientCredentials
  scope: UPDATE.metrics.MetricsExploration
- description: Update a 'metrics.ResourceConfiguration' resource.
  flows:
  - clientCredentials
  scope: UPDATE.metrics.ResourceConfiguration
- description: Update a 'mgmt.ConfigBackupFile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.mgmt.ConfigBackupFile
- description: Update a 'mgmt.ConfigBackupInstance' resource.
  flows:
  - clientCredentials
  scope: UPDATE.mgmt.ConfigBackupInstance
- description: Update a 'mgmt.ConfigBackupOperation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.mgmt.ConfigBackupOperation
- description: Update a 'mgmt.ConfigOperationSetting' resource.
  flows:
  - clientCredentials
  scope: UPDATE.mgmt.ConfigOperationSetting
- description: Update a 'network.Element' resource.
  flows:
  - clientCredentials
  scope: UPDATE.network.Element
- description: Update a 'network.FcZoneInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.network.FcZoneInfo
- description: Update a 'network.SecureRouter' resource.
  flows:
  - clientCredentials
  scope: UPDATE.network.SecureRouter
- description: Update a 'network.SecureRouterSetting' resource.
  flows:
  - clientCredentials
  scope: UPDATE.network.SecureRouterSetting
- description: Update a 'network.Vethernet' resource.
  flows:
  - clientCredentials
  scope: UPDATE.network.Vethernet
- description: Update a 'network.Vfc' resource.
  flows:
  - clientCredentials
  scope: UPDATE.network.Vfc
- description: Update a 'network.VlanPortInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.network.VlanPortInfo
- description: Update a 'networkconfig.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.networkconfig.Policy
- description: Update a 'notification.AccountSubscription' resource.
  flows:
  - clientCredentials
  scope: UPDATE.notification.AccountSubscription
- description: Update a 'ntp.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.ntp.Policy
- description: Update a 'oauth.Authorization' resource.
  flows:
  - clientCredentials
  scope: UPDATE.oauth.Authorization
- description: Update a 'onprem.Upgrade' resource.
  flows:
  - clientCredentials
  scope: UPDATE.onprem.Upgrade
- description: Update a 'onprem.UserPreference' resource.
  flows:
  - clientCredentials
  scope: UPDATE.onprem.UserPreference
- description: Update a 'openapi.OpenApiSpecification' resource.
  flows:
  - clientCredentials
  scope: UPDATE.openapi.OpenApiSpecification
- description: Update a 'openapi.TaskGenerationRequest' resource.
  flows:
  - clientCredentials
  scope: UPDATE.openapi.TaskGenerationRequest
- description: Update a 'oprs.Deployment' resource.
  flows:
  - clientCredentials
  scope: UPDATE.oprs.Deployment
- description: Update a 'oprs.SyncTargetListMessage' resource.
  flows:
  - clientCredentials
  scope: UPDATE.oprs.SyncTargetListMessage
- description: Update a 'organization.Organization' resource.
  flows:
  - clientCredentials
  scope: UPDATE.organization.Organization
- description: Update a 'os.ConfigurationFile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.os.ConfigurationFile
- description: Update a 'partnerintegration.DeviceConnector' resource.
  flows:
  - clientCredentials
  scope: UPDATE.partnerintegration.DeviceConnector
- description: Update a 'partnerintegration.Etl' resource.
  flows:
  - clientCredentials
  scope: UPDATE.partnerintegration.Etl
- description: Update a 'partnerintegration.File' resource.
  flows:
  - clientCredentials
  scope: UPDATE.partnerintegration.File
- description: Update a 'partnerintegration.Inventory' resource.
  flows:
  - clientCredentials
  scope: UPDATE.partnerintegration.Inventory
- description: Update a 'partnerintegration.Metrics' resource.
  flows:
  - clientCredentials
  scope: UPDATE.partnerintegration.Metrics
- description: Update a 'partnerintegration.Model' resource.
  flows:
  - clientCredentials
  scope: UPDATE.partnerintegration.Model
- description: Update a 'pci.Device' resource.
  flows:
  - clientCredentials
  scope: UPDATE.pci.Device
- description: Update a 'pci.Link' resource.
  flows:
  - clientCredentials
  scope: UPDATE.pci.Link
- description: Update a 'pci.Node' resource.
  flows:
  - clientCredentials
  scope: UPDATE.pci.Node
- description: Update a 'pci.NodeSetting' resource.
  flows:
  - clientCredentials
  scope: UPDATE.pci.NodeSetting
- description: Update a 'pci.Switch' resource.
  flows:
  - clientCredentials
  scope: UPDATE.pci.Switch
- description: Update a 'pool.IdMappingPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.pool.IdMappingPolicy
- description: Update a 'port.Group' resource.
  flows:
  - clientCredentials
  scope: UPDATE.port.Group
- description: Update a 'port.MacBinding' resource.
  flows:
  - clientCredentials
  scope: UPDATE.port.MacBinding
- description: Update a 'port.SubGroup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.port.SubGroup
- description: Update a 'power.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.power.Policy
- description: Update a 'power.PowerGroup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.power.PowerGroup
- description: Update a 'processor.Unit' resource.
  flows:
  - clientCredentials
  scope: UPDATE.processor.Unit
- description: Update a 'rack.UnitPersonality' resource.
  flows:
  - clientCredentials
  scope: UPDATE.rack.UnitPersonality
- description: Update a 'recommendation.HardwareExpansionRequest' resource.
  flows:
  - clientCredentials
  scope: UPDATE.recommendation.HardwareExpansionRequest
- description: Update a 'recommendation.HardwareExpansionRequestItem' resource.
  flows:
  - clientCredentials
  scope: UPDATE.recommendation.HardwareExpansionRequestItem
- description: Update a 'recommendation.PurchaseOrderEstimate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.recommendation.PurchaseOrderEstimate
- description: Update a 'recovery.BackupConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.recovery.BackupConfigPolicy
- description: Update a 'recovery.BackupProfile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.recovery.BackupProfile
- description: Update a 'recovery.OnDemandBackup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.recovery.OnDemandBackup
- description: Update a 'recovery.ScheduleConfigPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.recovery.ScheduleConfigPolicy
- description: Update a 'resource.Group' resource.
  flows:
  - clientCredentials
  scope: UPDATE.resource.Group
- description: Update a 'resource.Membership' resource.
  flows:
  - clientCredentials
  scope: UPDATE.resource.Membership
- description: Update a 'resource.Reservation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.resource.Reservation
- description: Update a 'resource.SelectionCriteria' resource.
  flows:
  - clientCredentials
  scope: UPDATE.resource.SelectionCriteria
- description: Update a 'resourcepool.MembershipReservation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.resourcepool.MembershipReservation
- description: Update a 'resourcepool.Pool' resource.
  flows:
  - clientCredentials
  scope: UPDATE.resourcepool.Pool
- description: Update a 'resourcepool.QualificationPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.resourcepool.QualificationPolicy
- description: Update a 'resourcepool.Reservation' resource.
  flows:
  - clientCredentials
  scope: UPDATE.resourcepool.Reservation
- description: Update a 'scheduler.SchedulePolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.scheduler.SchedulePolicy
- description: Update a 'scheduler.TaskSchedule' resource.
  flows:
  - clientCredentials
  scope: UPDATE.scheduler.TaskSchedule
- description: Update a 'sdaaci.Connection' resource.
  flows:
  - clientCredentials
  scope: UPDATE.sdaaci.Connection
- description: Update a 'sdaaci.ConnectionDetail' resource.
  flows:
  - clientCredentials
  scope: UPDATE.sdaaci.ConnectionDetail
- description: Update a 'sdcard.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.sdcard.Policy
- description: Update a 'security.Unit' resource.
  flows:
  - clientCredentials
  scope: UPDATE.security.Unit
- description: Update a 'server.DiagnosticStatus' resource.
  flows:
  - clientCredentials
  scope: UPDATE.server.DiagnosticStatus
- description: Update a 'server.Diagnostics' resource.
  flows:
  - clientCredentials
  scope: UPDATE.server.Diagnostics
- description: Update a 'server.Profile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.server.Profile
- description: Update a 'server.ProfileTemplate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.server.ProfileTemplate
- description: Update a 'smtp.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.smtp.Policy
- description: Update a 'smtp.PolicyTest' resource.
  flows:
  - clientCredentials
  scope: UPDATE.smtp.PolicyTest
- description: Update a 'snmp.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.snmp.Policy
- description: Update a 'software.ApplianceDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.ApplianceDistributable
- description: Update a 'software.HciBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.HciBundleDistributable
- description: Update a 'software.HciDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.HciDistributable
- description: Update a 'software.HyperflexBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.HyperflexBundleDistributable
- description: Update a 'software.HyperflexDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.HyperflexDistributable
- description: Update a 'software.IksBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.IksBundleDistributable
- description: Update a 'software.ReleaseMeta' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.ReleaseMeta
- description: Update a 'software.SolutionDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.SolutionDistributable
- description: Update a 'software.UcsdBundleDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.UcsdBundleDistributable
- description: Update a 'software.UcsdDistributable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.software.UcsdDistributable
- description: Update a 'softwarerepository.Authorization' resource.
  flows:
  - clientCredentials
  scope: UPDATE.softwarerepository.Authorization
- description: Update a 'softwarerepository.OperatingSystemFile' resource.
  flows:
  - clientCredentials
  scope: UPDATE.softwarerepository.OperatingSystemFile
- description: Update a 'sol.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.sol.Policy
- description: Update a 'ssh.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.ssh.Policy
- description: Update a 'storage.BatteryBackupUnit' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.BatteryBackupUnit
- description: Update a 'storage.Controller' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.Controller
- description: Update a 'storage.DiskGroup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.DiskGroup
- description: Update a 'storage.DriveGroup' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.DriveGroup
- description: Update a 'storage.DriveSecurityPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.DriveSecurityPolicy
- description: Update a 'storage.Enclosure' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.Enclosure
- description: Update a 'storage.EnclosureDisk' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.EnclosureDisk
- description: Update a 'storage.EnclosureDiskSlotEp' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.EnclosureDiskSlotEp
- description: Update a 'storage.FlexFlashController' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.FlexFlashController
- description: Update a 'storage.FlexFlashControllerProps' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.FlexFlashControllerProps
- description: Update a 'storage.FlexFlashPhysicalDrive' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.FlexFlashPhysicalDrive
- description: Update a 'storage.FlexFlashVirtualDrive' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.FlexFlashVirtualDrive
- description: Update a 'storage.FlexUtilController' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.FlexUtilController
- description: Update a 'storage.FlexUtilPhysicalDrive' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.FlexUtilPhysicalDrive
- description: Update a 'storage.FlexUtilVirtualDrive' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.FlexUtilVirtualDrive
- description: Update a 'storage.HitachiArray' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.HitachiArray
- description: Update a 'storage.NetAppCluster' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.NetAppCluster
- description: Update a 'storage.PhysicalDisk' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.PhysicalDisk
- description: Update a 'storage.PhysicalDiskExtension' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.PhysicalDiskExtension
- description: Update a 'storage.PhysicalDiskUsage' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.PhysicalDiskUsage
- description: Update a 'storage.PureArray' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.PureArray
- description: Update a 'storage.PureFlashBladeSystem' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.PureFlashBladeSystem
- description: Update a 'storage.SasExpander' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.SasExpander
- description: Update a 'storage.SasPort' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.SasPort
- description: Update a 'storage.Span' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.Span
- description: Update a 'storage.StoragePolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.StoragePolicy
- description: Update a 'storage.VdMemberEp' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.VdMemberEp
- description: Update a 'storage.VirtualDrive' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.VirtualDrive
- description: Update a 'storage.VirtualDriveContainer' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.VirtualDriveContainer
- description: Update a 'storage.VirtualDriveExtension' resource.
  flows:
  - clientCredentials
  scope: UPDATE.storage.VirtualDriveExtension
- description: Update a 'syslog.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.syslog.Policy
- description: Update a 'tam.AdvisoryInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.tam.AdvisoryInfo
- description: Update a 'techsupportmanagement.CollectionControlPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.techsupportmanagement.CollectionControlPolicy
- description: Update a 'thermal.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.thermal.Policy
- description: Update a 'top.System' resource.
  flows:
  - clientCredentials
  scope: UPDATE.top.System
- description: Update a 'uuidpool.Pool' resource.
  flows:
  - clientCredentials
  scope: UPDATE.uuidpool.Pool
- description: Update a 'virtualization.EsxiConsole' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.EsxiConsole
- description: Update a 'virtualization.Host' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.Host
- description: Update a 'virtualization.VirtualMachine' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VirtualMachine
- description: Update a 'virtualization.VmwareCluster' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareCluster
- description: Update a 'virtualization.VmwareDatacenter' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareDatacenter
- description: Update a 'virtualization.VmwareDatastore' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareDatastore
- description: Update a 'virtualization.VmwareDatastoreCluster' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareDatastoreCluster
- description: Update a 'virtualization.VmwareDistributedNetwork' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareDistributedNetwork
- description: Update a 'virtualization.VmwareDistributedSwitch' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareDistributedSwitch
- description: Update a 'virtualization.VmwareFolder' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareFolder
- description: Update a 'virtualization.VmwareHost' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareHost
- description: Update a 'virtualization.VmwareKernelNetwork' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareKernelNetwork
- description: Update a 'virtualization.VmwareNetwork' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareNetwork
- description: Update a 'virtualization.VmwarePhysicalNetworkInterface' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwarePhysicalNetworkInterface
- description: Update a 'virtualization.VmwareUplinkPort' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareUplinkPort
- description: Update a 'virtualization.VmwareVirtualDisk' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareVirtualDisk
- description: Update a 'virtualization.VmwareVirtualMachine' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareVirtualMachine
- description: Update a 'virtualization.VmwareVirtualMachineSnapshot' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareVirtualMachineSnapshot
- description: Update a 'virtualization.VmwareVirtualNetworkInterface' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareVirtualNetworkInterface
- description: Update a 'virtualization.VmwareVirtualSwitch' resource.
  flows:
  - clientCredentials
  scope: UPDATE.virtualization.VmwareVirtualSwitch
- description: Update a 'vmedia.Policy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vmedia.Policy
- description: Update a 'vmrc.Console' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vmrc.Console
- description: Update a 'vnic.EthAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.EthAdapterPolicy
- description: Update a 'vnic.EthIf' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.EthIf
- description: Update a 'vnic.EthNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.EthNetworkPolicy
- description: Update a 'vnic.EthQosPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.EthQosPolicy
- description: Update a 'vnic.FcAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.FcAdapterPolicy
- description: Update a 'vnic.FcIf' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.FcIf
- description: Update a 'vnic.FcNetworkPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.FcNetworkPolicy
- description: Update a 'vnic.FcQosPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.FcQosPolicy
- description: Update a 'vnic.IscsiAdapterPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.IscsiAdapterPolicy
- description: Update a 'vnic.IscsiBootPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.IscsiBootPolicy
- description: Update a 'vnic.IscsiStaticTargetPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.IscsiStaticTargetPolicy
- description: Update a 'vnic.LanConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.LanConnectivityPolicy
- description: Update a 'vnic.SanConnectivityPolicy' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.SanConnectivityPolicy
- description: Update a 'vnic.VhbaTemplate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.VhbaTemplate
- description: Update a 'vnic.VnicTemplate' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vnic.VnicTemplate
- description: Update a 'vrf.Vrf' resource.
  flows:
  - clientCredentials
  scope: UPDATE.vrf.Vrf
- description: Update a 'webhook.Endpoint' resource.
  flows:
  - clientCredentials
  scope: UPDATE.webhook.Endpoint
- description: Update a 'webhook.Schema' resource.
  flows:
  - clientCredentials
  scope: UPDATE.webhook.Schema
- description: Update a 'workflow.AnsibleBatchExecutor' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.AnsibleBatchExecutor
- description: Update a 'workflow.BatchApiExecutor' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.BatchApiExecutor
- description: Update a 'workflow.CatalogItemDefinition' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.CatalogItemDefinition
- description: Update a 'workflow.CatalogServiceRequest' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.CatalogServiceRequest
- description: Update a 'workflow.CustomDataTypeDefinition' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.CustomDataTypeDefinition
- description: Update a 'workflow.ErrorResponseHandler' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.ErrorResponseHandler
- description: Update a 'workflow.PowerShellBatchApiExecutor' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.PowerShellBatchApiExecutor
- description: Update a 'workflow.RollbackWorkflow' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.RollbackWorkflow
- description: Update a 'workflow.ServiceItemActionDefinition' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.ServiceItemActionDefinition
- description: Update a 'workflow.ServiceItemActionInstance' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.ServiceItemActionInstance
- description: Update a 'workflow.ServiceItemDefinition' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.ServiceItemDefinition
- description: Update a 'workflow.ServiceItemInstance' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.ServiceItemInstance
- description: Update a 'workflow.ServiceItemOutput' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.ServiceItemOutput
- description: Update a 'workflow.SshBatchExecutor' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.SshBatchExecutor
- description: Update a 'workflow.TaskDefinition' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.TaskDefinition
- description: Update a 'workflow.TaskInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.TaskInfo
- description: Update a 'workflow.UiDisplayMetadata' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.UiDisplayMetadata
- description: Update a 'workflow.Variable' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.Variable
- description: Update a 'workflow.WorkflowDefinition' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.WorkflowDefinition
- description: Update a 'workflow.WorkflowInfo' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workflow.WorkflowInfo
- description: Update a 'workload.Blueprint' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workload.Blueprint
- description: Update a 'workload.WorkloadDefinition' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workload.WorkloadDefinition
- description: Update a 'workload.WorkloadDeployment' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workload.WorkloadDeployment
- description: Update a 'workload.WorkloadInstance' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workload.WorkloadInstance
- description: Update a 'workload.WorkloadMetadata' resource.
  flows:
  - clientCredentials
  scope: UPDATE.workload.WorkloadMetadata
slug: intersight-scopes
source_filename: intersight-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: openapi/intersight-fabric-openapi.json, openapi/intersight-hyperflex-openapi.json, openapi/intersight-kubernetes-openapi.json,\n  openapi/intersight-nexus-insight-advisor-openapi.json, openapi/intersight-orchestrator-openapi.json,\n  openapi/intersight-server-openapi.json, openapi/intersight-storage-openapi.json, openapi/intersight-system-openapi.json,\n  openapi/intersight-telemetry-openapi.json, openapi/intersight-virtualization-openapi.json,\n  openapi/intersight-workflows-openapi.json\nschemes:\n- name: oAuth2\n  source: openapi/intersight-fabric-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration\
  \ resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name: oAuth2\n  source: openapi/intersight-hyperflex-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use\
  \ OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name: oAuth2\n  source: openapi/intersight-kubernetes-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl:\
  \ /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name: oAuth2\n\
  \  source: openapi/intersight-nexus-insight-advisor-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials\
  \ flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name: oAuth2\n  source: openapi/intersight-orchestrator-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the\
  \ scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name: oAuth2\n  source: openapi/intersight-server-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends\
  \ a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name: oAuth2\n  source: openapi/intersight-storage-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a\
  \ registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name: oAuth2\n  source: openapi/intersight-system-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the\
  \ iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name: oAuth2\n  source: openapi/intersight-telemetry-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security\
  \ scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name: oAuth2\n  source: openapi/intersight-virtualization-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n\
  \    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\n- name:\
  \ oAuth2\n  source: openapi/intersight-workflows-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorization code flow, the client sends a list of requested scopes to\n    the authorization URL (/iam/app-authorize). The scope in the authorization request\n    must be one of the scopes that have been configured in the corresponding\n    iam.AppRegistration resource.\n    **Client Credentials**\n    In the client credentials\
  \ flow, the scope is selected when the AppRegistration\n    is created. The client cannot select a specific scope in the token request.\nscopes:\n- scope: CREATE.aaa.RetentionPolicy\n  description: Create a 'aaa.RetentionPolicy' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.access.Policy\n  description: Create a 'access.Policy' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n\
  \  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.adapter.ConfigPolicy\n  description: Create a 'adapter.ConfigPolicy' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n\
  \  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.Backup\n  description: Create a 'appliance.Backup' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.BackupPolicy\n  description: Create a 'appliance.BackupPolicy' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  -\
  \ openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.ClusterInfo\n  description: Create a 'appliance.ClusterInfo' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n\
  \  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.ClusterReplaceNode\n  description: Create a 'appliance.ClusterReplaceNode' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.ClusterWorkerNode\n  description: Create a 'appliance.ClusterWorkerNode' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n\
  \  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.ClusterWorkerNodeReplace\n  description: Create a 'appliance.ClusterWorkerNodeReplace' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n\
  \  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.ClusterWorkerNodeReuse\n  description: Create a 'appliance.ClusterWorkerNodeReuse' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.DataExportPolicy\n  description: Create a 'appliance.DataExportPolicy' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n\
  \  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.DeviceClaim\n  description: Create a 'appliance.DeviceClaim' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n\
  \  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.DiagSetting\n  description: Create a 'appliance.DiagSetting' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.ExternalSyslogSetting\n  description: Create a 'appliance.ExternalSyslogSetting' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n\
  \  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.FqdnUpdate\n  description: Create a 'appliance.FqdnUpdate' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n\
  \  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.RemoteFileImport\n  description: Create a 'appliance.RemoteFileImport' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.appliance.Restore\n  description: Create a 'appliance.Restore' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n\
  \  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.asset.ClaimToken\n  description: Create a 'asset.ClaimToken' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n \
  \ - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.asset.DeviceClaim\n  description: Create a 'asset.DeviceClaim' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.asset.DeviceContractNotification\n  description: Create a 'asset.DeviceContractNotification' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n\
  \  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.asset.GeoLocation\n  description: Create a 'asset.GeoLocation' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n\
  \  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.asset.PreClaim\n  description: Create a 'asset.PreClaim' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.asset.Target\n  description: Create a 'asset.Target' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n\
  \  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.auditd.Policy\n  description: Create a 'auditd.Policy' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  -\
  \ openapi/intersight-workflows-openapi.json\n- scope: CREATE.bios.Policy\n  description: Create a 'bios.Policy' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.boot.PrecisionPolicy\n  description: Create a 'boot.PrecisionPolicy' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n\
  \  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.bulk.Export\n  description: Create a 'bulk.Export' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.bulk.MoCloner\n\
  \  description: Create a 'bulk.MoCloner' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.bulk.MoDeepCloner\n  description: Create a 'bulk.MoDeepCloner' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n\
  \  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.bulk.MoMerger\n  description: Create a 'bulk.MoMerger' resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- scope: CREATE.bulk.Request\n  description: Create a 'bulk.Request'\
  \ resource.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insig\n\n# --- truncated at 32 KB (2187 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/scopes/intersight-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/scopes/intersight-scopes.yml
summary_line: 3317 scopes · authorizationCode/clientCredentials
tags:
- Infrastructure
- Cloud Operations
- Data Center
- Compute
- Networking
- Enterprise
- Storage
- Virtualization
- Kubernetes
- Orchestration
- Telemetry
- Firmware Management
token_urls:
- /iam/token
---
