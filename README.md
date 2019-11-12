# terraform-test-conventions

What is the current state of naming conventions in Terraform AWS provider acceptance tests? I dunno. This repo performs analysis and rebuilds daily. Take a look below :point_down:. Or, in other words, Good ol' fashioned Perl and RegExes gone awry.
## Capital-T Test Functions

### All
Count: 3542

[List matches](./results/capT-Test.txt)

Example: `func TestAccAWSS3Account(`

### TestAcc
Count: 3110

[List matches](./results/capT-TestAcc.txt)

Example: `func TestAccAWSGlueJob_MaxRetries(`

### TestAccAWS
Count: 2810

[List matches](./results/capT-TestAcc-allCapAWS.txt)

Example: `func TestAccAWSIAMPolicyAttachment_Roles_RenamedRole(`

### TestAccAws
Count: 137

[List matches](./results/capT-TestAcc-iniCapAws.txt)

Example: `func TestAccAwsRoute53ResolverRule_updateName(`

### TestAcc and lowercase after first underscore
Count: 1993

[List matches](./results/capT-TestAcc-lowAfterUnderscore.txt)

Example: `func TestAccDataSourceAwsNetworkInterface_filters(`

### TestAcc and uppercase after first underscore
Count: 1065

[List matches](./results/capT-TestAcc-uppAfterUnderscore.txt)

Example: `func TestAccAWSNetworkAcl_Ingress_ConfigMode(`

## Lowercase-t test Functions

### All
Count: 4900

[List matches](./results/lowT-test.txt)

Example: `func testAccAWSPinpointBaiduChannelConfig_update(`

### testAcc
Count: 4728

[List matches](./results/lowT-testAcc.txt)

Example: `func testAccAWSLightsailInstanceConfig_tags2(`

### testAccAWS
Count: 2046

[List matches](./results/lowT-testAcc-allCapAWS.txt)

Example: `func testAccAWSStorageGateway_SmbFileShare_ActiveDirectoryBase(`

### testAccAws
Count: 238

[List matches](./results/lowT-testAcc-iniCapAws.txt)

Example: `func testAccAwsFsxWindowsFileSystemConfigSubnetIds1(`

### testAcc functions with lowercase after first underscore
Count: 925

[List matches](./results/lowT-testAcc-lowAfterUnderscore.txt)

Example: `func testAccAWSCloudWatchLogGroupConfig_withRetention(`

### testAcc functions with uppercase after first underscore
Count: 608

[List matches](./results/lowT-testAcc-uppAfterUnderscore.txt)

Example: `func testAccAWSDBInstanceConfig_ReplicateSourceDb_VpcSecurityGroupIds(`

### testAcc functions with config (any case)
Count: 2763

[List matches](./results/lowT-testAcc-anyConfigAnywhere.txt)

Example: `func testAccMskClusterConfigNumberOfBrokerNodes(`

### testAcc functions returning strings
Count: 2900

[List matches](./results/lowT-testAcc-returnStrings.txt)

Example: `func testAccAWSS3BucketPolicyConfig(bucketName string) string {`

### testAcc functions with config (any case) and returning strings
Count: 2624

[List matches](./results/lowT-testAcc-anyConfigAnywhereReturnStrings.txt)

Example: `func testAccAWSSpotFleetRequestConfigWithoutSpotPrice(rName string, rInt int) string {`

### testAcc functions with config (any case) and returning strings without underscores
Count: 1382

[List matches](./results/lowT-testAcc-anyConfigAnywhereReturnStringsNoUnderscore.txt)

Example: `func testAccAWSCloudFormationStackSetConfigExecutionRoleName(rName, executionRoleName string) string {`

## Any case-t Test Functions

### All
Count: 8442

[List matches](./results/anyT-Test.txt)

Example: `func testAccAWSSSMPatchBaselineBasicConfigUpdated(`

### TestAcc
Count: 7838

[List matches](./results/anyT-TestAcc.txt)

Example: `func TestAccAWSAppautoScalingPolicy_multiplePoliciesSameName(`

### TestAcc with lowercase after first underscore
Count: 2918

[List matches](./results/anyT-TestAcc-lowAfterUnderscore.txt)

Example: `func TestAccAWSLambdaPermission_basic(`

### TestAcc with uppercase after first underscore
Count: 1673

[List matches](./results/anyT-TestAcc-capAfterUnderscore.txt)

Example: `func TestAccAWSProvider_IgnoreTagPrefixes_One(`

### TestAcc with only one underscore
Count: 3615

[List matches](./results/anyT-TestAcc-onlyOneUnderscore.txt)

Example: `func TestAccAWSWafRule_Tags(`

### TestAcc with camel case after first underscore
Count: 1362

[List matches](./results/anyT-TestAcc-camelcase.txt)

Example: `func TestAccAWSSubnet_ignoreTags(`

### TestAcc with multiple underscores
Count: 976

[List matches](./results/anyT-TestAcc-multipleUnderscores.txt)

Example: `func TestAccAWSS3Bucket_disableDefaultEncryption_whenDefaultEncryptionIsEnabled(`

## Test Constants

### All
Count: 565

[List matches](./results/const-anyT-Test.txt)

Example: `const testAccVpnGatewayConfigChangeVPC =`

### TestAcc (any case)
Count: 556

[List matches](./results/const-anyT-TestAcc.txt)

Example: `const testAccAWSENIConfigUpdatedDescription =`

### testAcc (lowercase)
Count: 556

[List matches](./results/const-lowT-testAcc.txt)

Example: `const testAccCheckInternetGatewayConfigTagsUpdate =`

### TestAcc (any case) with lowercase after first underscore
Count: 172

[List matches](./results/const-anyT-TestAcc-underscoreLower.txt)

Example: `const testAccAwsSESIdentityNotificationTopicConfig_headers =`

### TestAcc (any case) with uppercase after first underscore
Count: 53

[List matches](./results/const-anyT-TestAcc-underscoreUpper.txt)

Example: `const testAccInstanceConfigForceNewAndTagsDrift_Update =`

### TestAcc (any case) with camel case after underscore
Count: 78

[List matches](./results/const-anyT-TestAcc-underscoreCamelcase.txt)

Example: `const testAccAWSAutoScalingGroupConfig_terminationPoliciesEmpty =`

### TestAcc (any case) with only one underscore
Count: 181

[List matches](./results/const-anyT-TestAcc-onlyOneUnderscore.txt)

Example: `const testAccAWSALBTargetGroupConfig_namePrefix =`

### TestAcc (any case) with multiple underscores
Count: 44

[List matches](./results/const-anyT-TestAcc-multipleUnderscores.txt)

Example: `const testAccAWSAutoScalingGroupConfig_ALB_TargetGroup_pre =`

### TestAcc (any case) with config (any case)
Count: 497

[List matches](./results/const-anyT-TestAcc-anyConfigAnywhere.txt)

Example: `const testAccDataSourceAwsCanonicalUserIdConfig =`

### TestAcc (any case) with config (any case) and no underscores
Count: 293

[List matches](./results/const-anyT-TestAcc-anyConfigAnywhereNoUnderscores.txt)

Example: `const testAccAwsOrganizationsOrganizationConfig =`

### TestAcc (any case) with underscore anywhere after config (any case)
Count: 202

[List matches](./results/const-anyT-TestAcc-underscoreAfterAnyConfig.txt)

Example: `const testAccInstanceDataSourceConfig_VPC =`

