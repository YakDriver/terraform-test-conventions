# terraform-test-conventions

What is the current state of naming conventions in Terraform AWS provider acceptance tests? I dunno. This repo performs analysis and rebuilds daily. Take a look below :point_down:. Or, in other words, Good ol' fashioned Perl and RegExes gone awry.
## Capital-T Test Functions

### All
Count: 3618

[List matches](./results/capT-Test.txt)

Example: `func TestAccAWSVpc_classiclinkOptionSet(`

### TestAcc
Count: 3262

[List matches](./results/capT-TestAcc.txt)

Example: `func TestAccAWSEMRCluster_Step_ConfigMode(`

### TestAccAWS
Count: 2954

[List matches](./results/capT-TestAcc-allCapAWS.txt)

Example: `func TestAccAWSIAMPolicyAttachment_Groups_RenamedGroup(`

### TestAccAws
Count: 143

[List matches](./results/capT-TestAcc-iniCapAws.txt)

Example: `func TestAccAwsAppsyncDatasource_HTTPConfig_Endpoint(`

### TestAcc and lowercase after first underscore
Count: 2065

[List matches](./results/capT-TestAcc-lowAfterUnderscore.txt)

Example: `func TestAccAWSWafRegionalWebAcl_changeNameForceNew(`

### TestAcc and uppercase after first underscore
Count: 1144

[List matches](./results/capT-TestAcc-uppAfterUnderscore.txt)

Example: `func TestAccAWSEc2TransitGatewayVpcAttachment_Ipv6Support(`

## Lowercase-t test Functions

### All
Count: 5214

[List matches](./results/lowT-test.txt)

Example: `func testAccCheckAWSEcsServiceDestroy(`

### testAcc
Count: 5037

[List matches](./results/lowT-testAcc.txt)

Example: `func testAccCheckAWSRedshiftParameterGroupExists(`

### testAccAWS
Count: 2237

[List matches](./results/lowT-testAcc-allCapAWS.txt)

Example: `func testAccAWSEcsClusterCapacityProviders(`

### testAccAws
Count: 257

[List matches](./results/lowT-testAcc-iniCapAws.txt)

Example: `func testAccAwsSecretsManagerSecretConfig_RotationLambdaARN(`

### testAcc functions with lowercase after first underscore
Count: 978

[List matches](./results/lowT-testAcc-lowAfterUnderscore.txt)

Example: `func testAccAWSKmsGrant_bare(`

### testAcc functions with uppercase after first underscore
Count: 637

[List matches](./results/lowT-testAcc-uppAfterUnderscore.txt)

Example: `func testAccConfigOrganizationManagedRule_TagKeyScope(`

### testAcc functions with config (any case)
Count: 3007

[List matches](./results/lowT-testAcc-anyConfigAnywhere.txt)

Example: `func testAccAWSCognitoIdentityPoolRolesAttachmentConfig_roleMappingsWithRulesTypeError(`

### testAcc functions returning strings
Count: 3154

[List matches](./results/lowT-testAcc-returnStrings.txt)

Example: `func testAccAWSSSMMaintenanceWindowTaskLambdaConfig(funcName, policyName, roleName, sgName, rName string, rInt int) string {`

### testAcc functions with config (any case) and returning strings
Count: 2862

[List matches](./results/lowT-testAcc-anyConfigAnywhereReturnStrings.txt)

Example: `func testAccDataSourceAWSMqBrokerConfig_base(brokerName, prefix string) string {`

### testAcc functions with config (any case) and returning strings without underscores
Count: 1546

[List matches](./results/lowT-testAcc-anyConfigAnywhereReturnStringsNoUnderscore.txt)

Example: `func testAccConfigOrganizationCustomRuleConfigLambdaFunctionArn2(rName string) string {`

## Any case-t Test Functions

### All
Count: 8832

[List matches](./results/anyT-Test.txt)

Example: `func TestAccAWSCodeDeployDeploymentGroup_autoRollbackConfiguration_create(`

### TestAcc
Count: 8299

[List matches](./results/anyT-TestAcc.txt)

Example: `func TestAccAWSRouteTable_ipv6(`

### TestAcc with lowercase after first underscore
Count: 3043

[List matches](./results/anyT-TestAcc-lowAfterUnderscore.txt)

Example: `func TestAccAWSBeanstalkEnv_outputs(`

### TestAcc with uppercase after first underscore
Count: 1781

[List matches](./results/anyT-TestAcc-capAfterUnderscore.txt)

Example: `func TestAccAWSLambdaFunction_DeadLetterConfig(`

### TestAcc with only one underscore
Count: 3780

[List matches](./results/anyT-TestAcc-onlyOneUnderscore.txt)

Example: `func testAccAWSDocDBClusterInstanceConfig_namePrefix(`

### TestAcc with camel case after first underscore
Count: 1406

[List matches](./results/anyT-TestAcc-camelcase.txt)

Example: `func TestAccAWSS3Bucket_generatedName(`

### TestAcc with multiple underscores
Count: 1044

[List matches](./results/anyT-TestAcc-multipleUnderscores.txt)

Example: `func testAccKinesisFirehoseDeliveryStreamConfig_ExtendedS3_DataFormatConversionConfiguration_HiveJsonSerDe_Empty(`

## Test Constants

### All
Count: 522

[List matches](./results/const-anyT-Test.txt)

Example: `const testAccAWSS3BucketConfig_generatedName =`

### TestAcc (any case)
Count: 513

[List matches](./results/const-anyT-TestAcc.txt)

Example: `const testAccAWSSecurityGroupConfigChange =`

### testAcc (lowercase)
Count: 513

[List matches](./results/const-lowT-testAcc.txt)

Example: `const testAccDataSourceAwsEipConfigPublicIpEc2Classic =`

### TestAcc (any case) with lowercase after first underscore
Count: 170

[List matches](./results/const-anyT-TestAcc-underscoreLower.txt)

Example: `const testAccAWSDocDBClusterParameterGroupConfig_generatedName =`

### TestAcc (any case) with uppercase after first underscore
Count: 51

[List matches](./results/const-anyT-TestAcc-underscoreUpper.txt)

Example: `const testAccDataSourceAwsDxGatewayConfig_NonExistent =`

### TestAcc (any case) with camel case after underscore
Count: 76

[List matches](./results/const-anyT-TestAcc-underscoreCamelcase.txt)

Example: `const testAccAWSSecurityGroupConfig_sourceSecurityGroup =`

### TestAcc (any case) with only one underscore
Count: 176

[List matches](./results/const-anyT-TestAcc-onlyOneUnderscore.txt)

Example: `const testAccAWSAPIGatewayClientCertificateConfig_basic =`

### TestAcc (any case) with multiple underscores
Count: 45

[List matches](./results/const-anyT-TestAcc-multipleUnderscores.txt)

Example: `const testAccAWSSecurityGroupConfig_ingressWithCidrAndSGs_classic =`

### TestAcc (any case) with config (any case)
Count: 454

[List matches](./results/const-anyT-TestAcc-anyConfigAnywhere.txt)

Example: `const testAccAWSPinpointEventStreamConfig_basic =`

### TestAcc (any case) with config (any case) and no underscores
Count: 254

[List matches](./results/const-anyT-TestAcc-anyConfigAnywhereNoUnderscores.txt)

Example: `const testAccAWSUserGroupMembershipConfigAddAll =`

### TestAcc (any case) with underscore anywhere after config (any case)
Count: 198

[List matches](./results/const-anyT-TestAcc-underscoreAfterAnyConfig.txt)

Example: `const testAccAWSPinpointEmailChannelConfig_basic =`

