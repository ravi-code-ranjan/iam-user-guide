# Actions, Resources, and Condition Keys for AWS Secrets Manager<a name="list_awssecretsmanager"></a>

AWS Secrets Manager \(service prefix: `secretsmanager`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/secretsmanager/latest/userguide/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/secretsmanager/latest/userguide/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/secretsmanager/latest/userguide/auth-and-access.html) permission policies\.

**Topics**
+ [Actions Defined by AWS Secrets Manager](#awssecretsmanager-actions-as-permissions)
+ [Resources Defined by Secrets Manager](#awssecretsmanager-resources-for-iam-policies)
+ [Condition Keys for AWS Secrets Manager](#awssecretsmanager-policy-keys)

## Actions Defined by AWS Secrets Manager<a name="awssecretsmanager-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_awssecretsmanager.html)

## Resources Defined by Secrets Manager<a name="awssecretsmanager-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#awssecretsmanager-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ Secret ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-resources)  |  arn:$\{Partition\}:secretsmanager:$\{Region\}:$\{Account\}:secret:$\{SecretId\}  |   [ secretsmanager:resource/AllowRotationLambdaArn ](#awssecretsmanager-secretsmanager_resource_AllowRotationLambdaArn)   | 

## Condition Keys for AWS Secrets Manager<a name="awssecretsmanager-policy-keys"></a>

AWS Secrets Manager defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   [ aws:RequestTag/tag\-key ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by a key that is present in the request the user makes to the Secrets Manager service\. | String | 
|   [ aws:TagKeys ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the list of all the tag key namespresent in the request the user makes to the Secrets Manager service\. | String | 
|   [ secretsmanager:Description ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the description text in the request\. | String | 
|   [ secretsmanager:ForceDeleteWithoutRecovery ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by whether the secret is to be deleted immediately without any recovery window\. | Boolean | 
|   [ secretsmanager:KmsKeyId ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the ARN of the KMS key in the request\. | String | 
|   [ secretsmanager:Name ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the friendly name of the secret in the request\. | String | 
|   [ secretsmanager:RecoveryWindowInDays ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the number of days that Secrets Manager waits before it can delete the secret\. | Long | 
|   [ secretsmanager:ResourceTag/tag\-key ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by a tag key and value pair\. | String | 
|   [ secretsmanager:RotationLambdaARN ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the ARN of the rotation Lambda function in the request\. | ARN | 
|   [ secretsmanager:SecretId ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the SecretID value in the request\. | ARN | 
|   [ secretsmanager:VersionId ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the unique identifier of the version of the secret in the request\. | String | 
|   [ secretsmanager:VersionStage ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the list of version stages in the request\. | String | 
|   [ secretsmanager:resource/AllowRotationLambdaArn ](https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the ARN of the rotation Lambda function associated with the secret\. | ARN | 