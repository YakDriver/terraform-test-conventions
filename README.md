# terraform-test-conventions

What is the current state of naming conventions in Terraform AWS provider acceptance tests? I dunno. This repo performs analysis and rebuilds daily. Take a look below :point_down:. Or, in other words, Good ol' fashioned Perl and RegExes gone awry.
## Capital-T Test Functions

### All
Count: 3707

[List matches](./results/capT-Test.txt)

Example: `func TestAccAWSEcsDataSource_ecsCluster(`

### TestAcc
Count: 3359

[List matches](./results/capT-TestAcc.txt)

Example: `func TestAccAWSCloudwatchLogDestination_basic(`

### TestAccAWS
Count: 3041

[List matches](./results/capT-TestAcc-allCapAWS.txt)

Example: `func TestAccAWSAPIGatewayDocumentationVersion_allFields(`

### TestAccAws
Count: 143

[List matches](./results/capT-TestAcc-iniCapAws.txt)

Example: `func TestAccAwsServiceQuotasServiceQuotaDataSource_QuotaCode(`

### TestAcc and lowercase after first underscore
Count: 2123

[List matches](./results/capT-TestAcc-lowAfterUnderscore.txt)

Example: `func TestAccAWSSecurityGroup_ruleLimitCidrBlockExceededAppend(`

### TestAcc and uppercase after first underscore
Count: 1185

[List matches](./results/capT-TestAcc-uppAfterUnderscore.txt)

Example: `func TestAccAWSCloudFormationStackSet_Parameters_NoEcho(`

## Lowercase-t test Functions

### All
Count: 5403

[List matches](./results/lowT-test.txt)

Example: `func testAccAWSS3MultiBucketConfigWithTags(`

### testAcc
Count: 5211

[List matches](./results/lowT-testAcc.txt)

Example: `func testAccCheckAWSLBTargetGroupAttachmentDestroy(`

### testAccAWS
Count: 2327

[List matches](./results/lowT-testAcc-allCapAWS.txt)

Example: `func testAccAWSRouteTabAssocImportStateIdFunc(`

### testAccAws
Count: 266

[List matches](./results/lowT-testAcc-iniCapAws.txt)

Example: `func testAccAwsSESEmailIdentityConfig(`

### testAcc functions with lowercase after first underscore
Count: 1003

[List matches](./results/lowT-testAcc-lowAfterUnderscore.txt)

Example: `func testAccDxHostedTransitVirtualInterfaceConfig_basic(`

### testAcc functions with uppercase after first underscore
Count: 650

[List matches](./results/lowT-testAcc-uppAfterUnderscore.txt)

Example: `func testAccAWSCodeBuildProjectConfig_Cache(`

### testAcc functions with config (any case)
Count: 3132

[List matches](./results/lowT-testAcc-anyConfigAnywhere.txt)

Example: `func testAccAWSIamPolicyAttachmentConfigRolesRenamedRole(`

### testAcc functions returning strings
Count: 3281

[List matches](./results/lowT-testAcc-returnStrings.txt)

Example: `func testAccAWSCodeDeployAppConfigComputePlatform(rName string, computePlatform string) string {`

### testAcc functions with config (any case) and returning strings
Count: 2984

[List matches](./results/lowT-testAcc-anyConfigAnywhereReturnStrings.txt)

Example: `func testAccAWSRouteTableConfigRouteConfigModeNoBlocks() string {`

### testAcc functions with config (any case) and returning strings without underscores
Count: 1634

[List matches](./results/lowT-testAcc-anyConfigAnywhereReturnStringsNoUnderscore.txt)

Example: `func testAccAWSClusterConfigIncludingIamRoles(n int) string {`

## Any case-t Test Functions

### All
Count: 9110

[List matches](./results/anyT-Test.txt)

Example: `func testAccCheckDocDBSubnetGroupDestroy(`

### TestAcc
Count: 8570

[List matches](./results/anyT-TestAcc.txt)

Example: `func testAccAWSWafRegionalByteMatchSetConfigChangeByteMatchTuples(`

### TestAcc with lowercase after first underscore
Count: 3126

[List matches](./results/anyT-TestAcc-lowAfterUnderscore.txt)

Example: `func TestAccAWSRedshiftEventSubscription_withSourceIds(`

### TestAcc with uppercase after first underscore
Count: 1835

[List matches](./results/anyT-TestAcc-capAfterUnderscore.txt)

Example: `func testAccAWSElasticacheClusterConfig_EngineVersion_Memcached(`

### TestAcc with only one underscore
Count: 3895

[List matches](./results/anyT-TestAcc-onlyOneUnderscore.txt)

Example: `func TestAccAWSELBUpdate_HealthCheck(`

### TestAcc with camel case after first underscore
Count: 1442

[List matches](./results/anyT-TestAcc-camelcase.txt)

Example: `func TestAccAWSInstance_sourceDestCheck(`

### TestAcc with multiple underscores
Count: 1066

[List matches](./results/anyT-TestAcc-multipleUnderscores.txt)

Example: `func TestAccAWSKinesisAnalyticsApplication_Outputs_Lambda_Add(`

## Test Constants

### All
Count: 517

[List matches](./results/const-anyT-Test.txt)

Example: `const testAccAWSEIPConfig_PublicIpv4Pool_default =`

### TestAcc (any case)
Count: 508

[List matches](./results/const-anyT-TestAcc.txt)

Example: `const testAccSubnetConfigPreIpv6 =`

### testAcc (lowercase)
Count: 508

[List matches](./results/const-lowT-testAcc.txt)

Example: `const testAccFirehoseKinesisStreamSource =`

### TestAcc (any case) with lowercase after first underscore
Count: 170

[List matches](./results/const-anyT-TestAcc-underscoreLower.txt)

Example: `const testAccAWSELB_namePrefix =`

### TestAcc (any case) with uppercase after first underscore
Count: 51

[List matches](./results/const-anyT-TestAcc-underscoreUpper.txt)

Example: `const testAccAWSDefaultNetworkConfig_Subnets =`

### TestAcc (any case) with camel case after underscore
Count: 76

[List matches](./results/const-anyT-TestAcc-underscoreCamelcase.txt)

Example: `const testAccAWSSecurityGroupConfig_generatedName =`

### TestAcc (any case) with only one underscore
Count: 176

[List matches](./results/const-anyT-TestAcc-onlyOneUnderscore.txt)

Example: `const testAccLicenseManagerAssociationConfig_basic =`

### TestAcc (any case) with multiple underscores
Count: 45

[List matches](./results/const-anyT-TestAcc-multipleUnderscores.txt)

Example: `const testAccAWSEIPConfig_PublicIpv4Pool_default =`

### TestAcc (any case) with config (any case)
Count: 449

[List matches](./results/const-anyT-TestAcc-anyConfigAnywhere.txt)

Example: `const testAccCheckAwsOrganizationConfig =`

### TestAcc (any case) with config (any case) and no underscores
Count: 249

[List matches](./results/const-anyT-TestAcc-anyConfigAnywhereNoUnderscores.txt)

Example: `const testAccCheckAwsAmiDataSourceConfig =`

### TestAcc (any case) with underscore anywhere after config (any case)
Count: 198

[List matches](./results/const-anyT-TestAcc-underscoreAfterAnyConfig.txt)

Example: `const testAccAWSSecurityGroupConfig_rulesDropOnError_AddBadRule =`

