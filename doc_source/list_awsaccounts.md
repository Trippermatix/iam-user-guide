# Actions, Resources, and Condition Keys for AWS Accounts<a name="list_awsaccounts"></a>

AWS Accounts \(service prefix: `account`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/general/latest/gr/regions_manage.html)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/general/latest/gr/regions_manage.html)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/general/latest/gr/regions_manage.html) permission policies\.

**Topics**
+ [Actions Defined by AWS Accounts](#awsaccounts-actions-as-permissions)
+ [Resources Defined by Account](#awsaccounts-resources-for-iam-policies)
+ [Condition Keys for AWS Accounts](#awsaccounts-policy-keys)

## Actions Defined by AWS Accounts<a name="awsaccounts-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   DisableRegion  | Grants permission to disable a region | Write |  |   [ account:TargetRegion ](#awsaccounts-account_TargetRegion)   |  | 
|   EnableRegion  | Grants permission to enable a region | Write |  |   [ account:TargetRegion ](#awsaccounts-account_TargetRegion)   |  | 
|   ListRegions  | Grants permission to list regions | List |  |  |  | 

## Resources Defined by Account<a name="awsaccounts-resources-for-iam-policies"></a>

AWS Accounts has no service\-defined resources that can be used as the `Resource` element of an IAM policy statement\.

## Condition Keys for AWS Accounts<a name="awsaccounts-policy-keys"></a>

AWS Accounts defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   account:TargetRegion  | Filters access by a list of regions | String | 