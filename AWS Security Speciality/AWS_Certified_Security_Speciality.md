# AWS Certified Security - Specialty Study Guide

## Introduction

This repository contains study materials and resources for the AWS Certified Security - Specialty exam. The content has been compiled from various AWS official sources and documentation during exam preparation.

## Table of Contents

- [Exam Overview](#exam-overview)
- [Domain 1: Infrastructure Security](#domain-1-infrastructure-security)
- [Domain 2: Security Logging and Monitoring](#domain-2-security-logging-and-monitoring)
- [Domain 3: Infrastructure Security](#domain-3-infrastructure-security)
- [Domain 4: Troubleshooting and Optimization](#domain-4-troubleshooting-and-optimization)
- [Domain 5: Infrastructure Security](#domain-5-infrastructure-security)
- [Domain 6: Management and Security Governance](#domain-6-management-and-security-governance)

## Exam Overview

- **Exam Duration**: 170 minutes
- **Number of Questions**: 65
- **Question Format**: Multiple choice, multiple answer
- **Passing Score**: 750/1000
- **Cost**: $300 USD

## Progress Tracking

- [ ] Domain 1 (30% of exam)
- [ ] Domain 2 (20% of exam)
- [ ] Domain 3 (20% of exam)
- [ ] Domain 4 (15% of exam)
- [ ] Domain 5 (10% of exam)
- [ ] Domain 6 (5% of exam)

## Domain 1: Infrastructure Security

Review these materials to learn more about the topics covered in this exam domain:

- [AWS Security and Incident Response Guide](https://docs.aws.amazon.com/whitepapers/latest/aws-security-incident-response-guide/introduction.html)

- [AWS Security Finding Format (ASFF)](https://docs.aws.amazon.com/securityhub/latest/userguide/securityhub-findings-format.html)

- [Required attributes](https://docs.aws.amazon.com/securityhub/latest/userguide/asff-required-attributes.html)

- [Playbooks](https://docs.aws.amazon.com/solutions/latest/automated-security-response-on-aws/playbooks-1.html)

- [Creating your own runbooks](https://docs.aws.amazon.com/systems-manager/latest/userguide/automation-documents.html)

- [Runbook](https://wa.aws.amazon.com/wellarchitected/2020-07-02T19-33-23/wat.concept.runbook.en.html)

- [What is AWS Systems Manager Incident Manager?](https://docs.aws.amazon.com/incident-manager/latest/userguide/what-is-incident-manager.html)

- [Working with Systems Manager Automation runbooks in Incident Manager](https://docs.aws.amazon.com/incident-manager/latest/userguide/runbooks.html)

- [How S3 Object Locks works](https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lock-overview.html)

- [CAPTCHA and Challenge actions in AWS WAF](https://docs.aws.amazon.com/waf/latest/developerguide/waf-captcha-and-challenge.html)

## Domain 2: Security Logging and Monitoring

### Key Concepts

- [ ] CloudWatch logs to an S3 bucket
  - [ ] logs:CreateLogDelivery
  - [ ] S3:PutBucketPolicy
  - [ ] S3:GetBucketPolicy
- [ ] AWS Network Firewall logs to Amazon Kinesis Data Firehose
  - [ ] logs:CreateLogDelivery
  - [ ] firehose:TagDeliveryStream
  - [ ] iam:CreateServiceLinkedRole
  - [ ] AWSServiceRoleForLogDelivery
- [ ] Kinesis uses Identity based policy where as other services uses Resource based policies
- [ ] In CloudTrail, event data stores do not use S3 buckets.
- [ ] In CloudTrail, by default data events are not logged, to record you must explicitly add the supported resources or resources types where you want to collect activity.
- [ ] Unwanted data movements use AWS global network for data transfers and doesn't touch any endpoints or network gateways, therefore related events only appear in Cloud Trail and AWS Config logs and not in the network.
- [ ] Implement structured logging using log levels. For unstructured, use glob or regular expression using a parse command.
- [ ] CloudWatch Insights cannot query CloudTrail logs directly.
- [ ] CloudTrail cannot send logs directly to Amazon Athena
- [ ] S3 Select gives you the ability to query one object at a time, it can't perform a complex queries
- [ ] S3 Select has size limitations of log and SQL queries that could further pose restrictions
- [ ] You can't use CloudTrail lake to query past CloudTrail logs, however you can use CloudTrail Lake to collect events from all future logs after CloudTrail lake is set up for an event data store.

Review these materials to learn more about the topics covered in this exam domain:

- [Using CloudWatch anomaly detection](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Anomaly_Detection.html)

- [AWS Security Incident Response Guide](https://docs.aws.amazon.com/whitepapers/latest/aws-security-incident-response-guide/introduction.html)

- [Insights in AWS Security Hub](https://docs.aws.amazon.com/securityhub/latest/userguide/securityhub-insights.html)

- [Logging IP traffic using VPC Flow Logs](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html)

- [Flow log record examples](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs-records-examples.html)

- [Troubleshooting access denied error messages](https://docs.aws.amazon.com/IAM/latest/UserGuide/troubleshoot_access-denied.html)

- [Centralized Logging with OpenSearch](https://aws.amazon.com/solutions/implementations/centralized-logging-with-opensearch/)

- [Using CloudTrail to identify unexpected behaviors in individual workloads](https://aws.amazon.com/blogs/security/using-cloudtrail-to-identify-unexpected-behaviors-in-individual-workloads/)

## Domain 3: Infrastructure Security

### Key Concepts

- [ ] Flow logs do not capture all IP traffic
- [ ] Network Access Analyser is a feature that identifies unintended network access to resources, you would not use this to test connectivity instead use VPC Reachability Analyser.
- [ ] Use Traffic Mirroring for out-of-band security and monitoring, a third-party tool is deployed on EC2 instance, and it can route network traffic and then examine the traffic to depth.

Review these materials to learn more about the topics covered in this exam domain:

- [AWS Well-Architected Framework's Security Pillar](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/design-principles.html)

- [Monitoring with Amazon CloudWatch](https://docs.aws.amazon.com/waf/latest/developerguide/monitoring-cloudwatch.html)

- [AWS Best Practices for DDoS Resiliency](https://docs.aws.amazon.com/whitepapers/latest/aws-best-practices-ddos-resiliency/aws-best-practices-ddos-resiliency.html)

- [Website endpoints](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteEndpoints.html)

- [Restricting access to files on custom origins](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-overview.html#forward-custom-headers-restrict-access)

- [Security perspective: compliance and assurance](https://docs.aws.amazon.com/whitepapers/latest/overview-aws-cloud-adoption-framework/security-perspective.html)

- [MAC Security](https://docs.aws.amazon.com/directconnect/latest/UserGuide/MACsec.html)

- [Amazon Elastic Block Store (Amazon EBS)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html)

- [AWS Systems Manager Patch Manager](https://docs.aws.amazon.com/systems-manager/latest/userguide/patch-manager.html)

- [Understanding findings in Amazon Inspector](https://docs.aws.amazon.com/inspector/latest/user/findings-understanding.html)

- [Amazon Inspector integration with AWS Security Hub](https://docs.aws.amazon.com/inspector/latest/user/securityhub-integration.html)

- [What is Reachability Analyzer?](https://docs.aws.amazon.com/vpc/latest/reachability/what-is-reachability-analyzer.html)

- [What is AWS Global Networks for Transit Gateways?](https://docs.aws.amazon.com/network-manager/latest/tgwnm/what-are-global-networks.html)

- [Flow log record examples](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs-records-examples.html)

- [Centralized logging solution on AWS](https://aws.amazon.com/solutions/centralized-logging/?ref=wellarchitected)

## Domain 4: Troubleshooting and Optimization

### Key Concepts

- [ ] IAM Identity Centre can hold sessions for up to 90 days.
- [ ] User pool is a user directory
  - [ ] Social identity provider
  - [ ] Third-party identity provider
  - [ ] Use Lambda for setting conditions
- [ ] Identity pool is a directory of federated identities
  - [ ] Basic and enhanced AuthFlows

### AWS Directory Service

- Simple Active Directory - basic AD, can handle 500 to 5000 users, doesn't support MFA, trust relationships with other domains and more.
- AWS Managed Microsoft AD - uses IAM Identity Center
- Active Directory Connector - directory gateway, which provides a proxy request back to your on-premises directory, when you do not want to store any directory information in AWS.

### Service Control Policies (SCPs)

- [ ] SCPs do not grant any permissions instead they specify the maximum permissions for an organisation OU or account.
- [ ] Any action that is not explicitly allowed or denied by the SCP affecting the account is blocked.
- [ ] By default, a full AWS access SCP policy is attached to every root organisation, unit, and account. This default SCP allows all actions and all services. For our scenario, we are creating a new organisation and until you start creating or manipulating the SCPs, all of your existing IAM permissions continue to operate as they were configured. But when you apply a new or modified SCP to a root or organisational unit that contains an account, the permissions that your users have in that account become filtered by the SCP. Permissions that used to work might now be denied if they're not allowed by the SCP at every level of the hierarchy down to the specific account.
- [ ] Let's say that you need to enable cross-account access to another AWS account as the principal in your resource-based policy. What is your solution? Well, adding a cross-account principal to a resource-based policy is one half of establishing the required access. Because the principal is in one AWS account and the resource is in another AWS account, you must also use an identity-based policy to grant the principal access to the resource.
- [ ] What if the principal is in the same AWS account as the resource? If a resource-based policy grants access to a principal in the same account, no additional identity-based policy is required.
- [ ] Cognito Identity pools can't authenticate with external IDPs.

Review these materials to learn more about the topics covered in this exam domain:

- [What is IAM?](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)

- [Security best practices in IAM](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)

- [Managing IAM users](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_manage.html)

- [Example IAM identity-based policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_examples.html)

- [IAM Access Analyzer](http://aws.amazon.com/iam/features/analyze-access/)

- [Actions, resources, and condition keys for AWS services](https://docs.aws.amazon.com/service-authorization/latest/reference/reference_policies_actions-resources-contextkeys.html)

- [Condition operators](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_elements_condition_operators.html)

- [Policy evaluation logic](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_evaluation-logic.html)

- [What is AWS CloudFormation Guard?](https://docs.aws.amazon.com/cfn-guard/latest/ug/what-is-guard.html)

## Domain 5: Infrastructure Security

### Key Concepts

- [ ] Kinesis Data Streams
  - StartStreamEncrpytion API
- [ ] The standard AWS asymmetric encryption algorithms that AWS KMS uses does not support encryption context.

### Amazon RDS and Secrets Management

- [ ] Amazon RDS volume snapshots Lifecycle policies
  - Automated snapshots can have a retention period from 1 to 35 days
  - Manual snapshots do not expire
- [ ] You can store your secrets in Secrets Manager and then reference the secret as a Parameter Store parameter.
- [ ] When you configure Parameter Store with Secrets Manager, the secret ID parameter store requires a forward slash before the name string.
- [ ] Secrets Manager provides automatic rotation of your secrets, but Parameter Store does not provide automatic rotation services for your stored secrets.

### Key Management

- [ ] Integrating Parameter Store and Secrets Manager gives you the benefits of Secret Manager and the ability to seamlessly support services that are referencing Parameter Store parameters.
  - [ ] Importing customer-provided key material
  - [ ] You remain responsible for managing key material
  - [ ] You can delete the key material
  - [ ] You can't change the key material or the key material origin
  - [ ] You can't export imported key material
  - [ ] You can create multi-Region keys
  - [ ] Removing customer-provided key material

Review these materials to learn more about the topics covered in this exam domain:

- [Encrypting Data-at-Rest and Data-in-Transit](https://docs.aws.amazon.com/whitepapers/latest/logical-separation/encrypting-data-at-rest-and--in-transit.html)

- [AWS Direct Connect + AWS Site-to-Site VPN](https://docs.aws.amazon.com/whitepapers/latest/aws-vpc-connectivity-options/aws-direct-connect-site-to-site-vpn.html)

- [Hybrid connectivity VPN](https://docs.aws.amazon.com/whitepapers/latest/building-scalable-secure-multi-vpc-network-infrastructure/hybrid-connectivity.html)

- [AWS Direct Connect](https://docs.aws.amazon.com/whitepapers/latest/building-scalable-secure-multi-vpc-network-infrastructure/direct-connect.html)

- [Building a global network using AWS Transit Gateway Inter-Region peering](https://aws.amazon.com/blogs/networking-and-content-delivery/building-a-global-network-using-aws-transit-gateway-inter-region-peering/)

- [AWS Prescriptive Guidance Encryption best practices and features for AWS services](https://docs.aws.amazon.com/pdfs/prescriptive-guidance/latest/encryption-best-practices/encryption-best-practices.pdf)

- [AWS Certificate Manager](https://docs.aws.amazon.com/acm/latest/userguide/acm-overview.html)

- [Amazon EC2 Instance Connect (EIC) Endpoint](https://aws.amazon.com/about-aws/whats-new/2023/06/amazon-ec2-instance-connect-ssh-rdp-public-ip-address/)

- [Secure Connectivity from Public to Private: Introducing EC2 Instance Connect Endpoint](https://aws.amazon.com/blogs/compute/secure-connectivity-from-public-to-private-introducing-ec2-instance-connect-endpoint-june-13-2023/)

- [Manage your storage lifecycle](https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lifecycle-mgmt.html)

- [Managing backups using backup plans](https://docs.aws.amazon.com/aws-backup/latest/devguide/about-backup-plans.html)

- [AWS KMS concepts](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html)

- [Asymmetric keys in AWS KMS](https://docs.aws.amazon.com/kms/latest/developerguide/symmetric-asymmetric.html)

- [Grants is AWS KMS](https://docs.aws.amazon.com/kms/latest/developerguide/grants.html)

- [What is AWS Nitro Enclaves?](https://docs.aws.amazon.com/enclaves/latest/user/nitro-enclave.html)

## Domain 6: Management and Security Governance

### AWS Control Tower

- [ ] Automate deployment of a multi-account environment according to AWS best practices
- [ ] Build a new AWS environment or start a new cloud initiative
- [ ] Provide control (guardrails) for ongoing governance
- [ ] Automate the creation of AWS accounts
- [ ] Existing OUs and accounts created outside of AWS Control Tower can be brought into AWS Control Tower governance at any time

### AWS Organizations

- [ ] Define your own custom multi-account environment with advanced management capabilities
- [ ] Create granular SCPs that centrally control the use of AWS services and resources across multiple accounts
- [ ] Currently you have multiple accounts such as engineering, finance, human resources, and more. And each of these accounts are managed by the team lead and have root access for their specific accounts. How can you centrally manage the policies and access needed to different AWS services across all of the AWS accounts and groups of accounts? Would you use AWS Control Tower or Organisation’s? I would use Organisations and create organisational units for the AWS accounts and group them as needed. You can control the access to the different AWS services using IAM policies and SCPs.

### AWS Firewall Manager

- Set up AWS WAF rules and configures security groups across multiple accounts and resources
- Automatically protect resources that are added to your account
- Only available for accounts that are members of Organizations

### Amazon Macie

- [ ] Predefined Macie allow don't accept wildcard entries
- [ ] Macie sensitive data discovery job must complete a full evaluation of the data in the S3 buckets
- [ ] Amazons Macie automated service evaluates a sample of objects in S3

### S3 Object Lock

- [ ] Object Lock provides two ways to manage object retention: retention periods and legal holds
- [ ] Retention modes:
  - [ ] Compliance mode
  - [ ] Governance mode
- [ ] In compliance mode, a protected object version can't be overwritten or deleted by any user, including the root user in your AWS account. When an object is locked in compliance mode, its retention mode can't be changed, and its retention period can't be shortened. Compliance mode helps ensure that an object version can't be overwritten or deleted for the duration of the retention period.
  > Note: The only way to delete an object under the compliance mode before its retention date expires is to delete the associated AWS account.
- [ ] In governance mode, users can't overwrite or delete an object version or alter its lock settings unless they have special permissions. With governance mode, you protect objects against being deleted by most users, but you can still grant some users permission to alter the retention settings or delete the objects if necessary. You can also use governance mode to test retention-period settings before creating a compliance-mode retention period.
- [ ] To override or remove governance-mode retention settings, you must have the s3:BypassGovernanceRetention permission and must explicitly include x-amz-bypass-governance-retention:true as a request header with any request that requires overriding governance mode.
  > Note: By default, the Amazon S3 console includes the x-amz-bypass-governance-retention:true header. If you try to delete objects protected by governance mode and have the s3:BypassGovernanceRetention permission, the operation will succeed.

Review these materials to learn more about the topics covered in this exam domain:

- [Governance](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/governance.html)

- [Security](https://docs.aws.amazon.com/wellarchitected/latest/framework/security.html)

- [Learn template basics](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/gettingstarted.templatebasics.html)

- [Working with AWS Firewall Manager policies](https://docs.aws.amazon.com/waf/latest/developerguide/working-with-policies.html)

- [Getting started with an AWS CloudFormation product](https://docs.aws.amazon.com/servicecatalog/latest/adminguide/getstarted-CFN.html)

- [AWS Config and AWS Organizations](https://docs.aws.amazon.com/organizations/latest/userguide/services-that-can-integrate-config.html)

- [AWS Audit Manager evidence](https://docs.aws.amazon.com/audit-manager/latest/userguide/evidence-finder.html#understanding-evidence-finder)

- [Mitigation techniques](https://docs.aws.amazon.com/whitepapers/latest/aws-best-practices-ddos-resiliency/mitigation-techniques.html)

- [Using CloudWatch anomaly detection](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Anomaly_Detection.html)

- [Guidance for baseline security assessment on AWS](https://aws.amazon.com/solutions/guidance/baseline-security-assessment-on-aws/#:~:text=Use%20the%20provided%20AWS%20CloudFormation,how%20to%20resolve%20the%20issues.)

## Contributing

Feel free to contribute by:

1. Opening issues for corrections
2. Submitting pull requests with improvements
3. Adding additional study resources

## Disclaimer

This is an unofficial study guide. All content has been compiled from AWS documentation and other official sources during exam preparation.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
