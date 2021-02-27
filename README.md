![Travis CI Status](https://travis-ci.org/YakDriver/terraform-aws-conventions.svg?branch=main)
# terraform-aws-conventions

Automatic daily builds :coffee:! Data below :point_down:. The current state of naming conventions in the Terraform AWS provider Go code.

Find out more:
* [AWS provider](https://github.com/terraform-providers/terraform-provider-aws)
* [AWS provider stats](https://github.com/YakDriver/terraform-aws-provider-stats)
* [AWS provider linter](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint)
* [AWS provider conventions](https://github.com/YakDriver/terraform-aws-conventions)
* [AWS provider static checks](https://github.com/YakDriver/terraform-aws-provider-static-checks)

# Conventions
## All Functions

### Exported
Count: 5267
[List matches](./results/functions-exported.txt)

Example: `func TestAccAWSKmsExternalKey_disappears(`

### Non-Exported
Count: 15120
[List matches](./results/functions-non-exported.txt)

Example: `func init(`

### Multicaps
Count: 9941
[List matches](./results/functions-multicaps.txt)

Example: `func resourceAwsS3BucketAnalyticsConfigurationParseID(`

### Non-AWS Multicaps
Count: 3955
[List matches](./results/functions-non-aws-multicaps.txt)

Example: `func TestAccAWSAPIGatewayUsagePlan_productCode(`

### Uppercase AWS
Count: 8823
[List matches](./results/functions-uppercase-aws.txt)

Example: `func testAccAWSEcsTaskDefinitionImportStateIdFunc(`

### Mixed case AWS
Count: 6183
[List matches](./results/functions-mixed-case-aws.txt)

Example: `func resourceAwsVpcEndpointServiceAllowedPrincipal(`

### Any underscores
Count: 7476
[List matches](./results/functions-any-underscores.txt)

Example: `func TestAccAWSS3BucketPublicAccessBlock_RestrictPublicBuckets(`

### Multiple underscores
Count: 1698
[List matches](./results/functions-multiple-underscores.txt)

Example: `func TestAccAWSCodeDeployDeploymentGroup_blueGreenDeploymentConfiguration_update_with_asg(`

### Lowercase after first underscore
Count: 4669
[List matches](./results/functions-lowercase-after-first-underscore.txt)

Example: `func TestAccAWSIAMRole_policyOutOfBandRemovalAddedBack_inlineNonEmpty(`

### Uppercase after first underscore
Count: 2806
[List matches](./results/functions-uppercase-after-first-underscore.txt)

Example: `func TestAccAWSLambdaEventSourceMapping_BisectBatch(`

## Capital-T Test Functions

### All
Count: 5234
[List matches](./results/capT-Test.txt)

Example: `func TestValidateAwsAccountId(`

### TestAcc
Count: 4876
[List matches](./results/capT-TestAcc.txt)

Example: `func TestAccAWSLBListener_BackwardsCompatibility(`

### TestAccAWS
Count: 4141
[List matches](./results/capT-TestAcc-allCapAWS.txt)

Example: `func TestAccAWSEMRCluster_instance_fleet(`

### TestAccAws
Count: 461
[List matches](./results/capT-TestAcc-iniCapAws.txt)

Example: `func TestAccAwsWafv2RuleGroup_ChangeMetricNameForceNew(`

### TestAccDataSourceAWS
Count: 65
[List matches](./results/capT-TestAccDataSourceAWS.txt)

Example: `func TestAccDataSourceAWSRDSCluster_basic(`

### TestAccDataSourceAws
Count: 188
[List matches](./results/capT-TestAccDataSourceAws.txt)

Example: `func TestAccDataSourceAwsVpcEndpointService_custom_filter_tags(`

### TestAccAWS+DataSource
Count: 210
[List matches](./results/capT-TestAccAWS-plus-DataSource.txt)

Example: `func TestAccAWSBackupVaultDataSource_basic(`

### TestAccAws+DataSource
Count: 16
[List matches](./results/capT-TestAccAws-plus-DataSource.txt)

Example: `func TestAccAwsImageBuilderImageDataSource_Arn_Aws(`

### TestAccAWSDataSource
Count: 31
[List matches](./results/capT-TestAccAWSDataSource.txt)

Example: `func TestAccAWSDataSourceIAMPolicyDocument_noStatementOverride(`

### TestAccAwsDataSource
Count: 0
### TestAccAWSData
Count: 74
[List matches](./results/capT-TestAccAWSData.txt)

Example: `func TestAccAWSDataSourceIAMPolicyDocument_sourceList(`

### TestAccAwsData
Count: 0
### TestAccResourceAWS
Count: 0
### TestAccResourceAws
Count: 3
[List matches](./results/capT-TestAccResourceAws.txt)

Example: `func TestAccResourceAwsKmsCiphertext_basic(`

### TestAccAWS+Resource
Count: 31
[List matches](./results/capT-TestAccAWS-plus-Resource.txt)

Example: `func TestAccAWSLakeFormationResource_updateSLRToRole(`

### TestAccAws+Resource
Count: 15
[List matches](./results/capT-TestAccAws-plus-Resource.txt)

Example: `func TestAccAwsRamResourceShare_Name(`

### TestAcc and lowercase after first underscore
Count: 3032
[List matches](./results/capT-TestAcc-lowAfterUnderscore.txt)

Example: `func TestAccAWSOpsworksGangliaLayer_tags(`

### TestAcc and uppercase after first underscore
Count: 1843
[List matches](./results/capT-TestAcc-uppAfterUnderscore.txt)

Example: `func TestAccAWSSecurityGroup_CIDRandGroups(`

## Lowercase-t test Functions

### All
Count: 7922
[List matches](./results/lowT-test.txt)

Example: `func testAccMskClusterConfigEncryptionInfoEncryptionInTransitClientBroker(`

### testAcc
Count: 7619
[List matches](./results/lowT-testAcc.txt)

Example: `func testAccAWSRedshiftClusterConfig_updatedTags(`

### testAccAWS
Count: 3321
[List matches](./results/lowT-testAcc-allCapAWS.txt)

Example: `func testAccAWSLBListenerRuleConfig_conditionHttpHeader_invalid(`

### testAccAws
Count: 712
[List matches](./results/lowT-testAcc-iniCapAws.txt)

Example: `func testAccAwsEc2ClientVpnNetworkAssociation_disappears(`

### testAcc functions with lowercase after first underscore
Count: 1501
[List matches](./results/lowT-testAcc-lowAfterUnderscore.txt)

Example: `func testAccAWSCloudTrail_basic(`

### testAcc functions with uppercase after first underscore
Count: 961
[List matches](./results/lowT-testAcc-uppAfterUnderscore.txt)

Example: `func testAccAWSS3BucketOwnershipControlsConfig_Rule_ObjectOwnership(`

### testAcc functions with config (any case)
Count: 4906
[List matches](./results/lowT-testAcc-anyConfigAnywhere.txt)

Example: `func testAccCheckAwsAvailabilityZonesConfigFilter(`

### testAcc functions returning strings
Count: 5132
[List matches](./results/lowT-testAcc-returnStrings.txt)

Example: `func testAccAWSCodeArtifactDomainPermissionsPolicyUpdatedConfig(rName string) string {`

### testAcc functions with config (any case) and returning strings
Count: 4720
[List matches](./results/lowT-testAcc-anyConfigAnywhereReturnStrings.txt)

Example: `func testAccAWSDataSyncTaskConfigTags2(rName, key1, value1, key2, value2 string) string {`

### testAcc functions with config (any case) and returning strings without underscores
Count: 2736
[List matches](./results/lowT-testAcc-anyConfigAnywhereReturnStringsNoUnderscore.txt)

Example: `func testAccBackupVaultPolicyConfigUpdated(rName string) string {`

## Any case-t Test Functions

### All
Count: 13156
[List matches](./results/anyT-Test.txt)

Example: `func testAccAWSGlueWorkflowConfigMaxConcurrentRuns(`

### TestAcc
Count: 12495
[List matches](./results/anyT-TestAcc.txt)

Example: `func TestAccAWSIoTTopicRule_firehose(`

### TestAcc with lowercase after first underscore
Count: 4533
[List matches](./results/anyT-TestAcc-lowAfterUnderscore.txt)

Example: `func testAccAWSCognitoIdentityPoolConfig_cognitoIdentityProviders(`

### TestAcc with uppercase after first underscore
Count: 2804
[List matches](./results/anyT-TestAcc-capAfterUnderscore.txt)

Example: `func TestAccAWSProvider_Region_AwsGovCloudUs(`

### TestAcc with only one underscore
Count: 5679
[List matches](./results/anyT-TestAcc-onlyOneUnderscore.txt)

Example: `func testAccESDomainConfig_WithDedicatedClusterMaster(`

### TestAcc with camel case after first underscore
Count: 1977
[List matches](./results/anyT-TestAcc-camelcase.txt)

Example: `func TestAccAWSLambdaPermission_withS3(`

### TestAcc with multiple underscores
Count: 1659
[List matches](./results/anyT-TestAcc-multipleUnderscores.txt)

Example: `func testAccAWSEc2FleetConfig_LaunchTemplateConfig_Override_Priority_Multiple(`

## Test Constants

### All
Count: 435
[List matches](./results/const-anyT-Test.txt)

Example: `const testAccAWSDefaultNetworkConfig_Subnets =`

### TestAcc (any case)
Count: 426
[List matches](./results/const-anyT-TestAcc.txt)

Example: `const testAccDBSubnetGroupConfig_namePrefix =`

### testAcc (lowercase)
Count: 426
[List matches](./results/const-lowT-testAcc.txt)

Example: `const testAccAWSEFSFileSystemConfigWithPerformanceMode =`

### TestAcc (any case) with lowercase after first underscore
Count: 131
[List matches](./results/const-anyT-TestAcc-underscoreLower.txt)

Example: `const testAccGuardDutyDetectorConfig_basic4 =`

### TestAcc (any case) with uppercase after first underscore
Count: 61
[List matches](./results/const-anyT-TestAcc-underscoreUpper.txt)

Example: `const testAccAWSTransferServerConfig_VpcUpdate =`

### TestAcc (any case) with camel case after underscore
Count: 58
[List matches](./results/const-anyT-TestAcc-underscoreCamelcase.txt)

Example: `const testAccDataSourceAwsPrefixListConfig_nameDoesNotOverrideFilter =`

### TestAcc (any case) with only one underscore
Count: 163
[List matches](./results/const-anyT-TestAcc-onlyOneUnderscore.txt)

Example: `const testAccDataSourceAwsSecretsManagerSecretRotationConfig_NonExistent =`

### TestAcc (any case) with multiple underscores
Count: 29
[List matches](./results/const-anyT-TestAcc-multipleUnderscores.txt)

Example: `const testAccAWSDBClusterParameterGroupConfig_generatedName_Parameter =`

### TestAcc (any case) with config (any case)
Count: 369
[List matches](./results/const-anyT-TestAcc-anyConfigAnywhere.txt)

Example: `const testAccVpcEndpointSubnetAssociationConfig_basic =`

### TestAcc (any case) with config (any case) and no underscores
Count: 192
[List matches](./results/const-anyT-TestAcc-anyConfigAnywhereNoUnderscores.txt)

Example: `const testAccAWSSecurityGroupConfig =`

### TestAcc (any case) with underscore anywhere after config (any case)
Count: 175
[List matches](./results/const-anyT-TestAcc-underscoreAfterAnyConfig.txt)

Example: `const testAccAWSTransferServerConfig_VpcDefault =`

## Resource Functions

### Resource
Count: 3522
[List matches](./results/resource-functions-resource.txt)

Example: `func resourceAwsElasticacheGlobalReplicationGroupDelete(`

### Resource Multi Caps
Count: 217
[List matches](./results/resource-functions-resource-multicap.txt)

Example: `func resourceAwsWafRegionalIPSet(`

### Non-test
Count: 5972
[List matches](./results/resource-functions-non-test.txt)

Example: `func unprocessedScramSecretsError(`

### Non-test Multi-caps
Count: 458
[List matches](./results/resource-functions-non-test-multicap.txt)

Example: `func resourceAwsIamOpenIDConnectProviderDelete(`

### Non-test, non-resource
Count: 2494
[List matches](./results/resource-functions-non-test-non-resource.txt)

Example: `func addIamManagedPolicies(`

## Function Capitalization

### acl
Count: 7
[List matches](./results/Function-Capitalization-acl.txt)

Example: `func TestAccAWSDBInstance_EnabledCloudwatchLogsExports_Oracle(`

### Acl
Count: 187
[List matches](./results/Function-Capitalization-Acl.txt)

Example: `func testAccCheckWafRegionalWebAclAssociationDisappears(`

### ACL
Count: 95
[List matches](./results/Function-Capitalization-ACL.txt)

Example: `func testAccAwsWafv2WebACLAssociationConfig(`

### ami
Count: 18
[List matches](./results/Function-Capitalization-ami.txt)

Example: `func amiDescriptionAttributes(`

### Ami
Count: 81
[List matches](./results/Function-Capitalization-Ami.txt)

Example: `func testAccAwsImageBuilderDistributionConfigurationConfigDistributionAmiDistributionConfigurationKmsKeyId2(`

### AMI
Count: 54
[List matches](./results/Function-Capitalization-AMI.txt)

Example: `func testAccAWSAMICopyConfigBase(`

### api
Count: 23
[List matches](./results/Function-Capitalization-api.txt)

Example: `func TestAccAWSAPIGatewayUsagePlan_apiStages(`

### Api
Count: 486
[List matches](./results/Function-Capitalization-Api.txt)

Example: `func resourceAwsApiGatewayDocumentationVersionRead(`

### API
Count: 605
[List matches](./results/Function-Capitalization-API.txt)

Example: `func testAccAWSAPIGatewayV2IntegrationConfig_dataMappingHttpUpdated(`

### arn
Count: 3
[List matches](./results/Function-Capitalization-arn.txt)

Example: `func TestCloudFrontStructure_expandViewerCertificate_acm_certificate_arn(`

### Arn
Count: 185
[List matches](./results/Function-Capitalization-Arn.txt)

Example: `func TestLambdaPermissionGetFunctionNameFromLambdaArn_valid(`

### ARN
Count: 54
[List matches](./results/Function-Capitalization-ARN.txt)

Example: `func testAccCheckResourceAttrRegionalARNIgnoreRegionAndAccount(`

### asg
Count: 5
[List matches](./results/Function-Capitalization-asg.txt)

Example: `func test_config_blue_green_deployment_config_create_with_asg(`

### Asg
Count: 5
[List matches](./results/Function-Capitalization-Asg.txt)

Example: `func flattenBeanstalkAsg(`

### ASG
Count: 16
[List matches](./results/Function-Capitalization-ASG.txt)

Example: `func testAccASGNotificationConfig_update(`

### aws
Count: 8
[List matches](./results/Function-Capitalization-aws.txt)

Example: `func awsElasticTranscoderNotifications_update(`

### Aws
Count: 6183
[List matches](./results/Function-Capitalization-Aws.txt)

Example: `func dataSourceAwsBatchJobQueue(`

### AWS
Count: 8823
[List matches](./results/Function-Capitalization-AWS.txt)

Example: `func TestAccAWSLB_applicationLoadBalancer_updateDeletionProtection(`

### cidr
Count: 1
[List matches](./results/Function-Capitalization-cidr.txt)

Example: `func cidrBlocksEqual(`

### Cidr
Count: 61
[List matches](./results/Function-Capitalization-Cidr.txt)

Example: `func TestAccAWSRoute_TransitGatewayID_DestinationCidrBlock(`

### CIDR
Count: 18
[List matches](./results/Function-Capitalization-CIDR.txt)

Example: `func suppressEqualCIDRBlockDiffs(`

### cors
Count: 5
[List matches](./results/Function-Capitalization-cors.txt)

Example: `func testAccAWSAPIGatewayV2ApiConfig_corsConfigurationUpdated(`

### Cors
Count: 9
[List matches](./results/Function-Capitalization-Cors.txt)

Example: `func TestAccAWSS3Bucket_Cors_EmptyOrigin(`

### CORS
Count: 2
[List matches](./results/Function-Capitalization-CORS.txt)

Example: `func testAccAWSS3BucketConfigWithCORS(`

### db
Count: 68
[List matches](./results/Function-Capitalization-db.txt)

Example: `func testAccDynamoDbGlobalTableConfig_multipleRegions_dynamodb_tables(`

### Db
Count: 438
[List matches](./results/Function-Capitalization-Db.txt)

Example: `func testAccAWSRdsOrderableDbInstanceDataSourceConfig_basic(`

### DB
Count: 553
[List matches](./results/Function-Capitalization-DB.txt)

Example: `func testAccCheckAWSDBEventSubscriptionExists(`

### dms
Count: 31
[List matches](./results/Function-Capitalization-dms.txt)

Example: `func dmsCertificateDestroy(`

### Dms
Count: 122
[List matches](./results/Function-Capitalization-Dms.txt)

Example: `func resourceAwsDmsReplicationTaskStateRefreshFunc(`

### DMS
Count: 0
### dns
Count: 13
[List matches](./results/Function-Capitalization-dns.txt)

Example: `func TestAccAWSAcmCertificateValidation_validationRecordFqdnsWildcard(`

### Dns
Count: 68
[List matches](./results/Function-Capitalization-Dns.txt)

Example: `func testAccServiceDiscoveryPublicDnsNamespaceConfigDescription(`

### DNS
Count: 8
[List matches](./results/Function-Capitalization-DNS.txt)

Example: `func testAccGetPartitionReverseDNSPrefix(`

### ec2
Count: 30
[List matches](./results/Function-Capitalization-ec2.txt)

Example: `func ec2CustomFiltersSchema(`

### Ec2
Count: 756
[List matches](./results/Function-Capitalization-Ec2.txt)

Example: `func TestAccAWSEc2TransitGatewayVpcAttachmentAccepter_Tags(`

### EC2
Count: 24
[List matches](./results/Function-Capitalization-EC2.txt)

Example: `func testAccAWSBatchComputeEnvironmentConfigEC2WithTags(`

### ecs
Count: 12
[List matches](./results/Function-Capitalization-ecs.txt)

Example: `func testAccAWSSagemakerAppImageConfigKernelGatewayImageConfigKernalSpecs2(`

### Ecs
Count: 262
[List matches](./results/Function-Capitalization-Ecs.txt)

Example: `func testAccAWSEcsServiceWithDaemonSchedulingStrategySetDeploymentMinimum(`

### ECS
Count: 4
[List matches](./results/Function-Capitalization-ECS.txt)

Example: `func TestAccAWSCodeDeployApp_computePlatform_ECS(`

### efs
Count: 1
[List matches](./results/Function-Capitalization-efs.txt)

Example: `func testAccCheckAWSSNSSMSPrefsDestroy(`

### Efs
Count: 78
[List matches](./results/Function-Capitalization-Efs.txt)

Example: `func testAccCheckAWSDataSyncLocationEfsDisappears(`

### EFS
Count: 62
[List matches](./results/Function-Capitalization-EFS.txt)

Example: `func testAccAWSEcsTaskDefinitionWithEFSAccessPoint(`

### eip
Count: 52
[List matches](./results/Function-Capitalization-eip.txt)

Example: `func TestAccAWSSESReceiptFilter_disappears(`

### Eip
Count: 15
[List matches](./results/Function-Capitalization-Eip.txt)

Example: `func resourceAwsEipDomain(`

### EIP
Count: 67
[List matches](./results/Function-Capitalization-EIP.txt)

Example: `func TestAccAWSEIP_twoEIPsOneNetworkInterface(`

### eks
Count: 0
### Eks
Count: 156
[List matches](./results/Function-Capitalization-Eks.txt)

Example: `func resourceAwsEksFargateProfileUpdate(`

### EKS
Count: 0
### elb
Count: 4
[List matches](./results/Function-Capitalization-elb.txt)

Example: `func testAccAWSAutoscalingAttachment_elb(`

### Elb
Count: 37
[List matches](./results/Function-Capitalization-Elb.txt)

Example: `func resourceAwsElbAttachment(`

### ELB
Count: 60
[List matches](./results/Function-Capitalization-ELB.txt)

Example: `func TestResourceAWSELB_validateElbNameCanBeAnEmptyString(`

### eni
Count: 6
[List matches](./results/Function-Capitalization-eni.txt)

Example: `func testAccAWSCognitoIdentityPoolConfig_openidConnectProviderArnsModified(`

### Eni
Count: 2
[List matches](./results/Function-Capitalization-Eni.txt)

Example: `func resourceAwsEniAttachmentHash(`

### ENI
Count: 33
[List matches](./results/Function-Capitalization-ENI.txt)

Example: `func testAccAWSENIIPV6ConfigBase(`

### iam
Count: 19
[List matches](./results/Function-Capitalization-iam.txt)

Example: `func TestAccAWSNeptuneCluster_iamAuth(`

### Iam
Count: 208
[List matches](./results/Function-Capitalization-Iam.txt)

Example: `func resourceAwsIamGroupMembership(`

### IAM
Count: 249
[List matches](./results/Function-Capitalization-IAM.txt)

Example: `func testAccCheckAWSIAMPolicyDisappears(`

### id
Count: 35
[List matches](./results/Function-Capitalization-id.txt)

Example: `func TestAccAWSDataSourceIAMPolicyDocument_duplicateSid(`

### Id
Count: 451
[List matches](./results/Function-Capitalization-Id.txt)

Example: `func TestParseRecordId(`

### ID
Count: 222
[List matches](./results/Function-Capitalization-ID.txt)

Example: `func testAccAwsServerlessApplicationRepositoryCloudFormationApplicationID(`

### iot
Count: 4
[List matches](./results/Function-Capitalization-iot.txt)

Example: `func testAccAWSIoTTopicRule_iot_events(`

### Iot
Count: 142
[List matches](./results/Function-Capitalization-Iot.txt)

Example: `func resourceAwsIotRoleAliasCreate(`

### IOT
Count: 4
[List matches](./results/Function-Capitalization-IOT.txt)

Example: `func TestAccAWSIotEndpointDataSource_EndpointType_IOTDataATS(`

### ip
Count: 1100
[List matches](./results/Function-Capitalization-ip.txt)

Example: `func TestAccAWSDmsEventSubscription_Enabled(`

### Ip
Count: 206
[List matches](./results/Function-Capitalization-Ip.txt)

Example: `func testAccAWSRouteTableConfigRouteIpv4LocalGateway(`

### IP
Count: 241
[List matches](./results/Function-Capitalization-IP.txt)

Example: `func testAccDataSourceAwsNetworkInterfaceConfigPublicIPAssociation(`

### json
Count: 1
[List matches](./results/Function-Capitalization-json.txt)

Example: `func jsonBytesEqual(`

### Json
Count: 42
[List matches](./results/Function-Capitalization-Json.txt)

Example: `func expandGlueJsonClassifierCreate(`

### JSON
Count: 10
[List matches](./results/Function-Capitalization-JSON.txt)

Example: `func testAccAWSIAMPolicyDocumentExpectedJSONStatementPrincipalIdentifiersMultiplePrincipalsGov(`

### kms
Count: 32
[List matches](./results/Function-Capitalization-kms.txt)

Example: `func TestAccAWSRedshiftCluster_kmsKey(`

### Kms
Count: 235
[List matches](./results/Function-Capitalization-Kms.txt)

Example: `func TestAccAWSKmsExternalKey_ValidTo(`

### KMS
Count: 26
[List matches](./results/Function-Capitalization-KMS.txt)

Example: `func TestAccAWSStorageGatewayNfsFileShare_KMSEncrypted(`

### mfa
Count: 0
### Mfa
Count: 11
[List matches](./results/Function-Capitalization-Mfa.txt)

Example: `func flattenCognitoSoftwareTokenMfaConfiguration(`

### MFA
Count: 4
[List matches](./results/Function-Capitalization-MFA.txt)

Example: `func TestAccAWSUser_ForceDestroy_MFADevice(`

### nat
Count: 185
[List matches](./results/Function-Capitalization-nat.txt)

Example: `func testAccCheckAWSCloudwatchLogDestinationPolicyDestroy(`

### Nat
Count: 22
[List matches](./results/Function-Capitalization-Nat.txt)

Example: `func testAccAWSElasticacheReplicationGroupNativeRedisClusterConfig(`

### NAT
Count: 0
### ram
Count: 384
[List matches](./results/Function-Capitalization-ram.txt)

Example: `func testAccCheckAWSRedshiftParameterGroupExists(`

### Ram
Count: 68
[List matches](./results/Function-Capitalization-Ram.txt)

Example: `func testAccCheckAwsRamPrincipalAssociationExists(`

### RAM
Count: 1
[List matches](./results/Function-Capitalization-RAM.txt)

Example: `func buildRAMTagFilters(`

### rds
Count: 41
[List matches](./results/Function-Capitalization-rds.txt)

Example: `func TestAccDataSourceAWSLB_BackwardsCompatibility(`

### Rds
Count: 91
[List matches](./results/Function-Capitalization-Rds.txt)

Example: `func waitForRdsGlobalClusterRemoval(`

### RDS
Count: 160
[List matches](./results/Function-Capitalization-RDS.txt)

Example: `func testAccAWSRDSClusterConfig_ScalingConfiguration(`

### sms
Count: 0
### Sms
Count: 28
[List matches](./results/Function-Capitalization-Sms.txt)

Example: `func TestValidateCognitoUserPoolSmsVerificationMessage(`

### SMS
Count: 15
[List matches](./results/Function-Capitalization-SMS.txt)

Example: `func resourceAwsPinpointSMSChannelRead(`

### sqs
Count: 9
[List matches](./results/Function-Capitalization-sqs.txt)

Example: `func testAccAWSLambdaEventSourceMappingConfigUpdate_sqs(`

### Sqs
Count: 31
[List matches](./results/Function-Capitalization-Sqs.txt)

Example: `func resourceAwsSqsQueuePolicyUpsert(`

### SQS
Count: 41
[List matches](./results/Function-Capitalization-SQS.txt)

Example: `func validateSQSQueueName(`

### sse
Count: 54
[List matches](./results/Function-Capitalization-sse.txt)

Example: `func resourceAwsInspectorAssessmentTemplateCreate(`

### Sse
Count: 5
[List matches](./results/Function-Capitalization-Sse.txt)

Example: `func sourceSseKmsObjectsHash(`

### SSE
Count: 73
[List matches](./results/Function-Capitalization-SSE.txt)

Example: `func testAccAWSSESEventDestinationConfig(`

### ssl
Count: 0
### Ssl
Count: 4
[List matches](./results/Function-Capitalization-Ssl.txt)

Example: `func resourceAwsOpsworksApplicationSsl(`

### SSL
Count: 16
[List matches](./results/Function-Capitalization-SSL.txt)

Example: `func TestAccAWSCodeBuildProject_Source_InsecureSSL(`

### tcp
Count: 8
[List matches](./results/Function-Capitalization-tcp.txt)

Example: `func testAccAppmeshRouteConfig_tcpRouteUpdated(`

### Tcp
Count: 6
[List matches](./results/Function-Capitalization-Tcp.txt)

Example: `func expandAppmeshTcpRoute(`

### TCP
Count: 10
[List matches](./results/Function-Capitalization-TCP.txt)

Example: `func TestAccAWSLBTargetGroup_TCP_HTTPHealthCheck(`

### url
Count: 0
### Url
Count: 14
[List matches](./results/Function-Capitalization-Url.txt)

Example: `func testAccAWSCloudFormationStackConfig_templateUrl_withParams_withYaml(`

### URL
Count: 6
[List matches](./results/Function-Capitalization-URL.txt)

Example: `func validateCognitoUserPoolClientURL(`

### vpc
Count: 41
[List matches](./results/Function-Capitalization-vpc.txt)

Example: `func testAccAWSS3AccessPointConfig_vpc(`

### Vpc
Count: 546
[List matches](./results/Function-Capitalization-Vpc.txt)

Example: `func testAccAWSRDSClusterConfig_SnapshotIdentifier_VpcSecurityGroupIds_Tags(`

### VPC
Count: 101
[List matches](./results/Function-Capitalization-VPC.txt)

Example: `func TestAccAWSVPCPeeringConnectionAccepter_sameRegionDifferentAccount(`

### vpn
Count: 6
[List matches](./results/Function-Capitalization-vpn.txt)

Example: `func testAccDxGatewayAssociationProposalConfigBase_vpnGateway(`

### Vpn
Count: 199
[List matches](./results/Function-Capitalization-Vpn.txt)

Example: `func resourceAwsEc2ClientVpnAuthorizationRuleImport(`

### VPN
Count: 3
[List matches](./results/Function-Capitalization-VPN.txt)

Example: `func TestAccAWSVPNGatewayRoutePropagation_basic(`

### waf
Count: 22
[List matches](./results/Function-Capitalization-waf.txt)

Example: `func wafv2StatementSchema(`

### Waf
Count: 841
[List matches](./results/Function-Capitalization-Waf.txt)

Example: `func TestAccAWSWafRateBasedRule_disappears(`

### WAF
Count: 8
[List matches](./results/Function-Capitalization-WAF.txt)

Example: `func flattenWAFLoggingConfiguration(`




[AWS EC2 Instance Types/Prices](https://github.com/YakDriver/aws-ec2-instance-types)
